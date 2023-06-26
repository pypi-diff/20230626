# Comparing `tmp/scikit-rt-0.4.9.tar.gz` & `tmp/scikit-rt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.4.9.tar", last modified: Wed May 31 09:23:05 2023, max compression
+gzip compressed data, was "scikit-rt-0.5.0.tar", last modified: Mon Jun 26 15:06:52 2023, max compression
```

## Comparing `scikit-rt-0.4.9.tar` & `scikit-rt-0.5.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.212740 scikit-rt-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 09:23:05.212740 scikit-rt-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-31 09:23:05.212740 scikit-rt-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.180740 scikit-rt-0.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.184740 scikit-rt-0.4.9/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 09:23:04.000000 scikit-rt-0.4.9/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-31 09:23:05.000000 scikit-rt-0.4.9/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:23:04.000000 scikit-rt-0.4.9/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-31 09:23:04.000000 scikit-rt-0.4.9/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 09:23:04.000000 scikit-rt-0.4.9/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.192740 scikit-rt-0.4.9/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.196740 scikit-rt-0.4.9/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132448 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    75993 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.180740 scikit-rt-0.4.9/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.196740 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.200740 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   257102 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118731 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   134908 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.200740 scikit-rt-0.4.9/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:23:05.212740 scikit-rt-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-31 09:18:51.000000 scikit-rt-0.4.9/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.431730 scikit-rt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-26 15:06:52.431730 scikit-rt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-26 15:06:52.431730 scikit-rt-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.391729 scikit-rt-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.395729 scikit-rt-0.5.0/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-26 15:06:52.000000 scikit-rt-0.5.0/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-26 15:06:52.000000 scikit-rt-0.5.0/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:06:52.000000 scikit-rt-0.5.0/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-26 15:06:52.000000 scikit-rt-0.5.0/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 15:06:52.000000 scikit-rt-0.5.0/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.407729 scikit-rt-0.5.0/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.411729 scikit-rt-0.5.0/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132535 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.391729 scikit-rt-0.5.0/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.411729 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.415729 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   257101 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118936 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151890 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.419730 scikit-rt-0.5.0/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:06:52.427730 scikit-rt-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-26 15:01:41.000000 scikit-rt-0.5.0/tests/test_viewer.py
```

### Comparing `scikit-rt-0.4.9/LICENSE` & `scikit-rt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/PKG-INFO` & `scikit-rt-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.9
+Version: 0.5.0
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.9/README.md` & `scikit-rt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/pypi.md` & `scikit-rt-0.5.0/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/setup.cfg` & `scikit-rt-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.4.9
+version = 0.5.0
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.4.9/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.5.0/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.9
+Version: 0.5.0
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.9/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.5.0/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.5.0/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/__init__.py` & `scikit-rt-0.5.0/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/application.py` & `scikit-rt-0.5.0/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.5.0/src/skrt/better_viewer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1116,15 +1116,17 @@
                     v.custom_ax_lims[view][1] = all_ax_lims[view][1]
 
     def make_ui(self, no_roi=False, no_intensity=False):
 
         # Only allow share_slider if images have same frame of reference
         if self.share_slider:
             self.share_slider *= all(
-                [v.image.has_same_geometry(self.viewers[0].image) for v in self.viewers]
+                [v.image.has_same_geometry(
+                    self.viewers[0].image, standardise=True)
+                 for v in self.viewers]
             )
 
         # Make UI for first image
         v0 = self.viewers[0]
         v0.make_ui(no_roi=no_roi, no_intensity=no_intensity)
 
         # Store needed UIs
@@ -1271,15 +1273,16 @@
         self.comp_ui = []
 
         # Multicomparison dropdown
         comp_opts = [
             'overlay',
             'chequerboard',
         ]
-        if all([v.image.has_same_geometry(self.viewers[0].image) for v in self.viewers]):
+        if all([v.image.has_same_geometry(
+            self.viewers[0].image, standardise=True) for v in self.viewers]):
             comp_opts.extend([
                 'difference',
                 'absolute difference',
                 'distance to agreement',
                 'gamma index',
             ])
         if self.comparison_only:
```

### Comparing `scikit-rt-0.4.9/src/skrt/better_viewer/options.py` & `scikit-rt-0.5.0/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/core.py` & `scikit-rt-0.5.0/src/skrt/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -912,35 +912,39 @@
             of output filename if not None, otherwise Ignored.
         """
         if not callable(getattr(self, "load", None)):
             raise NotImplementedError(
                     f"{type(self)}.copy_dicom() failed - "
                     "class has no load() method")
             return
-        self.load()
+
+        # Create clone for data loading.
+        # Clone is deleted once data are no longer needed.
+        obj = self.clone()
+        obj.load()
 
         # Check that object has dicom file to be copied.
-        path = Path(self.path)
-        ds = getattr(self, "dicom_dataset", None)
+        path = Path(obj.path)
+        ds = getattr(obj, "dicom_dataset", None)
         if not ds or not path.exists():
             raise NotImplementedError(
-                    f"{type(self)}.copy_dicom() failed - "
+                    f"{type(obj)}.copy_dicom() failed - "
                     "object has no associated DICOM file")
             return
 
         # Obtain the data modality.
         modality = getattr(ds, "Modality", "unknown")
 
         # Define the output directory.
         outdir = make_dir(outdir or modality, overwrite)
 
         # Define path to the output file.
         if sort:
             idx = "" if index is None else f"_{index+1:03}"
-            name = f"{modality}_{self.timestamp}{idx}.dcm"
+            name = f"{modality}_{obj.timestamp}{idx}.dcm"
         else:
             name = path.name()
         outpath = outdir / name
 
         # Copy file.
         if overwrite or not outpath.exists():
             shutil.copy2(path, outpath)
```

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 (Optimizer "AdaptiveStochasticGradientDescent")
 (Transform "AffineTransform")
 (Metric "AdvancedMattesMutualInformation")
 
 // ***************** Transformation **************************
 
 (AutomaticScalesEstimation "true")
-// (AutomaticTransformInitialization "false")
-(AutomaticTransformInitialization "true")
+(AutomaticTransformInitialization "false")
+// (AutomaticTransformInitialization "true")
 (HowToCombineTransforms "Compose")
 
 // ******************* Similarity measure *********************
 
 //(UseNormalization "true")
 (NumberOfHistogramBins 32)
 (ErodeMask "true")
```

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 (Optimizer "AdaptiveStochasticGradientDescent")
 (Transform "EulerTransform")
 (Metric "AdvancedMattesMutualInformation")
 
 // ***************** Transformation **************************
 
 (AutomaticScalesEstimation "true")
-// (AutomaticTransformInitialization "false")
-(AutomaticTransformInitialization "true")
+(AutomaticTransformInitialization "false")
+// (AutomaticTransformInitialization "true")
 (HowToCombineTransforms "Compose")
 
 // ******************* Similarity measure *********************
 
 (UseNormalization "true")
 (NumberOfHistogramBins 32)
 (ErodeMask "true")
```

### Comparing `scikit-rt-0.4.9/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.5.0/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 (Optimizer "AdaptiveStochasticGradientDescent")
 (Transform "TranslationTransform")
 (Metric "AdvancedMattesMutualInformation")
 
 // ***************** Transformation **************************
 
 (AutomaticScalesEstimation "true")
-// (AutomaticTransformInitialization "false")
-(AutomaticTransformInitialization "true")
+(AutomaticTransformInitialization "false")
+// (AutomaticTransformInitialization "true")
 (HowToCombineTransforms "Compose")
 
 // ******************* Similarity measure *********************
 
 (UseNormalization "true")
 (NumberOfHistogramBins 32)
 (ErodeMask "true")
```

### Comparing `scikit-rt-0.4.9/src/skrt/dicom_writer.py` & `scikit-rt-0.5.0/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/dose.py` & `scikit-rt-0.5.0/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/image.py` & `scikit-rt-0.5.0/src/skrt/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         # Check if the requested type is recognised.
         nii_type = itype in ['nii', 'nifti']
         dcm_type = itype in ['dcm', 'dicom']
 
         if nii_type or dcm_type:
             # Ensure that image is loaded, and create clone.
             self.load()
-            im = self.__class__(self)
+            im = self.clone()
 
             # Modify image data if source_type isn't the requested type.
             if ((nii_type and 'nifti' not in self.source_type)
                     or (dcm_type and 'nifti' in self.source_type)):
                 affine = self.affine.copy()
                 # Convert to nibabel/NIfTI representation.
                 if nii_type:
@@ -3779,15 +3779,15 @@
     def get_coords(self):
         """Get grids of x, y, and z coordinates for each voxel in the image."""
 
         # Make coordinates
         coords_1d = [
             np.arange(
                 self.origin[i],
-                self.origin[i] + self.n_voxels[i] * self.voxel_size[i],
+                self.origin[i] + (self.n_voxels[i] -0.5) * self.voxel_size[i],
                 self.voxel_size[i],
             )
             for i in range(3)
         ]
         return np.meshgrid(*coords_1d)
 
     def transform(self, scale=1, translation=[0, 0, 0], rotation=[0, 0, 0],
```

### Comparing `scikit-rt-0.4.9/src/skrt/multi.py` & `scikit-rt-0.5.0/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/patient.py` & `scikit-rt-0.5.0/src/skrt/patient.py`

 * *Files 1% similar despite different names*

```diff
@@ -960,25 +960,31 @@
         # Overwriting taken into account at study level,
         # so don't overwrite at sub-study level.
         for image_type in image_indices:
 
             # Loop over images of current type.
             for idx1, im in enumerate(self.image_types[image_type]):
 
+                # Create clone for data loading.
+                # Clone is deleted once data are no longer needed.
+                im2 = im.clone()
+
                 # Check that image can be loaded.
                 # If not, give warning and skip.
                 try:
-                    im.load()
+                    im2.load()
                 except:
-                    im.data = None
+                    im2.data = None
 
-                if im.data is None:
+                if im2.data is None:
                     print(f"Problems loading: {image_type}")
                     print(getattr(im, "dicom_paths", []))
+                    del im2
                     continue
+                del im2
                 
                 # Copy image.
                 im.copy_dicom_files(image_type, idx1, image_indices,
                         study_dir / image_type.upper()
                         / f"{im.timestamp}_{idx1+1:03}",
                         overwrite=False, sort=sort)
```

### Comparing `scikit-rt-0.4.9/src/skrt/registration.py` & `scikit-rt-0.5.0/src/skrt/registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 """
 import matplotlib.pyplot as plt
 import matplotlib.cm
 import matplotlib.colors
 import numbers
 import numpy as np
 import os
+import platform
 from pathlib import Path
 from pkg_resources import resource_filename
 import shutil
 import subprocess
 import warnings
 
 import skrt.image
@@ -53,14 +54,16 @@
 from skrt.core import (fullpath, get_logger, Data, is_list, to_list,
         Defaults, PathData)
 from skrt.dose import ImageOverlay, Dose
 from skrt.simulation import make_grid
 
 # Set default registration engine.
 Defaults({"registration_engine": "elastix"})
+Defaults().matlab_app = True
+Defaults().matlab_runtime = None
 
 engines = {}
 def add_engine(cls):
     """
     Decorator for adding skrt.registration.RegistrationEngine subclasses
     to the skrt.registartion.engines dictionary.
     """
@@ -939,14 +942,21 @@
         result_path = self.transform_data(im_path, step, params)
         if result_path is None:
             return
 
         # Copy to output dir if outfile is set
         if outfile is not None:
             shutil.copy(result_path, outfile)
+            df_path1 = Path(result_path).parent / "deformationField.nii"
+            # If file for deformation field created,
+            # copy to step's output directory if not already present.
+            if df_path1.exists():
+                df_path2 = Path(outfile).parent / df_path1.name
+                if not df_path2.exists():
+                    shutil.copy(df_path1, df_path2)
             return
 
         # Otherwise, return Image object
         if is_dose:
             final_im = Dose(result_path)
         else:
             final_im = skrt.image.Image(result_path)
@@ -961,24 +971,30 @@
             for ss in rois_to_transform:
                 ss2 = self.transform_structure_set(ss, step=step)
                 final_im.add_structure_set(ss2)
 
         self.rm_tmp_dir()
         return final_im
 
-    def transform_data(self, path, step=-1, params=None):
+    def transform_data(self, path, step=-1, params=None, recurse=True):
         """Transform a nifti file or point cloud at a given path
         for a given step, ensuring that the step has been run. Return
         the path to the transformed file inside self._tmp_dir."""
 
         # Check registration has been performed, and run it if not
         i = self.get_step_number(step)
         step = self.get_step_name(step)
         self.ensure_registered(step)
 
+        # If transform can't be applied directly to initial data,
+        # obtain transformed data resulting from preceding steps.
+        if i and self.engine.recursive_transform and recurse:
+            for istep in range(i):
+                path = self.transform_data(path, istep, params, False)
+
         # Make temporary modified parameter file if needed
         self.make_tmp_dir()
         tfile = self.tfiles[step]
 
         # Define parameters specific to data type.
         if '.txt' == os.path.splitext(path)[1]:
             outfile = 'outputpoints.txt' 
@@ -1471,23 +1487,23 @@
 
         # Ensure registration has been performed for this step
         self.ensure_registered(step)
 
         # Create new object
         storage[step] = self.run_transformix_on_all(
             is_jac, outdir=self.outdirs[step], tfile=self.tfiles[step], 
-            image=self.transformed_images[step]
+            image=self.transformed_images[step], step=step, force=force
         )
         return storage[step]
 
     def get_transformed_grid(self, step=-1, force=False,
             spacing=(30, 30, 30), thickness=(2, 2, 2),
             voxel_units=False, color='green'):
         '''
-        Obtaing transformed grid.
+        Obtain transformed grid.
 
         A three-dimensional grid is defined in the space of
         the moving image, and is transformed by applying the
         result of a registration step.
 
         **Parameters:**
 
@@ -1534,21 +1550,39 @@
 
         # Fixed intensities for foreground and background
         background = 0
         foreground = 1
 
         # Ensure that untransformed grid exists
         if not hasattr(self, 'moving_grid') or force:
-            self.set_moving_grid(make_grid(self.moving_image, spacing,
+            if issubclass(type(self.moving_source), skrt.image.Image):
+                image = self.moving_source
+            elif isinstance(self.moving_source, str):
+                image = skrt.image.Image(self.moving_source)
+            else:
+                image = getattr(self, 'moving_image', None)
+            self.set_moving_grid(make_grid(image, spacing,
                 thickness, background, foreground, voxel_units))
             self.moving_grid = Grid(self.moving_grid.path,
                     color=color, image=self.moving_image, title='Grid')
 
+        istep = self.get_step_number(step)
+        if self.engine.recursive_transform and istep:
+            # Start from transformed grid from previous step.
+            moving_grid = self.get_transformed_grid(
+                    step=(istep - 1), force=force, spacing=spacing,
+                    thickness=thickness, voxel_units=voxel_units, color=color)
+            moving_grid_path = moving_grid.path
+        else:
+            # Start from untransformed grid.
+            moving_grid_path = self.moving_grid_path
+
         grid_path = Path(
-                self.transform_data(path=self.moving_grid_path, step=step))
+                self.transform_data(
+                    path=moving_grid_path, step=step, recurse=False))
         grid_path = grid_path.rename(Path(self.outdirs[step]) / 'grid.nii')
 
         #self.transformed_grids[step] = skrt.image.Image(str(grid_path))
         self.transformed_grids[step] = Grid(str(grid_path), color=color,
                 image=self.transformed_images[step], title='Transformed grid')
 
         return self.transformed_grids[step]
@@ -1580,15 +1614,16 @@
             return self._get_jac_or_def(step, True, force)
 
     def get_deformation_field(self, step=-1, force=False):
         """Generate deformation field for a given registration step."""
         
         return self._get_jac_or_def(step, False, force)
 
-    def run_transformix_on_all(self, is_jac, outdir, tfile, image=None):
+    def run_transformix_on_all(
+            self, is_jac, outdir, tfile, image=None, step=-1, force=False):
         """
         Create a Jacobian determinant or deformation field file,
         and return either a Jacobian or DeformationField object initialised
         from the output file.
 
         This was first implemented by running transformix for an elastix
         transform file.  Creation of Jacobian or DeformationField object
@@ -1618,19 +1653,30 @@
                     cmd, capture_output=self.capture_output).returncode
             if code:
                 logfile = os.path.join(outdir, 'transform.log')
                 raise RuntimeError(
                         f"Creation of {title }failed. See {logfile} for"
                         " more info.")
 
-            # Create output object
-            output_file = os.path.join(outdir, expected_outname)
-            assert os.path.exists(output_file)
+        # Create output object
+        output_file = os.path.join(outdir, expected_outname)
+        if os.path.exists(output_file):
             kwargs = {} if is_jac else {"signs": self.engine.def_signs}
-            return dtype(path=output_file, image=image, title=title, **kwargs)
+            obj = dtype(path=output_file, image=image, title=title, **kwargs)
+            istep = self.get_step_number(step)
+            if is_jac or not (self.engine.recursive_transform and istep):
+                return obj
+
+            # If transforms applied recursively,
+            # add displacments from previous step.
+            df = self.get_deformation_field(istep - 1, force)
+            if df is not None:
+                obj._image.data += df._image.data
+                obj._image._data_canonical += df._image._data_canonical
+            return obj
 
     def get_comparison(self, step=-1, force=False, **kwargs):
         """
         Return a pandas DataFrame comparing fixed image
         and transformed moving image after step.
 
         **Parameters:**
@@ -1846,15 +1892,15 @@
             but should correspond to arrays of dimension 4.
             Otherwise, it can be loaded later with the load() method.
 
         load : bool, default=True
             If True, the deformation-field data will be immediately loaded.
 
         signs : tuple, default=None
-            Three element tuple of ints, indicating the igns to be applied to
+            Three element tuple of ints, indicating the signs to be applied to
             the (x, y, z) components of the deformation field, allowing
             for different conventions.  If None, components are taken to
             be as read from source.
 
         image : skrt.image.Image, default=None
             Image object to be associated with the deformation field.
 
@@ -1922,32 +1968,36 @@
 
         data = self._image.get_slice(view, sl=sl, idx=idx, pos=pos)
         x_ax, y_ax = skrt.image._plot_axes[view]
 
         # Get x/y displacement vectors
         df_x = np.squeeze(data[:, :, x_ax])
         df_y = np.squeeze(data[:, :, y_ax])
+        if 1 == y_ax:
+            df_y = - df_y
         if not scale_in_mm:
             df_x /= self._image.voxel_size[x_ax]
             df_y /= self._image.voxel_size[y_ax]
 
         # Get x/y coordinates of each point on the slice
         xs = np.arange(0, data.shape[1])
         ys = np.arange(0, data.shape[0])
         if scale_in_mm:
-            xs = self._image.origin[x_ax] + xs * self._image.voxel_size[x_ax]
+            xs = (self._image._sorigin[x_ax] + xs
+                  * self._image._svoxel_size[x_ax])
             if self._image.voxel_size[x_ax] < 0:
-                xs = xs[::-1]
-            ys = self._image.origin[y_ax] + ys * self._image.voxel_size[y_ax]
+                df_x = df_x[::-1]
+            ys = (self._image._sorigin[y_ax] + ys
+                  * self._image._svoxel_size[y_ax])
             if self._image.voxel_size[y_ax] < 0:
-                ys = ys[::-1]
+                df_y = df_y[::-1]
         y, x = np.meshgrid(ys, xs)
         x = x.T
         y = y.T
-        return x, y, df_x, -df_y
+        return x, y, df_x, df_y
 
     def get_displacement_image(self, displacement="3d"):
         """
         Get skrt.dose.ImageOverlay object representing point displacements.
 
         **Parameter:**
 
@@ -1964,23 +2014,28 @@
             print(f"Displacement type not known: '{displacement}'")
             print(f"Known displacement types: {list(self.displacement_images)}")
             return
 
         # Check if OverlayImage of displacement requested is already stored.
         # If not, then create and store it.
         if self.displacement_images[displacement] is None:
-            im_data = self._image.clone().get_data()
+            im_data = self._image.clone().get_standardised_data()
             idx = "xyz".find(displacement)
             if -1 == idx:
                 # Magnitudes of 3d displacements.
                 im_data = np.sqrt(np.sum(np.square(im_data), axis=idx))
             else:
                 # Signed displacements along axis.
                 im_data = np.squeeze(im_data[:, :, :, idx])
-            im = ImageOverlay(im_data, affine=self._image.get_affine())
+            im = ImageOverlay(
+                    im_data, affine=self._image.get_standardised_affine())
+            if "nifti" in self._image.source_type:
+                im = im.astype("nii")
+
+
             im._default_cmap = self._default_cmap
             if "3d" == displacement:
                 im._default_colorbar_label = self._3d_colorbar_label
             else:
                 im._default_colorbar_label = (
                         f"{displacement}-{self._default_colorbar_label}")
             im._default_opacity = self._default_opacity
@@ -2141,15 +2196,17 @@
 
         # Get arrow positions and lengths
         x_ax, y_ax = skrt.image._plot_axes[view]
         x, y, df_x, df_y = data_slice
         arrows_x = df_x[:: spacing[y_ax], :: spacing[x_ax]]
         arrows_y = df_y[:: spacing[y_ax], :: spacing[x_ax]]
         plot_x = x[:: spacing[y_ax], :: spacing[x_ax]]
-        plot_y = y[:: spacing[y_ax], :: spacing[x_ax]]
+        # Not clear why, but this inversion seems to be needed...
+        sign = -1 if 2 == y_ax else 1
+        plot_y = y[:: sign * spacing[y_ax], :: sign * spacing[x_ax]]
 
         # Make plotting kwargs
         mpl_kwargs = mpl_kwargs or {}
         vmin = mpl_kwargs.pop("vmin", 0)
         vmax = mpl_kwargs.pop("vmax",
                 self.get_displacement_image("3d").get_data().max() * 1.1)
         default_kwargs = {"cmap": "jet"}
@@ -2202,15 +2259,18 @@
         """Draw a grid plot."""
 
         # Get gridline positions
         #  self.ax.autoscale(False)
         x_ax, y_ax = skrt.image._plot_axes[view]
         x, y, df_x, df_y = data_slice
         grid_x = x + df_x
-        grid_y = y + df_y
+        if 1 == y_ax:
+            grid_y = y - df_y
+        else:
+            grid_y = y + df_y
 
         # Make plotting kwargs
         default_kwargs = {"color": "green", "linewidth": 2}
         if mpl_kwargs is not None:
             default_kwargs.update(mpl_kwargs)
 
         # Disregard kwargs that aren't valid here,
@@ -2330,14 +2390,17 @@
     in subclasses.
 
     This class defines the following variables and methods:
 
     **Class variables:**
     transform_points_implemented (bool): Indicate whether registration engine
         implements mapping of points from fixed image to moving images.
+    recursive_transform (bool): Indicate whether a transform for a
+        registration step other than the first requires the transform output
+        from the preceding step.
     def_signs (tuple/None): Indicate signs to be applied to
         (x, y, z) components of deformation field.
 
     **Methods:**
     __init__():  Create RegistrationEngine instance.
     adjust_parameters():
         Modify contents of a registration parameter file.
@@ -2371,14 +2434,18 @@
         for applying registration transform.
     """
 
     # Indicate whether registration engine implements mapping of points
     # from fixed image to moving images.
     transform_points_implemented = False
 
+    # Indicate whether a transform for a registration step other than the first
+    # requires the transform output from the preceding step.
+    recursive_transform = False
+
     # Indicate signs to be applied to (x, y, z) components of deformation field.
     # If None, components are taken to be as read from file.
     def_signs = None
 
     # Define engine executables.
     exes = []
 
@@ -2609,16 +2676,21 @@
         If False, modify environment based on <path> only if registration
         software can't be located in the existing environment.  If True, modify
         environment based on <path> in all cases.
         """
         exe_dir = None
 
         # Check if environment already set for running the registration engine.
+        if path is not None:
+            path = fullpath(path)
         if not (path and force):
-            exe_path = shutil.which(self.name)
+            if type(self).exes:
+                exe_path = shutil.which(type(self).exes[0])
+            else:
+                exe_path = None
             if exe_path is not None:
                 exe_dir = Path(exe_path).parent
 
         # Return if environment already set and not forcing new setup,
         # of if no value specified for path (no new setup possible).
         if (exe_dir and not force) or path is None:
             return
@@ -2918,14 +2990,325 @@
             file.write(line + "\n")
         file.close()
 
     @staticmethod
     def get_transform_strategies():
         return ["pull", "push"]
 
+@add_engine
+class Matlab(RegistrationEngine):
+    """
+    Class interfacing to MATLAB registration engine.
+    """
+    # Indicate signs to be applied to (x, y, z) components of deformation field.
+    # If None, components are taken to be as read from file.
+    #def_signs = (-1, -1, -1)
+
+    # Define engine executables.
+    exes = ["matlabreg"]
+
+    # Indicate whether a transform for a registration step other than the first
+    # requires the transform output from the preceding step.
+    recursive_transform = True
+
+    def adjust_parameters(self, infile, outfile, params):
+        # Modify MATLAB parameter file.
+        # MATLAB doesn't define its own file format.  Here adopt
+        # format used by elastix.  For information about this,
+        # see section 3.4 of elastix manual:
+        # https://elastix.lumc.nl/download/elastix-5.0.1-manual.pdf
+        return Elastix.adjust_parameters(self, infile, outfile, params)
+
+    def define_translation(self, dxdydz, fixed_image=None):
+        # Define translation parameters that are enough to allow
+        # application before a registration step.
+        # Tuple dxdydz defines (dx, dy, dz) translations for mapping a
+        # point from fixed image to moving image, but MATLAB's imwarp
+        # needs translations for mapping from moving image to fixed image.
+        # Negative signs allow for this.
+        translation = [
+                f"1 0 0 {-dxdydz[0]}",
+                f"0 1 0 {-dxdydz[1]}",
+                f"0 0 1 {-dxdydz[2]}",
+                "0 0 0 1",
+                ]
+
+        return translation
+
+    def get_def_cmd(self, fixed_path, outdir, tfile):
+        # Deformation field for MATLAB computed at registration time.
+        return
+
+    def get_jac_cmd(self, fixed_path, outdir, tfile):
+        # Jacobian determinant not computed for MATLAB registrations.
+        return
+
+    def get_registration_cmd(
+            self, fixed_path, moving_path, fixed_mask_path, moving_mask_path,
+            pfile, outdir, tfile=None):
+
+        # Read registration parameters from file.
+        params = self.read_parameters(pfile)
+
+        # Define path to output directory.
+        outdir = Path(outdir)
+
+        # If this isn't the first step, take as moving image the
+        # output image from the preceding step.
+        if tfile:
+            moving_path = str(Path(tfile).parent / "result.0.nii")
+
+        # Start command with execuable, paths to fixed and moving images,
+        # and path to output file (name following elastix convention).
+        cmd = [
+                params["exe"],
+                moving_path,
+                fixed_path,
+                str(outdir),
+            ]
+
+        # Add any other parameter-value pairs.
+        for param, val in params.items():
+            if "exe" != param and param not in cmd:
+                cmd.append(param)
+                if val != "":
+                    cmd.append(str(val))
+
+        if "matlab" in self.exe_cmd:
+            args = ",".join([f"'{arg}'" for arg in cmd])
+            cmd = self.exe_cmd + [f"{type(self).exes[0]}({args})"]
+        else:
+            cmd = self.exe_cmd + cmd
+
+        return cmd
+
+    def get_roi_params(self):
+        # Return parameters to include when transforming ROI masks.
+        return {"interp": "nearest"}
+
+    def get_transform_cmd(
+            self, fixed_path, moving_path, outdir, tfile, params=None):
+        # Construct part of command relating to any input parameters.
+        params = params or {}
+        interp = params.pop("interp", "nearest")
+        params = [str(val) for items in params.items() for val in items]
+
+        cmd = ["imwarp", moving_path, fixed_path,
+               str(Path(outdir)), tfile, interp] + params
+
+        if "matlab" in self.exe_cmd:
+            args = ",".join([f"'{arg}'" for arg in cmd])
+            cmd = self.exe_cmd + [f"{type(self).exes[0]}({args})"]
+        else:
+            cmd = self.exe_cmd + cmd
+
+        # Return command for applying registration transform.
+        return cmd
+
+    def read_affine(self, infile):
+        """
+        Read affine matrix from file. 
+
+        **Parameter:**
+        infile: str/pathlib.Path
+            Path to file from which to read affine matrix.
+        """
+        with open(infile) as file:
+            lines = [line.strip().split() for line in file.readlines()]
+        return [[float(item) for item in line] for line in lines]
+
+    def read_parameters(self, infile):
+        # Read MATLAB parameter file.
+        # MATLAB doesn't define its own file format.  Here adopt
+        # format used by elastix.  For information about this,
+        # see section 3.4 of elastix manual:
+        # https://elastix.lumc.nl/download/elastix-5.0.1-manual.pdf
+        return Elastix.read_parameters(self, infile)
+
+    def set_exe_env(self, path=None, force=False):
+        """
+        Set environment variables for running MATLAB registration.
+
+        MATLAB registration can be run using compiled or uncompiled MATLAB
+        code.  In both cases, the environment setup can be performed
+        before or after starting the Python session that runs scikit-rt.
+
+        **To run compiled MATLAB code:**
+
+        - To set environment from scikit-rt:
+          
+          1. Set skrt.registration.Defaults().matlab_runtime to be the path to
+             the MATLAB runtime installation directory.
+
+          2. When creating a skrt.registration.Matlab() instance, pass as the
+             <path> parameter the path to the directory that contains
+             the compiled MATLAB application.
+
+        - To set environment prior to starting Python:
+
+          1. Set platform dependent environment variable for MATLAB runtime:
+             https://uk.mathworks.com/help/compiler/mcr-path-settings-for-run-time-deployment.html
+
+          2. Add to PATH variable the path to the directory that contains
+             the compiled MATLAB application.
+
+          3. After starting Python and importing scikit-rt, set:
+             skrt.registration.Defaults().matlab_runtime = True
+
+        **To run uncompiled MATLAB code:**
+
+        - To set environment from scikit-rt:
+          
+          1. Set skrt.registration.Defaults().matlab_app to be the
+             path to the directory that contains the MATLAB executable.
+
+          2. When creating a skrt.registration.Matlab() instance, pass as the
+             <path> parameter the path to the directory that contains
+             the uncompiled MATLAB registration code.
+
+        - To set environment prior to starting Python:
+
+          1. Add to PATH variable the path to the directory that contains
+             the MATLAB executable.
+
+          2. Add to MATLABPATH variable the path to the directory that
+             contains the uncompiled MATLAB registration code.
+
+        **Parameters:**
+
+        path : str/pathlib.Path, default=None
+            If skrt.registration.Defaults().matlab_runtime evaluates to
+            True, this is the path to the directory containing the
+            compiled MATLAB application for image registration.  Otherwise,
+            this is the path to the directory that contains the MATLAB
+            executable.  Ignored if set to None.
+
+        force : bool, default=False
+            If False, modify environment based on <path> only if
+            registration software can't be located in the existing
+            environment.  If True, modify environment based on <path>
+            in all cases.
+        """
+        path = fullpath(path)
+        if Defaults().matlab_runtime:
+            # Use MATLAB runtime environment.
+            # If Defaults().matlab_runtime is a string or pathlib.Path,
+            # use it to define the runtime environment.
+            # Otherwise, assume that the environment has been set by the user.
+            if isinstance(Defaults().matlab_runtime, (Path, str)):
+                matlab_runtime = Path(fullpath(Defaults().matlab_runtime))
+                subdirs = ["runtime", "bin",
+                           Path("sys") / "os", Path("extern") / "bin"]
+                if "Linux" == platform.system():
+                    env_var = "LD_LIBRARY_PATH"
+                    arch = "glnxa64"
+                elif "Darwin" == platform.system():
+                    env_var = "DYLD_LIBRARY_PATH"
+                    arch = "maci64"
+                else:
+                    env_var = "PATH"
+                    subdirs = ["runtime"]
+                    arch = "win64"
+
+                runtime_ok = True
+
+                for subdir in subdirs:
+                    env_val = matlab_runtime / subdir / arch
+                    if (env_var not in os.environ
+                        or str(env_val) not in os.environ[env_var] or force):
+                        runtime_ok *= prepend_path(env_var, env_val)
+                        if not runtime_ok:
+                            raise RuntimeError(
+                                    "MATLAB runtime directory not found: "
+                                    + f"'{env_val}'")
+
+            # Check that the runtime application can be found.
+            exe = "matlabreg"
+            if force or shutil.which(exe) is None:
+                if isinstance(path, (Path, str)):
+                    if not prepend_path("PATH", path):
+                        raise RuntimeError(
+                                "Directory for MATLAB registration "
+                                f"application not found: '{path}'")
+
+            if shutil.which(exe) is None:
+                raise RuntimeError(
+                        "Application for running MATLAB registration "
+                        f"not found: '{exe}'")
+
+            self.exe_cmd = ["matlabreg"]
+
+        else:
+            # Uncompiled MATLAB code to be called from MATLAB executable.
+            # If Defaults().matlab_app is a string or pathlib.Path,
+            # use it to define the environment for running the executable.
+            # Otherwise, assume that the environment has been set by the user.
+            exe = "matlab"
+            if force or shutil.which(exe) is None:
+                if isinstance(Defaults().matlab_app, (Path, str)):
+                    matlab_app = Path(fullpath(Defaults().matlab_app))
+                    if not prepend_path("PATH", matlab_app):
+                        raise RuntimeError(
+                                "MATLAB application directory not found: "
+                                + f"'{matlab_app}'")
+
+            # Check that the MATLAB executable can be found.
+            if not shutil.which(exe):
+                raise RuntimeError("Path to MATLAB executable not found")
+
+            # If code directory is defined, check that it exists.
+            if isinstance(path, (Path, str)):
+                if not prepend_path("MATLABPATH", path):
+                    raise RuntimeError(
+                            "Directory to be added to MATLABPATH not found: "
+                            + f"'{path}'")
+
+            self.exe_cmd = ["matlab", "-batch"]
+
+    def shift_translation_parameters(
+            self, infile, dx=0, dy=0, dz=0, outfile=None):
+        # Add offsets to the translation parameters
+        # of a MATLAB transform file.
+        if outfile is None:
+            outfile = infile
+
+        affine = self.read_affine(infile)
+
+        # Offset translation parameters.
+        # Signs account for different conventions between NiftyReg and Elastix.
+        affine[0][3] -= dx
+        affine[1][3] += dy
+        affine[2][3] += dz
+
+        self.write_affine(affine, outfile)
+        return True
+
+    def write_affine(self, affine, outfile):
+        """
+        Write affine matrix fo file. 
+
+        **Parameter:**
+        outfile: str/pathlib.Path
+            Path to file to which to write affine matrix.
+        """
+        rows = [" ".join([str(val) for val in row]) for row in affine]
+        with open(outfile, "w") as file:
+            file.write("\n".join(rows))
+
+    def write_parameters(self, outfile, params):
+        # Write MATLAB parameter file.
+        # MATLAB doesn't define its own file format.  Here adopt
+        # format used by elastix.  For information about this,
+        # see section 3.4 of elastix manual:
+        # https://elastix.lumc.nl/download/elastix-5.0.1-manual.pdf
+        return Elastix.write_parameters(self, outfile, params)
+
+    @staticmethod
+    def get_transform_strategies():
+        return ["pull"]
 
 @add_engine
 class NiftyReg(RegistrationEngine):
     """
     Class interfacing to NiftyReg registration engine.
     """
     # Indicate signs to be applied to (x, y, z) components of deformation field.
@@ -3140,14 +3523,52 @@
     """
     return get_engine_cls(engine)().adjust_parameters(infile, outfile, params)
 
 def get_data_dir():
     """Return path to data directory within the scikit-rt package."""
     return Path(resource_filename("skrt", "data"))
 
+def get_parameters(pattern=None, engine=None, idx=0, params=None):
+    """
+    Obtain parameter dictionary from default parameter file.
+
+    **Parameter:**
+    pattern: str, default=None
+        Glob-style pattern for identifying default parameter file(s).
+
+    engine: str, default=None
+        Name of registration engine for which a default parameter file
+        is to be read.  If None, use value set for
+        skrt.core.Default().registration_engine.
+
+    idx: int, default=0
+        Index of parameter file to be read, from sorted list of those
+        matching <pattern>.  To avoid ambiguity, it's usually best to
+        choose <pattern> so that only one file is matched.  A list
+        of matching files can be obtained using get_default_pfiles().
+
+    params: dict, default=None
+        Dictionary of parameter-value pairs, with which to update dictionary
+        read from file.  Ignored if None.
+    """
+    # Obtain list of parameter files.
+    if pattern: 
+        pfiles = get_default_pfiles(pattern, engine)
+    else:
+        pfiles = []
+
+    # Read parameters from file.
+    all_params = read_parameters(pfiles[idx], engine) if pfiles else {}
+
+    # Update parameters.
+    if isinstance(params, dict):
+        all_params.update(params)
+
+    return all_params
+
 
 def get_default_pfiles(pattern="*.txt", engine=None, basename_only=False):
     """
     Get list of default parameter files.
 
     **Parameter:**
 
@@ -3419,19 +3840,26 @@
     if path_must_exist:
         if not os.path.exists(path):
             path_ok = False
 
     if path_ok:
         if variable in os.environ:
             if os.environ[variable]:
-                os.environ[variable] = os.pathsep.join(
-                        [path, os.environ[variable]])
+                items = os.environ[variable].split(os.pathsep)
+                if path in items:
+                    items.remove(path)
+                if items:
+                    os.environ[variable] = os.pathsep.join([path] + items)
+                else:
+                    os.environ[variable] = path
         else:
             os.environ[variable] = path
 
+    return path_ok
+
 
 def read_parameters(infile, engine=None):
     """
     Get dictionary of parameters from a registration parameter file.
 
     **Parameters:**
     infile: str, pathlib.Path
```

### Comparing `scikit-rt-0.4.9/src/skrt/segmentation.py` & `scikit-rt-0.5.0/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/simulation.py` & `scikit-rt-0.5.0/src/skrt/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
             If true and no valid timestamp is found within the path string,
             timestamp generated from current date and time.
         """
 
         # Assign properties
         shape = skrt.core.to_list(shape)
         self.shape = [shape[1], shape[0], shape[2]]
+        self.n_voxels = shape
         #self.voxel_size = [abs(v) for v in skrt.core.to_list(voxel_size)]
         self.voxel_size = skrt.core.to_list(voxel_size)
         self.origin = origin
         self.max_hu = 0 if noise_std is None else noise_std * 3
         self.min_hu = -self.max_hu if self.max_hu != 0 else -20
         self.noise_std = noise_std
         self.bg_intensity = intensity
```

### Comparing `scikit-rt-0.4.9/src/skrt/structures.py` & `scikit-rt-0.5.0/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/viewer/core.py` & `scikit-rt-0.5.0/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/src/skrt/viewer/viewer.py` & `scikit-rt-0.5.0/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_01_setup.py` & `scikit-rt-0.5.0/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_application.py` & `scikit-rt-0.5.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_core.py` & `scikit-rt-0.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_dose.py` & `scikit-rt-0.5.0/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_image.py` & `scikit-rt-0.5.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_multi.py` & `scikit-rt-0.5.0/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_patient.py` & `scikit-rt-0.5.0/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_qv_image.py` & `scikit-rt-0.5.0/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_qv_quickviewer.py` & `scikit-rt-0.5.0/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_qv_struct_loader.py` & `scikit-rt-0.5.0/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_qv_struct_metrics.py` & `scikit-rt-0.5.0/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_qv_structs.py` & `scikit-rt-0.5.0/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_registration.py` & `scikit-rt-0.5.0/tests/test_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from skrt import Image
 from skrt.core import Defaults, fullpath
 from skrt.simulation import SyntheticImage
 from skrt.registration import (
         Elastix, NiftyReg, Registration, RegistrationEngine,
         add_engine, engines, get_default_pfiles, get_default_pfiles_dir,
-        get_engine_cls, get_jacobian_colormap, read_parameters,
+        get_engine_cls, get_jacobian_colormap, get_parameters, read_parameters,
         set_elastix_dir, set_engine_dir)
 
 from test_structs import compare_rois
 
 # Define directory containing default parameter files.
 pfiles_dir = get_default_pfiles_dir()
 
@@ -359,14 +359,35 @@
     new_file = "tmp/tmp_pfile.txt"
     adjust_parameters(pfile, new_file, {"DefaultPixelValue": 10})
     assert os.path.exists(new_file)
     text = open(new_file).read()
     assert "(DefaultPixelValue 10)" in text
     os.remove(new_file)
 
+def test_get_parameters():
+    """Test parameter retrieval from an elastix parameter file."""
+    
+    pattern = "MI_Translation.txt"
+
+    params = {"DefaultPixelValue": 0}
+    parameters = get_parameters(pattern)
+    for key, value in params.items():
+        assert key in parameters
+        assert parameters[key] == value
+
+    params = {"DefaultPixelValue": 10}
+    parameters = get_parameters(pattern, params=params)
+    for key, value in params.items():
+        assert key in parameters
+        assert parameters[key] == value
+
+    with pytest.raises(IndexError) as error_info:
+        get_parameters(pattern, idx=5)
+    assert ("list index out of range" in str(error_info.value))
+
 @needs_elastix
 def test_shift_parameters():
     """Test shifting translation parameters by a given amount."""
 
     from skrt.registration import read_parameters, shift_translation_parameters
     reg = Registration("tmp/reg")
     input_file = reg.tfiles[reg.steps[0]]
@@ -598,15 +619,15 @@
 
     # Check that exception is raised if engine software not installed
     # in specified directory.
     for engine in engines:
         with pytest.raises(RuntimeError) as error_info:
             set_engine_dir(path="unknown", engine=engine)
         assert ("not implemented" in str(error_info.value)
-                or "executable(s) not found" in str(error_info.value))
+                or "not found" in str(error_info.value))
 
     # Check that exception is raised if engine name is unknown.
     with pytest.raises(RuntimeError) as error_info:
         set_engine_dir(path="unknown", engine="unknown")
     assert "executable(s) not found" in str(error_info.value)
```

### Comparing `scikit-rt-0.4.9/tests/test_roi_metrics.py` & `scikit-rt-0.5.0/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_segmentation.py` & `scikit-rt-0.5.0/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_structs.py` & `scikit-rt-0.5.0/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_synthetic_image.py` & `scikit-rt-0.5.0/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.9/tests/test_viewer.py` & `scikit-rt-0.5.0/tests/test_viewer.py`

 * *Files identical despite different names*

