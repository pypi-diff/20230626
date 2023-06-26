# Comparing `tmp/Jord-0.0.9.tar.gz` & `tmp/Jord-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.0.9.tar", last modified: Fri Jun 23 15:08:07 2023, max compression
+gzip compressed data, was "Jord-0.1.0.tar", last modified: Mon Jun 26 14:05:07 2023, max compression
```

## Comparing `Jord-0.0.9.tar` & `Jord-0.1.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.417179 Jord-0.0.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 15:08:02.000000 Jord-0.0.9/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-23 15:08:02.000000 Jord-0.0.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 15:08:02.000000 Jord-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 15:08:07.433179 Jord-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-23 15:08:02.000000 Jord-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 15:08:02.000000 Jord-0.0.9/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:08:02.000000 Jord-0.0.9/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/geometry_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/rasters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/spatialite_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/spatialite_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 15:08:02.000000 Jord-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:08:02.000000 Jord-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 15:08:07.433179 Jord-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-23 15:08:02.000000 Jord-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.823305 Jord-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 14:05:03.000000 Jord-0.1.0/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-26 14:05:03.000000 Jord-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 14:05:03.000000 Jord-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-26 14:05:07.839305 Jord-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 14:05:03.000000 Jord-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 14:05:03.000000 Jord-0.1.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:05:03.000000 Jord-0.1.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/geometry_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/rasters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/jord/spatialite_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/spatialite_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 14:05:03.000000 Jord-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 14:05:03.000000 Jord-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 14:05:07.839305 Jord-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-26 14:05:03.000000 Jord-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/test_sanity.py
```

### Comparing `Jord-0.0.9/.github/CODE_OF_CONDUCT.md` & `Jord-0.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/.github/CONTRIBUTING.md` & `Jord-0.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/Jord.egg-info/PKG-INFO` & `Jord-0.1.0/Jord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.9 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.0 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.0.9/Jord.egg-info/SOURCES.txt` & `Jord-0.1.0/Jord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/LICENSE.md` & `Jord-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/PKG-INFO` & `Jord-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.9 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.0 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.0.9/README.md` & `Jord-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/SECURITY.md` & `Jord-0.1.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/__init__.py` & `Jord-0.1.0/jord/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pkg_resources
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
```

### Comparing `Jord-0.0.9/jord/gdal_utilities/__init__.py` & `Jord-0.1.0/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/gdal_utilities/cloning.py` & `Jord-0.1.0/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/gdal_utilities/context.py` & `Jord-0.1.0/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/gdal_utilities/conversion.py` & `Jord-0.1.0/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/gdal_utilities/importing.py` & `Jord-0.1.0/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/gdal_utilities/persistence.py` & `Jord-0.1.0/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/geojson_utilities/geometry_types.py` & `Jord-0.1.0/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/geopandas_utilities/geometry_filtering.py` & `Jord-0.1.0/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/__init__.py` & `Jord-0.1.0/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/categorisation.py` & `Jord-0.1.0/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.1.0/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.1.0/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/enums.py` & `Jord-0.1.0/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/geometry_types.py` & `Jord-0.1.0/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/actions.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/environment.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/models.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/signals.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.1.0/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py` & `Jord-0.1.0/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qgis_utilities/styling.py` & `Jord-0.1.0/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qlive_utilities/client.py` & `Jord-0.1.0/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qlive_utilities/procedures.py` & `Jord-0.1.0/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qlive_utilities/serialisation.py` & `Jord-0.1.0/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qlive_utilities/uri_utilities.py` & `Jord-0.1.0/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/qt_utilities/enums.py` & `Jord-0.1.0/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/__init__.py` & `Jord-0.1.0/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/clamp.py` & `Jord-0.1.0/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/geometry_types.py` & `Jord-0.1.0/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/lines.py` & `Jord-0.1.0/jord/shapely_utilities/lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,33 @@
            Created on 1/23/23
            """
 
 __all__ = [
     "to_lines",
     "to_single_line",
     "explode_line",
+    "explode_lines",
     "strip_multiline_dangles",
     "strip_line_dangles",
+    "azimuth",
+    "linestring_azimuth",
 ]
 
 import collections
-from typing import Union, List, Sequence
+import logging
+from typing import Union, List, Sequence, Iterable
 
 import shapely.ops
 from shapely.geometry import LineString, MultiLineString, Point, MultiPoint, box
 from shapely.geometry.base import BaseGeometry
 
 from jord.shapely_utilities.points import (
     unique_line_points,
     nearest_neighbor_within,
+    azimuth,
 )
 
 
 def to_single_line(s: Union[LineString, MultiLineString]) -> LineString:
     """
     assume that lines are ordered, NOTE closes of gaps!
 
@@ -211,29 +216,49 @@
                     working_segments.append(s2)
 
         working_multi = MultiLineString(working_segments)
 
     return working_multi
 
 
-def explode_line(line: LineString) -> List[LineString]:
+def explode_line(line: Union[LineString, MultiLineString]) -> List[LineString]:
     """
 
     :param line:
     :return:
     """
+
+    if isinstance(line, MultiLineString):
+        out = []
+        for ls in line.geoms:
+            out.extend(explode_line(ls))
+        return out
+
     out = []
     for pt1, pt2 in zip(
         line.coords, line.coords[1:]
     ):  # iterate from first cord, iterate from second coords to get
         # endpoints of each segment
         out.append(LineString([pt1, pt2]))
     return out
 
 
+def explode_lines(
+    lines: Iterable[Union[LineString, MultiLineString]]
+) -> list[LineString]:
+    """
+    :param lines: List of LineStrings or MultiLineStrings to be exploded
+    :return: Exploded LineStrings
+    """
+    out = []
+    for ls in lines:
+        out.extend(explode_line(ls))
+    return out
+
+
 def find_isolated_endpoints(
     lines: Sequence[Union[LineString, MultiLineString]],
 ) -> Sequence[Point]:
     """
     Find endpoints of lines that don't touch another line.
 
     :param lines: A list of LineStrings or a MultiLineString
@@ -430,14 +455,35 @@
     :param of: The LineString which must be touched
     :param lines: List of LineStrings in which to search for neighbors
     :return: list of indices, so that all lines[indices] touch the LineString of
     """
     return [line for line in (lines) if line.touches(of)]
 
 
+def linestring_azimuth(linestring: LineString, verbose: bool = False) -> float:
+    """
+    # Calculates the angle of a LineString in degrees, meant for linestrings with only two vertices.
+
+    :param verbose:
+    :param linestring: Shapely linestring to get the angle of.
+    :return: modulo_angle: The angle of the linestring, between 0 and 180 degrees
+    """
+    coords = linestring.coords
+    num_coords = len(coords)
+
+    assert num_coords > 1
+
+    if verbose and num_coords > 2:
+        logging.warning(
+            f"Linestring has more than 2 vertices {num_coords}, calculating angle of first and last vertices"
+        )
+
+    return azimuth(Point(coords[0]), Point(coords[-1]))
+
+
 if __name__ == "__main__":
 
     def iashdh():
         print(
             to_single_line(MultiLineString([[[0, 0], [0, 1]], [[0, 2], [0, 3]]]))
         )  # LINESTRING (0 0, 0 1, 0 2, 0 3)
 
@@ -446,8 +492,26 @@
 
         pol1 = MultiPolygon([Point(0, 0).buffer(2.0), Point(1, 1).buffer(2.0)])
         pol2 = Point(7, 8).buffer(1.0)
         pols = [pol1, pol2]
 
         print(to_lines(pols))
 
-    ausdh()
+    def juashud():
+        print(
+            explode_lines(
+                [
+                    MultiLineString([[[0, 0], [0, 1]], [[0, 2], [0, 3]]]),
+                    MultiLineString(
+                        [
+                            [[0, 0], [0, 1]],
+                            [[0, 2], [0, 3]],
+                            [[0, 1], [1, 2], [2, 3], [3, 4]],
+                        ]
+                    ),
+                    MultiLineString([[[0, 0], [0, 1]], [[0, 2], [0, 3]]]),
+                ]
+            )
+        )
+
+    juashud()
+    # ausdh()
```

### Comparing `Jord-0.0.9/jord/shapely_utilities/mirroring.py` & `Jord-0.1.0/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/morphology.py` & `Jord-0.1.0/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/projection.py` & `Jord-0.1.0/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.1.0/jord/shapely_utilities/sanitise_poly.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/jord/shapely_utilities/transformation.py` & `Jord-0.1.0/jord/shapely_utilities/transformation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from typing import List, Sequence
+from typing import List, Sequence, Iterable, Union
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import transform
 import pyproj
 
 __all__ = ["crs_transform_shapely"]
 
 
 def crs_transform_shapely(
-    geoms: Sequence[BaseGeometry],
+    geoms: Union[BaseGeometry, Iterable[BaseGeometry]],
     from_coordinate_system: str,
     to_coordinate_system: str,
-) -> List[BaseGeometry]:
+) -> Union[BaseGeometry, List[BaseGeometry]]:
     """
     Project space geometries from one coordinate system to another
 
     :param geoms: A list of SpacePolygons to project
     :param from_coordinate_system: The source coordinate system
     :param to_coordinate_system: The destination coordinate system
     :return: A list of SpacePolygons projected
     """
 
     source = pyproj.CRS(from_coordinate_system)
     destination = pyproj.CRS(to_coordinate_system)
     projection = pyproj.Transformer.from_crs(
         source, destination, always_xy=True
     ).transform
+    #    project = pyproj.Transformer.from_proj(
+    #    pyproj.Proj(init="epsg:4326"),  # source coordinate system
+    #    pyproj.Proj(init="epsg:3857"),  # destination coordinate system
+    # )
 
-    return [transform(projection, geometry) for geometry in geoms]
+    if isinstance(geoms, Iterable):
+        return [transform(projection, geometry) for geometry in geoms]
+
+    return transform(projection, geoms)
```

### Comparing `Jord-0.0.9/setup.py` & `Jord-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.9/tests/test_import.py` & `Jord-0.1.0/tests/test_import.py`

 * *Files identical despite different names*

