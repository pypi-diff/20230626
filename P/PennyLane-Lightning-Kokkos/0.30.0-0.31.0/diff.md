# Comparing `tmp/PennyLane-Lightning-Kokkos-0.30.0.tar.gz` & `tmp/PennyLane-Lightning-Kokkos-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane-Lightning-Kokkos-0.30.0.tar", last modified: Mon May  1 20:15:25 2023, max compression
+gzip compressed data, was "PennyLane-Lightning-Kokkos-0.31.0.tar", last modified: Mon Jun 26 14:52:44 2023, max compression
```

## Comparing `PennyLane-Lightning-Kokkos-0.30.0.tar` & `PennyLane-Lightning-Kokkos-0.31.0.tar`

### file list

```diff
@@ -1,24 +1,60 @@
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.937004 PennyLane-Lightning-Kokkos-0.30.0/.github/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6769 2023-05-01 19:56:53.000000 PennyLane-Lightning-Kokkos-0.30.0/.github/CHANGELOG.md
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/LICENSE
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       53 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/MANIFEST.in
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/PKG-INFO
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.937004 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      591 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/dependency_links.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       82 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/entry_points.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       16 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/requires.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/top_level.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4509 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/README.rst
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      730 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/__init__.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10963 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_serialize.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      697 2023-05-01 19:57:30.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_version.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    31177 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/lightning_kokkos.py
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/src/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      469 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/src/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       99 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/requirements.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/setup.cfg
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7670 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/setup.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.332427 PennyLane-Lightning-Kokkos-0.31.0/
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.325760 PennyLane-Lightning-Kokkos-0.31.0/.github/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7888 2023-06-26 13:53:47.000000 PennyLane-Lightning-Kokkos-0.31.0/.github/CHANGELOG.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/LICENSE
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       53 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/MANIFEST.in
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6747 2023-06-26 14:52:44.332427 PennyLane-Lightning-Kokkos-0.31.0/PKG-INFO
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.325760 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6747 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2460 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/dependency_links.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       82 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/entry_points.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       16 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/requires.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-06-26 14:52:44.000000 PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/top_level.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5658 2023-06-26 13:15:02.000000 PennyLane-Lightning-Kokkos-0.31.0/README.rst
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.329093 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      730 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/__init__.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10963 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/_serialize.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      697 2023-06-26 13:45:25.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/_version.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    30640 2023-06-26 13:15:02.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/lightning_kokkos.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.329093 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      469 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/CMakeLists.txt
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.329093 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/algorithms/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      243 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/algorithms/AdjointDiffKokkos.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    18327 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/algorithms/AdjointDiffKokkos.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      598 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/algorithms/CMakeLists.txt
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.329093 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/bindings/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    43744 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/bindings/Bindings.cpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.329093 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1045 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12083 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/ExpValFunctors.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)   119060 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/GateFunctors.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    53819 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/GatesHost.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7154 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/MeasuresFunctors.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      216 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/MeasuresKokkos.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24295 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/MeasuresKokkos.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    17115 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/ObservablesKokkos.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      774 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/StateVectorKokkos.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    67947 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/simulator/StateVectorKokkos.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.332427 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1842 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5421 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/TestHelpers.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    21078 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_AdjointDiffKokkos.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5373 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_Backend_info.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3565 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_LinearAlgebra.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    21557 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_Expval.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)   103858 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_Generator.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6831 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_Measure.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    53221 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_NonParam.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    61845 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_Param.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5298 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/Test_StateVectorKokkos_Var.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      385 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/tests/runner_main.cpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:52:44.332427 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      332 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5271 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/Error.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5535 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/GetConfigInfo.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7676 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/LinearAlgebraKokkos.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    18404 2023-06-26 13:13:49.000000 PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/src/util/UtilKokkos.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       99 2023-06-26 13:15:02.000000 PennyLane-Lightning-Kokkos-0.31.0/requirements.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-06-26 14:52:44.332427 PennyLane-Lightning-Kokkos-0.31.0/setup.cfg
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6038 2023-06-26 13:53:59.000000 PennyLane-Lightning-Kokkos-0.31.0/setup.py
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/.github/CHANGELOG.md` & `PennyLane-Lightning-Kokkos-0.31.0/.github/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,67 @@
+# Release 0.31.0
+
+### Breaking changes
+
+* Deprecate `kokkos_config_info`, replaced by Kokkos' `print_configuration`.
+  [(#55)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/55)
+
+* Update tests to be compliant with PennyLane v0.31.0 development changes and deprecations.
+  [(#66)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/66)
+
+### Improvements
+
+* Upgrade Kokkos version to v4.0.01.
+  [(#55)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/55)
+
+* Remove logic from `setup.py` and transfer paths and definitions into workflow files.
+  [(#58)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/58)
+
+* Use `Operator.name` instead of `Operation.base_name`.
+  [(#67)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/67)
+
+### Contributors
+
+This release contains contributions from (in alphabetical order):
+
+Christina Lee, Vincent Michaud-Rioux
+
+---
+
 # Release 0.30.0
 
 ### New features since last release
 
 * Add native support for `expval` and `var` of generic observables. Refactor measurements support.
-[(#47)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/47)
+  [(#47)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/47)
 
 ### Breaking changes
 
 * Provide support for PennyLane-Lightning-Kokkos to coexist with PennyLane-Lightning.
-[(#49)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/49)
+  [(#49)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/49)
 
 ### Improvements
 
+* Replace deprecated InitArguments by InitializationSettings.
+  [(#57)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/57)
+
 * Remove deprecated `set-output` commands from workflow files.
-[(#56)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/56)
+  [(#56)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/56)
 
 * `setup.py` works on MacOS without `brew` (which is required by Conda-Forge runners).
-[(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
+  [(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
 
 * MacOS::Intel wheels are built for the SERIAL and THREADS Kokkos backends.
-[(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
+  [(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
 
 * Wheels are now checked with `twine check` post-creation for PyPI compatibility.
-[(#50)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/50)
+  [(#50)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/50)
 
 * Template n-qubit gate methods.
-[(#40)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/40)
+  [(#40)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/40)
 
 ### Bug fixes
 
 * Updates to use the new call signature for `QuantumScript.get_operation`.
   [(#52)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/52)
 
 
@@ -42,20 +74,20 @@
 ---
 
 # Release 0.29.1
 
 ### Improvements
 
 * Use CMake `find_package` to bind pre-installed Kokkos libraries.
-[(#43)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/43)
+  [(#43)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/43)
 
 ### Bug fixes
 
 * Ensure Kokkos finalize is only called at the end of process execution.
-[(#45)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/45)
+  [(#45)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/45)
 
 ### Contributors
 
 This release contains contributions from (in alphabetical order):
 
 Vincent Michaud-Rioux, Lee James O'Riordan
 
@@ -64,61 +96,61 @@
 # Release 0.29.0
 
 ### New features since last release
 
  * Add support for building X86-64 Linux wheels with OpenMP and SERIAL backends with Github Actions.
  [(#14)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/14)
 
- * Add the `kokkos_config` class variable, which stores the kokkos build and runtime information such as `Backend`, `Architecture`, `Kokkos Version`, `Compiler`, to LightningKokkos for users' query purpose. Users can also access other information such as `Options`, `Memory`, `Atomics` and `Vectorization` from `kokkos_config`.
- The workflow for build and runtime information query is:
+* Add the `kokkos_config` class variable, which stores the kokkos build and runtime information such as `Backend`, `Architecture`, `Kokkos Version`, `Compiler`, to LightningKokkos for users' query purpose. Users can also access other information such as `Options`, `Memory`, `Atomics` and `Vectorization` from `kokkos_config`.
+  The workflow for build and runtime information query is:
 
- ```python
- >>> import pennylane as qml
- >>> dev = qml.device('lightning.kokkos', wires=3)
- >>> dev.kokkos_config["Backend"]
- {'Parallel': 'OpenMP'}
- ```
-[(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
+  ```python
+  >>> import pennylane as qml
+  >>> dev = qml.device('lightning.kokkos', wires=3)
+  >>> dev.kokkos_config["Backend"]
+  {'Parallel': 'OpenMP'}
+  ```
+  [(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
 
 
 ### Breaking changes
 
 * Change LightningKokkos to inherit from QubitDevice instead of LightningQubit. Numpy data initialization is decoupled.
-[(#31)] (https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/31)
+  [(#31)] (https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/31)
 
 ### Improvements
 
 * Use CMake `find_package` to bind pre-installed Kokkos libraries.
-[(#43)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/43)
+  [(#43)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/43)
 
 * Update `inv()` methods in Python unit tests with `qml.adjoint()`.
-[(#33)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/33)
+  [(#33)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/33)
 
 * Remove explicit Numpy requirement.
-[(#35)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/35)
+  [(#35)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/35)
 
 * Add Kokkos::InitArguments support.
-[(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
+  [(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
 
 * Add Nvidia GPU support for CI checks.
-[(#37)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/37)
+  [(#37)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/37)
 
 * Add VJP support.
-[(#32)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/32)
+  [(#32)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/32)
 
 ### Bug fixes
 
 * Ensure early-failure rather than return of incorrect results from out of order probs wires.
-[(#41)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/41)
+  [(#41)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/41)
 
 * Fix the CI environment variables for building wheels with the OpenMP backend.
-[(#36)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/36)
+  [(#36)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/36)
 
 * Fix the failures of pl_device_test tests with shots set.
-[(#38)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/38)
+  [(#38)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/38)
 
 ### Contributors
 
 This release contains contributions from (in alphabetical order):
 
 Amintor Dusko, Vincent Michaud-Rioux, Lee James O'Riordan, Shuli Shu
 
@@ -127,62 +159,62 @@
 # Release 0.28.0
 
 ### Breaking changes
 
 * Drop python3.7 and deprecate the Python and C++ tests with threading backend in workflows.
 Note this deprecation is based on the fact that Kokkos cannot promise that its Threads back-end will
 not conflict with the application's direct use of operating system threads.
-[(#23)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/23)
+  [(#23)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/23)
 
 * Remove the unused `supports_reversible_diff` device capability from `LightningKokkos`
-[(#20)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/20)
+  [(#20)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/20)
 
 ### Improvements
 
 * Improve the stopping condition method.
-[(#25)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/25)
+  [(#25)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/25)
 
 ### Documentation
 
 * Update version string in package for release.
-[(#27)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/27)
+  [(#27)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/27)
 
 ### Bug fixes
 
 * Avoid integer overflow in middle value calculation of binary search in `Sampler`.
-[#18] (https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/18)
+  [#18](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/18)
 
 ### Contributors
 
 This release contains contributions from (in alphabetical order):
 
 Amintor Dusko, Lee J. O'Riordan, Shuli Shu, Matthew Silverman
 
 --
 
 # Release 0.27.0
 
 ### New features since last release
 
- * Add probability support.
- [(#11)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/11)
+* Add probability support.
+  [(#11)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/11)
 
- * Add sample generation support.
- [(#9)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/9)
+* Add sample generation support.
+  [(#9)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/9)
 
 ### Breaking changes
 
 
 ### Improvements
 
- * Add tests for MacOS.
+* Add tests for MacOS.
   [(#3)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/3)
 
- * Update `LightningKokkos` device following changes in `LightningQubit` inheritance from `DefaultQubit` to `QubitDevice`.
- [(#16)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/16)
+* Update `LightningKokkos` device following changes in `LightningQubit` inheritance from `DefaultQubit` to `QubitDevice`.
+  [(#16)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/16)
 
 ### Documentation
 
 ### Bug fixes
 
 ### Contributors
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/LICENSE` & `PennyLane-Lightning-Kokkos-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/PKG-INFO` & `PennyLane-Lightning-Kokkos-0.31.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning-Kokkos
-Version: 0.30.0
+Version: 0.31.0
 Summary: PennyLane-Lightning-Kokkos plugin
 Home-page: https://github.com/PennyLaneAI/pennylane-lightning-kokkos
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -26,50 +26,64 @@
 License-File: LICENSE
 
 PennyLane-Lightning-Kokkos Plugin
 #################################
 
 .. header-start-inclusion-marker-do-not-remove
 
-The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin extends the `Pennylane-Lightning <https://github.com/PennyLaneAI/pennylane-lightning>`_ state-vector simulator written in C++, and offloads to the `Kokkos library <https://github.com/kokkos/kokkos>`__ for accelerated circuit simulation.
+The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin provides a fast state-vector simulator written in C++.
+It enables parallel execution with various parallel backends, including C++ threads, OpenMP, CUDA, ROCM/HIP and SYCL via the `Kokkos library <https://github.com/kokkos/kokkos>`_.
+For more details, have a look at our `blog post <https://pennylane.ai/blog/2023/04/pennylane-goes-kokkos-a-novel-hardware-agnostic-parallel-backend-for-quantum-simulations>`_.
 
-`PennyLane <https://docs.pennylane.ai>`_ is a cross-platform Python library for quantum machine
-learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+PennyLane is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 .. header-end-inclusion-marker-do-not-remove
 
 .. installation-start-inclusion-marker-do-not-remove
 
 Installation
 ============
 
+We suggest first installing Kokkos with the wanted configuration following the instruction found in the `Kokkos documentation <https://kokkos.github.io/kokkos-core-wiki/building.html>`_.
+Next, append the install location to ``CMAKE_PREFIX_PATH``.
+If an installation is not found, our builder will install it from scratch nevertheless.
+
+The simplest way to install PennyLane-Lightning-Kokkos (OpenMP backend) is using ``pip``.
+
 .. code-block:: console
 
-   cmake -Bbuild -DKokkos_ENABLE_OPENMP=On -DPLKOKKOS_BUILD_TESTS=On -G Ninja
-   cmake --build ./build
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install .
 
-You can install the python interface with:
+or for an editable ``pip`` installation with:
 
 .. code-block:: console
 
-   python setup.py build_ext --backend="OPENMP"
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install -e .
+
+Alternatively, you can install the python interface with:
+
+.. code-block:: console
+
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python setup.py build_ext
    python setup.py bdist_wheel
    pip install ./dist/PennyLane*.whl --force-reinstall
 
-
-or for an editable `pip` installation with:
+To build the plugin directly with CMake:
 
 .. code-block:: console
 
-   BACKEND="OPENMP" python -m pip install -e .
+   cmake -B build -DKokkos_ENABLE_OPENMP=ON -DPLKOKKOS_BUILD_TESTS=ON -G Ninja
+   cmake --build build
 
-
-Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA". For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
-For explicit targeting of a given supported architecture, the environment variable `ARCH` can also be specified which directly sets the `-DKokkos_ARCH_{...}=ON` build option. Note that "THREADS"
-backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
+Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA" and the corresponding build switches are ``-DKokkos_ENABLE_BACKEND=ON``, where one needs to replace ``BACKEND``.
+One can activate simultaneously one serial, one parallel CPU host (e.g. "OPENMP", "THREADS") and one parallel GPU device backend (e.g. "HIP", "CUDA"), but not two of any category at the same time.
+For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
+Similarly, the CMake option ``-DKokkos_ARCH_{...}=ON`` must also be specified to target a given architecture.
+A list of the architectures is found on the `Kokkos wiki <https://github.com/kokkos/kokkos/wiki/Macros#architectures>`_.
+Note that "THREADS" backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
 
 .. installation-end-inclusion-marker-do-not-remove
 
 Testing
 =======
 
 To test with the ROCm stack using a manylinux2014 container we must first mount the repository into the container:
@@ -80,33 +94,33 @@
 
 Next, within the container, we install the ROCm software stack:
 
 .. code-block:: console
 
     yum install -y https://repo.radeon.com/amdgpu-install/21.40.2/rhel/7.9/amdgpu-install-21.40.2.40502-1.el7.noarch.rpm
     amdgpu-install --usecase=hiplibsdk,rocm --no-dkms
-    
+
 We next build the test-suite, with a given AMD GPU target in mind, as listed `here <https://github.com/kokkos/kokkos/blob/master/Makefile.kokkos>`_.
 
 .. code-block:: console
 
     cd /io
-    export PATH=$PATH:/opt/rocm/bin/ 
+    export PATH=$PATH:/opt/rocm/bin/
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/rocm/lib
-    export CXX=/opt/rocm/hip/bin/hipcc 
-    cmake -Bbuild -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=on -DPLKOKKOS_BUILD_TESTS=On -DKokkos_ARCH_VEGA90A=ON
-    cmake --build ./build --verbose
+    export CXX=/opt/rocm/hip/bin/hipcc
+    cmake -B build -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=ON -DPLKOKKOS_BUILD_TESTS=ON -DKokkos_ARCH_VEGA90A=ON
+    cmake --build build --verbose
 
-We may now leave the container, and run the built test-suite on a machine with access to the targetted GPU.
+We may now leave the container, and run the built test-suite on a machine with access to the targeted GPU.
 
-For a system with access to the ROCm stack outside of a manylinux container, an editable `pip` installation can be built and installed as:
+For a system with access to the ROCm stack outside of a manylinux container, an editable ``pip`` installation can be built and installed as:
 
 .. code-block:: console
 
-   BACKEND="HIP" ARCH="VEGA90A" python -m pip install -e .
+   CMAKE_ARGS="-DKokkos_ENABLE_HIP=ON -DKokkos_ARCH_VEGA90A=ON" python -m pip install -e .
 
 
 .. support-start-inclusion-marker-do-not-remove
 
 Support
 =======
 
@@ -121,15 +135,15 @@
 .. license-start-inclusion-marker-do-not-remove
 
 
 License
 =======
 
 The PennyLane-Lightning-Kokkos plugin is **free** and **open source**, released under
-the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_. 
+the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_.
 The PennyLane-Lightning-Kokkos plugin makes use of the `Kokkos <https://github.com/kokkos/kokkos>`__ library, which is held to their own respective licenses.
 
 .. license-end-inclusion-marker-do-not-remove
 .. acknowledgements-start-inclusion-marker-do-not-remove
 
 Acknowledgements
 ================
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO` & `PennyLane-Lightning-Kokkos-0.31.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning-Kokkos
-Version: 0.30.0
+Version: 0.31.0
 Summary: PennyLane-Lightning-Kokkos plugin
 Home-page: https://github.com/PennyLaneAI/pennylane-lightning-kokkos
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -26,50 +26,64 @@
 License-File: LICENSE
 
 PennyLane-Lightning-Kokkos Plugin
 #################################
 
 .. header-start-inclusion-marker-do-not-remove
 
-The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin extends the `Pennylane-Lightning <https://github.com/PennyLaneAI/pennylane-lightning>`_ state-vector simulator written in C++, and offloads to the `Kokkos library <https://github.com/kokkos/kokkos>`__ for accelerated circuit simulation.
+The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin provides a fast state-vector simulator written in C++.
+It enables parallel execution with various parallel backends, including C++ threads, OpenMP, CUDA, ROCM/HIP and SYCL via the `Kokkos library <https://github.com/kokkos/kokkos>`_.
+For more details, have a look at our `blog post <https://pennylane.ai/blog/2023/04/pennylane-goes-kokkos-a-novel-hardware-agnostic-parallel-backend-for-quantum-simulations>`_.
 
-`PennyLane <https://docs.pennylane.ai>`_ is a cross-platform Python library for quantum machine
-learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+PennyLane is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 .. header-end-inclusion-marker-do-not-remove
 
 .. installation-start-inclusion-marker-do-not-remove
 
 Installation
 ============
 
+We suggest first installing Kokkos with the wanted configuration following the instruction found in the `Kokkos documentation <https://kokkos.github.io/kokkos-core-wiki/building.html>`_.
+Next, append the install location to ``CMAKE_PREFIX_PATH``.
+If an installation is not found, our builder will install it from scratch nevertheless.
+
+The simplest way to install PennyLane-Lightning-Kokkos (OpenMP backend) is using ``pip``.
+
 .. code-block:: console
 
-   cmake -Bbuild -DKokkos_ENABLE_OPENMP=On -DPLKOKKOS_BUILD_TESTS=On -G Ninja
-   cmake --build ./build
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install .
 
-You can install the python interface with:
+or for an editable ``pip`` installation with:
 
 .. code-block:: console
 
-   python setup.py build_ext --backend="OPENMP"
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install -e .
+
+Alternatively, you can install the python interface with:
+
+.. code-block:: console
+
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python setup.py build_ext
    python setup.py bdist_wheel
    pip install ./dist/PennyLane*.whl --force-reinstall
 
-
-or for an editable `pip` installation with:
+To build the plugin directly with CMake:
 
 .. code-block:: console
 
-   BACKEND="OPENMP" python -m pip install -e .
+   cmake -B build -DKokkos_ENABLE_OPENMP=ON -DPLKOKKOS_BUILD_TESTS=ON -G Ninja
+   cmake --build build
 
-
-Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA". For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
-For explicit targeting of a given supported architecture, the environment variable `ARCH` can also be specified which directly sets the `-DKokkos_ARCH_{...}=ON` build option. Note that "THREADS"
-backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
+Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA" and the corresponding build switches are ``-DKokkos_ENABLE_BACKEND=ON``, where one needs to replace ``BACKEND``.
+One can activate simultaneously one serial, one parallel CPU host (e.g. "OPENMP", "THREADS") and one parallel GPU device backend (e.g. "HIP", "CUDA"), but not two of any category at the same time.
+For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
+Similarly, the CMake option ``-DKokkos_ARCH_{...}=ON`` must also be specified to target a given architecture.
+A list of the architectures is found on the `Kokkos wiki <https://github.com/kokkos/kokkos/wiki/Macros#architectures>`_.
+Note that "THREADS" backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
 
 .. installation-end-inclusion-marker-do-not-remove
 
 Testing
 =======
 
 To test with the ROCm stack using a manylinux2014 container we must first mount the repository into the container:
@@ -80,33 +94,33 @@
 
 Next, within the container, we install the ROCm software stack:
 
 .. code-block:: console
 
     yum install -y https://repo.radeon.com/amdgpu-install/21.40.2/rhel/7.9/amdgpu-install-21.40.2.40502-1.el7.noarch.rpm
     amdgpu-install --usecase=hiplibsdk,rocm --no-dkms
-    
+
 We next build the test-suite, with a given AMD GPU target in mind, as listed `here <https://github.com/kokkos/kokkos/blob/master/Makefile.kokkos>`_.
 
 .. code-block:: console
 
     cd /io
-    export PATH=$PATH:/opt/rocm/bin/ 
+    export PATH=$PATH:/opt/rocm/bin/
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/rocm/lib
-    export CXX=/opt/rocm/hip/bin/hipcc 
-    cmake -Bbuild -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=on -DPLKOKKOS_BUILD_TESTS=On -DKokkos_ARCH_VEGA90A=ON
-    cmake --build ./build --verbose
+    export CXX=/opt/rocm/hip/bin/hipcc
+    cmake -B build -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=ON -DPLKOKKOS_BUILD_TESTS=ON -DKokkos_ARCH_VEGA90A=ON
+    cmake --build build --verbose
 
-We may now leave the container, and run the built test-suite on a machine with access to the targetted GPU.
+We may now leave the container, and run the built test-suite on a machine with access to the targeted GPU.
 
-For a system with access to the ROCm stack outside of a manylinux container, an editable `pip` installation can be built and installed as:
+For a system with access to the ROCm stack outside of a manylinux container, an editable ``pip`` installation can be built and installed as:
 
 .. code-block:: console
 
-   BACKEND="HIP" ARCH="VEGA90A" python -m pip install -e .
+   CMAKE_ARGS="-DKokkos_ENABLE_HIP=ON -DKokkos_ARCH_VEGA90A=ON" python -m pip install -e .
 
 
 .. support-start-inclusion-marker-do-not-remove
 
 Support
 =======
 
@@ -121,15 +135,15 @@
 .. license-start-inclusion-marker-do-not-remove
 
 
 License
 =======
 
 The PennyLane-Lightning-Kokkos plugin is **free** and **open source**, released under
-the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_. 
+the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_.
 The PennyLane-Lightning-Kokkos plugin makes use of the `Kokkos <https://github.com/kokkos/kokkos>`__ library, which is held to their own respective licenses.
 
 .. license-end-inclusion-marker-do-not-remove
 .. acknowledgements-start-inclusion-marker-do-not-remove
 
 Acknowledgements
 ================
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/README.rst` & `PennyLane-Lightning-Kokkos-0.31.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 PennyLane-Lightning-Kokkos Plugin
 #################################
 
 .. header-start-inclusion-marker-do-not-remove
 
-The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin extends the `Pennylane-Lightning <https://github.com/PennyLaneAI/pennylane-lightning>`_ state-vector simulator written in C++, and offloads to the `Kokkos library <https://github.com/kokkos/kokkos>`__ for accelerated circuit simulation.
+The `PennyLane-Lightning-Kokkos <https://github.com/PennyLaneAI/pennylane-lightning-kokkos>`_ plugin provides a fast state-vector simulator written in C++.
+It enables parallel execution with various parallel backends, including C++ threads, OpenMP, CUDA, ROCM/HIP and SYCL via the `Kokkos library <https://github.com/kokkos/kokkos>`_.
+For more details, have a look at our `blog post <https://pennylane.ai/blog/2023/04/pennylane-goes-kokkos-a-novel-hardware-agnostic-parallel-backend-for-quantum-simulations>`_.
 
-`PennyLane <https://docs.pennylane.ai>`_ is a cross-platform Python library for quantum machine
-learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+PennyLane is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 .. header-end-inclusion-marker-do-not-remove
 
 .. installation-start-inclusion-marker-do-not-remove
 
 Installation
 ============
 
+We suggest first installing Kokkos with the wanted configuration following the instruction found in the `Kokkos documentation <https://kokkos.github.io/kokkos-core-wiki/building.html>`_.
+Next, append the install location to ``CMAKE_PREFIX_PATH``.
+If an installation is not found, our builder will install it from scratch nevertheless.
+
+The simplest way to install PennyLane-Lightning-Kokkos (OpenMP backend) is using ``pip``.
+
 .. code-block:: console
 
-   cmake -Bbuild -DKokkos_ENABLE_OPENMP=On -DPLKOKKOS_BUILD_TESTS=On -G Ninja
-   cmake --build ./build
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install .
 
-You can install the python interface with:
+or for an editable ``pip`` installation with:
 
 .. code-block:: console
 
-   python setup.py build_ext --backend="OPENMP"
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python -m pip install -e .
+
+Alternatively, you can install the python interface with:
+
+.. code-block:: console
+
+   CMAKE_ARGS="-DKokkos_ENABLE_OPENMP=ON" python setup.py build_ext
    python setup.py bdist_wheel
    pip install ./dist/PennyLane*.whl --force-reinstall
 
-
-or for an editable `pip` installation with:
+To build the plugin directly with CMake:
 
 .. code-block:: console
 
-   BACKEND="OPENMP" python -m pip install -e .
+   cmake -B build -DKokkos_ENABLE_OPENMP=ON -DPLKOKKOS_BUILD_TESTS=ON -G Ninja
+   cmake --build build
 
-
-Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA". For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
-For explicit targeting of a given supported architecture, the environment variable `ARCH` can also be specified which directly sets the `-DKokkos_ARCH_{...}=ON` build option. Note that "THREADS"
-backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
+Supported backend options are "SERIAL", "OPENMP", "THREADS", "HIP" and "CUDA" and the corresponding build switches are ``-DKokkos_ENABLE_BACKEND=ON``, where one needs to replace ``BACKEND``.
+One can activate simultaneously one serial, one parallel CPU host (e.g. "OPENMP", "THREADS") and one parallel GPU device backend (e.g. "HIP", "CUDA"), but not two of any category at the same time.
+For "HIP" and "CUDA", the appropriate software stacks are required to enable compilation and subsequent use.
+Similarly, the CMake option ``-DKokkos_ARCH_{...}=ON`` must also be specified to target a given architecture.
+A list of the architectures is found on the `Kokkos wiki <https://github.com/kokkos/kokkos/wiki/Macros#architectures>`_.
+Note that "THREADS" backend is not recommended since `Kokkos <https://github.com/kokkos/kokkos-core-wiki/blob/17f08a6483937c26e14ec3c93a2aa40e4ce081ce/docs/source/ProgrammingGuide/Initialization.md?plain=1#L67>`_ does not guarantee its safety.
 
 .. installation-end-inclusion-marker-do-not-remove
 
 Testing
 =======
 
 To test with the ROCm stack using a manylinux2014 container we must first mount the repository into the container:
@@ -53,33 +67,33 @@
 
 Next, within the container, we install the ROCm software stack:
 
 .. code-block:: console
 
     yum install -y https://repo.radeon.com/amdgpu-install/21.40.2/rhel/7.9/amdgpu-install-21.40.2.40502-1.el7.noarch.rpm
     amdgpu-install --usecase=hiplibsdk,rocm --no-dkms
-    
+
 We next build the test-suite, with a given AMD GPU target in mind, as listed `here <https://github.com/kokkos/kokkos/blob/master/Makefile.kokkos>`_.
 
 .. code-block:: console
 
     cd /io
-    export PATH=$PATH:/opt/rocm/bin/ 
+    export PATH=$PATH:/opt/rocm/bin/
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/rocm/lib
-    export CXX=/opt/rocm/hip/bin/hipcc 
-    cmake -Bbuild -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=on -DPLKOKKOS_BUILD_TESTS=On -DKokkos_ARCH_VEGA90A=ON
-    cmake --build ./build --verbose
+    export CXX=/opt/rocm/hip/bin/hipcc
+    cmake -B build -DCMAKE_CXX_COMPILER=/opt/rocm/hip/bin/hipcc -DKokkos_ENABLE_HIP=ON -DPLKOKKOS_BUILD_TESTS=ON -DKokkos_ARCH_VEGA90A=ON
+    cmake --build build --verbose
 
-We may now leave the container, and run the built test-suite on a machine with access to the targetted GPU.
+We may now leave the container, and run the built test-suite on a machine with access to the targeted GPU.
 
-For a system with access to the ROCm stack outside of a manylinux container, an editable `pip` installation can be built and installed as:
+For a system with access to the ROCm stack outside of a manylinux container, an editable ``pip`` installation can be built and installed as:
 
 .. code-block:: console
 
-   BACKEND="HIP" ARCH="VEGA90A" python -m pip install -e .
+   CMAKE_ARGS="-DKokkos_ENABLE_HIP=ON -DKokkos_ARCH_VEGA90A=ON" python -m pip install -e .
 
 
 .. support-start-inclusion-marker-do-not-remove
 
 Support
 =======
 
@@ -94,15 +108,15 @@
 .. license-start-inclusion-marker-do-not-remove
 
 
 License
 =======
 
 The PennyLane-Lightning-Kokkos plugin is **free** and **open source**, released under
-the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_. 
+the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_.
 The PennyLane-Lightning-Kokkos plugin makes use of the `Kokkos <https://github.com/kokkos/kokkos>`__ library, which is held to their own respective licenses.
 
 .. license-end-inclusion-marker-do-not-remove
 .. acknowledgements-start-inclusion-marker-do-not-remove
 
 Acknowledgements
 ================
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/__init__.py` & `PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_serialize.py` & `PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/_serialize.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_version.py` & `PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.30.0"
+__version__ = "0.31.0"
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/lightning_kokkos.py` & `PennyLane-Lightning-Kokkos-0.31.0/pennylane_lightning_kokkos/lightning_kokkos.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,23 @@
 interfaces with Kokkos-enabled calculations to run efficiently on different kinds of shared memory
 hardware systems, such as AMD and Nvidia GPUs, or many-core CPUs. 
 """
 from typing import List
 from warnings import warn
 from itertools import product
 
-import re
 import numpy as np
 from pennylane import (
     active_return,
     math,
     QubitDevice,
     BasisState,
     QubitStateVector,
     DeviceError,
     Projector,
-    Hamiltonian,
-    SparseHamiltonian,
     Hermitian,
     Rot,
     QuantumFunctionError,
     QubitStateVector,
 )
 from pennylane_lightning import LightningQubit
 from pennylane.operation import Tensor, Operation
@@ -48,28 +45,20 @@
 tolerance = 1e-10
 
 import pennylane as qml
 from ._version import __version__
 
 try:
     from .lightning_kokkos_qubit_ops import (
-        InitArguments,
+        InitializationSettings,
         LightningKokkos_C128,
         LightningKokkos_C64,
         AdjointJacobianKokkos_C128,
         AdjointJacobianKokkos_C64,
-        NamedObsKokkos_C64,
-        NamedObsKokkos_C128,
-        TensorProdObsKokkos_C64,
-        TensorProdObsKokkos_C128,
-        HamiltonianKokkos_C64,
-        HamiltonianKokkos_C128,
-        SparseHamiltonianKokkos_C64,
-        SparseHamiltonianKokkos_C128,
-        kokkos_config_info,
+        print_configuration,
     )
 
     from ._serialize import _serialize_observables, _serialize_ops
 
     CPP_BINARY_AVAILABLE = True
 except (ImportError, ValueError, PLException) as e:
     warn(str(e), UserWarning)
@@ -79,20 +68,15 @@
 def _kokkos_dtype(dtype):
     if dtype not in [np.complex128, np.complex64]:
         raise ValueError(f"Data type is not supported for state-vector computation: {dtype}")
     return LightningKokkos_C128 if dtype == np.complex128 else LightningKokkos_C64
 
 
 def _kokkos_configuration():
-    config_info = kokkos_config_info()
-    for key in config_info.keys():
-        if "Runtime Configuration" in key:
-            for sub_key, value in config_info[key].items():
-                config_info[key][sub_key] = re.sub("\x00", ":", value)
-    return config_info
+    return print_configuration()
 
 
 allowed_operations = {
     "Identity",
     "BasisState",
     "QubitStateVector",
     "QubitUnitary",
@@ -155,20 +139,20 @@
 
     class LightningKokkos(QubitDevice):
         """PennyLane-Lightning-Kokkos device.
         Args:
             wires (int): the number of wires to initialize the device with
             sync (bool): immediately sync with host-sv after applying operations
             c_dtype: Datatypes for statevector representation. Must be one of ``np.complex64`` or ``np.complex128``.
-            kokkos_args (InitArguments): binding for Kokkos::InitArguments (threading parameters).
+            kokkos_args (InitializationSettings): binding for Kokkos::InitializationSettings (threading parameters).
         """
 
         name = "PennyLane plugin for Kokkos-backed Lightning device"
         short_name = "lightning.kokkos"
-        pennylane_requires = ">=0.26"
+        pennylane_requires = ">=0.30"
         version = __version__
         author = "Xanadu Inc."
         _CPP_BINARY_AVAILABLE = True
         kokkos_config = {}
 
         operations = allowed_operations
         observables = {
@@ -201,18 +185,18 @@
                 r_dtype = np.float64
                 self.use_csingle = False
             else:
                 raise TypeError(f"Unsupported complex Type: {c_dtype}")
             super().__init__(wires, shots=shots, r_dtype=r_dtype, c_dtype=c_dtype)
             if kokkos_args is None:
                 self._kokkos_state = _kokkos_dtype(c_dtype)(self.num_wires)
-            elif isinstance(kokkos_args, InitArguments):
+            elif isinstance(kokkos_args, InitializationSettings):
                 self._kokkos_state = _kokkos_dtype(c_dtype)(self.num_wires, kokkos_args)
             else:
-                raise TypeError("Argument kokkos_args must be of type InitArguments.")
+                raise TypeError("Argument kokkos_args must be of type InitializationSettings.")
             self._sync = sync
 
             if not LightningKokkos.kokkos_config:
                 LightningKokkos.kokkos_config = _kokkos_configuration()
 
         def reset(self):
             super().reset()
@@ -382,15 +366,15 @@
         def apply_kokkos(self, operations, **kwargs):
             # Skip over identity operations instead of performing
             # matrix multiplication with the identity.
             skipped_ops = ["Identity"]
             invert_param = False
 
             for o in operations:
-                if o.base_name in skipped_ops:
+                if str(o.name) in skipped_ops:
                     continue
                 name = o.name
                 if isinstance(o, Adjoint):
                     name = o.base.name
                     invert_param = True
                 method = getattr(self._kokkos_state, name, None)
 
@@ -429,16 +413,15 @@
                 elif isinstance(operations[0], BasisState):
                     self._apply_basis_state_kokkos(operations[0].parameters[0], operations[0].wires)
                     del operations[0]
 
             for operation in operations:
                 if isinstance(operation, (QubitStateVector, BasisState)):
                     raise DeviceError(
-                        "Operation {} cannot be used after other Operations have already been "
-                        "applied on a {} device.".format(operation.name, self.short_name)
+                        f"Operation {operation.name} cannot be used after other Operations have already been applied on a {self.short_name} device."
                     )
 
             self.apply_kokkos(operations)
 
         def generate_samples(self):
             """Generate samples
 
@@ -454,22 +437,22 @@
                 samples = self.sample(observable, shot_range=shot_range, bin_size=bin_size)
                 return np.squeeze(np.var(samples, axis=0))
 
             adjoint_matrix = math.T(math.conj(qml.matrix(observable)))
             sqr_matrix = np.matmul(adjoint_matrix, qml.matrix(observable))
 
             mean = self._kokkos_state.ExpectationValue(
-                [i + "_var" for i in observable.name],
+                [f"{i}_var" for i in observable.name],
                 self.wires.indices(observable.wires),
                 observable.parameters,
                 qml.matrix(observable).ravel(order="C"),
             )
 
             squared_mean = self._kokkos_state.ExpectationValue(
-                [i + "_sqr" for i in observable.name],
+                [f"{i}_sqr" for i in observable.name],
                 self.wires.indices(observable.wires),
                 observable.parameters,
                 sqr_matrix.ravel(order="C"),
             )
 
             return squared_mean - (mean**2)
 
@@ -573,30 +556,32 @@
                 observable.name,
                 self.wires.indices(observable.wires),
                 par,  # observables should not pass parameters, use matrix instead
                 qml.matrix(observable).ravel(order="C"),
             )
 
         @staticmethod
-        def _check_adjdiff_supported_measurements(measurements: List[MeasurementProcess]):
+        def _check_adjdiff_supported_measurements(
+            measurements: List[MeasurementProcess],
+        ):
             """Check whether given list of measurement is supported by adjoint_diff.
             Args:
                 measurements (List[MeasurementProcess]): a list of measurement processes to check.
             Returns:
                 Expectation or State: a common return type of measurements.
             """
-            if len(measurements) == 0:
+            if not measurements:
                 return None
 
             if len(measurements) == 1 and measurements[0].return_type is State:
                 # return State
                 raise QuantumFunctionError("Not supported")
 
             # The return_type of measurement processes must be expectation
-            if not all([m.return_type is Expectation for m in measurements]):
+            if any(m.return_type is not Expectation for m in measurements):
                 raise QuantumFunctionError(
                     "Adjoint differentiation method does not support expectation return type "
                     "mixed with other return types"
                 )
 
             for m in measurements:
                 if not isinstance(m.obs, Tensor):
@@ -605,19 +590,19 @@
                             "Adjoint differentiation method does not support the Projector observable"
                         )
                     if isinstance(m.obs, Hermitian):
                         raise QuantumFunctionError(
                             "LightningKokkos adjoint differentiation method does not currently support the Hermitian observable"
                         )
                 else:
-                    if any([isinstance(o, Projector) for o in m.obs.non_identity_obs]):
+                    if any(isinstance(o, Projector) for o in m.obs.non_identity_obs):
                         raise QuantumFunctionError(
                             "Adjoint differentiation method does not support the Projector observable"
                         )
-                    if any([isinstance(o, Hermitian) for o in m.obs.non_identity_obs]):
+                    if any(isinstance(o, Hermitian) for o in m.obs.non_identity_obs):
                         raise QuantumFunctionError(
                             "LightningKokkos adjoint differentiation method does not currently support the Hermitian observable"
                         )
             return Expectation
 
         @staticmethod
         def _check_adjdiff_supported_operations(operations):
@@ -649,18 +634,17 @@
 
             # Check adjoint diff support
             self._check_adjdiff_supported_operations(tape.operations)
 
             # Initialization of state
             if starting_state is not None:
                 ket = np.ravel(starting_state, order="C")
-            else:
-                if not use_device_state:
-                    self.reset()
-                    self.execute(tape)
+            elif not use_device_state:
+                self.reset()
+                self.execute(tape)
 
             if self.use_csingle:
                 adj = AdjointJacobianKokkos_C64()
                 ket = ket.astype(np.complex64)
             else:
                 adj = AdjointJacobianKokkos_C128()
 
@@ -744,27 +728,28 @@
 
         def _get_diagonalizing_gates(self, circuit: qml.tape.QuantumTape) -> List[Operation]:
             skip_diagonalizing = lambda obs: isinstance(obs, qml.Hamiltonian) or (
                 isinstance(obs, qml.ops.Sum) and obs._pauli_rep is not None
             )
             meas_filtered = list(
                 filter(
-                    lambda m: m.obs is None or not skip_diagonalizing(m.obs), circuit.measurements
+                    lambda m: m.obs is None or not skip_diagonalizing(m.obs),
+                    circuit.measurements,
                 )
             )
             return super()._get_diagonalizing_gates(
                 qml.tape.QuantumScript(measurements=meas_filtered)
             )
 
 else:  # CPP_BINARY_AVAILABLE:
 
     class LightningKokkos(LightningQubit):
         name = "PennyLane plugin for Kokkos-backed Lightning device"
         short_name = "lightning.kokkos"
-        pennylane_requires = ">=0.22"
+        pennylane_requires = ">=0.30"
         version = __version__
         author = "Xanadu Inc."
         _CPP_BINARY_AVAILABLE = False
 
         def __init__(self, wires, *, c_dtype=np.complex128, **kwargs):
             w_msg = """
             !!!#####################################################################################
```

### Comparing `PennyLane-Lightning-Kokkos-0.30.0/setup.py` & `PennyLane-Lightning-Kokkos-0.31.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,25 +33,19 @@
         """
         This class is based upon the build infrastructure of Pennylane-Lightning-Kokkos.
         """
 
         user_options = build_ext.user_options + [
             ("define=", "D", "Define variables for CMake"),
             ("verbosity", "V", "Increase CMake build verbosity"),
-            ("backend=", "B", "Define compiled Kokkos backend"),
-            ("arch=", "A", "Define backend targetted architecture"),
         ]
 
-        backends = {"CUDA", "HIP", "OPENMP", "THREADS", "SERIAL"}
-
         def initialize_options(self):
             super().initialize_options()
             self.define = None
-            self.backend = None
-            self.arch = None
             self.verbosity = ""
 
         def finalize_options(self):
             # Parse the custom CMake options and store them in a new attribute
             defines = [] if self.define is None else self.define.split(";")
             self.cmake_defines = [f"-D{define}" for define in defines]
             if self.verbosity != "":
@@ -61,105 +55,84 @@
 
         def build_extension(self, ext: CMakeExtension):
             extdir = str(Path(self.get_ext_fullpath(ext.name)).parent.absolute())
             debug = int(os.environ.get("DEBUG", 0)) if self.debug is None else self.debug
             cfg = "Debug" if debug else "Release"
             ninja_path = str(shutil.which("ninja"))
 
-            # Set Python_EXECUTABLE instead if you use PYBIND11_FINDPYTHON
             configure_args = [
                 "-DCMAKE_CXX_FLAGS=-fno-lto",
+                "-DKokkos_ENABLE_SERIAL=ON",  # always build serial backend
                 f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extdir}",
-                f"-DPYTHON_EXECUTABLE={sys.executable}",
                 f"-DCMAKE_BUILD_TYPE={cfg}",  # not used on MSVC, but no harm
                 *(self.cmake_defines),
             ]
+            configure_args += (
+                [f"-DPYTHON_EXECUTABLE={sys.executable}"]
+                if platform.system() == "Linux"
+                else [f"-DPython_EXECUTABLE={sys.executable}"]
+            )
 
             if platform.system() == "Windows":
                 configure_args += [
                     "-T clangcl",
                 ]
             else:
                 configure_args += [
                     "-GNinja",
                     f"-DCMAKE_MAKE_PROGRAM={ninja_path}",
                 ]
 
-            build_args = []
-            if os.getenv("BACKEND") and not self.backend:
-                self.backend = os.getenv("BACKEND")
-            if os.getenv("ARCH") and not self.arch:
-                self.arch = os.getenv("ARCH")
-
-            if self.backend:
-                if self.backend in self.backends:
-                    configure_args.append(f"-DKokkos_ENABLE_{self.backend}=ON")
-                else:
-                    raise RuntimeError(f"Unsupported backend: '{self.backend}'")
-                if self.arch:
-                    configure_args.append(f"-DKokkos_ARCH_{self.arch}=ON")
-
             # Add more platform dependent options
-            if platform.system() == "Darwin":
-                # To support ARM64
-                if os.getenv("ARCHS") == "arm64":
-                    configure_args += [
-                        "-DCMAKE_CXX_COMPILER_TARGET=arm64-apple-macos11",
-                        "-DCMAKE_SYSTEM_NAME=Darwin",
-                        "-DCMAKE_SYSTEM_PROCESSOR=ARM64",
-                    ]
-                else:  # X64 arch
-                    if shutil.which("brew"):
-                        llvmpath = (
-                            subprocess.check_output(["brew", "--prefix", "llvm"]).decode().strip()
-                        )
-                    else:
-                        llvmpath = shutil.which("clang++")
-                        llvmpath = Path(llvmpath).parent.parent
-                    configure_args += [
-                        f"-DCMAKE_CXX_COMPILER={llvmpath}/bin/clang++",
-                        f"-DCMAKE_LINKER={llvmpath}/bin/lld",
-                    ]  # Use clang instead of appleclang
-                # Disable OpenMP in M1 Macs
-                configure_args += ["-DKokkos_ENABLE_OPENMP=OFF"]
-            elif platform.system() == "Windows":
+            if platform.system() == "Windows":
                 configure_args += [
                     "-DKokkos_ENABLE_OPENMP=OFF"
                 ]  # only build with Clang under Windows
-            elif platform.system() != "Linux":
+            elif platform.system() not in ["Darwin", "Linux"]:
                 raise RuntimeError(f"Unsupported '{platform.system()}' platform")
-            for var, opt in zip(["CC", "CXX"], ["C", "CXX"]):
-                if os.getenv(var):
-                    tmp = os.getenv(var)
-                    configure_args += [f"-DCMAKE_{opt}_COMPILER={tmp}"]
+
             if not Path(self.build_temp).exists():
                 os.makedirs(self.build_temp)
 
+            if "CMAKE_ARGS" not in os.environ.keys():
+                os.environ["CMAKE_ARGS"] = ""
+
+            subprocess.check_call(
+                ["cmake"]
+                + os.environ["CMAKE_ARGS"].split(" ")
+                + [str(ext.sourcedir)]
+                + configure_args,
+                cwd=self.build_temp,
+                env=os.environ,
+            )
             subprocess.check_call(
-                ["cmake", str(ext.sourcedir)] + configure_args, cwd=self.build_temp
+                ["cmake", "--build", ".", "--verbose"],
+                cwd=self.build_temp,
+                env=os.environ,
             )
-            subprocess.check_call(["cmake", "--build", "."] + build_args, cwd=self.build_temp)
 
 
 with open("pennylane_lightning_kokkos/_version.py") as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 requirements = [
-    "pennylane>=0.28",
+    "pennylane>=0.30",
 ]
 
 info = {
     "name": "PennyLane-Lightning-Kokkos",
     "version": version,
     "maintainer": "Xanadu Inc.",
     "maintainer_email": "software@xanadu.ai",
     "url": "https://github.com/PennyLaneAI/pennylane-lightning-kokkos",
     "license": "Apache License 2.0",
     "packages": find_packages(where="."),
-    "package_data": {"pennylane_lightning_kokkos": ["src/*"]},
+    "package_data": {
+        "pennylane_lightning_kokkos": [os.path.join("src", "*"), os.path.join("src", "**", "*")]
+    },
     "entry_points": {
         "pennylane.plugins": [
             "lightning.kokkos = pennylane_lightning_kokkos:LightningKokkos",
         ],
     },
     "description": "PennyLane-Lightning-Kokkos plugin",
     "long_description": open("README.rst").read(),
```

