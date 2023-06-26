# Comparing `tmp/ocf_datapipes-1.2.8.tar.gz` & `tmp/ocf_datapipes-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocf_datapipes-1.2.8.tar", last modified: Wed Mar 29 13:39:48 2023, max compression
+gzip compressed data, was "ocf_datapipes-1.2.9.tar", last modified: Thu Mar 30 06:53:20 2023, max compression
```

## Comparing `ocf_datapipes-1.2.8.tar` & `ocf_datapipes-1.2.9.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.966354 ocf_datapipes-1.2.8/ocf_datapipes/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.966354 ocf_datapipes-1.2.8/ocf_datapipes/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.966354 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/fake_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/nwp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/sun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/merge_batchml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/merge_numpy_examples_to_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/batch/merge_numpy_modalities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.966354 ocf_datapipes-1.2.8/ocf_datapipes/config/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/config/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/config/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/config/on_premises.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/config/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/nwp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/convert/satellite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/experimental/ensure_n_nwp_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/experimental/set_system_id_to_one.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/fake/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/fake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/load/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/gsp_national.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/nwp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/nwp_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.970354 ocf_datapipes-1.2.8/ocf_datapipes/load/pv/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/pv/live.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/pv/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/pv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/load/topographic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.974354 ocf_datapipes-1.2.8/ocf_datapipes/production/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/production/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/production/power_perceiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/production/xgnational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.974354 ocf_datapipes-1.2.8/ocf_datapipes/select/
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/drop_national_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/drop_overnight_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/drop_pv_sys_generating_overnight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/drop_pv_sys_with_only_nan_in_a_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/location_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/number_of_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/offset_t0.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/remove_bad_pv_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_live_t0_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_live_time_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_overlapping_time_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_pv_systems_on_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_spatial_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_t0_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_time_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/select_train_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/select/trim_dates_with_insufficent_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.978354 ocf_datapipes-1.2.8/ocf_datapipes/training/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.978354 ocf_datapipes-1.2.8/ocf_datapipes/training/datamodules/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/datamodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/datamodules/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/gsp_national.py
--rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/gsp_pv_satellite_nwp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_gsp_national.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_national.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_national_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_pv_national.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_pv_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/nwp_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/pseudo_irradience.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/pv_satellite_nwp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/training/simple_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.978354 ocf_datapipes-1.2.8/ocf_datapipes/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.978354 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.978354 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_topographic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_zeroed_future_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/align_gsp_to_5_min.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/change_np_float32.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/encode_space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/extend_timestamps_to_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/save_t0_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/sun_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_satellite_to_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_to_numpy_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_to_nwp_target_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/create_sun_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/create_time_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/get_contiguous_time_periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/remove_northern_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/interpolate_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/metnet_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_history_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/remove_nans.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/reproject_topographic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/eso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/pvlive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/utils/split/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/split/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/split/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/split/split.py
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.982354 ocf_datapipes-1.2.8/ocf_datapipes/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/validation/check_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/validation/check_for_nans.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/validation/check_statistical_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/ocf_datapipes/validation/check_vars_and_dims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.966354 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-29 13:39:48.000000 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-29 13:39:48.000000 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:39:48.000000 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-29 13:39:48.000000 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-29 13:39:48.000000 ocf_datapipes-1.2.8/ocf_datapipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:48.986354 ocf_datapipes-1.2.8/tests/transform/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_add_nwp_target_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_assign_daynight_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_convert_satellite_to_int8.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_convert_to_numpy_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_create_time_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_drop_nans.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_get_contiguous_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_metnet_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-29 13:39:37.000000 ocf_datapipes-1.2.8/tests/transform/xarray/test_time_picker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.190932 ocf_datapipes-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-30 06:53:20.190932 ocf_datapipes-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.170932 ocf_datapipes-1.2.9/ocf_datapipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.170932 ocf_datapipes-1.2.9/ocf_datapipes/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/fake_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/merge_batchml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/merge_numpy_examples_to_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/batch/merge_numpy_modalities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/config/on_premises.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/config/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/convert/satellite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/experimental/ensure_n_nwp_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/experimental/set_system_id_to_one.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/fake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/gsp_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.174932 ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/nwp_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.178932 ocf_datapipes-1.2.9/ocf_datapipes/load/pv/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/pv/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/pv/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/pv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/load/topographic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.178932 ocf_datapipes-1.2.9/ocf_datapipes/production/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/production/power_perceiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/production/xgnational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.178932 ocf_datapipes-1.2.9/ocf_datapipes/select/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/drop_national_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/drop_overnight_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/drop_pv_sys_generating_overnight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/drop_pv_sys_with_only_nan_in_a_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/location_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/number_of_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/offset_t0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/remove_bad_pv_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_live_t0_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_live_time_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_overlapping_time_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_pv_systems_on_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_spatial_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_t0_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_time_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/select_train_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/select/trim_dates_with_insufficent_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.182932 ocf_datapipes-1.2.9/ocf_datapipes/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.182932 ocf_datapipes-1.2.9/ocf_datapipes/training/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/datamodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/datamodules/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/gsp_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/gsp_pv_satellite_nwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_gsp_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_national_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_pv_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_pv_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/nwp_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/pseudo_irradience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/pv_satellite_nwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/training/simple_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.182932 ocf_datapipes-1.2.9/ocf_datapipes/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.182932 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.182932 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_topographic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_zeroed_future_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/align_gsp_to_5_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/change_np_float32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/encode_space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/extend_timestamps_to_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/save_t0_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/sun_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_satellite_to_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_to_numpy_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_to_nwp_target_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/create_sun_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/create_time_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/get_contiguous_time_periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/remove_northern_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/interpolate_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/metnet_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_history_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/remove_nans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/reproject_topographic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/eso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/pvlive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/utils/split/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/split/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/split/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/split/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/ocf_datapipes/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/validation/check_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/validation/check_for_nans.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/validation/check_statistical_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/ocf_datapipes/validation/check_vars_and_dims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.170932 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-30 06:53:20.000000 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-30 06:53:20.000000 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 06:53:20.000000 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-30 06:53:20.000000 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 06:53:20.000000 ocf_datapipes-1.2.9/ocf_datapipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 06:53:20.190932 ocf_datapipes-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.186932 ocf_datapipes-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-03-30 06:53:08.000000 ocf_datapipes-1.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.190932 ocf_datapipes-1.2.9/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:20.190932 ocf_datapipes-1.2.9/tests/transform/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_add_nwp_target_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_assign_daynight_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_convert_satellite_to_int8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_convert_to_numpy_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_create_time_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_drop_nans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_get_contiguous_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_metnet_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-30 06:53:09.000000 ocf_datapipes-1.2.9/tests/transform/xarray/test_time_picker.py
```

### Comparing `ocf_datapipes-1.2.8/LICENSE` & `ocf_datapipes-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/PKG-INFO` & `ocf_datapipes-1.2.9/ocf_datapipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocf_datapipes
-Version: 1.2.8
+Name: ocf-datapipes
+Version: 1.2.9
 Summary: Pytorch Datapipes built for use in Open Climate Fix's forecasting work
 Author: Jacob Bieker, Jack Kelly, Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocf_datapipes-1.2.8/README.md` & `ocf_datapipes-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/fake_batch.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/fake_batch.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/nwp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/satellite.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/sun.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/sun.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/fake/utils.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/fake/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/merge_numpy_examples_to_batch.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/merge_numpy_examples_to_batch.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/batch/merge_numpy_modalities.py` & `ocf_datapipes-1.2.9/ocf_datapipes/batch/merge_numpy_modalities.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/config/load.py` & `ocf_datapipes-1.2.9/ocf_datapipes/config/load.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/config/model.py` & `ocf_datapipes-1.2.9/ocf_datapipes/config/model.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/config/on_premises.yaml` & `ocf_datapipes-1.2.9/ocf_datapipes/config/on_premises.yaml`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/config/save.py` & `ocf_datapipes-1.2.9/ocf_datapipes/config/save.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/__init__.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/coordinates.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/coordinates.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/batch/pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/batch/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/numpy/pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/numpy/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/nwp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/convert/satellite.py` & `ocf_datapipes-1.2.9/ocf_datapipes/convert/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/experimental/ensure_n_nwp_variables.py` & `ocf_datapipes-1.2.9/ocf_datapipes/experimental/ensure_n_nwp_variables.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/experimental/set_system_id_to_one.py` & `ocf_datapipes-1.2.9/ocf_datapipes/experimental/set_system_id_to_one.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/__init__.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/configuration.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/configuration.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/database.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/database.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/gsp_national.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/gsp_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/gsp/utils.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/gsp/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/gfs.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/gfs.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/nwp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/nwp/nwp_id.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/nwp/nwp_id.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/pv/live.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/pv/live.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/pv/pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/pv/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/pv/utils.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/pv/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/satellite.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/load/topographic.py` & `ocf_datapipes-1.2.9/ocf_datapipes/load/topographic.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/production/power_perceiver.py` & `ocf_datapipes-1.2.9/ocf_datapipes/production/power_perceiver.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/production/xgnational.py` & `ocf_datapipes-1.2.9/ocf_datapipes/production/xgnational.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/__init__.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/drop_national_gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/drop_national_gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/drop_pv_sys_generating_overnight.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/drop_pv_sys_generating_overnight.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/drop_pv_sys_with_only_nan_in_a_day.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/drop_pv_sys_with_only_nan_in_a_day.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/location_picker.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/location_picker.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/number_of_location.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/number_of_location.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/offset_t0.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/offset_t0.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/remove_bad_pv_systems.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/remove_bad_pv_systems.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_channels.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_channels.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_id.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_id.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_live_t0_time.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_live_t0_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_live_time_slice.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_live_time_slice.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_overlapping_time_slices.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_overlapping_time_slices.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_pv_systems_on_capacity.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_pv_systems_on_capacity.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_spatial_slice.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_spatial_slice.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_t0_time.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_t0_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_time_periods.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_time_slice.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_time_slice.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/select_train_test.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/select_train_test.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/select/trim_dates_with_insufficent_data.py` & `ocf_datapipes-1.2.9/ocf_datapipes/select/trim_dates_with_insufficent_data.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/common.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/common.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/datamodules/default.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/datamodules/default.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/gsp_national.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/gsp_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/gsp_pv_satellite_nwp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/gsp_pv_satellite_nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_gsp_national.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_gsp_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_national.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_national_class.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_national_class.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_pv_national.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_pv_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/metnet_pv_site.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/metnet_pv_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
     used_datapipes = add_selected_time_slices_from_datapipes(used_datapipes)
 
     # Now do the extra processing
     pv_history = used_datapipes["pv"].normalize(normalize_fn=normalize_pv)
     pv_datapipe = used_datapipes["pv_future"].normalize(normalize_fn=normalize_pv)
     # Split into GSP for target, only national, and one for history
     pv_datapipe, pv_loc_datapipe = pv_datapipe.fork(2)
-    pv_loc_datapipe, pv_id_datapipe = LocationPicker(pv_loc_datapipe).fork(2)
+    loc_datapipe = LocationPicker(pv_loc_datapipe).sharding_filter() # Ensure each worker gets a different location
+    pv_loc_datapipe, pv_id_datapipe = loc_datapipe.fork(2)
     pv_history = pv_history.select_id(pv_id_datapipe, data_source_name="pv")
 
     if "nwp" in used_datapipes.keys():
         # take nwp time slices
         logger.debug("Take NWP time slices")
         nwp_datapipe = used_datapipes["nwp"].normalize(mean=NEW_NWP_MEAN, std=NEW_NWP_STD)
         pv_loc_datapipe, pv_nwp_image_loc_datapipe = pv_loc_datapipe.fork(2)
```

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/nwp_pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/nwp_pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/pseudo_irradience.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/pseudo_irradience.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/pv_satellite_nwp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/pv_satellite_nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/training/simple_pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/training/simple_pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/__init__.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_length.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_length.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_topographic_data.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_topographic_data.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/add_zeroed_future_pv.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/add_zeroed_future_pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/align_gsp_to_5_min.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/align_gsp_to_5_min.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/change_np_float32.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/change_np_float32.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/encode_space_time.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/encode_space_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/extend_timestamps_to_future.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/extend_timestamps_to_future.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/save_t0_time.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/save_t0_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/numpy/batch/sun_position.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/numpy/batch/sun_position.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/__init__.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_satellite_to_int.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_satellite_to_int.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_to_numpy_stack.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_to_numpy_stack.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/convert_to_nwp_target_times.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/convert_to_nwp_target_times.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/create_sun_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/create_sun_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/create_time_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/create_time_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/downsample.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/downsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/get_contiguous_time_periods.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/get_contiguous_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/gsp/remove_northern_gsp.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/gsp/remove_northern_gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/metnet_preprocessor.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/metnet_preprocessor.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/normalize.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/normalize.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_history_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_history_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/remove_nans.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/remove_nans.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/transform/xarray/reproject_topographic_data.py` & `ocf_datapipes-1.2.9/ocf_datapipes/transform/xarray/reproject_topographic_data.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/consts.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/consts.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/eso.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/eso.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/geospatial.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/geospatial.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/pvlive.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/pvlive.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/split/method.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/split/method.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/split/model.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/split/model.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/split/split.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/split/split.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/utils/utils.py` & `ocf_datapipes-1.2.9/ocf_datapipes/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/validation/check_equality.py` & `ocf_datapipes-1.2.9/ocf_datapipes/validation/check_equality.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/validation/check_for_nans.py` & `ocf_datapipes-1.2.9/ocf_datapipes/validation/check_for_nans.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes/validation/check_vars_and_dims.py` & `ocf_datapipes-1.2.9/ocf_datapipes/validation/check_vars_and_dims.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes.egg-info/PKG-INFO` & `ocf_datapipes-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocf-datapipes
-Version: 1.2.8
+Name: ocf_datapipes
+Version: 1.2.9
 Summary: Pytorch Datapipes built for use in Open Climate Fix's forecasting work
 Author: Jacob Bieker, Jack Kelly, Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocf_datapipes-1.2.8/ocf_datapipes.egg-info/SOURCES.txt` & `ocf_datapipes-1.2.9/ocf_datapipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/setup.py` & `ocf_datapipes-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="ocf_datapipes",
-    version="1.2.8",
+    version="1.2.9",
     license="MIT",
     description="Pytorch Datapipes built for use in Open Climate Fix's forecasting work",
     author="Jacob Bieker, Jack Kelly, Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `ocf_datapipes-1.2.8/tests/conftest.py` & `ocf_datapipes-1.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_add_nwp_target_time.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_add_nwp_target_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_assign_daynight_status.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_assign_daynight_status.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_convert_to_numpy_stack.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_convert_to_numpy_stack.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_downsample.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_downsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_drop_nans.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_drop_nans.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_get_contiguous_time_periods.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_get_contiguous_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_metnet_preprocessor.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_metnet_preprocessor.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_normalize.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_normalize.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-1.2.8/tests/transform/xarray/test_time_picker.py` & `ocf_datapipes-1.2.9/tests/transform/xarray/test_time_picker.py`

 * *Files identical despite different names*

