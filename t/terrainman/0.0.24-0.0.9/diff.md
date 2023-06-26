# Comparing `tmp/terrainman-0.0.24.tar.gz` & `tmp/terrainman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrainman-0.0.24.tar", max compression
+gzip compressed data, was "terrainman-0.0.9.tar", max compression
```

## Comparing `terrainman-0.0.24.tar` & `terrainman-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.24/LICENSE
--rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.24/README.md
--rw-r--r--   0        0        0     1001 2023-06-26 03:00:09.909342 terrainman-0.0.24/pyproject.toml
--rw-r--r--   0        0        0      654 2023-05-11 16:30:21.002263 terrainman-0.0.24/src/terrainman/__init__.py
--rw-r--r--   0        0        0    10693 2023-05-11 16:30:32.969038 terrainman-0.0.24/src/terrainman/tile_io.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 terrainman-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.9/LICENSE
+-rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.9/README.md
+-rw-r--r--   0        0        0      969 2023-05-10 17:54:37.102852 terrainman-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-08 00:34:50.893087 terrainman-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     9650 2023-05-09 02:23:25.027650 terrainman-0.0.9/src/tile_io.py
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 terrainman-0.0.9/PKG-INFO
```

### Comparing `terrainman-0.0.24/LICENSE` & `terrainman-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terrainman-0.0.24/pyproject.toml` & `terrainman-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "terrainman"
-version = "0.0.24"
+version = "0.0.9"
 description = "A package for downloading and managing high-fidelity terrain files"
 authors = ["Liam Robinson <robin502@purdue.edu>"]
 readme = "README.md"
-packages = [{include = "terrainman", from = "src"}]
-exclude = ['src/terrainman/data', 'src/terrainman/__pycache']
+packages = [{include = "src"}]
+include = [{path = "src", format = "sdist"}]
 documentation = "https://python-poetry.org/docs/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-numpy = "^1.24.2"
-scipy = "^1.10.1"
-pyvista = "^0.38.5"
-python-dotenv = "^1.0.0"
-trimesh = "^3.21.5"
-rtree = "^1.0.1"
-pyembree = "^0.1.12"
-rasterio = "^1.3.6"
-netCDF4 = "^1.6.3"
+numpy = "==1.24.2"
+scipy = "==1.10.1"
+pyvista = "==0.38.5"
+python-dotenv = "1.0.0"
+trimesh = "==3.21.5"
+rtree = "==1.0.1"
+pyembree = "==0.1.12"
+rasterio = "==1.3.6"
+netCDF4 = "==1.6.3"
 
 [project.urls]
 "Homepage" = "https://github.com/liamrobinson1/PyLightCurves"
 "Bug Tracker" = "https://github.com/liamrobinson1/PyLightCurves/issues"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `terrainman-0.0.24/src/terrainman/tile_io.py` & `terrainman-0.0.9/src/tile_io.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 import urllib.request
 import base64
 import zipfile
 import io
 import os
 import rasterio
 import numpy as np
+import inspect
 import pickle
-from typing import Union, Tuple
+from typing import Tuple
 from abc import ABC
 from netCDF4 import Dataset
-import scipy
+import datetime
 
-def _strip_tuple(t: tuple) -> tuple:
+
+_SRC_DIR = os.path.dirname(
+    os.path.abspath(inspect.getsourcefile(lambda: 0))
+)
+_DATA_DIRECTORY = os.path.join(_SRC_DIR, 'data')
+
+def strip_tuple(t: tuple) -> tuple:
     """Returns a copy of a tuple-of-tuples with no extra layers such that `t[0][0]` is not a tuple
 
     :param t: Input tuple
     :type t: tuple
     :return: Same tuple, stripped of outer layers past the first
     :rtype: tuple
     """
@@ -32,20 +39,14 @@
     def _after_init(self):
         self._bad_input_path = os.path.join(self._storage_dir, 'bad_inputs.pkl')
         if not os.path.exists(self._bad_input_path):
             with open(os.path.join(self._bad_input_path), 'wb') as f:
                 pickle.dump([], f)
 
     def _before_request(self, *args):
-        try:
-            os.environ['EARTHDATA_USERNAME']
-            os.environ['EARTHDATA_PASSWORD']
-        except KeyError as e:
-            print("\nEnvironmental variables 'EARTHDATA_USERNAME' and 'EARTHDATA_PASSWORD' must be set!\nRegister at https://urs.earthdata.nasa.gov/users/new and set them with either:\n    - os.environ['EARTHDATA_USERNAME'] = '<your_username>'\n      os.environ['EARTHDATA_PASSWORD'] = '<your_password>'\n    - Create a .env.shared file in the calling directory containing\nEARTHDATA_USERNAME=<your_username>\nEARTHDATA_PASSWORD=<your_password>")
-            raise
         efname = self._set_fnames(*args)
         if self._is_fname_bad(efname):
             print(self.DNE_MSG)
             return False
         print(f"Checking if {efname} is in {self._storage_dir}")
         if efname in os.listdir(self._storage_dir):
             print(self.EXISTS_MSG)
@@ -103,43 +104,43 @@
         x.append(fname)
         with open(self._bad_input_path, 'wb') as f:
             pickle.dump(x, f)
     
     def _store_bad_input(self, *args) -> None:
         self._store_bad_fname(self._set_fnames(*args))
     
-    def _load(self, *args) -> Union[np.ndarray, Dataset]:
+    def _load(self, args: tuple[tuple]) -> np.ndarray | Dataset:
         efname = self._set_fnames(*args)
         fpath = os.path.join(self._storage_dir, efname)
         if self.save_format == "hgt":
             with rasterio.open(fpath) as src:
                 return src.read().squeeze()
         elif self.save_format == "nc":
             return Dataset(fpath, "r", format="NETCDF4")
 
     def _load_from_args(self, args: tuple[tuple], /, squeeze: bool = True):
         data = []
-        for input_set in _strip_tuple(args):
+        for input_set in strip_tuple(args):
             if self._is_input_bad(*input_set):
-                print(f"Loading tile for {input_set} skipped, tile does not exist")
+                print(f"Loading tile skipped, tile does not exist")
                 data.append(None)
                 continue
-            data.append(self._load(*input_set))
+            data.append(self._load(args))
         return data
     
-    def _download_from_args(self, *args: Union[tuple[tuple], tuple]):
-        for input_set in _strip_tuple(args):
+    def _download_from_args(self, *args: tuple[tuple] | tuple):
+        for input_set in strip_tuple(args):
             if self._before_request(*input_set):
                 self._make_request(*input_set)
                 self._after_request()
 
 
 class TerrainDataHandler(DataProduct):
     def __init__(self) -> None:
-        self._storage_dir = os.path.join(os.environ['TERRAIN_DATA'], 'terrain')
+        self._storage_dir = os.path.join(_DATA_DIRECTORY, 'terrain')
         self.url_base = 'https://e4ftl01.cr.usgs.gov/DP133/SRTM/SRTMGL1.003/2000.02.11/'
         self.download_format = "zip"
         self.save_format = "hgt"
         self.HTTP_ERR_MSG = "HTTP error occured, likely because tile is ocean, aborting..."
         self.DNE_MSG = "Tile does not exist, likely because it's ocean, skipping"
         self.EXISTS_MSG = "Tile already downloaded, skipping"
 
@@ -161,28 +162,19 @@
         :type lat: int
         :param lon: Longitude [deg]
         :type lon: int
         """
         self._download_from_args((lat, lon))
     
     def load_tile(self, lat: int, lon: int) -> np.ndarray:
-        elev_grid = self._load_from_args((lat, lon))[0]
-        if elev_grid is not None:
-            lat_space = (lat+1) - np.linspace(0,1,elev_grid.shape[0])
-            lon_space = lon + np.linspace(0,1,elev_grid.shape[0])
-            return SrtmTile(lat_space, lon_space, elev_grid)
-            return tile
-        return None
+        return self._load_from_args((lat, lon))[0]
 
     def load_tiles_containing(self, lat: np.ndarray, lon: np.ndarray) -> list[np.ndarray]:
-        lat, lon = np.array([lat]).flatten(), np.array([lon]).flatten()
-        self.download_tiles_containing(lat, lon)
         unique_lat_lons = self._unique_tile_lat_lon_pairs(lat, lon)
-        return [self.load_tile(*args) for args in unique_lat_lons] if len(unique_lat_lons) > 1 \
-            else self.load_tile(*unique_lat_lons[0])
+        return self._load_from_args(unique_lat_lons)
 
     def download_tiles_containing(self, lat: np.ndarray, lon: np.ndarray) -> None:
         """Downloads [1 deg x 1 deg] SRTM 30 meter resolution terrain tiles to cover all latitude and longitudes input, requires `os.environ['EARTHDATA_USERNAME']` and `os.environ['EARTHDATA_PASSWORD']` to be defined
 
         :param lat: Latitude [deg]
         :type lat: np.ndarray
         :param lon: Longitude [deg]
@@ -190,45 +182,45 @@
         """
         unique_lat_lons = self._unique_tile_lat_lon_pairs(lat, lon)
         print(f"Downloading tiles for {', '.join([self._set_fnames(*args) for args in unique_lat_lons])}")
         self._download_from_args(unique_lat_lons)
 
     def _unique_tile_lat_lon_pairs(self, lat: np.ndarray, lon: np.ndarray) -> list[Tuple[int, int]]:
         lat_lon_dec = np.vstack((lat.flatten(), lon.flatten())).T
-        # lat_lon_int = np.hstack((np.floor(lat_lon_dec[:,[0]]), np.ceil(lat_lon_dec[:,[1]])))
         lat_lon_int = np.floor(lat_lon_dec)
         unique_lat_lons = np.unique(lat_lon_int, axis=0)
         unique_lat_lons = np.array(unique_lat_lons, np.int32)
         return tuple(map(tuple, unique_lat_lons))
+
+        
+class AerosolDataHandler(DataProduct):
+    def __init__(self) -> None:
+        # Signature (dates, cadence)
+        self._storage_dir = os.path.join(_DATA_DIRECTORY, 'aerosol')
+        self.url_base = 'https://ladsweb.modaps.eosdis.nasa.gov'
+        self.download_format = "nc"
+        self.save_format = "nc"
+        self._VIIRS_AEROSOL_CADENCES = ["daily", "monthly"]
+
+        self._after_init()
     
+    def _set_fnames(self, date: datetime.datetime, cadence: str) -> str:
+        assert cadence in self._VIIRS_AEROSOL_CADENCES, f"Cadence must be in {self._VIIRS_AEROSOL_CADENCES}!"
+        with open(f'src/data/viirs_aerosol_{cadence}.csv', 'r') as f:
+            csv_els = f.read().split(',')
+            if cadence == "daily":
+                fnames = [c for c in csv_els if f'/{date.year}/{date.strftime("%j")}/' in c][-1]
+            elif cadence == "monthly":
+                month_first = datetime.datetime(year=date.year, month=date.month, day=1)
+                month_first_doy = int(month_first.strftime("%j"))
+                possible_date_strs = [f'/{date.year}/{d}/' for d in range(month_first_doy, month_first_doy+32)]
+                fnames = [c for c in csv_els if any(map(c.__contains__, possible_date_strs))]
+        self.extracted_fname = fnames.split('/')[-1]
+        self.url_fname = fnames
+        return self.extracted_fname
+
+    def download(self, date: datetime.datetime, cadence: str):
+        self._download_from_args((date, cadence))
+    
+    def load(self, date: datetime.datetime, cadence: str):
+        return self._load_from_args((date, cadence))[0]
 
-class SrtmTile():
-    """Represents a 1 x 1 degree terrain tile for Shuttle Radar Terrain Mission (SRTM) data
-    """
-    def __init__(self, lat_space: np.ndarray, lon_space: np.ndarray, elev_grid: np.ndarray) -> None:
-        self.lat_space, self.lon_space = lat_space, lon_space
-        self.lat_grid, self.lon_grid = np.meshgrid(lat_space, lon_space)
-        self.elev_grid = elev_grid
-    
-    def interpolate(self, lat_deg: Union[float, np.ndarray], lon_deg: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        """Interpolates within the latitude/longitude 
-
-        :param lat_deg: _description_
-        :type lat_deg: float or np.ndarray
-        :param lon_deg: _description_
-        :type lon_deg: float or np.ndarray
-        :raises NotImplemented: _description_
-        :return: _description_
-        :rtype: float or np.ndarray
-        """
-        kwargs = {'points': (self.lat_space, self.lon_space), 
-                  'values': self.elev_grid,
-                  'fill_value': np.nan,
-                  'bounds_error': False}
-        if isinstance(lat_deg, np.ndarray):
-            return scipy.interpolate.interpn(**kwargs,
-                                    xi=np.hstack((lat_deg.reshape(lat_deg.size,1), lon_deg.reshape(lat_deg.size,1)))).reshape(lat_deg.shape)
-        elif isinstance(lat_deg, float):
-            return scipy.interpolate.interpn(**kwargs,
-                                    xi=np.hstack((lat_deg, lon_deg)))[0]
-        else:
-            raise NotImplemented("Inputs must be either floats or np.ndarrays")
```

