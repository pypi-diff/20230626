# Comparing `tmp/v_quantum_annealing-0.0.8.tar.gz` & `tmp/v_quantum_annealing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v_quantum_annealing-0.0.8.tar", last modified: Mon Jun 12 04:05:23 2023, max compression
+gzip compressed data, was "v_quantum_annealing-0.0.9.tar", last modified: Tue Jun 13 08:16:18 2023, max compression
```

## Comparing `v_quantum_annealing-0.0.8.tar` & `v_quantum_annealing-0.0.9.tar`

### file list

```diff
@@ -1,183 +1,209 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:23.131735 v_quantum_annealing-0.0.8/
--rw-rw-rw-   0        0        0     9483 2023-06-10 04:35:48.000000 v_quantum_annealing-0.0.8/CMakeLists.txt
--rw-rw-rw-   0        0        0    11560 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1289 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1278 2023-06-12 04:05:23.131735 v_quantum_annealing-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9339 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:15.682691 v_quantum_annealing-0.0.8/cmake/
--rw-rw-rw-   0        0        0     5390 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/FindGcov.cmake
--rw-rw-rw-   0        0        0    13074 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/FindLcov.cmake
--rw-rw-rw-   0        0        0     9299 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/Findcodecov.cmake
--rw-rw-rw-   0        0        0     4712 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/GenerateDocs.cmake
--rw-rw-rw-   0        0        0     2000 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/PythonAutoDetectOSX.cmake
--rw-rw-rw-   0        0        0     1129 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.8/cmake/llvm-cov-wrapper
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:16.270828 v_quantum_annealing-0.0.8/external/
--rw-rw-rw-   0        0        0     1025 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/external/cimod.cmake
--rw-rw-rw-   0        0        0     1976 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/external/eigen.cmake
--rw-rw-rw-   0        0        0     1043 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.8/external/googletest.cmake
--rw-rw-rw-   0        0        0      781 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/external/json.cmake
--rw-rw-rw-   0        0        0      465 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/external/pybind11-json.cmake
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:16.313713 v_quantum_annealing-0.0.8/include/
--rw-rw-rw-   0        0        0     2243 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:13.487318 v_quantum_annealing-0.0.8/include/v_quantum_annealing/
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:16.611933 v_quantum_annealing-0.0.8/include/v_quantum_annealing/algorithm/
--rw-rw-rw-   0        0        0     3244 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/algorithm/algorithm.hpp
--rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/algorithm/all.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:16.824574 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/
--rw-rw-rw-   0        0        0    45689 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    68880 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
--rw-rw-rw-   0        0        0    42393 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
--rw-rw-rw-   0        0        0     1158 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     2684 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/hash.hpp
--rw-rw-rw-   0        0        0      654 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/json.hpp
--rw-rw-rw-   0        0        0     4884 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/utilities.hpp
--rw-rw-rw-   0        0        0     1624 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/vartypes.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:17.824017 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/
--rw-rw-rw-   0        0        0     1154 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/all.hpp
--rw-rw-rw-   0        0        0     9658 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    15482 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/chimera.hpp
--rw-rw-rw-   0        0        0      899 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/converter.hpp
--rw-rw-rw-   0        0        0     5269 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/csr_sparse.hpp
--rw-rw-rw-   0        0        0     7702 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/dense.hpp
--rw-rw-rw-   0        0        0     2615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/graph.hpp
--rw-rw-rw-   0        0        0     9603 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:17.870211 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/json/
--rw-rw-rw-   0        0        0     4569 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/json/parse.hpp
--rw-rw-rw-   0        0        0    11286 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     8327 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/sparse.hpp
--rw-rw-rw-   0        0        0    10622 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/square.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:17.928005 v_quantum_annealing-0.0.8/include/v_quantum_annealing/result/
--rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/result/all.hpp
--rw-rw-rw-   0        0        0     5217 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/result/get_solution.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:17.944953 v_quantum_annealing-0.0.8/include/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0    10635 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/sampler/sa_sampler.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:18.618121 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/
--rw-rw-rw-   0        0        0     1410 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/all.hpp
--rw-rw-rw-   0        0        0     6308 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     7264 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/classical_ising.hpp
--rw-rw-rw-   0        0        0    21835 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0    15181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/continuous_time_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:19.143827 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:19.356745 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/
--rw-rw-rw-   0        0        0     5615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
--rw-rw-rw-   0        0        0    14615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
--rw-rw-rw-   0        0        0     1750 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
--rw-rw-rw-   0        0        0     2898 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
--rw-rw-rw-   0        0        0    16618 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
--rw-rw-rw-   0        0        0     5502 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0    24738 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/k_local_polynomial.hpp
--rw-rw-rw-   0        0        0      856 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/sa_system.hpp
--rw-rw-rw-   0        0        0     3417 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/system.hpp
--rw-rw-rw-   0        0        0    19954 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/transverse_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:20.166493 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/
--rw-rw-rw-   0        0        0     1089 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/all.hpp
--rw-rw-rw-   0        0        0    19616 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
--rw-rw-rw-   0        0        0     5468 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/gpu.hpp
--rw-rw-rw-   0        0        0     3889 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/k_local.hpp
--rw-rw-rw-   0        0        0    13765 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/single_spin_flip.hpp
--rw-rw-rw-   0        0        0     6522 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:21.123223 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/
--rw-rw-rw-   0        0        0     1055 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/create_geometric_progression.hpp
--rw-rw-rw-   0        0        0     1179 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     5958 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/eigen.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:21.220619 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/fmath/
--rw-rw-rw-   0        0        0    26304 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/fmath/fmath.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:21.498731 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/
--rw-rw-rw-   0        0        0     8427 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/cublas.hpp
--rw-rw-rw-   0        0        0     3061 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/handle_error.hpp
--rw-rw-rw-   0        0        0     2701 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/memory.hpp
--rw-rw-rw-   0        0        0     1102 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/index_type.hpp
--rw-rw-rw-   0        0        0     1337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/insert_or_assign.hpp
--rw-rw-rw-   0        0        0     1118 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/memory.hpp
--rw-rw-rw-   0        0        0     3673 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/pairhash.hpp
--rw-rw-rw-   0        0        0     4054 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/random.hpp
--rw-rw-rw-   0        0        0    10636 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/schedule_list.hpp
--rw-rw-rw-   0        0        0      853 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/thres_hold.hpp
--rw-rw-rw-   0        0        0     2444 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/type_traits.hpp
--rw-rw-rw-   0        0        0     2309 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/union_find.hpp
--rw-rw-rw-   0        0        0     4681 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1578 2023-06-12 04:05:23.134779 v_quantum_annealing-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-06-12 04:04:58.000000 v_quantum_annealing-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.099316 v_quantum_annealing-0.0.8/tests/
--rw-rw-rw-   0        0        0     2064 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0        0 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.152460 v_quantum_annealing-0.0.8/tests/cxxtest/
--rw-rw-rw-   0        0        0     1979 2023-06-10 10:04:30.000000 v_quantum_annealing-0.0.8/tests/cxxtest/cxxtest.cpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.269466 v_quantum_annealing-0.0.8/tests/cxxtest/graph/
--rw-rw-rw-   0        0        0      809 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/graph/all.hpp
--rw-rw-rw-   0        0        0     6134 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0     5917 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-rw-rw-   0        0        0     4663 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/tests/cxxtest/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     7083 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/graph/quadratic.hpp
--rw-rw-rw-   0        0        0    39029 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/polynomial_test.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.292349 v_quantum_annealing-0.0.8/tests/cxxtest/result/
--rw-rw-rw-   0        0        0      700 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/result/all.hpp
--rw-rw-rw-   0        0        0     2777 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/result/result.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.403009 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/
--rw-rw-rw-   0        0        0      891 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/all.hpp
--rw-rw-rw-   0        0        0     2441 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     3200 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/gpu.hpp
--rw-rw-rw-   0        0        0     2429 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     4313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/k_local.hpp
--rw-rw-rw-   0        0        0     5337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/polynomial.hpp
--rw-rw-rw-   0        0        0     6406 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/quadraitc.hpp
--rw-rw-rw-   0        0        0     6808 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.483319 v_quantum_annealing-0.0.8/tests/cxxtest/system/
--rw-rw-rw-   0        0        0      861 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/all.hpp
--rw-rw-rw-   0        0        0     7840 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     1390 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/classical_ising.hpp
--rw-rw-rw-   0        0        0     4090 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0     9332 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     2447 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/system/k_local.hpp
--rw-rw-rw-   0        0        0    15821 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.8/tests/cxxtest/testcase.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:22.539093 v_quantum_annealing-0.0.8/tests/cxxtest/utility/
--rw-rw-rw-   0        0        0      744 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/utility/all.hpp
--rw-rw-rw-   0        0        0     3829 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/utility/eigen.hpp
--rw-rw-rw-   0        0        0     6403 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/utility/gpu.hpp
--rw-rw-rw-   0        0        0     1965 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/cxxtest/utility/union_find.hpp
--rw-rw-rw-   0        0        0    28004 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_cxx.py
--rw-rw-rw-   0        0        0     5754 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_gpu.py
--rw-rw-rw-   0        0        0    60920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_hubo.py
--rw-rw-rw-   0        0        0     6313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_model.py
--rw-rw-rw-   0        0        0    10119 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_sampler.py
--rw-rw-rw-   0        0        0     1181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_sqa.py
--rw-rw-rw-   0        0        0     1973 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:23.067339 v_quantum_annealing-0.0.8/v_quantum_annealing/
--rw-rw-rw-   0        0        0     1086 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/__init__.py
--rw-rw-rw-   0        0        0     2988 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/compile_config.hpp
--rw-rw-rw-   0        0        0    44951 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/declare.hpp
--rw-rw-rw-   0        0        0    15576 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/main.cpp
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:14.643561 v_quantum_annealing-0.0.8/v_quantum_annealing/model/
--rw-rw-rw-   0        0        0      887 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/model/__init__.py
--rw-rw-rw-   0        0        0    14286 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/model/chimera_model.py
--rw-rw-rw-   0        0        0     9035 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/model/king_graph.py
--rw-rw-rw-   0        0        0    23582 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/model/model.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:14.673473 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0      529 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/__init__.py
--rw-rw-rw-   0        0        0     4272 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/base_sa_sample_hubo.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:14.759263 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/
--rw-rw-rw-   0        0        0      320 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
--rw-rw-rw-   0        0        0     5010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-rw-rw-   0        0        0     5847 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-rw-rw-   0        0        0     5240 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/csqa_sampler.py
--rw-rw-rw-   0        0        0     1124 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/response.py
--rw-rw-rw-   0        0        0    25532 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sa_sampler.py
--rw-rw-rw-   0        0        0     8979 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sampler.py
--rw-rw-rw-   0        0        0    12920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sqa_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:14.852971 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/
--rw-rw-rw-   0        0        0      767 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/__init__.py
--rw-rw-rw-   0        0        0    10152 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/benchmark.py
--rw-rw-rw-   0        0        0     1283 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/cxx_cast.py
--rw-rw-rw-   0        0        0      855 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/decorator.py
--rw-rw-rw-   0        0        0      992 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/graph_utils.py
--rw-rw-rw-   0        0        0     2120 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/res_convertor.py
--rw-rw-rw-   0        0        0       36 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/utils/time_measure.py
--rw-rw-rw-   0        0        0     1010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing/variable_type.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:05:23.121756 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-06-12 04:05:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7360 2023-06-12 04:05:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 04:05:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-12 02:10:08.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-06-12 04:05:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-12 04:05:12.000000 v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.725101 v_quantum_annealing-0.0.9/
+-rw-rw-rw-   0        0        0     3438 2023-06-09 05:03:50.000000 v_quantum_annealing-0.0.9/CMakeCache.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.246551 v_quantum_annealing-0.0.9/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.253524 v_quantum_annealing-0.0.9/CMakeFiles/3.26.3/
+-rw-rw-rw-   0        0        0      395 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/CMakeFiles/3.26.3/CMakeSystem.cmake
+-rw-rw-rw-   0        0        0      284 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/CMakeFiles/CMakeConfigureLog.yaml
+-rw-rw-rw-   0        0        0       86 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/CMakeFiles/cmake.check_cache
+-rw-rw-rw-   0        0        0     9483 2023-06-10 04:35:48.000000 v_quantum_annealing-0.0.9/CMakeLists.txt
+-rw-rw-rw-   0        0        0       72 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11560 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1289 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1345 2023-06-13 08:16:18.726098 v_quantum_annealing-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9339 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.259507 v_quantum_annealing-0.0.9/_cmake_test_compile/
+-rw-rw-rw-   0        0        0      486 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/_cmake_test_compile/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.370226 v_quantum_annealing-0.0.9/cmake/
+-rw-rw-rw-   0        0        0     5390 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/FindGcov.cmake
+-rw-rw-rw-   0        0        0    13074 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/FindLcov.cmake
+-rw-rw-rw-   0        0        0     9299 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/Findcodecov.cmake
+-rw-rw-rw-   0        0        0     4712 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/GenerateDocs.cmake
+-rw-rw-rw-   0        0        0     2000 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/PythonAutoDetectOSX.cmake
+-rw-rw-rw-   0        0        0     1129 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/cmake/llvm-cov-wrapper
+-rw-rw-rw-   0        0        0     1257 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.9/doc-requirements.in
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.426061 v_quantum_annealing-0.0.9/external/
+-rw-rw-rw-   0        0        0     1025 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/external/cimod.cmake
+-rw-rw-rw-   0        0        0     1976 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/external/eigen.cmake
+-rw-rw-rw-   0        0        0     1043 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.9/external/googletest.cmake
+-rw-rw-rw-   0        0        0      781 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/external/json.cmake
+-rw-rw-rw-   0        0        0      465 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/external/pybind11-json.cmake
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.437031 v_quantum_annealing-0.0.9/include/
+-rw-rw-rw-   0        0        0     2243 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:16.839628 v_quantum_annealing-0.0.9/include/v_quantum_annealing/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.456978 v_quantum_annealing-0.0.9/include/v_quantum_annealing/algorithm/
+-rw-rw-rw-   0        0        0     3244 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/algorithm/algorithm.hpp
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/algorithm/all.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.534777 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/
+-rw-rw-rw-   0        0        0    45689 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    68880 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
+-rw-rw-rw-   0        0        0    42393 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
+-rw-rw-rw-   0        0        0     1158 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     2684 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/hash.hpp
+-rw-rw-rw-   0        0        0      654 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/json.hpp
+-rw-rw-rw-   0        0        0     4884 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/utilities.hpp
+-rw-rw-rw-   0        0        0     1624 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/vartypes.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.640502 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/
+-rw-rw-rw-   0        0        0     1154 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/all.hpp
+-rw-rw-rw-   0        0        0     9658 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    15482 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/chimera.hpp
+-rw-rw-rw-   0        0        0      899 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/converter.hpp
+-rw-rw-rw-   0        0        0     5269 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/csr_sparse.hpp
+-rw-rw-rw-   0        0        0     7702 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/dense.hpp
+-rw-rw-rw-   0        0        0     2615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/graph.hpp
+-rw-rw-rw-   0        0        0     9603 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.644990 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/json/
+-rw-rw-rw-   0        0        0     4569 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/json/parse.hpp
+-rw-rw-rw-   0        0        0    11286 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     8327 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/sparse.hpp
+-rw-rw-rw-   0        0        0    10622 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/square.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.658959 v_quantum_annealing-0.0.9/include/v_quantum_annealing/result/
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/result/all.hpp
+-rw-rw-rw-   0        0        0     5217 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/result/get_solution.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.663948 v_quantum_annealing-0.0.9/include/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0    10635 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/sampler/sa_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.756690 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/
+-rw-rw-rw-   0        0        0     1410 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/all.hpp
+-rw-rw-rw-   0        0        0     6308 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     7264 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0    21835 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0    15181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/continuous_time_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.772648 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.785612 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/
+-rw-rw-rw-   0        0        0     5615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
+-rw-rw-rw-   0        0        0    14615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
+-rw-rw-rw-   0        0        0     1750 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
+-rw-rw-rw-   0        0        0     2898 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
+-rw-rw-rw-   0        0        0    16618 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
+-rw-rw-rw-   0        0        0     5502 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0    24738 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/k_local_polynomial.hpp
+-rw-rw-rw-   0        0        0      856 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/sa_system.hpp
+-rw-rw-rw-   0        0        0     3417 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/system.hpp
+-rw-rw-rw-   0        0        0    19954 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/transverse_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.823511 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/
+-rw-rw-rw-   0        0        0     1089 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/all.hpp
+-rw-rw-rw-   0        0        0    19616 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
+-rw-rw-rw-   0        0        0     5468 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/gpu.hpp
+-rw-rw-rw-   0        0        0     3889 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/k_local.hpp
+-rw-rw-rw-   0        0        0    13765 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/single_spin_flip.hpp
+-rw-rw-rw-   0        0        0     6522 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.906290 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/
+-rw-rw-rw-   0        0        0     1055 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/create_geometric_progression.hpp
+-rw-rw-rw-   0        0        0     1179 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     5958 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.915277 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/fmath/
+-rw-rw-rw-   0        0        0    26304 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/fmath/fmath.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.939203 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/
+-rw-rw-rw-   0        0        0     8427 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/cublas.hpp
+-rw-rw-rw-   0        0        0     3061 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/handle_error.hpp
+-rw-rw-rw-   0        0        0     2701 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/memory.hpp
+-rw-rw-rw-   0        0        0     1102 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/index_type.hpp
+-rw-rw-rw-   0        0        0     1337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/insert_or_assign.hpp
+-rw-rw-rw-   0        0        0     1118 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/memory.hpp
+-rw-rw-rw-   0        0        0     3673 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/pairhash.hpp
+-rw-rw-rw-   0        0        0     4054 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/random.hpp
+-rw-rw-rw-   0        0        0    10636 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/schedule_list.hpp
+-rw-rw-rw-   0        0        0      853 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/thres_hold.hpp
+-rw-rw-rw-   0        0        0     2444 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/type_traits.hpp
+-rw-rw-rw-   0        0        0     2309 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/union_find.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.991064 v_quantum_annealing-0.0.9/lib/
+-rw-rw-rw-   0        0        0  2675778 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.9/lib/gtest.lib
+-rw-rw-rw-   0        0        0     4654 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.9/lib/gtest_main.lib
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.010013 v_quantum_annealing-0.0.9/myenv/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.058883 v_quantum_annealing-0.0.9/myenv/Scripts/
+-rw-rw-rw-   0        0        0    19880 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/Activate.ps1
+-rw-rw-rw-   0        0        0     1982 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/activate
+-rwxrwxrwx   0        0        0      974 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/activate.bat
+-rwxrwxrwx   0        0        0      368 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/deactivate.bat
+-rw-rw-rw-   0        0        0     1021 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/f2py-script.py
+-rw-rw-rw-   0        0        0     1069 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/Scripts/normalizer-script.py
+-rw-rw-rw-   0        0        0      117 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/myenv/pyvenv.cfg
+-rw-rw-rw-   0        0        0     4689 2023-06-13 04:23:52.000000 v_quantum_annealing-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1612 2023-06-13 08:16:18.730088 v_quantum_annealing-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-06-13 08:15:46.000000 v_quantum_annealing-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.188536 v_quantum_annealing-0.0.9/tests/
+-rw-rw-rw-   0        0        0     2064 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.205491 v_quantum_annealing-0.0.9/tests/cxxtest/
+-rw-rw-rw-   0        0        0     1979 2023-06-10 10:04:30.000000 v_quantum_annealing-0.0.9/tests/cxxtest/cxxtest.cpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.320189 v_quantum_annealing-0.0.9/tests/cxxtest/graph/
+-rw-rw-rw-   0        0        0      809 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/graph/all.hpp
+-rw-rw-rw-   0        0        0     6134 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     5917 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     4663 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/tests/cxxtest/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     7083 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/graph/quadratic.hpp
+-rw-rw-rw-   0        0        0    39029 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/polynomial_test.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.339146 v_quantum_annealing-0.0.9/tests/cxxtest/result/
+-rw-rw-rw-   0        0        0      700 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/result/all.hpp
+-rw-rw-rw-   0        0        0     2777 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/result/result.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.442857 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/
+-rw-rw-rw-   0        0        0      891 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/all.hpp
+-rw-rw-rw-   0        0        0     2441 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     3200 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/gpu.hpp
+-rw-rw-rw-   0        0        0     2429 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     4313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/k_local.hpp
+-rw-rw-rw-   0        0        0     5337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/polynomial.hpp
+-rw-rw-rw-   0        0        0     6406 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/quadraitc.hpp
+-rw-rw-rw-   0        0        0     6808 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.501699 v_quantum_annealing-0.0.9/tests/cxxtest/system/
+-rw-rw-rw-   0        0        0      861 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/all.hpp
+-rw-rw-rw-   0        0        0     7840 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     1390 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0     4090 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0     9332 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     2447 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/system/k_local.hpp
+-rw-rw-rw-   0        0        0    15821 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.9/tests/cxxtest/testcase.hpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.517655 v_quantum_annealing-0.0.9/tests/cxxtest/utility/
+-rw-rw-rw-   0        0        0      744 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/utility/all.hpp
+-rw-rw-rw-   0        0        0     3829 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/utility/eigen.hpp
+-rw-rw-rw-   0        0        0     6403 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/utility/gpu.hpp
+-rw-rw-rw-   0        0        0     1965 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/cxxtest/utility/union_find.hpp
+-rw-rw-rw-   0        0        0    28004 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_cxx.py
+-rw-rw-rw-   0        0        0     5754 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_gpu.py
+-rw-rw-rw-   0        0        0    60920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_hubo.py
+-rw-rw-rw-   0        0        0     6313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_model.py
+-rw-rw-rw-   0        0        0    10119 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_sampler.py
+-rw-rw-rw-   0        0        0     1181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_sqa.py
+-rw-rw-rw-   0        0        0     1973 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.540594 v_quantum_annealing-0.0.9/v_quantum_annealing/
+-rw-rw-rw-   0        0        0     1086 2023-06-13 07:37:49.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.692189 v_quantum_annealing-0.0.9/v_quantum_annealing/__pycache__/
+-rw-rw-rw-   0        0        0     1302 2023-06-13 07:22:24.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1629 2023-06-13 03:43:38.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      215 2023-06-13 08:00:09.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/_version.py
+-rw-rw-rw-   0        0        0     2988 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/compile_config.hpp
+-rw-rw-rw-   0        0        0    44951 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/declare.hpp
+-rw-rw-rw-   0        0        0    15576 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.084973 v_quantum_annealing-0.0.9/v_quantum_annealing/model/
+-rw-rw-rw-   0        0        0      887 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/model/__init__.py
+-rw-rw-rw-   0        0        0    14322 2023-06-12 08:02:22.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/model/chimera_model.py
+-rw-rw-rw-   0        0        0     9035 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/model/king_graph.py
+-rw-rw-rw-   0        0        0    23582 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/model/model.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.168748 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0      529 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/__init__.py
+-rw-rw-rw-   0        0        0     4272 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/base_sa_sample_hubo.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.186700 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/
+-rw-rw-rw-   0        0        0      320 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-rw-rw-   0        0        0     5010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-rw-rw-   0        0        0     5847 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-rw-rw-   0        0        0     5240 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/csqa_sampler.py
+-rw-rw-rw-   0        0        0     1124 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/response.py
+-rw-rw-rw-   0        0        0    25532 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sa_sampler.py
+-rw-rw-rw-   0        0        0     8981 2023-06-12 08:33:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sampler.py
+-rw-rw-rw-   0        0        0    12920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sqa_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:17.235571 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/
+-rw-rw-rw-   0        0        0      767 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10152 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/benchmark.py
+-rw-rw-rw-   0        0        0     1283 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/cxx_cast.py
+-rw-rw-rw-   0        0        0      855 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/decorator.py
+-rw-rw-rw-   0        0        0      992 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/graph_utils.py
+-rw-rw-rw-   0        0        0     2120 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/res_convertor.py
+-rw-rw-rw-   0        0        0       36 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/utils/time_measure.py
+-rw-rw-rw-   0        0        0     1010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.9/v_quantum_annealing/variable_type.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:16:18.645315 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/
+-rw-rw-rw-   0        0        0     1345 2023-06-13 08:16:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7945 2023-06-13 08:16:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:16:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 02:10:08.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-06-13 08:16:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-13 08:16:16.000000 v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/top_level.txt
```

### Comparing `v_quantum_annealing-0.0.8/CMakeLists.txt` & `v_quantum_annealing-0.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/LICENSE` & `v_quantum_annealing-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/MANIFEST.in` & `v_quantum_annealing-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/PKG-INFO` & `v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
-Name: v_quantum_annealing
-Version: 0.0.8
+Name: v-quantum-annealing
+Version: 0.0.9
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
 Project-URL: Reference, https://ref.v_quantum_annealing.org/index.html
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 "file: README.md"
+
```

### Comparing `v_quantum_annealing-0.0.8/README.md` & `v_quantum_annealing-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/FindGcov.cmake` & `v_quantum_annealing-0.0.9/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/FindLcov.cmake` & `v_quantum_annealing-0.0.9/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/Findcodecov.cmake` & `v_quantum_annealing-0.0.9/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/GenerateDocs.cmake` & `v_quantum_annealing-0.0.9/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/PythonAutoDetectOSX.cmake` & `v_quantum_annealing-0.0.9/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/cmake/llvm-cov-wrapper` & `v_quantum_annealing-0.0.9/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/external/cimod.cmake` & `v_quantum_annealing-0.0.9/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/external/eigen.cmake` & `v_quantum_annealing-0.0.9/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/external/googletest.cmake` & `v_quantum_annealing-0.0.9/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/external/json.cmake` & `v_quantum_annealing-0.0.9/external/json.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/CMakeLists.txt` & `v_quantum_annealing-0.0.9/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/algorithm/algorithm.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/algorithm/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/algorithm/all.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/algorithm/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/hash.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/hash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/json.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/json.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/utilities.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/utilities.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/cimod/vartypes.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/cimod/vartypes.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/all.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/chimera.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/chimera.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/converter.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/converter.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/csr_sparse.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/csr_sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/dense.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/dense.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/graph.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/graph.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/json/parse.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/json/parse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/polynomial.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/sparse.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/graph/square.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/graph/square.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/result/all.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/result/get_solution.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/result/get_solution.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/sampler/sa_sampler.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/sampler/sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/all.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/classical_ising.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/continuous_time_ising.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/continuous_time_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/k_local_polynomial.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/k_local_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/sa_system.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/system.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/system/transverse_ising.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/system/transverse_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/all.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/gpu.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/k_local.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/single_spin_flip.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/single_spin_flip.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/updater/swendsen_wang.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/updater/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/create_geometric_progression.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/create_geometric_progression.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/eigen.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/fmath/fmath.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/cublas.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/cublas.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/handle_error.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/handle_error.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/gpu/memory.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/gpu/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/index_type.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/index_type.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/insert_or_assign.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/insert_or_assign.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/memory.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/pairhash.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/pairhash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/random.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/random.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/schedule_list.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/schedule_list.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/thres_hold.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/thres_hold.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/type_traits.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/include/v_quantum_annealing/utility/union_find.hpp` & `v_quantum_annealing-0.0.9/include/v_quantum_annealing/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/pyproject.toml` & `v_quantum_annealing-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 combine_star = true
 combine_straight_imports = true
 group_by_package = true
 auto_identify_namespace_packages = true
 src_paths = ["v_quantum_annealing", "tests"]
 
 [tool.black]
-target-version = ['py39', 'py310']
+target-version = ['py39', 'py310','py311']
 
 [tool.mypy]
 ignore_missing_imports = true
 #show_traceback = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unreachable = true
```

### Comparing `v_quantum_annealing-0.0.8/setup.cfg` & `v_quantum_annealing-0.0.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 00000140: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000150: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000160: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
 00000170: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
 00000180: 204c 4943 454e 5345 0d0a 6c69 6365 6e73   LICENSE..licens
 00000190: 6520 3d20 2241 7061 6368 6520 4c69 6365  e = "Apache Lice
 000001a0: 6e73 6520 322e 3022 0d0a 7665 7273 696f  nse 2.0"..versio
-000001b0: 6e20 3d20 2230 2e30 2e38 220d 0a63 6c61  n = "0.0.8"..cla
+000001b0: 6e20 3d20 2230 2e30 2e39 220d 0a63 6c61  n = "0.0.9"..cla
 000001c0: 7373 6966 6965 7273 203d 200d 0a09 4c69  ssifiers = ...Li
 000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
 000001e0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 000001f0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 00000200: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
 00000210: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
 00000220: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
@@ -43,57 +43,59 @@
 000002a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 000002b0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
 000002c0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
 000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 000002e0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
 000002f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000300: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000310: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
-00000320: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000330: 3a3a 2050 7974 686f 6e20 3a3a 2049 6d70  :: Python :: Imp
-00000340: 6c65 6d65 6e74 6174 696f 6e20 3a3a 2043  lementation :: C
-00000350: 5079 7468 6f6e 0d0a 094f 7065 7261 7469  Python...Operati
-00000360: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
-00000370: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
-00000380: 730d 0a09 4f70 6572 6174 696e 6720 5379  s...Operating Sy
-00000390: 7374 656d 203a 3a20 504f 5349 580d 0a09  stem :: POSIX...
-000003a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000003b0: 203a 3a20 556e 6978 0d0a 094f 7065 7261   :: Unix...Opera
-000003c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-000003d0: 6163 4f53 0d0a 7072 6f6a 6563 745f 7572  acOS..project_ur
-000003e0: 6c73 203d 200d 0a09 536f 7572 6365 3d68  ls = ...Source=h
-000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000400: 6d2f 762d 7175 616e 7475 6d2d 6a73 632f  m/v-quantum-jsc/
-00000410: 562d 5155 414e 5455 4d2d 414e 4e45 414c  V-QUANTUM-ANNEAL
-00000420: 494e 470d 0a09 446f 6375 6d65 6e74 6174  ING...Documentat
-00000430: 696f 6e3d 6874 7470 733a 2f2f 765f 7175  ion=https://v_qu
-00000440: 616e 7475 6d5f 616e 6e65 616c 696e 672e  antum_annealing.
-00000450: 6769 7468 7562 2e69 6f2f 765f 7175 616e  github.io/v_quan
-00000460: 7475 6d5f 616e 6e65 616c 696e 670d 0a09  tum_annealing...
-00000470: 5265 6665 7265 6e63 653d 6874 7470 733a  Reference=https:
-00000480: 2f2f 7265 662e 765f 7175 616e 7475 6d5f  //ref.v_quantum_
-00000490: 616e 6e65 616c 696e 672e 6f72 672f 696e  annealing.org/in
-000004a0: 6465 782e 6874 6d6c 0d0a 0d0a 5b6f 7074  dex.html....[opt
-000004b0: 696f 6e73 5d0d 0a70 7974 686f 6e5f 7265  ions]..python_re
-000004c0: 7175 6972 6573 203d 203e 3d33 2e37 2c20  quires = >=3.7, 
-000004d0: 3c33 2e31 310d 0a69 6e73 7461 6c6c 5f72  <3.11..install_r
-000004e0: 6571 7569 7265 7320 3d20 0d0a 096e 756d  equires = ...num
-000004f0: 7079 203e 3d31 2e31 372e 332c 203c 2031  py >=1.17.3, < 1
-00000500: 2e32 352e 300d 0a09 6469 6d6f 6420 3c20  .25.0...dimod < 
-00000510: 302e 3133 2e30 0d0a 0973 6369 7079 203e  0.13.0...scipy >
-00000520: 3d20 312e 372e 332c 203c 2031 2e31 312e  = 1.7.3, < 1.11.
-00000530: 300d 0a09 7265 7175 6573 7473 203e 3d20  0...requests >= 
-00000540: 322e 3237 2e30 2c20 3c20 322e 3239 2e30  2.27.0, < 2.29.0
-00000550: 0d0a 096a 696a 2d63 696d 6f64 203e 3d20  ...jij-cimod >= 
-00000560: 312e 302e 302c 203c 2031 2e32 2e33 0d0a  1.0.0, < 1.2.3..
-00000570: 0974 7970 696e 672d 6578 7465 6e73 696f  .typing-extensio
-00000580: 6e73 203e 3d20 342e 322e 300d 0a74 6573  ns >= 4.2.0..tes
-00000590: 7473 5f72 6571 7569 7265 203d 200d 0a09  ts_require = ...
-000005a0: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
-000005b0: 6d6f 636b 0d0a 0970 7974 6573 742d 636f  mock...pytest-co
-000005c0: 760d 0a09 7079 7465 7374 2d72 756e 6e65  v...pytest-runne
-000005d0: 720d 0a09 7079 7465 7374 2d72 616e 646f  r...pytest-rando
-000005e0: 6d6c 790d 0a09 7079 7465 7374 2d73 7065  mly...pytest-spe
-000005f0: 630d 0a09 636f 7665 7261 6765 0d0a 0d0a  c...coverage....
-00000600: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000610: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000620: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000310: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000320: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000330: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
+00000340: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
+00000350: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000360: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000370: 7469 6f6e 203a 3a20 4350 7974 686f 6e0d  tion :: CPython.
+00000380: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000390: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
+000003a0: 3a3a 2057 696e 646f 7773 0d0a 094f 7065  :: Windows...Ope
+000003b0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000003c0: 2050 4f53 4958 0d0a 094f 7065 7261 7469   POSIX...Operati
+000003d0: 6e67 2053 7973 7465 6d20 3a3a 2055 6e69  ng System :: Uni
+000003e0: 780d 0a09 4f70 6572 6174 696e 6720 5379  x...Operating Sy
+000003f0: 7374 656d 203a 3a20 4d61 634f 530d 0a70  stem :: MacOS..p
+00000400: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000410: 0953 6f75 7263 653d 6874 7470 733a 2f2f  .Source=https://
+00000420: 6769 7468 7562 2e63 6f6d 2f76 2d71 7561  github.com/v-qua
+00000430: 6e74 756d 2d6a 7363 2f56 2d51 5541 4e54  ntum-jsc/V-QUANT
+00000440: 554d 2d41 4e4e 4541 4c49 4e47 0d0a 0944  UM-ANNEALING...D
+00000450: 6f63 756d 656e 7461 7469 6f6e 3d68 7474  ocumentation=htt
+00000460: 7073 3a2f 2f76 5f71 7561 6e74 756d 5f61  ps://v_quantum_a
+00000470: 6e6e 6561 6c69 6e67 2e67 6974 6875 622e  nnealing.github.
+00000480: 696f 2f76 5f71 7561 6e74 756d 5f61 6e6e  io/v_quantum_ann
+00000490: 6561 6c69 6e67 0d0a 0952 6566 6572 656e  ealing...Referen
+000004a0: 6365 3d68 7474 7073 3a2f 2f72 6566 2e76  ce=https://ref.v
+000004b0: 5f71 7561 6e74 756d 5f61 6e6e 6561 6c69  _quantum_anneali
+000004c0: 6e67 2e6f 7267 2f69 6e64 6578 2e68 746d  ng.org/index.htm
+000004d0: 6c0d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  l....[options]..
+000004e0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+000004f0: 3d20 3e3d 332e 370d 0a69 6e73 7461 6c6c  = >=3.7..install
+00000500: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
+00000510: 756d 7079 203e 3d31 2e31 372e 332c 203c  umpy >=1.17.3, <
+00000520: 2031 2e32 352e 300d 0a09 6469 6d6f 6420   1.25.0...dimod 
+00000530: 3c20 302e 3133 2e30 0d0a 0973 6369 7079  < 0.13.0...scipy
+00000540: 203e 3d20 312e 372e 332c 203c 2031 2e31   >= 1.7.3, < 1.1
+00000550: 312e 300d 0a09 7265 7175 6573 7473 203e  1.0...requests >
+00000560: 3d20 322e 3237 2e30 2c20 3c20 322e 3239  = 2.27.0, < 2.29
+00000570: 2e30 0d0a 096a 696a 2d63 696d 6f64 203e  .0...jij-cimod >
+00000580: 3d20 312e 302e 302c 203c 2031 2e32 2e33  = 1.0.0, < 1.2.3
+00000590: 0d0a 0974 7970 696e 672d 6578 7465 6e73  ...typing-extens
+000005a0: 696f 6e73 203e 3d20 342e 322e 300d 0a74  ions >= 4.2.0..t
+000005b0: 6573 7473 5f72 6571 7569 7265 203d 200d  ests_require = .
+000005c0: 0a09 7079 7465 7374 0d0a 0970 7974 6573  ..pytest...pytes
+000005d0: 742d 6d6f 636b 0d0a 0970 7974 6573 742d  t-mock...pytest-
+000005e0: 636f 760d 0a09 7079 7465 7374 2d72 756e  cov...pytest-run
+000005f0: 6e65 720d 0a09 7079 7465 7374 2d72 616e  ner...pytest-ran
+00000600: 646f 6d6c 790d 0a09 7079 7465 7374 2d73  domly...pytest-s
+00000610: 7065 630d 0a09 636f 7665 7261 6765 0d0a  pec...coverage..
+00000620: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000630: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000640: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `v_quantum_annealing-0.0.8/setup.py` & `v_quantum_annealing-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup_requires = [
     "numpy",
     "pybind11 >=2.10.0, < 2.11.0",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 setup(
     name="v_quantum_annealing", 
     version=__version__,  
     author = "V-QUANTUM JSC",
     author_email = "nqthinh@v-quantum-technology.com",
     setup_requires=setup_requires,
```

### Comparing `v_quantum_annealing-0.0.8/tests/CMakeLists.txt` & `v_quantum_annealing-0.0.9/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/cxxtest.cpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/graph/all.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/graph/polynomial.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/graph/quadratic.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/polynomial_test.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/result/all.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/result/result.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/all.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/gpu.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/k_local.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/polynomial.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/quadraitc.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/sampler/swendsen_wang.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/all.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/classical_ising.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/system/k_local.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/testcase.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/testcase.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/utility/all.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/utility/eigen.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/utility/gpu.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/cxxtest/utility/union_find.hpp` & `v_quantum_annealing-0.0.9/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_cxx.py` & `v_quantum_annealing-0.0.9/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_gpu.py` & `v_quantum_annealing-0.0.9/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_hubo.py` & `v_quantum_annealing-0.0.9/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_model.py` & `v_quantum_annealing-0.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_sampler.py` & `v_quantum_annealing-0.0.9/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_sqa.py` & `v_quantum_annealing-0.0.9/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/tests/test_utils.py` & `v_quantum_annealing-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/__init__.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/compile_config.hpp` & `v_quantum_annealing-0.0.9/v_quantum_annealing/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/declare.hpp` & `v_quantum_annealing-0.0.9/v_quantum_annealing/declare.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/main.cpp` & `v_quantum_annealing-0.0.9/v_quantum_annealing/main.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/model/__init__.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/model/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/model/chimera_model.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/model/chimera_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from dimod import SPIN
+
+import dimod
+# from dimod import SPIN
 
 import v_quantum_annealing.cxxvqa as cj
 
 from v_quantum_annealing.model.model import make_BinaryQuadraticModel
 
 
 def make_ChimeraModel(linear, quadratic):
     """ChimeraModel factory.
 
     Returns:
         generated ChimeraModel class
     """
 
-    class ChimeraModel(make_BinaryQuadraticModel(linear, quadratic)):
+    class ChimeraModel(make_BinaryQuadraticModel(linear, quadratic,False)):
         """Binary quadnratic model dealing with chimera graph This model deal
 
         with chimera graph. ChimeraModel provide methods to verify whether a
         given interaction graph matches a Chimera graph and to convert it to
         cxxvqa.graph.Chimera.
 
         Examples::
@@ -43,15 +45,15 @@
         """
 
         def __init__(
             self,
             linear=None,
             quadratic=None,
             offset=0.0,
-            vartype=SPIN,
+            vartype=dimod.SPIN,
             unit_num_L=None,
             model=None,
             gpu=False,
         ):
             self.gpu = gpu
             if model:
                 super().__init__(
@@ -322,15 +324,15 @@
     return make_ChimeraModel(mock_linear, {})
 
 
 def ChimeraModel(
     linear: dict = None,
     quadratic: dict = None,
     offset: float = 0.0,
-    vartype=SPIN,
+    vartype=dimod.SPIN,
     unit_num_L: int = None,
     model=None,
     gpu: bool = False,
 ):
     """Generate ChimeraModel object
 
     This model deal with chimera graph.
```

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/model/king_graph.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/model/model.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/model/model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/__init__.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/base_sa_sample_hubo.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/csqa_sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/response.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/response.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sa_sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import dimod
 import numpy as np
 
 from cimod.utils import get_state_and_energy
 from dimod import BINARY, SPIN
 from dimod.core.sampler import samplemixinmethod
 
-import v_quantum_annealing
+# import v_quantum_annealing
 import v_quantum_annealing as oj
 import v_quantum_annealing.cxxvqa as cxxvqa
 
 
 def measure_time(func):
     """Decorator for measuring calculation time.
```

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/sampler/sqa_sampler.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/__init__.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/benchmark.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/cxx_cast.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/decorator.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/graph_utils.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/utils/res_convertor.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing/variable_type.py` & `v_quantum_annealing-0.0.9/v_quantum_annealing/variable_type.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/PKG-INFO` & `v_quantum_annealing-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
-Name: v-quantum-annealing
-Version: 0.0.8
+Name: v_quantum_annealing
+Version: 0.0.9
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
 Project-URL: Reference, https://ref.v_quantum_annealing.org/index.html
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 "file: README.md"
+
```

### Comparing `v_quantum_annealing-0.0.8/v_quantum_annealing.egg-info/SOURCES.txt` & `v_quantum_annealing-0.0.9/v_quantum_annealing.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+CMakeCache.txt
 CMakeLists.txt
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+doc-requirements.in
 pyproject.toml
 setup.cfg
 setup.py
 ./v_quantum_annealing/__init__.py
+./v_quantum_annealing/_version.py
 ./v_quantum_annealing/variable_type.py
 ./v_quantum_annealing/model/__init__.py
 ./v_quantum_annealing/model/chimera_model.py
 ./v_quantum_annealing/model/king_graph.py
 ./v_quantum_annealing/model/model.py
 ./v_quantum_annealing/sampler/__init__.py
 ./v_quantum_annealing/sampler/base_sa_sample_hubo.py
@@ -25,14 +29,18 @@
 ./v_quantum_annealing/utils/__init__.py
 ./v_quantum_annealing/utils/benchmark.py
 ./v_quantum_annealing/utils/cxx_cast.py
 ./v_quantum_annealing/utils/decorator.py
 ./v_quantum_annealing/utils/graph_utils.py
 ./v_quantum_annealing/utils/res_convertor.py
 ./v_quantum_annealing/utils/time_measure.py
+CMakeFiles/CMakeConfigureLog.yaml
+CMakeFiles/cmake.check_cache
+CMakeFiles/3.26.3/CMakeSystem.cmake
+_cmake_test_compile/CMakeLists.txt
 cmake/FindGcov.cmake
 cmake/FindLcov.cmake
 cmake/Findcodecov.cmake
 cmake/GenerateDocs.cmake
 cmake/PythonAutoDetectOSX.cmake
 cmake/llvm-cov-wrapper
 external/cimod.cmake
@@ -99,14 +107,23 @@
 include/v_quantum_annealing/utility/thres_hold.hpp
 include/v_quantum_annealing/utility/type_traits.hpp
 include/v_quantum_annealing/utility/union_find.hpp
 include/v_quantum_annealing/utility/fmath/fmath.hpp
 include/v_quantum_annealing/utility/gpu/cublas.hpp
 include/v_quantum_annealing/utility/gpu/handle_error.hpp
 include/v_quantum_annealing/utility/gpu/memory.hpp
+lib/gtest.lib
+lib/gtest_main.lib
+myenv/pyvenv.cfg
+myenv/Scripts/Activate.ps1
+myenv/Scripts/activate
+myenv/Scripts/activate.bat
+myenv/Scripts/deactivate.bat
+myenv/Scripts/f2py-script.py
+myenv/Scripts/normalizer-script.py
 tests/CMakeLists.txt
 tests/__init__.py
 tests/test_cxx.py
 tests/test_gpu.py
 tests/test_hubo.py
 tests/test_model.py
 tests/test_sampler.py
@@ -137,24 +154,27 @@
 tests/cxxtest/system/ising_polynomial_sa_system.hpp
 tests/cxxtest/system/k_local.hpp
 tests/cxxtest/utility/all.hpp
 tests/cxxtest/utility/eigen.hpp
 tests/cxxtest/utility/gpu.hpp
 tests/cxxtest/utility/union_find.hpp
 v_quantum_annealing/__init__.py
+v_quantum_annealing/_version.py
 v_quantum_annealing/compile_config.hpp
 v_quantum_annealing/declare.hpp
 v_quantum_annealing/main.cpp
 v_quantum_annealing/variable_type.py
 v_quantum_annealing.egg-info/PKG-INFO
 v_quantum_annealing.egg-info/SOURCES.txt
 v_quantum_annealing.egg-info/dependency_links.txt
 v_quantum_annealing.egg-info/not-zip-safe
 v_quantum_annealing.egg-info/requires.txt
 v_quantum_annealing.egg-info/top_level.txt
+v_quantum_annealing/__pycache__/__init__.cpython-310.pyc
+v_quantum_annealing/__pycache__/__init__.cpython-311.pyc
 v_quantum_annealing/model/__init__.py
 v_quantum_annealing/model/chimera_model.py
 v_quantum_annealing/model/king_graph.py
 v_quantum_annealing/model/model.py
 v_quantum_annealing/sampler/__init__.py
 v_quantum_annealing/sampler/base_sa_sample_hubo.py
 v_quantum_annealing/sampler/csqa_sampler.py
```

