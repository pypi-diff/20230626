# Comparing `tmp/power-grid-model-1.5.0rc9187210536722.tar.gz` & `tmp/power-grid-model-1.5.0rc9188807400796.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9187210536722.tar", last modified: Fri Jun 23 13:39:27 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9188807400796.tar", last modified: Mon Jun 26 08:34:02 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9187210536722.tar` & `power-grid-model-1.5.0rc9188807400796.tar`

### file list

```diff
@@ -1,620 +1,620 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 13:38:48.000000 power-grid-model-1.5.0rc9187210536722/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.655275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.647275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.655275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.659275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    69656 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.647275 power-grid-model-1.5.0rc9187210536722/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.667275 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.663275 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-23 13:39:27.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37119 2023-06-23 13:39:27.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:39:27.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-23 13:39:27.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 13:39:27.000000 power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.667275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.667275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.667275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.667275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.671275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.671275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.675275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.679275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.683275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.683275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.683275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.687275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.687275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.687275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.691275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.691275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.695275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.695275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.695275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.699275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.699275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.703275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.703275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.707275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.707275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.707275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.711274 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.711274 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.715275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.715275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.719275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.719275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.719275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.723275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.723275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.727275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.727275 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.731274 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.731274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)    60746 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.735274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.735274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)    60902 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.739274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/sym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/sym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.739274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)    59648 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.743274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)    58856 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.747274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)    58682 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.751274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)    60884 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.751274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)    60740 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.751274 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)    60629 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.651275 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.751274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.751274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.755274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:39:27.759274 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-23 13:38:42.000000 power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.707017 power-grid-model-1.5.0rc9188807400796/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 08:34:02.707017 power-grid-model-1.5.0rc9188807400796/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 08:33:08.000000 power-grid-model-1.5.0rc9188807400796/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.587017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.591017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.575017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.595017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.595017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.599017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    69656 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.599017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.599017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.603017 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:34:02.707017 power-grid-model-1.5.0rc9188807400796/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.579017 power-grid-model-1.5.0rc9188807400796/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.603017 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.603017 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.607017 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.603017 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 08:34:02.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37119 2023-06-26 08:34:02.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:34:02.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 08:34:02.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 08:34:02.000000 power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.587017 power-grid-model-1.5.0rc9188807400796/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.607017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.607017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.611017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.611017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.615017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.615017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.619017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.619017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.623017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.623017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.623017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.627017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.579017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.579017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.627017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.631017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.631017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.631017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.635017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.635017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.639017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.639017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.647017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.651017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.655017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.659017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.659017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.659017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.663017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.663017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.663017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.667017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.667017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.671017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.671017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.671017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.675017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.675017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.675017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.679017 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.583016 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.679017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)    60746 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.683017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.683017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)    60902 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.687017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/sym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/sym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.687017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)    59648 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.687017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)    58856 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.691017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)    58682 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.691017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)    60884 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.691017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)    60740 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.695017 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)    60629 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.587017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.695017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.695017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.699017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.699017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.699017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.699017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.703017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.703017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.703017 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.707017 power-grid-model-1.5.0rc9188807400796/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:34:02.707017 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-26 08:33:03.000000 power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9187210536722/LICENSE` & `power-grid-model-1.5.0rc9188807400796/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/PKG-INFO` & `power-grid-model-1.5.0rc9188807400796/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9187210536722
+Version: 1.5.0rc9188807400796
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9187210536722/README.md` & `power-grid-model-1.5.0rc9188807400796/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 enum class WindingType : IntS { wye = 0, wye_n = 1, delta = 2, zigzag = 3, zigzag_n = 4 };
 
 enum class BranchSide : IntS { from = 0, to = 1 };
 
 enum class Branch3Side : IntS { side_1 = 0, side_2 = 1, side_3 = 2 };
 
 enum class CalculationMethod : IntS {
+    default_method = -128,
     linear = 0,
     newton_raphson = 1,
     iterative_linear = 2,
     iterative_current = 3,
-    linear_current = 4
+    linear_current = 4,
+    iec60909 = 5,
 };
 
 enum class MeasuredTerminalType : IntS {
     branch_from = 0,
     branch_to = 1,
     source = 2,
     shunt = 3,
```

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
     MathOutput<sym> run_power_flow(PowerFlowInput<sym> const& input, double err_tol, Idx max_iter,
                                    CalculationInfo& calculation_info, CalculationMethod calculation_method) {
         // set method to always linear if all load_gens have const_y
         calculation_method = all_const_y_ ? CalculationMethod::linear : calculation_method;
 
         switch (calculation_method) {
+            case CalculationMethod::default_method:
+                [[fallthrough]];  // use Newton-Raphson by default
             case CalculationMethod::newton_raphson:
                 return run_power_flow_newton_raphson(input, err_tol, max_iter, calculation_info);
             case CalculationMethod::linear:
                 return run_power_flow_linear(input, err_tol, max_iter, calculation_info);
             case CalculationMethod::linear_current:
                 return run_power_flow_linear_current(input, err_tol, max_iter, calculation_info);
             case CalculationMethod::iterative_current:
@@ -53,15 +55,16 @@
             default:
                 throw InvalidCalculationMethod{};
         }
     }
 
     MathOutput<sym> run_state_estimation(StateEstimationInput<sym> const& input, double err_tol, Idx max_iter,
                                          CalculationInfo& calculation_info, CalculationMethod calculation_method) {
-        if (calculation_method != CalculationMethod::iterative_linear) {
+        if (calculation_method != CalculationMethod::default_method &&
+            calculation_method != CalculationMethod::iterative_linear) {
             throw InvalidCalculationMethod{};
         }
 
         // construct model if needed
         if (!iterative_linear_se_solver_.has_value()) {
             Timer timer(calculation_info, 2210, "Create math solver");
             iterative_linear_se_solver_.emplace(y_bus_, topo_ptr_);
```

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files 2% similar despite different names*

```diff
@@ -75,28 +75,33 @@
 
 // enums
 /**
  * @brief Enumeration for calculation type
  *
  */
 enum PGM_CalculationType {
-    PGM_power_flow = 0,      /**< power flow calculation */
-    PGM_state_estimation = 1 /**< state estimation calculation */
+    PGM_power_flow = 0,       /**< power flow calculation */
+    PGM_state_estimation = 1, /**< state estimation calculation */
+    PGM_short_circuit = 2     /**< short circuit calculation */
 };
+
 /**
  * @brief Enumeration for calculation method
  *
  */
 enum PGM_CalculationMethod {
+    PGM_default_method = -128, /**< the default method for each calculation type, e.g. Newton-Raphson for power flow */
     PGM_linear = 0,            /**< linear constant impedance method for power flow */
     PGM_newton_raphson = 1,    /**< Newton-Raphson method for power flow */
     PGM_iterative_linear = 2,  /**< iterative linear method for state estimation */
     PGM_iterative_current = 3, /**< linear current method for power flow */
-    PGM_linear_current = 4     /**< iterative constant impedance method for power flow */
+    PGM_linear_current = 4,    /**< iterative constant impedance method for power flow */
+    PGM_iec60909 = 5           /**< fault analysis for short circuits using the iec60909 standard*/
 };
+
 /**
  * @brief Enumeration of error codes
  *
  */
 enum PGM_ErrorCode {
     PGM_no_error = 0,      /**< no error occurred */
     PGM_regular_error = 1, /**< some error occurred which is not in the batch calculation */
@@ -396,15 +401,15 @@
 
 /**
  * @brief Create an option instance.
  *
  * The option is needed to run calculations.
  * This function create a new option instance with the following default values:
  *   - calculation_type: PGM_power_flow
- *   - calculation_method: PGM_newton_raphson
+ *   - calculation_method: PGM_default_method
  *   - symmetric: 1
  *   - err_tol: 1e-8
  *   - max_iter: 20
  *   - threading: -1
  *
  * @param handle
  * @return a pointer to the option instance. Should be freed by PGM_destroy_options()
```

### Comparing `power-grid-model-1.5.0rc9187210536722/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9188807400796/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 #include "power_grid_model/auxiliary/meta_data_gen.hpp"
 #include "power_grid_model/main_model.hpp"
 #include "power_grid_model/power_grid_model.hpp"
 
 using namespace power_grid_model;
 
-static meta_data::AllPowerGridMetaData const& pgm_meta = meta_data::meta_data();
+namespace {
+meta_data::AllPowerGridMetaData const& pgm_meta = meta_data::meta_data();
+}  // namespace
 
 // assert index type
 static_assert(std::is_same_v<PGM_Idx, Idx>);
 static_assert(std::is_same_v<PGM_ID, ID>);
 
 // main model
 struct PGM_PowerGridModel : public MainModel {
@@ -35,53 +37,57 @@
     mutable std::vector<char const*> batch_errs_c_str;
     BatchParameter batch_parameter;
 };
 
 // options
 struct PGM_Options {
     Idx calculation_type{PGM_power_flow};
-    Idx calculation_method{PGM_newton_raphson};
+    Idx calculation_method{PGM_default_method};
     Idx symmetric{1};
     double err_tol{1e-8};
     Idx max_iter{20};
     Idx threading{-1};
 };
 
+namespace {
 // helper functions
 std::vector<std::string> list_of_datasets() {
     std::vector<std::string> res;
     auto const& meta = pgm_meta;
     std::transform(meta.cbegin(), meta.cend(), std::back_inserter(res), [](auto const& x) {
         return x.first;
     });
     return res;
 }
+
 std::map<std::string, std::vector<std::string>> list_of_classes() {
     std::map<std::string, std::vector<std::string>> res;
     for (auto const& [key, val] : pgm_meta) {
         std::vector<std::string> vec;
         std::transform(val.cbegin(), val.cend(), std::back_inserter(vec), [](auto const& x) {
             return x.first;
         });
         res[key] = vec;
     }
     return res;
 }
+
 template <class Functor>
 auto call_with_bound(PGM_Handle* handle, Functor func) -> std::invoke_result_t<Functor> {
     static std::remove_cv_t<std::remove_reference_t<std::invoke_result_t<Functor>>> const empty{};
     try {
         return func();
     }
     catch (std::out_of_range& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = std::string(e.what()) + "\n You supplied wrong name and/or index!\n";
         return empty;
     }
 }
+}  // namespace
 
 // create and destroy handle
 PGM_Handle* PGM_create_handle() {
     return new PGM_Handle{};
 }
 void PGM_destroy_handle(PGM_Handle* handle) {
     delete handle;
@@ -200,14 +206,16 @@
     if (data_class.name == "") {
         return;
     }
     for (Idx i = 0; i != size; ++i) {
         data_class.set_nan(ptr, i);
     }
 }
+
+namespace {
 // template for get and set attribute
 template <bool is_get, class BufferPtr, class ValuePtr>
 void buffer_get_set_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
                           BufferPtr buffer_ptr, ValuePtr value_ptr, PGM_Idx size, PGM_Idx stride) {
     auto const& data_class = call_with_bound(handle, [&]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component);
     });
@@ -228,14 +236,15 @@
             data_class.get_attr(buffer_ptr, shifted_value_ptr, attr, i);
         }
         else {
             data_class.set_attr(buffer_ptr, shifted_value_ptr, attr, i);
         }
     }
 }
+}  // namespace
 void PGM_buffer_set_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
                           void* buffer_ptr, void const* src_ptr, PGM_Idx size, PGM_Idx src_stride) {
     buffer_get_set_value<false>(handle, dataset, component, attribute, buffer_ptr, src_ptr, size, src_stride);
 }
 void PGM_buffer_get_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
                           void const* buffer_ptr, void* dest_ptr, PGM_Idx size, PGM_Idx dest_stride) {
     buffer_get_set_value<true>(handle, dataset, component, attribute, buffer_ptr, dest_ptr, size, dest_stride);
@@ -381,14 +390,16 @@
                 }
                 else {
                     handle->batch_parameter = model->calculate_state_estimation<false>(
                         opt->err_tol, opt->max_iter, (CalculationMethod)opt->calculation_method, output_dataset,
                         update_dataset, opt->threading);
                 }
                 break;
+            case PGM_short_circuit:
+                [[fallthrough]];
             default:
                 throw MissingCaseForEnumError{"CalculationType", opt->calculation_type};
         }
     }
     catch (BatchCalculationError& e) {
         handle->err_code = PGM_batch_error;
         handle->err_msg = e.what();
```

### Comparing `power-grid-model-1.5.0rc9187210536722/pyproject.toml` & `power-grid-model-1.5.0rc9188807400796/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/setup.py` & `power-grid-model-1.5.0rc9188807400796/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9187210536722
+Version: 1.5.0rc9188807400796
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9187210536722/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9188807400796/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9188807400796/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/sym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/sym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9188807400796/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/utils.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9187210536722/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9188807400796/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

