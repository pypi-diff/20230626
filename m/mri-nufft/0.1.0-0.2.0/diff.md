# Comparing `tmp/mri-nufft-0.1.0.tar.gz` & `tmp/mri-nufft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri-nufft-0.1.0.tar", last modified: Wed Jun  7 15:54:31 2023, max compression
+gzip compressed data, was "mri-nufft-0.2.0.tar", last modified: Mon Jun 26 14:36:26 2023, max compression
```

## Comparing `mri-nufft-0.1.0.tar` & `mri-nufft-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/nufft.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/example_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/example_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mri_nufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mrinufft/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/pynufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/off_resonnance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/trajectories/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/expansions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.378014 mri-nufft-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.362013 mri-nufft-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.366014 mri-nufft-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-26 14:36:26.378014 mri-nufft-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.366014 mri-nufft-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.366014 mri-nufft-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/docs/nufft.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.370014 mri-nufft-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/examples/example_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/examples/example_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:36:26.378014 mri-nufft-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.362013 mri-nufft-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.370014 mri-nufft-0.2.0/src/mri_nufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mri_nufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mri_nufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mri_nufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mri_nufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mri_nufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.370014 mri-nufft-0.2.0/src/mrinufft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 14:36:26.000000 mri-nufft-0.2.0/src/mrinufft/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.370014 mri-nufft-0.2.0/src/mrinufft/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.370014 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.374014 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.374014 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/pynufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/operators/off_resonnance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.374014 mri-nufft-0.2.0/src/mrinufft/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/expansions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/trajectory2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/trajectory3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/src/mrinufft/trajectories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:36:26.378014 mri-nufft-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-26 14:35:52.000000 mri-nufft-0.2.0/tests/test_interface.py
```

### Comparing `mri-nufft-0.1.0/.github/workflows/master-cd.yml` & `mri-nufft-0.2.0/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/.github/workflows/tags-release.yml` & `mri-nufft-0.2.0/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/.github/workflows/test-ci.yml` & `mri-nufft-0.2.0/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/LICENSE.txt` & `mri-nufft-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/README.rst` & `mri-nufft-0.2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -26,48 +26,40 @@
 
 Usage
 =====
 
 .. TODO use a include file directive.
 .. code:: python
 
-      import matplotlib.pyplot as plt
-      from scipy.datasets import face
-
+      from scipy.datasets import face # For demo
+      import numpy as np
       import mrinufft
       from mrinufft.trajectories import display
+      from mrinufft.trajectories.density import voronoi
 
       # Create a 2D Radial trajectory for demo
       samples_loc = mrinufft.initialize_2D_radial(Nc=100, Ns=500)
-      # Get a 2D image for the demo
-      image = face(gray=True)[256:768, 256:768]
+      # Get a 2D image for the demo (512x512)
+      image = np.complex64(face(gray=True)[256:768, 256:768])
 
       ## The real deal starts here ##
       # Choose your NUFFT backend (installed independly from the package)
-      # And create the associated operator.
       NufftOperator = mrinufft.get_operator("finufft")
+
+      # For better image quality we use a density compensation
+      density = voronoi(samples_loc.reshape(-1, 2))
+
+      # And create the associated operator.
       nufft = NufftOperator(
-          samples_loc.reshape(-1, 2), shape=(512, 512), density=True, n_coils=1
+          samples_loc.reshape(-1, 2), shape=image.shape, density=density, n_coils=1
       )
 
       kspace_data = nufft.op(image)  # Image -> Kspace
       image2 = nufft.adj_op(kspace_data)  # Kspace -> Image
 
-      # Show the results
-      fig, ax = plt.subplots(1, 3)
-
-      ax[0].imshow(image)
-      ax[0].set_title("original image")
-      display.display_2D_trajectory(samples_loc, subfigure=ax[1])
-      ax[1].set_aspect("equal")
-      ax[1].set_title("Sampled points in k-space")
-      ax[2].imshow(abs(image2))
-      ax[2].set_title("Auto adjoint image")
-      plt.show()
-
 
 .. TODO Add image
 
 For best image quality, embed these steps in a more complex reconstruction pipeline (for instance using `PySAP <https://github.com/CEA-COSMIC/pysap-mri>`_).
 
 Want to see more ?
```

### Comparing `mri-nufft-0.1.0/docs/Makefile` & `mri-nufft-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/docs/_templates/custom-class-template.rst` & `mri-nufft-0.2.0/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/docs/_templates/custom-module-template.rst` & `mri-nufft-0.2.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/docs/conf.py` & `mri-nufft-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/docs/nufft.rst` & `mri-nufft-0.2.0/docs/nufft.rst`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 The coefficients :math:`B=(b_{m, \ell}) \in \mathbb{C}^{M\times L}` and :math:`C=(c_\ell, n) \in \mathbb{C}^{L\times N}` can be (optimally) estimated for any given :math:`L` by solving the following matrix factorisation problem [3]_:
 
 .. math::
 
    \hat{B}, \hat{C} = \arg\min_{B,C} \| E- BC\|_{fro}^2
 
-Where :math:`E_mn = e^i\Delta\omega_0(u_n}t_m`.
+Where :math:`E_mn = e^i\Delta\omega_0(u_n)t_m`.
 
 
 .. TODO Add Reference to the Code doing this.
 .. TODO Reference for SVI, MTI, MFI and pointers to pysap-mri for their estimation.
 
 
 .. _nufft-algo:
```

### Comparing `mri-nufft-0.1.0/examples/example_readme.py` & `mri-nufft-0.2.0/examples/example_readme.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,44 +6,54 @@
 """
 
 import matplotlib.pyplot as plt
 from scipy.datasets import face
 import numpy as np
 import mrinufft
 from mrinufft.trajectories import display
+from mrinufft.trajectories.density import voronoi
 
 # Create a 2D Radial trajectory for demo
 samples_loc = mrinufft.initialize_2D_radial(Nc=100, Ns=500)
 # Get a 2D image for the demo (512x512)
 image = np.complex64(face(gray=True)[256:768, 256:768])
 
 ## The real deal starts here ##
 # Choose your NUFFT backend (installed independly from the package)
-# And create the associated operator.
 NufftOperator = mrinufft.get_operator("finufft")
+
+# For better image quality we use a density compensation
+density = voronoi(samples_loc.reshape(-1, 2))
+
+# And create the associated operator.
 nufft = NufftOperator(
-    samples_loc.reshape(-1, 2), shape=image.shape, density=True, n_coils=1
+    samples_loc.reshape(-1, 2), shape=image.shape, density=density, n_coils=1
 )
 
 kspace_data = nufft.op(image)  # Image -> Kspace
 image2 = nufft.adj_op(kspace_data)  # Kspace -> Image
 
 # Show the results
-fig, ax = plt.subplots(1, 4)
+fig, ax = plt.subplots(2, 2)
+ax = ax.flatten()
 
 ax[0].imshow(abs(image), cmap="gray")
 ax[0].axis("off")
 ax[0].set_title("original image")
 display.display_2D_trajectory(samples_loc, subfigure=ax[1])
 ax[1].set_aspect("equal")
 ax[1].set_title("Sampled points in k-space")
 ax[2].imshow(abs(image2), cmap="gray")
 ax[2].axis("off")
 ax[2].set_title("Auto adjoint image")
-ax[3].imshow(abs(image2) - abs(image))
+ax[3].imshow(
+    abs(image2) / np.max(abs(image2)) - abs(image) / np.max(abs(image)), cmap="gray"
+)
+ax[3].axis("off")
+ax[3].set_title("Rescaled Error")
 plt.show()
 
 
 # %%
 # .. note::
 # This image is not the same as the original one because the NUFFT operator
 # is not a perfect adjoint, and we undersampled by a factor of 5.
```

### Comparing `mri-nufft-0.1.0/examples/example_trajectories.py` & `mri-nufft-0.2.0/examples/example_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/pyproject.toml` & `mri-nufft-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mri_nufft.egg-info/SOURCES.txt` & `mri-nufft-0.2.0/src/mri_nufft.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/mrinufft/operators/interfaces/gpu/css_colors.py
 src/mrinufft/operators/interfaces/gpu/cufinufft.py
 src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
 src/mrinufft/operators/interfaces/gpu/pynufft.py
 src/mrinufft/operators/interfaces/gpu/tfnufft.py
 src/mrinufft/operators/interfaces/gpu/utils.py
 src/mrinufft/trajectories/__init__.py
+src/mrinufft/trajectories/density.py
 src/mrinufft/trajectories/display.py
 src/mrinufft/trajectories/expansions.py
 src/mrinufft/trajectories/trajectory2D.py
 src/mrinufft/trajectories/trajectory3D.py
 src/mrinufft/trajectories/utils.py
 tests/test_cpu.py
 tests/test_interface.py
```

### Comparing `mri-nufft-0.1.0/src/mrinufft/__init__.py` & `mri-nufft-0.2.0/src/mrinufft/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/__init__.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/base.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/base.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/base.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/css_colors.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/css_colors.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/utils.py` & `mri-nufft-0.2.0/src/mrinufft/operators/interfaces/gpu/utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/operators/off_resonnance.py` & `mri-nufft-0.2.0/src/mrinufft/operators/off_resonnance.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/__init__.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/display.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/display.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/expansions.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/expansions.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory2D.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/trajectory2D.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory3D.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/trajectory3D.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.1.0/src/mrinufft/trajectories/utils.py` & `mri-nufft-0.2.0/src/mrinufft/trajectories/utils.py`

 * *Files identical despite different names*

