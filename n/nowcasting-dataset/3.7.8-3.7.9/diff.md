# Comparing `tmp/nowcasting_dataset-3.7.8.tar.gz` & `tmp/nowcasting_dataset-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_dataset-3.7.8.tar", last modified: Wed Aug  3 14:33:59 2022, max compression
+gzip compressed data, was "nowcasting_dataset-3.7.9.tar", last modified: Fri Aug  5 08:03:38 2022, max compression
```

## Comparing `nowcasting_dataset-3.7.8.tar` & `nowcasting_dataset-3.7.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.688576 nowcasting_dataset-3.7.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-03 14:33:30.000000 nowcasting_dataset-3.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-03 14:33:30.000000 nowcasting_dataset-3.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-08-03 14:33:59.688576 nowcasting_dataset-3.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8433 2022-08-03 14:33:30.000000 nowcasting_dataset-3.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-03 14:33:30.000000 nowcasting_dataset-3.7.8/extra-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.680576 nowcasting_dataset-3.7.8/nowcasting_dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.680576 nowcasting_dataset-3.7.8/nowcasting_dataset/config/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/gcp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/load.py
--rw-r--r--   0 runner    (1001) docker     (121)    26498 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/on_premises.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/config/save.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20475 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     6433 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/datasource_output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26659 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7510 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/eso.py
--rw-r--r--   0 runner    (1001) docker     (121)    24790 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/gsp_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/gsp_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/live.py
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/pvlive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/metadata/metadata_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9679 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/nwp_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/nwp_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/format_images.py
--rw-r--r--   0 runner    (1001) docker     (121)    12788 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/optical_flow_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/optical_flow_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/live.py
--rw-r--r--   0 runner    (1001) docker     (121)    21794 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/pv_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/pv_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20793 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/satellite_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/satellite_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5401 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/raw_data_load_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/sun_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/sun_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/topographic_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/topographic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13543 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8015 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/split.py
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/xr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.684576 nowcasting_dataset-3.7.8/nowcasting_dataset/filesystem/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/filesystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/geospatial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.688576 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    21493 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    11555 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/manager_live.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/square.py
--rw-r--r--   0 runner    (1001) docker     (121)    12645 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     8745 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/nowcasting_dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.680576 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-08-03 14:33:59.000000 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-08-03 14:33:59.000000 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 14:33:59.000000 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-08-03 14:33:59.000000 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 14:33:59.000000 nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 14:33:59.688576 nowcasting_dataset-3.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-08-03 14:33:46.000000 nowcasting_dataset-3.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:59.688576 nowcasting_dataset-3.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/test_square.py
--rw-r--r--   0 runner    (1001) docker     (121)     7249 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-08-03 14:33:31.000000 nowcasting_dataset-3.7.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8433 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/extra-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.308902 nowcasting_dataset-3.7.9/nowcasting_dataset/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.308902 nowcasting_dataset-3.7.9/nowcasting_dataset/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/gcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26498 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/on_premises.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/config/save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.308902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20475 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6433 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/datasource_output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26659 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7510 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/eso.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24790 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/gsp_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/gsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/live.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/pvlive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/metadata/metadata_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9679 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/nwp_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/nwp_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/format_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12788 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/optical_flow_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/optical_flow_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/live.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21794 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/pv_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/pv_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20793 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/satellite_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/satellite_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5401 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/raw_data_load_save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/sun_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/sun_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/topographic_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/topographic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13543 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.312902 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8015 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/split.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/xr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/nowcasting_dataset/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/filesystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/geospatial.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5410 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21493 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11555 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/manager_live.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/square.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12645 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8745 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/nowcasting_dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.308902 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-08-05 08:03:38.000000 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-08-05 08:03:38.000000 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 08:03:38.000000 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-08-05 08:03:38.000000 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-05 08:03:38.000000 nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-08-05 08:03:25.000000 nowcasting_dataset-3.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:38.316902 nowcasting_dataset-3.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-08-05 08:03:09.000000 nowcasting_dataset-3.7.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-08-05 08:03:10.000000 nowcasting_dataset-3.7.9/tests/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-05 08:03:10.000000 nowcasting_dataset-3.7.9/tests/test_square.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7249 2022-08-05 08:03:10.000000 nowcasting_dataset-3.7.9/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-08-05 08:03:10.000000 nowcasting_dataset-3.7.9/tests/test_utils.py
```

### Comparing `nowcasting_dataset-3.7.8/LICENSE` & `nowcasting_dataset-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/PKG-INFO` & `nowcasting_dataset-3.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_dataset
-Version: 3.7.8
+Version: 3.7.9
 Summary: Nowcasting Dataset
 Author: Jack Kelly, Peter Dudfield, Jacob Bieker
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
```

### Comparing `nowcasting_dataset-3.7.8/README.md` & `nowcasting_dataset-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/config/gcp.yaml` & `nowcasting_dataset-3.7.9/nowcasting_dataset/config/gcp.yaml`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/config/load.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/config/load.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/config/model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/config/model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/config/on_premises.yaml` & `nowcasting_dataset-3.7.9/nowcasting_dataset/config/on_premises.yaml`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/config/save.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/config/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/consts.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/consts.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/datasource_output.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/datasource_output.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/batch.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/batch.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/coordinates.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/coordinates.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/fake/utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/fake/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/eso.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/eso.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/gsp_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/gsp_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/gsp_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/gsp_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/live.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/live.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/gsp/pvlive.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/gsp/pvlive.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/map.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/map.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/metadata/metadata_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/metadata/metadata_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/nwp_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/nwp_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/nwp/nwp_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/nwp/nwp_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/format_images.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/format_images.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/optical_flow_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/optical_flow_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/optical_flow/optical_flow_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/optical_flow/optical_flow_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/live.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/live.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/pv_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/pv_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/pv_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/pv_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/pv/utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/pv/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/satellite_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/satellite_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/satellite/satellite_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/satellite/satellite_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/raw_data_load_save.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/raw_data_load_save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/sun_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/sun_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/sun/sun_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/sun/sun_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/topographic_data_source.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/topographic_data_source.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/data_sources/topographic/topographic_model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/data_sources/topographic/topographic_model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/batch.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/batch.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/method.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/method.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/model.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/model.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/split/split.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/split/split.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/dataset/xr_utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/dataset/xr_utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/filesystem/utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/filesystem/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/geospatial.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/geospatial.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/manager/base.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/manager/base.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/manager/manager.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/manager/manager.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/manager/manager_live.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/manager/manager_live.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/manager/utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/manager/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/square.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/square.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/time.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/time.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset/utils.py` & `nowcasting_dataset-3.7.9/nowcasting_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/PKG-INFO` & `nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-dataset
-Version: 3.7.8
+Version: 3.7.9
 Summary: Nowcasting Dataset
 Author: Jack Kelly, Peter Dudfield, Jacob Bieker
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
```

### Comparing `nowcasting_dataset-3.7.8/nowcasting_dataset.egg-info/SOURCES.txt` & `nowcasting_dataset-3.7.9/nowcasting_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/setup.py` & `nowcasting_dataset-3.7.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 extra_install_requires = (this_directory / "extra-requirements.txt").read_text().splitlines()
 
 setup(
     name="nowcasting_dataset",
-    version="3.7.8",
+    version="3.7.9",
     license="MIT",
     description="Nowcasting Dataset",
     author="Jack Kelly, Peter Dudfield, Jacob Bieker",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `nowcasting_dataset-3.7.8/tests/conftest.py` & `nowcasting_dataset-3.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/tests/test_geospatial.py` & `nowcasting_dataset-3.7.9/tests/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/tests/test_square.py` & `nowcasting_dataset-3.7.9/tests/test_square.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/tests/test_time.py` & `nowcasting_dataset-3.7.9/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `nowcasting_dataset-3.7.8/tests/test_utils.py` & `nowcasting_dataset-3.7.9/tests/test_utils.py`

 * *Files identical despite different names*

