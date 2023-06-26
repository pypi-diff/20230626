# Comparing `tmp/tondortools-1.0.8.tar.gz` & `tmp/tondortools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tondortools-1.0.8.tar", last modified: Mon Sep 19 13:20:49 2022, max compression
+gzip compressed data, was "dist/tondortools-1.0.9.tar", last modified: Sat Oct 22 11:35:39 2022, max compression
```

## Comparing `tondortools-1.0.8.tar` & `tondortools-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-09-19 13:20:49.000000 tondortools-1.0.8/
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      925 2022-06-24 15:36:58.000000 tondortools-1.0.8/setup.py
-drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools/
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     2954 2022-06-24 15:36:59.000000 tondortools-1.0.8/tondortools/postgres.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       21 2022-09-19 13:20:47.000000 tondortools-1.0.8/tondortools/__init__.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     8979 2022-06-24 15:36:59.000000 tondortools-1.0.8/tondortools/creodias.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)    37100 2022-09-19 13:20:47.000000 tondortools-1.0.8/tondortools/tool.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     1288 2022-06-24 15:36:59.000000 tondortools-1.0.8/tondortools/grassland.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)    12288 2022-06-24 15:36:59.000000 tondortools-1.0.8/tondortools/geo.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      748 2022-06-24 15:36:59.000000 tondortools-1.0.8/tondortools/lsru.py
-drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools/tiles_gpkg/
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)        0 2022-06-24 15:36:58.000000 tondortools-1.0.8/tondortools/tiles_gpkg/__init__.py
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      122 2022-06-24 14:08:51.000000 tondortools-1.0.8/README.md
-drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools.egg-info/
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       12 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools.egg-info/top_level.txt
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)        1 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools.egg-info/dependency_links.txt
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      349 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools.egg-info/SOURCES.txt
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      677 2022-09-19 13:20:49.000000 tondortools-1.0.8/tondortools.egg-info/PKG-INFO
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      677 2022-09-19 13:20:49.000000 tondortools-1.0.8/PKG-INFO
--rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       38 2022-09-19 13:20:49.000000 tondortools-1.0.8/setup.cfg
+drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-10-22 11:35:39.000000 tondortools-1.0.9/
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      925 2022-06-24 15:36:58.000000 tondortools-1.0.9/setup.py
+drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools/
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     2954 2022-06-24 15:36:59.000000 tondortools-1.0.9/tondortools/postgres.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       21 2022-10-22 11:32:36.000000 tondortools-1.0.9/tondortools/__init__.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     8979 2022-06-24 15:36:59.000000 tondortools-1.0.9/tondortools/creodias.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)    37122 2022-10-22 11:25:56.000000 tondortools-1.0.9/tondortools/tool.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)     1288 2022-06-24 15:36:59.000000 tondortools-1.0.9/tondortools/grassland.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)    12288 2022-06-24 15:36:59.000000 tondortools-1.0.9/tondortools/geo.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      748 2022-06-24 15:36:59.000000 tondortools-1.0.9/tondortools/lsru.py
+drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools/tiles_gpkg/
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)        0 2022-06-24 15:36:58.000000 tondortools-1.0.9/tondortools/tiles_gpkg/__init__.py
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      122 2022-06-24 14:08:51.000000 tondortools-1.0.9/README.md
+drwxrwxr-x   0 siv0021   (1000) siv0021   (1000)        0 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools.egg-info/
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       12 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools.egg-info/top_level.txt
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)        1 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools.egg-info/dependency_links.txt
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      349 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools.egg-info/SOURCES.txt
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      677 2022-10-22 11:35:39.000000 tondortools-1.0.9/tondortools.egg-info/PKG-INFO
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)      677 2022-10-22 11:35:39.000000 tondortools-1.0.9/PKG-INFO
+-rw-rw-r--   0 siv0021   (1000) siv0021   (1000)       38 2022-10-22 11:35:39.000000 tondortools-1.0.9/setup.cfg
```

### Comparing `tondortools-1.0.8/setup.py` & `tondortools-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools/postgres.py` & `tondortools-1.0.9/tondortools/postgres.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools/creodias.py` & `tondortools-1.0.9/tondortools/creodias.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools/tool.py` & `tondortools-1.0.9/tondortools/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,31 +14,41 @@
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from shutil import copy
 from shutil import copytree
 from tempfile import mkdtemp
 
-import osgeo.gdal as gdal
-import ogr, osr
+try:
+    import ogr
+except ImportError:
+    from osgeo import ogr
+
+try:
+    import osr
+except ImportError:
+    from osgeo import osr
+
+try:
+    import gdal
+except ImportError:
+    from osgeo import gdal
+
 import numpy as np
 from shapely.geometry import box
 
 KEEP_FILENAME = ".tondor_keep"
 
 
 log = logging.getLogger(__name__)
 
-
 def run_subprocess(args, work_dir):
     log.debug("Calling subprocess, args={:s}.".format(repr(args)))
-    pr = subprocess.run(args, cwd=work_dir, check=False)
-    log.info("Subprocess exited with code {:d}, args={:s}.".format(pr.returncode, repr(args)))
-    pr.check_returncode()
-
+    cmd_output = subprocess.run(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    log.info("Subprocess exited with code {:d}, args={:s}.".format(cmd_output.returncode, repr(args)))
 
 def log_subprocess(args, work_dir, log_filepath, timeout=None):
     log.debug("Calling subprocess: {:s}, logging to {:s}.".format(repr(args), str(log_filepath)))
     with open(str(log_filepath), "at", encoding="utf-8") as logf:
         logf.write("\n{:s} Calling subprocess: {:s}.\n".format(datetime.utcnow().isoformat()[:23], repr(args)))
         logf.flush()
         pr = subprocess.run(args, cwd=work_dir, stdout=logf, stderr=logf, timeout=timeout, check=False)
@@ -364,50 +374,41 @@
         copy_singlefile_from_archive(scrfiles_path, copied_path)
 
 def copy_singlefile_from_archive(scrfile_path, dstfile_path):
     shutil.copy(str(scrfile_path), str(dstfile_path))
 #################################################################################################
 #################################################################################################
 
-def read_raster_info(raster_filepath):
-    ds = gdal.Open(str(raster_filepath))
-
-    gt = ds.GetGeoTransform()
-    ulx_raster = gt[0]
-    uly_raster = gt[3]
-    lrx_raster = gt[0] + gt[1] * ds.RasterXSize + gt[2] * ds.RasterYSize
-    lry_raster = gt[3] + gt[4] * ds.RasterXSize + gt[5] * ds.RasterYSize
-    imagery_extent_box = box(lrx_raster, uly_raster, ulx_raster, lry_raster)
-    ds = None
-
-    xmin = gt[0]
-    ymax = gt[3]
-    pixel_width = gt[1]
-    yres = gt[5]
-
-    projection = ds.GetProjection()
-    datatype = ds.GetRasterBand(1).DataType
-    n_bands = ds.RasterCount
-    epsg = ds.GetSpatialRef().GetAuthorityCode(None)
-
-    return (xmin, ymax, ds.RasterXSize, ds.RasterYSize, pixel_width, projection, epsg, datatype, n_bands, imagery_extent_box)
-
 def reproject_multibandraster_toextent(composite_filepath, warped_filepath, target_epsg, pixel_size, xmin, xmax, ymin, ymax, work_dir, method ='bilinear'):
 
     cmd = ["gdalwarp",
            "-t_srs", "EPSG:{}".format(target_epsg),
            "-tr", str(pixel_size), str(pixel_size),
            "-te",str(xmin),str(ymin),str(xmax),str(ymax),
            "-r", method,
            "-co", "COMPRESS=DEFLATE",
            str(composite_filepath),
            str(warped_filepath)
            ]
     run_subprocess(cmd, work_dir)
 
+def reproject_multibandraster_toextent_withnodata(composite_filepath, warped_filepath, target_epsg, pixel_size, xmin, xmax, ymin, ymax, work_dir, nodata_value, method ='bilinear'):
+
+    cmd = ["gdalwarp",
+           "-t_srs", "EPSG:{}".format(target_epsg),
+           "-tr", str(pixel_size), str(pixel_size),
+           "-te",str(xmin),str(ymin),str(xmax),str(ymax),
+           "-r", method,
+           "-ot", "Float32",
+           "-dstnodata", nodata_value,
+           "-co", "COMPRESS=DEFLATE",
+           str(composite_filepath),
+           str(warped_filepath)
+           ]
+    run_subprocess(cmd, work_dir)
 
 def reproject_multibandraster(composite_filepath, warped_filepath, target_epsg, pixel_size, work_dir, method ='bilinear'):
 
     cmd = ["gdalwarp",
            "-t_srs", "EPSG:{}".format(target_epsg),
            "-tr", str(pixel_size), str(pixel_size),
            "-r", method,
```

### Comparing `tondortools-1.0.8/tondortools/grassland.py` & `tondortools-1.0.9/tondortools/grassland.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools/geo.py` & `tondortools-1.0.9/tondortools/geo.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools/lsru.py` & `tondortools-1.0.9/tondortools/lsru.py`

 * *Files identical despite different names*

### Comparing `tondortools-1.0.8/tondortools.egg-info/PKG-INFO` & `tondortools-1.0.9/tondortools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tondortools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package inludes tools for Tondor
 Home-page: https://github.com/gisat/tondor_tools
 Author: Michal Opetal, Sivasankar Arul
 Author-email: michal.opletal@gisat.cz, sivasankar.arul@gisat.cz
 License: MIT
 Description: Tondor - Tool
```

### Comparing `tondortools-1.0.8/PKG-INFO` & `tondortools-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tondortools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package inludes tools for Tondor
 Home-page: https://github.com/gisat/tondor_tools
 Author: Michal Opetal, Sivasankar Arul
 Author-email: michal.opletal@gisat.cz, sivasankar.arul@gisat.cz
 License: MIT
 Description: Tondor - Tool
```

