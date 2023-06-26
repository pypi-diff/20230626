# Comparing `tmp/fast-matrix-market-1.7.0.tar.gz` & `tmp/fast-matrix-market-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-matrix-market-1.7.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "fast-matrix-market-1.7.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fast-matrix-market-1.7.0.tar` & `fast-matrix-market-1.7.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/CMakeLists.txt
--rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/LICENSE.txt
--rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/README.md
--rw-r--r--   0        0        0     8422 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/bench_fmm.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/requirements.txt
--rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/run.sh
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/CMakeLists.txt
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Blaze.cmake
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Dragonbox.cmake
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Eigen.cmake
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GoogleBenchmark.cmake
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GoogleTest.cmake
--rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GraphBLAS.cmake
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/fast_float.cmake
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/from_chars_tests.cmake
--rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/to_chars_tests.cmake
--rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/README.md
--rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
--rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
--rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
--rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
--rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
--rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
--rw-r--r--   0        0        0   115829 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
--rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost
--rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/common.h
--rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
--rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
--rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c
--rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
--rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
--rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
--rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
--rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
--rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
--rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h
--rw-r--r--   0        0        0     4017 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
--rw-r--r--   0        0        0    15563 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
--rw-r--r--   0        0        0     2967 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
--rw-r--r--   0        0        0     7211 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
--rw-r--r--   0        0        0    57614 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
--rw-r--r--   0        0        0     4562 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp
--rw-r--r--   0        0        0     4344 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
--rw-r--r--   0        0        0     5854 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
--rw-r--r--   0        0        0     3424 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp
--rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
--rw-r--r--   0        0        0    21988 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
--rw-r--r--   0        0        0    14748 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp
--rw-r--r--   0        0        0    10484 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/header.hpp
--rw-r--r--   0        0        0     9566 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
--rw-r--r--   0        0        0    22808 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp
--rw-r--r--   0        0        0     7373 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
--rw-r--r--   0        0        0    15554 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp
--rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/types.hpp
--rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp
--rw-r--r--   0        0        0     2746 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    17100 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/__init__.py
--rw-r--r--   0        0        0     9584 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core.cpp
--rw-r--r--   0        0        0     9435 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core.hpp
--rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_array.cpp
--rw-r--r--   0        0        0     2599 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_coo.cpp
--rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_array.cpp
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_32.cpp
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_64.cpp
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_32.cpp
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_64.cpp
--rw-r--r--   0        0        0    20198 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/pystreambuf.h
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/eye3.mtx
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longcomplex_array.mtx
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longcomplex_coordinate.mtx
--rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longdouble_array.mtx
--rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longdouble_coordinate.mtx
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_complex_general.mtx
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_integer_general.mtx
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_real_general.mtx
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_complex_general.mtx
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_complex_hermitian.mtx
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_integer_general.mtx
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_pattern_general.mtx
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx.bz2
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx.gz
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_symmetric.mtx
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/misc/windows_newlines.mtx
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/vector_array_real_general.mtx
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
--rw-r--r--   0        0        0     2272 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_array.py
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_basic.py
--rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_coo.py
--rw-r--r--   0        0        0     3903 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_header.py
--rw-r--r--   0        0        0    19343 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_scipy.py
--rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/testsuite_scipy/test_scipy_suite.py
--rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/README.md
+-rw-r--r--   0        0        0     8422 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/benchmark/bench_fmm.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/benchmark/requirements.txt
+-rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/benchmark/run.sh
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/CMakeLists.txt
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/Blaze.cmake
+-rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/Dragonbox.cmake
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/Eigen.cmake
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/GoogleBenchmark.cmake
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/GoogleTest.cmake
+-rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/GraphBLAS.cmake
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/fast_float.cmake
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/from_chars_tests.cmake
+-rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/cmake/to_chars_tests.cmake
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/README.md
+-rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
+-rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
+-rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
+-rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
+-rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
+-rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
+-rw-r--r--   0        0        0   115829 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
+-rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost
+-rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/common.h
+-rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
+-rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
+-rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c
+-rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
+-rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
+-rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
+-rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
+-rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
+-rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h
+-rw-r--r--   0        0        0     4017 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
+-rw-r--r--   0        0        0    15563 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
+-rw-r--r--   0        0        0     2967 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
+-rw-r--r--   0        0        0     7211 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
+-rw-r--r--   0        0        0    57614 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
+-rw-r--r--   0        0        0     4562 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp
+-rw-r--r--   0        0        0     4344 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
+-rw-r--r--   0        0        0     5854 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
+-rw-r--r--   0        0        0     3424 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp
+-rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
+-rw-r--r--   0        0        0    21988 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
+-rw-r--r--   0        0        0    14748 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp
+-rw-r--r--   0        0        0    10484 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/header.hpp
+-rw-r--r--   0        0        0     9566 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
+-rw-r--r--   0        0        0    22808 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp
+-rw-r--r--   0        0        0     7373 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
+-rw-r--r--   0        0        0    15554 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp
+-rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/types.hpp
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp
+-rw-r--r--   0        0        0     2746 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    18271 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/__init__.py
+-rw-r--r--   0        0        0     9614 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core.cpp
+-rw-r--r--   0        0        0    10063 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core.hpp
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_read_array.cpp
+-rw-r--r--   0        0        0     2619 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_read_coo.cpp
+-rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_array.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_coo_32.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_coo_64.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_csc_32.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_csc_64.cpp
+-rw-r--r--   0        0        0    20198 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/src/fast_matrix_market/pystreambuf.h
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/eye3.mtx
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/long_double/longcomplex_array.mtx
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/long_double/longcomplex_coordinate.mtx
+-rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/long_double/longdouble_array.mtx
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/long_double/longdouble_coordinate.mtx
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_array_complex_general.mtx
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_array_integer_general.mtx
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_array_real_general.mtx
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_complex_general.mtx
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_complex_hermitian.mtx
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_integer_general.mtx
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_pattern_general.mtx
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_real_general.mtx
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_real_general.mtx.bz2
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_real_general.mtx.gz
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/matrix_coordinate_real_symmetric.mtx
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/misc/windows_newlines.mtx
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/scipy_crashes/vector_array_real_general.mtx
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
+-rw-r--r--   0        0        0     2272 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/test_array.py
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/test_basic.py
+-rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/test_coo.py
+-rw-r--r--   0        0        0     3903 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/test_header.py
+-rw-r--r--   0        0        0    19343 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/tests/test_scipy.py
+-rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/testsuite_scipy/test_scipy_suite.py
+-rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.1/PKG-INFO
```

### Comparing `fast-matrix-market-1.7.0/CMakeLists.txt` & `fast-matrix-market-1.7.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/LICENSE.txt` & `fast-matrix-market-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/README.md` & `fast-matrix-market-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/benchmark/bench_fmm.py` & `fast-matrix-market-1.7.1/benchmark/bench_fmm.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/benchmark/run.sh` & `fast-matrix-market-1.7.1/benchmark/run.sh`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/CMakeLists.txt` & `fast-matrix-market-1.7.1/fast_matrix_market/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/cmake/GraphBLAS.cmake` & `fast-matrix-market-1.7.1/fast_matrix_market/cmake/GraphBLAS.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/cmake/from_chars_tests.cmake` & `fast-matrix-market-1.7.1/fast_matrix_market/cmake/from_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/cmake/to_chars_tests.cmake` & `fast-matrix-market-1.7.1/fast_matrix_market/cmake/to_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/README.md` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/common.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/common.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h` & `fast-matrix-market-1.7.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 namespace fast_matrix_market {
 
     // Version macros.
     // Keep in sync with python/pyproject.toml
 #define FAST_MATRIX_MARKET_VERSION_MAJOR 1
 #define FAST_MATRIX_MARKET_VERSION_MINOR 7
-#define FAST_MATRIX_MARKET_VERSION_PATCH 0
+#define FAST_MATRIX_MARKET_VERSION_PATCH 1
 
     constexpr std::string_view kSpace = " ";
     constexpr std::string_view kNewline = "\n";
 
     template<class T> struct is_complex : std::false_type {};
     template<class T> struct is_complex<std::complex<T>> : std::true_type {};
```

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/header.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/header.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/types.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/types.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp` & `fast-matrix-market-1.7.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/pyproject.toml` & `fast-matrix-market-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "fast_matrix_market"
-version = "1.7.0"
+version = "1.7.1"
 description="Fast and full-featured Matrix Market file I/O"
 readme = "README.md"
 authors = [
     { name = "Adam Lugowski"},
 ]
 requires-python = ">=3.7"
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/__init__.py` & `fast-matrix-market-1.7.1/src/fast_matrix_market/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,18 @@
 def read_header(source) -> header:
     """
     Read a Matrix Market header from a file or open file-like object.
 
     :param source: filename or open file-like object
     :return: parsed header object
     """
-    return _get_read_cursor(source, 1).header
+    cursor = _get_read_cursor(source, 1)
+    h = cursor.header
+    cursor.close()
+    return h
 
 
 def write_header(target, h: header):
     """
     Write a Matrix Market header to a file or open file-like object.
 
     :param target: filename or open file-like object.
@@ -374,15 +377,15 @@
     else:
         from scipy.sparse import coo_matrix
         triplet, shape = _read_body_coo(cursor, long_type=long_type, generalize_symmetry=True)
         return coo_matrix(triplet, shape=shape)
 
 
 def mmwrite(target, a, comment=None, field=None, precision=None, symmetry="AUTO",
-                parallelism=None, find_symmetry=False):
+            parallelism=None, find_symmetry=False):
     """
     Write a matrix to a MatrixMarket file or file-like object.
 
     Interchangeable with scipy.io.mmwrite() but faster.
 
     :param target: path to MatrixMarket file or open file-like object
     :param a: a 2D ndarray (or an array convertible to one) or a scipy.sparse matrix
@@ -421,38 +424,69 @@
 
     if isinstance(a, np.ndarray):
         # Write dense numpy arrays
         a = _apply_field(a, field, no_pattern=True)
         _core.write_body_array(cursor, a)
         return
 
-    if scipy.sparse.isspmatrix(a):
+    # handle both scipy.sparse.*_matrix and scipy.sparse.*_array
+    # Both have the same interface as far as this method is concerned, so let duck typing do its thing.
+    # Support for these types varies between scipy versions, so attempt to support all possibilities.
+    is_sparse = False
+    is_compressed = False
+    coo_type = None
+    csr_types = []
+
+    # check for *_matrix
+    try:
+        if scipy.sparse.isspmatrix(a):
+            is_sparse = True
+            from scipy.sparse import coo_matrix
+            coo_type = coo_matrix
+            # CSC and CSR have specialized writers.
+            is_compressed = (isinstance(a, scipy.sparse.csc_matrix) or isinstance(a, scipy.sparse.csr_matrix))
+            csr_types.append(scipy.sparse.csr_matrix)
+    except ImportError:
+        pass
+
+    # check for *_array
+    try:
+        if scipy.sparse.issparse(a):
+            is_sparse = True
+            from scipy.sparse import coo_array
+            coo_type = coo_array
+            # CSC and CSR have specialized writers. The type may already be a cs*_matrix.
+            is_compressed = is_compressed or \
+                            (isinstance(a, scipy.sparse.csc_array) or isinstance(a, scipy.sparse.csr_array))
+            csr_types.append(scipy.sparse.csr_array)
+    except ImportError:
+        pass
+
+    if is_sparse:
         # Write sparse scipy matrices
         if symmetry is not None and symmetry != "general":
             # A symmetric matrix only specifies the elements below the diagonal.
             # Ensure that the matrix satisfies this requirement.
-            from scipy.sparse import coo_matrix
+
             a = a.tocoo()
             lower_triangle_mask = a.row >= a.col
-            a = coo_matrix((a.data[lower_triangle_mask],
-                            (a.row[lower_triangle_mask],
-                             a.col[lower_triangle_mask])), shape=a.shape)
-
-        # CSC and CSR have specialized writers.
-        is_compressed = (isinstance(a, scipy.sparse.csc_matrix) or isinstance(a, scipy.sparse.csr_matrix))
+            a = coo_type((a.data[lower_triangle_mask],
+                          (a.row[lower_triangle_mask],
+                           a.col[lower_triangle_mask])), shape=a.shape)
+            is_compressed = False
 
         if not is_compressed:
             # convert everything except CSC/CSR to coo
             a = a.tocoo()
 
         data = _apply_field(a.data, field)
 
         if is_compressed:
             # CSC and CSR can be written directly
-            is_csr = isinstance(a, scipy.sparse.csr_matrix)
+            is_csr = any([isinstance(a, t) for t in csr_types])
             _core.write_body_csc(cursor, a.shape, a.indptr, a.indices, data, is_csr)
         else:
             _core.write_body_coo(cursor, a.shape, a.row, a.col, data)
         return
 
     raise ValueError("unknown matrix type: %s" % type(a))
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     cursor.header = header;
     return cursor;
 }
 
 #ifndef FMM_SCIPY_PRUNE
 void write_header_only(write_cursor& cursor) {
     fmm::write_header(cursor.stream(), cursor.header, cursor.options);
-    cursor.stream().flush();
+    cursor.close();
 }
 #endif
 
 ////////////////////////////////////////////////
 //// pybind11 module definition
 //// Define the _core module here, it is used by __init__.py
 ////////////////////////////////////////////////
@@ -221,15 +221,16 @@
 
 #ifndef FMM_SCIPY_PRUNE
     m.def("write_header_only", &write_header_only);
 #endif
     ///////////////////////////////
     // Read methods
     py::class_<read_cursor>(m, "_read_cursor")
-    .def_readonly("header", &read_cursor::header);
+    .def_readonly("header", &read_cursor::header)
+    .def("close", &read_cursor::close);
 
     m.def("open_read_file", &open_read_file);
     m.def("open_read_stream", &open_read_stream);
 
     init_read_array(m);
     init_read_coo(m);
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core.hpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 
     fmm::matrix_market_header header{};
     fmm::read_options options{};
 
     std::istream& stream() {
         return *stream_ptr;
     }
+
+    /**
+     * Finish using the cursor. If a file has been opened it will be closed.
+     */
+    void close() {
+        // Remove this reference to the stream.
+        // If stream is a std::ofstream() then this is the only reference and the file is closed.
+        stream_ptr.reset();
+    }
 };
 
 /**
  * A structure that represents an open MatrixMarket file or stream (for writing)
  */
 struct write_cursor {
     /**
@@ -73,14 +82,25 @@
 
     fmm::matrix_market_header header{};
     fmm::write_options options{};
 
     std::ostream& stream() {
         return *stream_ptr;
     }
+
+    /**
+     * Finish using the cursor. Flush the backing stream, and if a file has been opened it will be closed.
+     */
+    void close() {
+        stream_ptr->flush();
+
+        // Remove this reference to the stream.
+        // If stream is a std::ofstream() then this is the only reference and the file is closed.
+        stream_ptr.reset();
+    }
 };
 
 /**
  * An iterator adapter over py::array_t numpy arrays.
  *
  * This allows using the iterator-based fast_matrix_market methods.
  */
@@ -157,15 +177,15 @@
                                             py_array_iterator<decltype(rows_unchecked), IT>(rows_unchecked),
                                             py_array_iterator<decltype(rows_unchecked), IT>(rows_unchecked, rows_unchecked.size()),
                                             py_array_iterator<decltype(cols_unchecked), IT>(cols_unchecked),
                                             py_array_iterator<decltype(cols_unchecked), IT>(cols_unchecked, cols_unchecked.size()),
                                             py_array_iterator<decltype(data_unchecked), VT>(data_unchecked),
                                             py_array_iterator<decltype(data_unchecked), VT>(data_unchecked, data_unchecked.size()));
     fmm::write_body(cursor.stream(), formatter, cursor.options);
-    cursor.stream().flush();
+    cursor.close();
 }
 
 #ifndef FMM_SCIPY_PRUNE
 /**
  * Write Python CSC/CSR to MatrixMarket.
  */
 template <typename IT, typename VT>
@@ -201,15 +221,15 @@
                                         py_array_iterator<decltype(indptr_unchecked), IT>(indptr_unchecked, indptr_unchecked.size() - 1),
                                         py_array_iterator<decltype(indices_unchecked), IT>(indices_unchecked),
                                         py_array_iterator<decltype(indices_unchecked), IT>(indices_unchecked, indices_unchecked.size()),
                                         py_array_iterator<decltype(data_unchecked), VT>(data_unchecked),
                                         py_array_iterator<decltype(data_unchecked), VT>(data_unchecked, data_unchecked.size()),
                                         is_csr);
     fmm::write_body(cursor.stream(), formatter, cursor.options);
-    cursor.stream().flush();
+    cursor.close();
 }
 #endif
 
 void init_read_array(py::module_ &);
 void init_write_array(py::module_ &);
 void init_read_coo(py::module_ &);
 void init_write_coo_32(py::module_ &);
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_array.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_read_array.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     // The mmread() will only call this method if the matrix is an array. Disable the code paths for reading
     // coordinate matrices here to reduce final library size and compilation time.
 #ifdef FMM_SCIPY_PRUNE
     fmm::read_matrix_market_body<decltype(handler), fmm::compile_array_only>(cursor.stream(), cursor.header, handler, 1, cursor.options);
 #else
     fmm::read_matrix_market_body<decltype(handler), fmm::compile_all>(cursor.stream(), cursor.header, handler, 1, cursor.options);
 #endif
+    cursor.close();
 }
 
 
 void init_read_array(py::module_ &m) {
     m.def("read_body_array", &read_body_array<int64_t>);
     m.def("read_body_array", &read_body_array<uint64_t>);
     m.def("read_body_array", &read_body_array<double>);
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_coo.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_read_coo.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     // The mmread() will only call this method if the matrix is a coordinate. Disable the code paths for reading
     // array matrices here to reduce final library size and compilation time.
 #ifdef FMM_SCIPY_PRUNE
     fmm::read_matrix_market_body<decltype(handler), fmm::compile_coordinate_only>(cursor.stream(), cursor.header, handler, 1, cursor.options);
 #else
     fmm::read_matrix_market_body<decltype(handler), fmm::compile_all>(cursor.stream(), cursor.header, handler, 1, cursor.options);
 #endif
+    cursor.close();
 }
 
 
 void init_read_coo(py::module_ &m) {
     m.def("read_body_coo", &read_body_coo<int32_t, int64_t>);
     m.def("read_body_coo", &read_body_coo<int32_t, uint64_t>);
     m.def("read_body_coo", &read_body_coo<int32_t, double>);
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_array.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_array.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     fmm::write_header(cursor.stream(), cursor.header, cursor.options);
 
     auto unchecked = array.unchecked();
     fmm::line_formatter<int64_t, T> lf(cursor.header, cursor.options);
     auto formatter = fmm::dense_2d_call_formatter<decltype(lf), decltype(unchecked), int64_t>(
         lf, unchecked, cursor.header.nrows, cursor.header.ncols);
     fmm::write_body(cursor.stream(), formatter, cursor.options);
-    cursor.stream().flush();
+    cursor.close();
 }
 
 
 void init_write_array(py::module_ &m) {
     m.def("write_body_array", &write_body_array<int32_t>);
     m.def("write_body_array", &write_body_array<uint32_t>);
     m.def("write_body_array", &write_body_array<int64_t>);
```

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_32.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_coo_32.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_64.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_coo_64.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_32.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_csc_32.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_64.cpp` & `fast-matrix-market-1.7.1/src/fast_matrix_market/_core_write_csc_64.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/src/fast_matrix_market/pystreambuf.h` & `fast-matrix-market-1.7.1/src/fast_matrix_market/pystreambuf.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/tests/test_array.py` & `fast-matrix-market-1.7.1/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/tests/test_coo.py` & `fast-matrix-market-1.7.1/tests/test_coo.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/tests/test_header.py` & `fast-matrix-market-1.7.1/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/tests/test_scipy.py` & `fast-matrix-market-1.7.1/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/testsuite_scipy/test_scipy_suite.py` & `fast-matrix-market-1.7.1/testsuite_scipy/test_scipy_suite.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.7.0/PKG-INFO` & `fast-matrix-market-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-matrix-market
-Version: 1.7.0
+Version: 1.7.1
 Summary: Fast and full-featured Matrix Market file I/O
 Home-page: https://github.com/alugowski/fast_matrix_market
 Author: Adam Lugowski
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

