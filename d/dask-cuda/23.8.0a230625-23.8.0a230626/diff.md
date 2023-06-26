# Comparing `tmp/dask-cuda-23.8.0a230625.tar.gz` & `tmp/dask-cuda-23.8.0a230626.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.8.0a230625.tar", last modified: Sun Jun 25 05:07:42 2023, max compression
+gzip compressed data, was "dask-cuda-23.8.0a230626.tar", last modified: Mon Jun 26 05:07:41 2023, max compression
```

## Comparing `dask-cuda-23.8.0a230625.tar` & `dask-cuda-23.8.0a230626.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.945844 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15870 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.945844 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.945844 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20056 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    11150 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15940 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23370 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9452 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29398 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.945844 dask-cuda-23.8.0a230625/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-25 05:07:42.000000 dask-cuda-23.8.0a230625/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.941844 dask-cuda-23.8.0a230625/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3251 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 05:07:42.949844 dask-cuda-23.8.0a230625/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-25 05:07:35.000000 dask-cuda-23.8.0a230625/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.398229 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15870 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.398229 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.398229 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20056 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15940 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23370 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29398 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.398229 dask-cuda-23.8.0a230626/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-26 05:07:41.000000 dask-cuda-23.8.0a230626/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.390229 dask-cuda-23.8.0a230626/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 05:07:41.402230 dask-cuda-23.8.0a230626/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-26 05:07:33.000000 dask-cuda-23.8.0a230626/setup.py
```

### Comparing `dask-cuda-23.8.0a230625/LICENSE` & `dask-cuda-23.8.0a230626/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/PKG-INFO` & `dask-cuda-23.8.0a230626/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230625
+Version: 23.8.0a230626
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230625/README.md` & `dask-cuda-23.8.0a230626/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/__init__.py` & `dask-cuda-23.8.0a230626/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/common.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.8.0a230626/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/cli.py` & `dask-cuda-23.8.0a230626/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/cuda_worker.py` & `dask-cuda-23.8.0a230626/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/device_host_file.py` & `dask-cuda-23.8.0a230626/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/disk_io.py` & `dask-cuda-23.8.0a230626/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.8.0a230626/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.8.0a230626/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/initialize.py` & `dask-cuda-23.8.0a230626/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/is_device_object.py` & `dask-cuda-23.8.0a230626/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/is_spillable_object.py` & `dask-cuda-23.8.0a230626/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.8.0a230626/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.8.0a230626/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/proxify_host_file.py` & `dask-cuda-23.8.0a230626/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/proxy_object.py` & `dask-cuda-23.8.0a230626/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_gds.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_spill.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_utils.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.8.0a230626/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/utils.py` & `dask-cuda-23.8.0a230626/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda/worker_spec.py` & `dask-cuda-23.8.0a230626/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.8.0a230626/dask_cuda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230625
+Version: 23.8.0a230626
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230625/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.8.0a230626/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/examples/ucx/client_initialize.py` & `dask-cuda-23.8.0a230626/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.8.0a230626/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/pyproject.toml` & `dask-cuda-23.8.0a230626/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/rtd/conf.py` & `dask-cuda-23.8.0a230626/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230625/setup.py` & `dask-cuda-23.8.0a230626/setup.py`

 * *Files identical despite different names*

