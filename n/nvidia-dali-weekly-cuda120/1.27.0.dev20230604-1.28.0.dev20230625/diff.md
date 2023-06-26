# Comparing `tmp/nvidia-dali-weekly-cuda120-1.27.0.dev20230604.tar.gz` & `tmp/nvidia-dali-weekly-cuda120-1.28.0.dev20230625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-weekly-cuda120-1.27.0.dev20230604.tar", last modified: Mon Jun  5 07:24:53 2023, max compression
+gzip compressed data, was "nvidia-dali-weekly-cuda120-1.28.0.dev20230625.tar", last modified: Mon Jun 26 13:24:54 2023, max compression
```

## Comparing `nvidia-dali-weekly-cuda120-1.27.0.dev20230604.tar` & `nvidia-dali-weekly-cuda120-1.28.0.dev20230625.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-05 07:24:53.819546 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      458 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       26 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1664 2023-06-05 07:24:53.819546 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      283 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-05 07:24:53.819546 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1664 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      253 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-05 07:24:53.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-05 07:24:53.819546 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-weekly-cuda120-1.27.0.dev20230604/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-26 13:24:54.795267 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      458 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       26 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1664 2023-06-26 13:24:54.795267 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      283 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-26 13:24:54.795267 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1664 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      253 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-26 13:24:54.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-26 13:24:54.795267 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-weekly-cuda120-1.28.0.dev20230625/setup.py
```

### Comparing `nvidia-dali-weekly-cuda120-1.27.0.dev20230604/LICENSE.md` & `nvidia-dali-weekly-cuda120-1.28.0.dev20230625/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-weekly-cuda120-1.27.0.dev20230604/PKG-INFO` & `nvidia-dali-weekly-cuda120-1.28.0.dev20230625/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-weekly-cuda120
-Version: 1.27.0.dev20230604
+Version: 1.28.0.dev20230625
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-weekly-cuda120-1.27.0.dev20230604/nvidia_dali_weekly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-weekly-cuda120-1.28.0.dev20230625/nvidia_dali_weekly_cuda120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-weekly-cuda120
-Version: 1.27.0.dev20230604
+Version: 1.28.0.dev20230625
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-weekly-cuda120-1.27.0.dev20230604/setup.py` & `nvidia-dali-weekly-cuda120-1.28.0.dev20230625/setup.py`

 * *Files identical despite different names*

