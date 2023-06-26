# Comparing `tmp/osm-flex-0.1.0.tar.gz` & `tmp/osm-flex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-flex-0.1.0.tar", last modified: Thu Jun 22 08:30:07 2023, max compression
+gzip compressed data, was "osm-flex-1.0.1.tar", last modified: Mon Jun 26 14:38:40 2023, max compression
```

## Comparing `osm-flex-0.1.0.tar` & `osm-flex-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:30:07.211353 osm-flex-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 08:29:52.000000 osm-flex-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 08:29:52.000000 osm-flex-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 08:30:07.211353 osm-flex-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 08:29:52.000000 osm-flex-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 08:29:52.000000 osm-flex-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:30:07.211353 osm-flex-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:30:07.207353 osm-flex-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:30:07.207353 osm-flex-0.1.0/src/osm_flex/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-22 08:29:52.000000 osm-flex-0.1.0/src/osm_flex/osmconf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:30:07.211353 osm-flex-0.1.0/src/osm_flex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 08:30:07.000000 osm-flex-0.1.0/src/osm_flex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 08:30:07.000000 osm-flex-0.1.0/src/osm_flex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:30:07.000000 osm-flex-0.1.0/src/osm_flex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 08:30:07.000000 osm-flex-0.1.0/src/osm_flex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 08:30:07.000000 osm-flex-0.1.0/src/osm_flex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:30:07.211353 osm-flex-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-22 08:29:52.000000 osm-flex-0.1.0/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-22 08:29:52.000000 osm-flex-0.1.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-22 08:29:52.000000 osm-flex-0.1.0/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:38:40.053650 osm-flex-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 14:38:27.000000 osm-flex-1.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 14:38:27.000000 osm-flex-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-26 14:38:40.053650 osm-flex-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-26 14:38:27.000000 osm-flex-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 14:38:27.000000 osm-flex-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:38:40.053650 osm-flex-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:38:40.049649 osm-flex-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:38:40.049649 osm-flex-1.0.1/src/osm_flex/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-26 14:38:27.000000 osm-flex-1.0.1/src/osm_flex/osmconf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:38:40.053650 osm-flex-1.0.1/src/osm_flex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-26 14:38:40.000000 osm-flex-1.0.1/src/osm_flex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-26 14:38:40.000000 osm-flex-1.0.1/src/osm_flex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:38:40.000000 osm-flex-1.0.1/src/osm_flex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 14:38:40.000000 osm-flex-1.0.1/src/osm_flex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 14:38:40.000000 osm-flex-1.0.1/src/osm_flex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:38:40.053650 osm-flex-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-26 14:38:27.000000 osm-flex-1.0.1/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-26 14:38:27.000000 osm-flex-1.0.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-26 14:38:27.000000 osm-flex-1.0.1/tests/test_extract.py
```

### Comparing `osm-flex-0.1.0/LICENSE` & `osm-flex-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/pyproject.toml` & `osm-flex-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "osm-flex"
-version = "0.1.0"
+version = "1.0.1"
 maintainers = [
   { name = "Elco Koks", email = "elco.koks@vu.nl" },
 ]
 description = "Python package for flexible data extraction from OpenStreetMap"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `osm-flex-0.1.0/src/osm_flex/__init__.py` & `osm-flex-1.0.1/src/osm_flex/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/src/osm_flex/clip.py` & `osm-flex-1.0.1/src/osm_flex/clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,29 +158,29 @@
         a string/Path to the .poly file path delimiting the bounds.
     osmpbf_clip_from: str or pathlib.Path
         file path to planet.osm.pbf or other osm.pbf file to clip
     osmpbf_output : str or pathlib.Path
         file path (incl. name & ending) under which extract will be stored
     """
 
-    if isinstance(shape, (pathlib.PosixPath, str)):
+    if isinstance(shape, (pathlib.Path, str)):
         return [str(OSMCONVERT_PATH), str(osmpbf_clip_from), f'-B={str(shape)}',
-                '--complete-ways', '--complete-multipolygons', 
+                '--complete-ways', '--complete-multipolygons',
                 f'-o={osmpbf_output}'
                 ]
     if isinstance(shape[0], (float, int)):
-        return [str(OSMCONVERT_PATH), str(osmpbf_clip_from), 
+        return [str(OSMCONVERT_PATH), str(osmpbf_clip_from),
                 '-b='+str(shape[0])+','+str(shape[1])+','+str(shape[2])+','+str(shape[3]),
                 '--complete-ways', '--complete-multipolygons',
                 f'-o={osmpbf_output}'
                 ]
-    
+
 def _osmconvert_clip(shape, osmpbf_clip_from, osmpbf_output,
                      overwrite=False):
-        
+
     osmpbf_clip_from = pathlib.Path(osmpbf_clip_from)
     if not osmpbf_clip_from.suffix:
         osmpbf_clip_from = osmpbf_clip_from.with_suffix('.osm.pbf')
     if not osmpbf_clip_from.is_file():
         raise ValueError(f"OSM file {osmpbf_clip_from} to clip from not found.")
 
     if ((not pathlib.Path(osmpbf_output).is_file()) or
@@ -207,29 +207,29 @@
         list containing [xmin, ymin, xmax, ymax] for a bounding box or
         a string/Path to the .poly file path delimiting the bounds.
     osmpbf_clip_from: str or pathlib.Path
         file path to planet.osm.pbf or other osm.pbf file to clip
     osmpbf_output : str or pathlib.Path
         file path (incl. name & ending) under which extract will be stored
     """
-    if isinstance(shape, (pathlib.PosixPath, str)):
+    if isinstance(shape, (pathlib.Path, str)):
         return ['osmosis', '--read-pbf', 'file='+str(osmpbf_clip_from),
             '--bounding-polygon', 'file='+str(shape), '--write-pbf',
             'file='+str(osmpbf_output)]
     if isinstance(shape[0], (float, int)):
         return['osmosis', '--read-pbf', 'file='+str(osmpbf_clip_from),
             '--bounding-box', f'top={shape[3]}', f'left={shape[0]}',
             f'bottom={shape[1]}', f'right={shape[2]}',
             '--write-pbf', 'file='+str(osmpbf_output)]
 
     raise ValueError('''shape does not have the correct format.
-                        Only bounding boxes, shapely (multi-)polygons or 
+                        Only bounding boxes, shapely (multi-)polygons or
                         filepaths to .poly files are allowed''')
 
-    
+
 def _osmosis_clip(shape, osmpbf_clip_from, osmpbf_output,
                   overwrite=False):
     """
     Runs the command line tool osmosis to cut out all map info within
     shape (bounding box or poygon(s)), from a bigger parent file.
 
     If your device doesn't have osmosis yet, see installation instructions:
```

### Comparing `osm-flex-0.1.0/src/osm_flex/config.py` & `osm-flex-1.0.1/src/osm_flex/config.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/src/osm_flex/download.py` & `osm-flex-1.0.1/src/osm_flex/download.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/src/osm_flex/extract.py` & `osm-flex-1.0.1/src/osm_flex/extract.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/src/osm_flex/osmconf.ini` & `osm-flex-1.0.1/src/osm_flex/osmconf.ini`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/tests/test_clip.py` & `osm-flex-1.0.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/tests/test_download.py` & `osm-flex-1.0.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `osm-flex-0.1.0/tests/test_extract.py` & `osm-flex-1.0.1/tests/test_extract.py`

 * *Files identical despite different names*

