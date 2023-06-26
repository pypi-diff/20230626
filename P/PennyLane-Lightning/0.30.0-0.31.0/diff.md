# Comparing `tmp/PennyLane-Lightning-0.30.0.tar.gz` & `tmp/PennyLane-Lightning-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane-Lightning-0.30.0.tar", last modified: Mon May  1 17:21:51 2023, max compression
+gzip compressed data, was "PennyLane-Lightning-0.31.0.tar", last modified: Mon Jun 26 14:08:57 2023, max compression
```

## Comparing `PennyLane-Lightning-0.30.0.tar` & `PennyLane-Lightning-0.31.0.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/LICENSE
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       46 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/MANIFEST.in
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10009 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/PKG-INFO
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10009 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9526 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       73 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/entry_points.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       47 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/requires.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       40 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/top_level.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8829 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/README.rst
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      716 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/__init__.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6972 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/_serialize.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      693 2023-05-01 17:21:46.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/_version.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    38964 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/lightning_qubit.py
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1449 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/CMakeLists.txt
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1034 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6028 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6450 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AlgUtil.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      726 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      862 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10403 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1093 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4893 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6882 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/AllOperations.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11137 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4589 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5702 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    17914 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3978 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4092 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    28627 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/README.md
--rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)      108 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/benchmark_all.sh
--rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)     3853 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    20837 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11906 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.531184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2923 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14641 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Constant.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19322 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2282 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateOperation.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1776 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3191 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19656 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Gates.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      950 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/KernelType.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26198 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9620 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernel.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1068 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1078 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1308 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1791 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      843 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.531184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3438 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3889 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26076 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    27378 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    90687 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    25048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    61514 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2239 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.534517 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4208 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4013 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1456 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1433 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11500 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7384 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12414 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12550 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12070 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11384 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8773 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5210 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5690 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4958 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2961 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3408 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7069 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10159 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7776 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6778 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2678 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3323 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2450 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5139 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3669 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3639 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3864 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4122 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6674 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7335 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5009 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3238 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12798 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1628 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8315 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    22206 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.534517 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4794 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      894 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5090 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      899 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12598 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      830 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3100 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13533 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1066 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2570 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      851 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    21397 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1103 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14331 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14520 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorBase.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5476 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      781 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5924 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      769 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4719 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1730 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Threading.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      405 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/TransitionKernels.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4965 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/TransitionKernels.hpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4494 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      416 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CompareVector.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1083 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2824 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      790 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/README.md
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4291 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestConstant.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15278 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestHelpers.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      380 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestKernels.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15564 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    42963 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24194 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2675 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Bindings.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      947 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5897 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2051 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Error.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7642 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5714 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2528 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    55833 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24510 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)   106877 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3127 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateUtil.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5904 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Internal.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8032 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_KernelMap.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5507 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    39241 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15851 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3273 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15067 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Observables.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12496 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      487 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_RuntimeInfo.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11147 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7625 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2867 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1864 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12910 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Util.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26684 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      153 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/compile_time_tests.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/runner_main.cpp
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2764 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/BitUtil.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      446 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7443 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/ConstantUtil.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5161 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Error.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      276 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Generators.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3318 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/IntegerInterval.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8856 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    31572 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/LinearAlgebra.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7129 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Macros.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5723 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Memory.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4061 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.cpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2095 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2562 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeList.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1874 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeTraits.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13409 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Util.hpp
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       67 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/requirements.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/setup.cfg
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7938 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/setup.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.499112 PennyLane-Lightning-0.31.0/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/LICENSE
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       46 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/MANIFEST.in
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10300 2023-06-26 14:08:57.499112 PennyLane-Lightning-0.31.0/PKG-INFO
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.479112 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10300 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9526 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       73 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/entry_points.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       47 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/requires.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       40 2023-06-26 14:08:57.000000 PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/top_level.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9120 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/README.rst
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.479112 PennyLane-Lightning-0.31.0/pennylane_lightning/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      716 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/__init__.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6972 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/_serialize.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      693 2023-06-26 13:54:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/_version.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    38968 2023-06-26 13:14:18.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/lightning_qubit.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.479112 PennyLane-Lightning-0.31.0/pennylane_lightning/src/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1516 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/CMakeLists.txt
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.479112 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1034 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6028 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6450 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AlgUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      726 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      862 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/JacobianTape.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10403 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/JacobianTape.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1093 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4893 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.482446 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6882 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/AllOperations.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11137 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4589 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5702 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    17914 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3978 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4092 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    28627 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/README.md
+-rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)      108 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/benchmark_all.sh
+-rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)     3853 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.482446 PennyLane-Lightning-0.31.0/pennylane_lightning/src/bindings/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    20837 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/bindings/Bindings.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11906 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/bindings/Bindings.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.482446 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2923 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14641 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/Constant.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19322 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2282 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateOperation.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1776 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3191 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19656 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/Gates.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      950 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/KernelType.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26198 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9620 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernel.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1068 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1078 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1308 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1791 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      843 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.482446 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3438 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3889 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26076 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    27378 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    90687 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    25048 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    61514 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2239 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.489112 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4208 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4013 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1456 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1433 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11500 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7384 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12414 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12550 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12070 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11384 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4048 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8773 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5210 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5690 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4958 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2961 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3408 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7069 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10159 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7776 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6778 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2678 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3323 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2450 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5139 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3669 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3639 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3864 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4122 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6674 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7335 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5009 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3238 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12798 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1628 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8315 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    22218 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.489112 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4794 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      894 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5090 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      899 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12598 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      830 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1048 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3100 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13533 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1066 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2570 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      851 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Measures.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    21397 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Measures.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1103 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Observables.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14325 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Observables.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14520 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorBase.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5476 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      781 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5924 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      769 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4719 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1730 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Threading.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      405 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/TransitionKernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4965 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/TransitionKernels.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.495779 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4494 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      416 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CompareVector.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1083 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CreateAllWires.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2824 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CreateAllWires.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      790 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/README.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4291 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/TestConstant.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15278 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/TestHelpers.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      380 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/TestKernels.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15564 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    42963 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24194 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2675 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Bindings.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      947 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5897 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2051 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Error.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7642 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5714 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2528 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    55833 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24510 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)   106877 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3127 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5904 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Internal.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8032 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_KernelMap.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5507 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    39241 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15851 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Measures.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3273 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15067 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Observables.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12496 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      487 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_RuntimeInfo.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11147 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7625 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2867 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1864 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12910 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Util.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26684 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      153 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/compile_time_tests.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/runner_main.cpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-06-26 14:08:57.499112 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2764 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/BitUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      446 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7443 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/ConstantUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5161 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Error.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      276 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Generators.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3318 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/IntegerInterval.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9418 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    31572 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/LinearAlgebra.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7129 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Macros.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5645 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Memory.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4061 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/RuntimeInfo.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2095 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/RuntimeInfo.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2562 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/TypeList.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1874 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/TypeTraits.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13409 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Util.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       67 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/requirements.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-06-26 14:08:57.499112 PennyLane-Lightning-0.31.0/setup.cfg
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6797 2023-06-26 13:13:45.000000 PennyLane-Lightning-0.31.0/setup.py
```

### Comparing `PennyLane-Lightning-0.30.0/LICENSE` & `PennyLane-Lightning-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/PKG-INFO` & `PennyLane-Lightning-0.31.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning
-Version: 0.30.0
+Version: 0.31.0
 Summary: PennyLane-Lightning plugin
 Home-page: https://github.com/XanaduAI/pennylane-lightning
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -93,21 +93,27 @@
 
 To build PennyLane-Lightning from source you can run
 
 .. code-block:: console
 
     $ pip install pybind11 pennylane-lightning --no-binary :all:
 
-A C++ compiler such as ``g++``, ``clang``, or ``MSVC`` is required. On Debian-based systems, this
-can be installed via ``apt``:
+A C++ compiler such as ``g++``, ``clang++``, or ``MSVC`` is required.
+On Debian-based systems, this can be installed via ``apt``:
 
 .. code-block:: console
 
     $ sudo apt install g++
 
+On MacOS, we recommend using the latest version of ``clang++`` and ``libomp``:
+
+.. code-block:: console
+
+    $ brew install llvm libomp
+
 The `pybind11 <https://pybind11.readthedocs.io/en/stable/>`_ library is also used for binding the
 C++ functionality to Python.
 
 Alternatively, for development and testing, you can install by cloning the repository:
 
 .. code-block:: console
 
@@ -115,31 +121,33 @@
     $ cd pennylane-lightning
     $ pip install -r requirements.txt
     $ pip install -e .
 
 Note that subsequent calls to ``pip install -e .`` will use cached binaries stored in the
 ``build`` folder. Run ``make clean`` if you would like to recompile.
 
-You can also pass ``cmake`` options with ``build_ext``:
+You can also pass ``cmake`` options with ``CMAKE_ARGS`` as follows:
 
 .. code-block:: console
 
-    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_NATIVE=ON"
+    $ CMAKE_ARGS="-DENABLE_OPENMP=OFF -DENABLE_BLAS=OFF -DENABLE_KOKKOS=OFF" pip install -e . -vv
 
-and install the compiled library with
+or with ``build_ext`` and the ``--define`` flag as follows:
 
 .. code-block:: console
 
+    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_BLAS=OFF;ENABLE_KOKKOS=OFF"
     $ python3 setup.py develop
 
 
 GPU support
 -----------
 
-For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_ can be installed by providing the optional ``[gpu]`` tag:
+For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_
+can be installed by providing the optional ``[gpu]`` tag:
 
 .. code-block:: console
 
     $ pip install pennylane-lightning[gpu]
 
 For more information, please refer to the PennyLane Lightning GPU `documentation <https://docs.pennylane.ai/projects/lightning-gpu>`_.
 
@@ -174,26 +182,34 @@
 
 .. code-block:: console
 
     $ mkdir build && cd build
     $ cmake -DBUILD_TESTS=ON -DCMAKE_BUILD_TYPE=Debug ..
     $ make
 
-Other supported options are ``-DENABLE_WARNINGS=ON``,
-``-DENABLE_NATIVE=ON`` (for ``-march=native``),
-``-DENABLE_BLAS=ON``, ``-DENABLE_OPENMP=ON``,
-``-DENABLE_KOKKOS=ON``, and ``-DENABLE_CLANG_TIDY=ON``.
+Other supported options are
+
+- ``-DENABLE_WARNINGS=ON``
+- ``-DENABLE_NATIVE=ON`` (for ``-march=native``)
+- ``-DENABLE_BLAS=ON``
+- ``-DENABLE_OPENMP=ON``
+- ``-DENABLE_KOKKOS=ON``
+- ``-DENABLE_CLANG_TIDY=ON``
 
 Compile on Windows with MSVC
 ----------------------------
 
-You can also compile Pennylane-Lightning on Windows using `Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler. You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment (e.g. using `Anaconda <https://www.anaconda.com/>`_).
+You can also compile Pennylane-Lightning on Windows using
+`Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler.
+You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment
+(e.g. using `Anaconda <https://www.anaconda.com/>`_).
 
 
-We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library. Be sure that ``cmake`` and ``python`` can be called within the prompt.
+We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library.
+Be sure that ``cmake`` and ``python`` can be called within the prompt.
 
 
 .. code-block:: console
 
     $ cmake --version
     $ python --version
```

### Comparing `PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/PKG-INFO` & `PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning
-Version: 0.30.0
+Version: 0.31.0
 Summary: PennyLane-Lightning plugin
 Home-page: https://github.com/XanaduAI/pennylane-lightning
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -93,21 +93,27 @@
 
 To build PennyLane-Lightning from source you can run
 
 .. code-block:: console
 
     $ pip install pybind11 pennylane-lightning --no-binary :all:
 
-A C++ compiler such as ``g++``, ``clang``, or ``MSVC`` is required. On Debian-based systems, this
-can be installed via ``apt``:
+A C++ compiler such as ``g++``, ``clang++``, or ``MSVC`` is required.
+On Debian-based systems, this can be installed via ``apt``:
 
 .. code-block:: console
 
     $ sudo apt install g++
 
+On MacOS, we recommend using the latest version of ``clang++`` and ``libomp``:
+
+.. code-block:: console
+
+    $ brew install llvm libomp
+
 The `pybind11 <https://pybind11.readthedocs.io/en/stable/>`_ library is also used for binding the
 C++ functionality to Python.
 
 Alternatively, for development and testing, you can install by cloning the repository:
 
 .. code-block:: console
 
@@ -115,31 +121,33 @@
     $ cd pennylane-lightning
     $ pip install -r requirements.txt
     $ pip install -e .
 
 Note that subsequent calls to ``pip install -e .`` will use cached binaries stored in the
 ``build`` folder. Run ``make clean`` if you would like to recompile.
 
-You can also pass ``cmake`` options with ``build_ext``:
+You can also pass ``cmake`` options with ``CMAKE_ARGS`` as follows:
 
 .. code-block:: console
 
-    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_NATIVE=ON"
+    $ CMAKE_ARGS="-DENABLE_OPENMP=OFF -DENABLE_BLAS=OFF -DENABLE_KOKKOS=OFF" pip install -e . -vv
 
-and install the compiled library with
+or with ``build_ext`` and the ``--define`` flag as follows:
 
 .. code-block:: console
 
+    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_BLAS=OFF;ENABLE_KOKKOS=OFF"
     $ python3 setup.py develop
 
 
 GPU support
 -----------
 
-For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_ can be installed by providing the optional ``[gpu]`` tag:
+For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_
+can be installed by providing the optional ``[gpu]`` tag:
 
 .. code-block:: console
 
     $ pip install pennylane-lightning[gpu]
 
 For more information, please refer to the PennyLane Lightning GPU `documentation <https://docs.pennylane.ai/projects/lightning-gpu>`_.
 
@@ -174,26 +182,34 @@
 
 .. code-block:: console
 
     $ mkdir build && cd build
     $ cmake -DBUILD_TESTS=ON -DCMAKE_BUILD_TYPE=Debug ..
     $ make
 
-Other supported options are ``-DENABLE_WARNINGS=ON``,
-``-DENABLE_NATIVE=ON`` (for ``-march=native``),
-``-DENABLE_BLAS=ON``, ``-DENABLE_OPENMP=ON``,
-``-DENABLE_KOKKOS=ON``, and ``-DENABLE_CLANG_TIDY=ON``.
+Other supported options are
+
+- ``-DENABLE_WARNINGS=ON``
+- ``-DENABLE_NATIVE=ON`` (for ``-march=native``)
+- ``-DENABLE_BLAS=ON``
+- ``-DENABLE_OPENMP=ON``
+- ``-DENABLE_KOKKOS=ON``
+- ``-DENABLE_CLANG_TIDY=ON``
 
 Compile on Windows with MSVC
 ----------------------------
 
-You can also compile Pennylane-Lightning on Windows using `Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler. You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment (e.g. using `Anaconda <https://www.anaconda.com/>`_).
+You can also compile Pennylane-Lightning on Windows using
+`Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler.
+You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment
+(e.g. using `Anaconda <https://www.anaconda.com/>`_).
 
 
-We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library. Be sure that ``cmake`` and ``python`` can be called within the prompt.
+We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library.
+Be sure that ``cmake`` and ``python`` can be called within the prompt.
 
 
 .. code-block:: console
 
     $ cmake --version
     $ python --version
```

### Comparing `PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/SOURCES.txt` & `PennyLane-Lightning-0.31.0/PennyLane_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/README.rst` & `PennyLane-Lightning-0.31.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -63,21 +63,27 @@
 
 To build PennyLane-Lightning from source you can run
 
 .. code-block:: console
 
     $ pip install pybind11 pennylane-lightning --no-binary :all:
 
-A C++ compiler such as ``g++``, ``clang``, or ``MSVC`` is required. On Debian-based systems, this
-can be installed via ``apt``:
+A C++ compiler such as ``g++``, ``clang++``, or ``MSVC`` is required.
+On Debian-based systems, this can be installed via ``apt``:
 
 .. code-block:: console
 
     $ sudo apt install g++
 
+On MacOS, we recommend using the latest version of ``clang++`` and ``libomp``:
+
+.. code-block:: console
+
+    $ brew install llvm libomp
+
 The `pybind11 <https://pybind11.readthedocs.io/en/stable/>`_ library is also used for binding the
 C++ functionality to Python.
 
 Alternatively, for development and testing, you can install by cloning the repository:
 
 .. code-block:: console
 
@@ -85,31 +91,33 @@
     $ cd pennylane-lightning
     $ pip install -r requirements.txt
     $ pip install -e .
 
 Note that subsequent calls to ``pip install -e .`` will use cached binaries stored in the
 ``build`` folder. Run ``make clean`` if you would like to recompile.
 
-You can also pass ``cmake`` options with ``build_ext``:
+You can also pass ``cmake`` options with ``CMAKE_ARGS`` as follows:
 
 .. code-block:: console
 
-    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_NATIVE=ON"
+    $ CMAKE_ARGS="-DENABLE_OPENMP=OFF -DENABLE_BLAS=OFF -DENABLE_KOKKOS=OFF" pip install -e . -vv
 
-and install the compiled library with
+or with ``build_ext`` and the ``--define`` flag as follows:
 
 .. code-block:: console
 
+    $ python3 setup.py build_ext -i --define="ENABLE_OPENMP=OFF;ENABLE_BLAS=OFF;ENABLE_KOKKOS=OFF"
     $ python3 setup.py develop
 
 
 GPU support
 -----------
 
-For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_ can be installed by providing the optional ``[gpu]`` tag:
+For GPU support, `PennyLane-Lightning-GPU <https://github.com/PennyLaneAI/pennylane-lightning-gpu>`_
+can be installed by providing the optional ``[gpu]`` tag:
 
 .. code-block:: console
 
     $ pip install pennylane-lightning[gpu]
 
 For more information, please refer to the PennyLane Lightning GPU `documentation <https://docs.pennylane.ai/projects/lightning-gpu>`_.
 
@@ -144,26 +152,34 @@
 
 .. code-block:: console
 
     $ mkdir build && cd build
     $ cmake -DBUILD_TESTS=ON -DCMAKE_BUILD_TYPE=Debug ..
     $ make
 
-Other supported options are ``-DENABLE_WARNINGS=ON``,
-``-DENABLE_NATIVE=ON`` (for ``-march=native``),
-``-DENABLE_BLAS=ON``, ``-DENABLE_OPENMP=ON``,
-``-DENABLE_KOKKOS=ON``, and ``-DENABLE_CLANG_TIDY=ON``.
+Other supported options are
+
+- ``-DENABLE_WARNINGS=ON``
+- ``-DENABLE_NATIVE=ON`` (for ``-march=native``)
+- ``-DENABLE_BLAS=ON``
+- ``-DENABLE_OPENMP=ON``
+- ``-DENABLE_KOKKOS=ON``
+- ``-DENABLE_CLANG_TIDY=ON``
 
 Compile on Windows with MSVC
 ----------------------------
 
-You can also compile Pennylane-Lightning on Windows using `Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler. You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment (e.g. using `Anaconda <https://www.anaconda.com/>`_).
+You can also compile Pennylane-Lightning on Windows using
+`Microsoft Visual C++ <https://visualstudio.microsoft.com/vs/features/cplusplus/>`_ compiler.
+You need `cmake <https://cmake.org/download/>`_ and appropriate Python environment
+(e.g. using `Anaconda <https://www.anaconda.com/>`_).
 
 
-We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library. Be sure that ``cmake`` and ``python`` can be called within the prompt.
+We recommend to use ``[x64 (or x86)] Native Tools Command Prompt for VS [version]`` for compiling the library.
+Be sure that ``cmake`` and ``python`` can be called within the prompt.
 
 
 .. code-block:: console
 
     $ cmake --version
     $ python --version
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/__init__.py` & `PennyLane-Lightning-0.31.0/pennylane_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/_serialize.py` & `PennyLane-Lightning-0.31.0/pennylane_lightning/_serialize.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/_version.py` & `PennyLane-Lightning-0.31.0/pennylane_lightning/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
 
-__version__ = "0.30.0"
+__version__ = "0.31.0"
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/lightning_qubit.py` & `PennyLane-Lightning-0.31.0/pennylane_lightning/lightning_qubit.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,22 +162,22 @@
             variances analytically.
         mcmc (bool): Determine whether to use the approximate Markov Chain Monte Carlo sampling method when generating samples.
         kernel_name (str): name of transition kernel. The current version supports two kernels: ``"Local"`` and ``"NonZeroRandom"``.
             The local kernel conducts a bit-flip local transition between states. The local kernel generates a
             random qubit site and then generates a random number to determine the new bit at that qubit site. The ``"NonZeroRandom"`` kernel
             randomly transits between states that have nonzero probability.
         num_burnin (int): number of steps that will be dropped. Increasing this value will
-        result in a closer approximation but increased runtime.
+            result in a closer approximation but increased runtime.
         batch_obs (bool): Determine whether we process observables parallelly when computing the
             jacobian. This value is only relevant when the lightning qubit is built with OpenMP.
     """
 
     name = "Lightning Qubit PennyLane plugin"
     short_name = "lightning.qubit"
-    pennylane_requires = ">=0.26"
+    pennylane_requires = ">=0.30"
     version = __version__
     author = "Xanadu Inc."
     _CPP_BINARY_AVAILABLE = True
     operations = allowed_operations
     observables = allowed_observables
 
     def __init__(
@@ -975,15 +975,15 @@
 
 
 if not CPP_BINARY_AVAILABLE:
 
     class LightningQubit(DefaultQubit):  # pragma: no cover
         name = "Lightning Qubit PennyLane plugin"
         short_name = "lightning.qubit"
-        pennylane_requires = ">=0.26"
+        pennylane_requires = ">=0.30"
         version = __version__
         author = "Xanadu Inc."
         _CPP_BINARY_AVAILABLE = False
 
         def __init__(self, wires, *, c_dtype=np.complex128, **kwargs):
             warn(
                 "Pre-compiled binaries for lightning.qubit are not available. Falling back to "
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     )
 endif()
 
 
 ###############################################################################
 # Process options
 ###############################################################################
+list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/../../cmake")
 include("${PROJECT_SOURCE_DIR}/../../cmake/process_options.cmake")
 
 
 ###############################################################################
 # Include all nested sources directories
 ###############################################################################
 set(COMPONENT_SUBDIRS      algorithms;
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AlgUtil.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/AlgUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/JacobianTape.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/JacobianTape.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/AllOperations.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/AllOperations.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/README.md` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/bindings/Bindings.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/bindings/Bindings.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Constant.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/Constant.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateOperation.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateOperation.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/GateUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Gates.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/Gates.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/KernelType.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/KernelType.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernel.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernel.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -91,30 +91,30 @@
 constexpr auto
 InternalFunctions_Iter([[maybe_unused]] std::index_sequence<rev_wire...> dummy)
     -> decltype(auto) {
     return std::array{&AVXImpl::template applyInternal<rev_wire, ParamT>...};
 }
 
 /**
- * @brief Generate an array of function pointers to ``applyInternal`` functions
- * with different rev_wires.
+ * @brief Generate an array of function pointers to ``applyInternal``
+ * functions with different rev_wires.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gates without parameters
  */
 template <SingleQubitGateWithoutParam AVXImpl>
 constexpr auto InternalFunctions() -> decltype(auto) {
     constexpr size_t internal_wires =
         Util::log2PerfectPower(AVXImpl::packed_size_ / 2);
     return InternalFunctions_Iter<AVXImpl>(
         std::make_index_sequence<internal_wires>());
 }
 
 /**
- * @brief Generate an array of function pointers to ``applyInternal`` functions
- * with different rev_wires.
+ * @brief Generate an array of function pointers to ``applyInternal``
+ * functions with different rev_wires.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gate with a parameter
  */
 template <SingleQubitGateWithParam AVXImpl, typename ParamT>
 constexpr auto InternalFunctions() -> decltype(auto) {
     constexpr size_t internal_wires =
         Util::log2PerfectPower(AVXImpl::packed_size_ / 2);
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
         Util::log2PerfectPower(AVXImpl::packed_size_ / 2);
     return Util::tuple_to_array(std::tuple{
         InternalInternalFunctions_IterTargets<AVXImpl, ParamT, control>(
             std::make_index_sequence<internal_wires>())...});
 }
 /**
  * @brief Generate an array of function pointers
- * to ``applyInternalInternal`` functions with different internal (control and
- * target) wires.
+ * to ``applyInternalInternal`` functions with different internal (control
+ * and target) wires.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gates which are symmetric and
  * with a parameter
  */
 template <TwoQubitGateWithParam AVXImpl, typename ParamT>
 constexpr auto InternalInternalFunctions() {
     constexpr size_t internal_wires =
@@ -202,16 +202,16 @@
     return Util::tuple_to_array(
         std::tuple{InternalInternalFunctions_IterTargets<AVXImpl, control>(
             std::make_index_sequence<internal_wires>())...});
 }
 
 /**
  * @brief Generate an array of function pointers
- * to ``applyInternalInternal`` functions with different internal (control and
- * target) wires.
+ * to ``applyInternalInternal`` functions with different internal (control
+ * and target) wires.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gates which are symmetric and
  * without parameters
  */
 template <TwoQubitGateWithoutParam AVXImpl>
 constexpr auto InternalInternalFunctions() -> decltype(auto) {
     constexpr size_t internal_wires =
@@ -227,17 +227,19 @@
 constexpr auto ExternalInternalFunctions_Iter(
     [[maybe_unused]] std::index_sequence<targets...> dummy) -> decltype(auto) {
     return Util::tuple_to_array(
         std::tuple{&AVXImpl::template applyExternalInternal<targets>...});
 }
 
 /**
- * @brief Generate an array of function pointers to ``applyExternalInternal``
- * functions with different internal (target) wires. Note that
- * ``applyExternalInternal`` functions are only defined for asymmetric gates.
+ * @brief Generate an array of function pointers to
+ * ``applyExternalInternal`` functions with different internal (target)
+ * wires. Note that
+ * ``applyExternalInternal`` functions are only defined for asymmetric
+ * gates.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gates which are symmetric and
  * without parameters
  */
 template <AsymmetricTwoQubitGateWithoutParam AVXImpl>
 constexpr auto ExternalInternalFunctions() -> decltype(auto) {
     constexpr size_t internal_wires =
@@ -253,17 +255,19 @@
 constexpr auto ExternalInternalFunctions_Iter(
     [[maybe_unused]] std::index_sequence<targets...> dummy) -> decltype(auto) {
     return Util::tuple_to_array(std::tuple{
         &AVXImpl::template applyExternalInternal<targets, ParamT>...});
 }
 
 /**
- * @brief Generate an array of function pointers to ``applyExternalInternal``
- * functions with different internal (target) wires. Note that
- * ``applyExternalInternal`` functions are only defined for asymmetric gates.
+ * @brief Generate an array of function pointers to
+ * ``applyExternalInternal`` functions with different internal (target)
+ * wires. Note that
+ * ``applyExternalInternal`` functions are only defined for asymmetric
+ * gates.
  *
  * @tparam AVXImpl Class implementing AVX2/512 gates which are symmetric and
  * with a parameter
  * @tparam ParamT Gate parameter type
  */
 template <AsymmetricTwoQubitGateWithParam AVXImpl, typename ParamT>
 constexpr auto ExternalInternalFunctions() -> decltype(auto) {
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Measures.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Measures.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Observables.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Observables.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 };
 #if defined(_OPENMP)
 template <class T> struct HamiltonianApplyInPlace<T, true> {
     static void run(const std::vector<T> &coeffs,
                     const std::vector<std::shared_ptr<Observable<T>>> &terms,
                     StateVectorManagedCPU<T> &sv) {
         const size_t length = sv.getLength();
-        const auto allocator = sv.allocator();
+        auto allocator = sv.allocator();
 
         std::vector<std::complex<T>, decltype(allocator)> sum(
             length, std::complex<T>{}, allocator);
 
 #pragma omp parallel default(none) firstprivate(length, allocator)             \
     shared(coeffs, terms, sv, sum)
         {
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorBase.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorBase.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Threading.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/Threading.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/TransitionKernels.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/simulator/TransitionKernels.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CMakeLists.txt` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CreateAllWires.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/CreateAllWires.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/README.md` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestConstant.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/TestConstant.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestHelpers.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/TestHelpers.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Error.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Error.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateUtil.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_GateUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Internal.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Internal.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_KernelMap.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_KernelMap.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Measures.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Observables.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Observables.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Util.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_Util.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/BitUtil.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/BitUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/ConstantUtil.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/ConstantUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Error.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Error.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/IntegerInterval.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/IntegerInterval.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,19 @@
                           device_type, Kokkos::MemoryTraits<Kokkos::Unmanaged>>;
 
 template <class fp_precision>
 using const_data_view_type =
     typename Kokkos::View<const data_type<fp_precision> *, default_layout,
                           device_type, Kokkos::MemoryTraits<Kokkos::Unmanaged>>;
 
+namespace {
+std::mutex kokkos_init_mutex;  // NOLINT
+bool kokkos_final_reg = false; // NOLINT
+} // namespace
+
 /**
  * @brief Create a Kokkos Sparse Matrix object with unmanaged views.
  *
  * @param row_map_ptr   Pointer to the row_map array. Elements of this array
  * return the number of non-zero terms in all rows before it.
  * @param numRows       Matrix total number or rows.
  * @param entries_ptr   Pointer to the array with the non-zero elements column
@@ -120,32 +125,46 @@
 template <class fp_precision, class index_type>
 void apply_Sparse_Matrix_Kokkos(
     const std::complex<fp_precision> *vector_ptr, const index_type vector_size,
     const index_type *row_map_ptr, const index_type row_map_size,
     const index_type *entries_ptr, const std::complex<fp_precision> *values_ptr,
     const index_type numNNZ, std::vector<std::complex<fp_precision>> &result) {
 
-    Kokkos::initialize();
+    {
+        const std::lock_guard<std::mutex> lock(kokkos_init_mutex);
+        if (!Kokkos::is_initialized()) {
+            Kokkos::initialize();
+        }
+    } // namespace Pennylane::Util
     {
         const_data_view_type<fp_precision> vector_view(vector_ptr, vector_size);
         result.resize(vector_size);
         data_view_type<fp_precision> result_view(result.data(), vector_size);
 
         const_crs_matrix_type<fp_precision> sparse_matrix =
             create_Kokkos_Sparse_Matrix(row_map_ptr, row_map_size - 1,
                                         entries_ptr, values_ptr, numNNZ);
 
         const data_type<fp_precision> alpha(1.0);
         const data_type<fp_precision> beta;
         KokkosSparse::spmv("N", alpha, sparse_matrix, vector_view, beta,
                            result_view);
     }
-    Kokkos::finalize();
-};
-
+    {
+        const std::lock_guard<std::mutex> lock(kokkos_init_mutex);
+        if (!kokkos_final_reg) {
+            kokkos_final_reg = true;
+            std::atexit([]() {
+                if (!Kokkos::is_finalized()) {
+                    Kokkos::finalize();
+                }
+            });
+        }
+    }
+}
 } // namespace Pennylane::Util
 #else
 constexpr bool USE_KOKKOS = false;
 namespace Pennylane::Util {
 
 /**
  * @brief Apply a sparse matrix to a vector with Kokkos.
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/LinearAlgebra.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/LinearAlgebra.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Macros.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Macros.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Memory.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Memory.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,14 @@
     }
 
     /**
      * @brief Get alignment of the allocator
      */
     [[nodiscard]] inline uint32_t alignment() const { return alignment_; }
 
-    template <class U> struct rebind { using other = AlignedAllocator<U>; };
-
     template <typename U>
     explicit constexpr AlignedAllocator(
         [[maybe_unused]] const AlignedAllocator<U> &rhs) noexcept
         : alignment_{rhs.alignment()} {}
 
     /**
      * @brief Allocate memory with for the given number of datatype T
```

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.cpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/RuntimeInfo.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/RuntimeInfo.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeList.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/TypeList.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeTraits.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/TypeTraits.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Util.hpp` & `PennyLane-Lightning-0.31.0/pennylane_lightning/src/util/Util.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.30.0/setup.py` & `PennyLane-Lightning-0.31.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import platform
-import sys
 import subprocess
 import shutil
+import sys
 from pathlib import Path
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
 
 
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=""):
@@ -33,157 +33,134 @@
     """
 
     user_options = build_ext.user_options + [("define=", "D", "Define variables for CMake")]
 
     def initialize_options(self):
         super().initialize_options()
         self.define = None
+        self.verbosity = ""
 
     def finalize_options(self):
         # Parse the custom CMake options and store them in a new attribute
         defines = [] if self.define is None else self.define.split(";")
         self.cmake_defines = [f"-D{define}" for define in defines]
+        if self.verbosity != "":
+            self.verbosity = "--verbose"
 
         super().finalize_options()
 
     def build_extension(self, ext: CMakeExtension):
         extdir = str(Path(self.get_ext_fullpath(ext.name)).parent.absolute())
-
         debug = int(os.environ.get("DEBUG", 0)) if self.debug is None else self.debug
+        build_type = "Debug" if debug else "RelWithDebInfo"
         ninja_path = str(shutil.which("ninja"))
 
-        # Set Python_EXECUTABLE instead if you use PYBIND11_FINDPYTHON
+        build_args = ["--config", "Debug"] if debug else ["--config", "RelWithDebInfo"]
         configure_args = [
             f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extdir}",
-            f"-DPython_EXECUTABLE={sys.executable}",  # (Windows)
-            f"-DPYTHON_EXECUTABLE={sys.executable}",  # (Ubuntu)
+            f"-DCMAKE_BUILD_TYPE={build_type}",  # not used on MSVC, but no harm
             "-DENABLE_WARNINGS=OFF",  # Ignore warnings
         ]
+        configure_args += (
+            [f"-DPYTHON_EXECUTABLE={sys.executable}"]
+            if platform.system() == "Linux"
+            else [f"-DPython_EXECUTABLE={sys.executable}"]
+        )
 
         if platform.system() == "Windows":
             # As Ninja does not support long path for windows yet:
             #  (https://github.com/ninja-build/ninja/pull/2056)
             configure_args += [
                 "-T clangcl",
             ]
         elif ninja_path:
             configure_args += [
                 "-GNinja",
                 f"-DCMAKE_MAKE_PROGRAM={ninja_path}",
             ]
 
-        build_args = []
-
-        if debug:
-            configure_args += ["-DCMAKE_BUILD_TYPE=Debug"]
-            build_args += ["--config", "Debug"]
-        else:
-            build_args += ["--config", "RelWithDebInfo"]
-
         configure_args += self.cmake_defines
 
         # Add more platform dependent options
         if platform.system() == "Darwin":
-            # To support ARM64
-            if os.getenv("ARCHS") == "arm64":
-                configure_args += [
-                    "-DCMAKE_CXX_COMPILER_TARGET=arm64-apple-macos11",
-                    "-DCMAKE_SYSTEM_NAME=Darwin",
-                    "-DCMAKE_SYSTEM_PROCESSOR=ARM64",
-                    "-DENABLE_OPENMP=OFF",
-                ]
-            else:  # X64 arch
-                # If we explicitly request a brew LLVM version, use that
-                if os.getenv("BREW_LLVM_VERSION") and shutil.which("brew"):
-                    brew_llvm_version = os.getenv("BREW_LLVM_VERSION")
-                    llvmpath = subprocess.run(
-                        [
-                            "brew",
-                            "--prefix",
-                            "llvm" + f"@{brew_llvm_version}" if brew_llvm_version else "",
-                        ],
-                        check=True,
-                        capture_output=True,
-                        text=True,
-                    ).stdout.strip()
-                
-                else:
-                    # No brew, use the default clang++ install provided by MacOS
-                    llvmpath = shutil.which("clang++")
-                    llvmpath = Path(llvmpath).parent.parent
-
-                # Ensure the appropriate compiler and linker are chosen
-                configure_args += [
-                    f"-DCMAKE_CXX_COMPILER={llvmpath}/bin/clang++",
-                    f"-DCMAKE_LINKER={llvmpath}/bin/lld",
-                ]  # Use clang instead of appleclang
-
-                # Try to support OpenMP through libomp if available
-                if os.environ.get("USE_OMP") and shutil.which("brew"):
-                    libomp_path = subprocess.run(
-                        [
-                            "brew",
-                            "--prefix",
-                            "libomp",
-                        ],
-                        check=False,
-                        capture_output=True,
-                        text=True,
-                    ).stdout.strip()
-                    configure_args += (
-                        [f"-DOpenMP_ROOT={libomp_path}/"] if libomp_path else ["-DENABLE_OPENMP=OFF"]
-                    )
+            clang_path = Path(shutil.which("clang++")).parent.parent
+            configure_args += [
+                f"-DCMAKE_CXX_COMPILER={clang_path}/bin/clang++",
+                f"-DCMAKE_LINKER={clang_path}/bin/lld",
+            ]
+            if shutil.which("brew"):
+                libomp_path = subprocess.run(
+                    "brew --prefix libomp".split(" "),
+                    check=False,
+                    capture_output=True,
+                    text=True,
+                ).stdout.strip()
+                if not Path(libomp_path).exists():
+                    libomp_path = ""
+                configure_args += (
+                    [f"-DOpenMP_ROOT={libomp_path}/"] if libomp_path else ["-DENABLE_OPENMP=OFF"]
+                )
         elif platform.system() == "Windows":
             configure_args += ["-DENABLE_OPENMP=OFF", "-DENABLE_BLAS=OFF"]
-        elif platform.system() != "Linux":
+        elif platform.system() not in ["Linux"]:
             raise RuntimeError(f"Unsupported '{platform.system()}' platform")
 
         if not Path(self.build_temp).exists():
             os.makedirs(self.build_temp)
 
-        subprocess.run(
-            ["cmake", str(ext.sourcedir)] + configure_args, cwd=self.build_temp, check=True
+        if "CMAKE_ARGS" in os.environ.keys():
+            configure_args += os.environ["CMAKE_ARGS"].split(" ")
+
+        subprocess.check_call(
+            ["cmake", str(ext.sourcedir)] + configure_args,
+            cwd=self.build_temp,
+            env=os.environ,
         )
-        subprocess.run(
-            ["cmake", "--build", ".", "--verbose"] + build_args, cwd=self.build_temp, check=True
+        subprocess.check_call(
+            ["cmake", "--build", ".", "--verbose"] + build_args,
+            cwd=self.build_temp,
+            env=os.environ,
         )
 
 
 with open(os.path.join("pennylane_lightning", "_version.py")) as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 requirements = [
-    "pennylane>=0.28",
+    "pennylane>=0.30",
 ]
 
 info = {
     "name": "PennyLane-Lightning",
     "version": version,
     "maintainer": "Xanadu Inc.",
     "maintainer_email": "software@xanadu.ai",
     "url": "https://github.com/XanaduAI/pennylane-lightning",
     "license": "Apache License 2.0",
     "packages": find_packages(where="."),
     "package_data": {
-        "pennylane_lightning": [os.path.join("src", "*"), os.path.join("src", "**", "*")]
+        "pennylane_lightning": [
+            os.path.join("src", "*"),
+            os.path.join("src", "**", "*"),
+        ]
     },
     "include_package_data": True,
     "entry_points": {
         "pennylane.plugins": [
             "lightning.qubit = pennylane_lightning:LightningQubit",
         ],
     },
     "description": "PennyLane-Lightning plugin",
     "long_description": open("README.rst").read(),
     "long_description_content_type": "text/x-rst",
     "provides": ["pennylane_lightning"],
     "install_requires": requirements,
-    "ext_modules": [CMakeExtension("lightning_qubit_ops")]
-    if not os.environ.get("SKIP_COMPILATION", False)
-    else [],
+    "ext_modules": []
+    if os.environ.get("SKIP_COMPILATION", False)
+    else [CMakeExtension("lightning_qubit_ops")],
     "cmdclass": {"build_ext": CMakeBuild},
     "ext_package": "pennylane_lightning",
     "extras_require": {"gpu": ["pennylane-lightning-gpu"]},
 }
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

