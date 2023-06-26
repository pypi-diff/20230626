# Comparing `tmp/ensembleperturbation-1.2.1.tar.gz` & `tmp/ensembleperturbation-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembleperturbation-1.2.1.tar", max compression
+gzip compressed data, was "ensembleperturbation-1.2.2.tar", max compression
```

## Comparing `ensembleperturbation-1.2.1.tar` & `ensembleperturbation-1.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     7048 2023-05-03 16:37:41.880276 ensembleperturbation-1.2.1/LICENSE
--rw-r--r--   0        0        0     1554 2023-05-03 16:37:41.880276 ensembleperturbation-1.2.1/README.md
--rw-r--r--   0        0        0        3 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/__init__.py
--rw-r--r--   0        0        0     3803 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/combine_results.py
--rw-r--r--   0        0        0     1952 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/make_storm_ensemble.py
--rw-r--r--   0        0        0     5792 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/perturb_tracks.py
--rw-r--r--   0        0        0     2566 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/plot_results.py
--rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/__init__.py
--rw-r--r--   0        0        0    32929 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/adcirc.py
--rw-r--r--   0        0        0    24828 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/comparison.py
--rw-r--r--   0        0        0    46714 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/schism.py
--rw-r--r--   0        0        0      545 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/utilities.py
--rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/perturbation/__init__.py
--rw-r--r--   0        0        0    74561 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/perturbation/atcf.py
--rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/__init__.py
--rw-r--r--   0        0        0    10510 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/gdal_dataset.py
--rw-r--r--   0        0        0     5453 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/geometry.py
--rw-r--r--   0        0        0     1590 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/map.py
--rw-r--r--   0        0        0     9135 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/nodes.py
--rw-r--r--   0        0        0    13796 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/perturbation.py
--rw-r--r--   0        0        0    20101 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/surrogate.py
--rw-r--r--   0        0        0     4623 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/taylor_diagram.py
--rw-r--r--   0        0        0      908 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/utilities.py
--rw-r--r--   0        0        0        0 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/__init__.py
--rw-r--r--   0        0        0     2663 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/ensemble_array.py
--rw-r--r--   0        0        0    11112 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
--rw-r--r--   0        0        0     5332 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
--rw-r--r--   0        0        0    23410 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/surrogate.py
--rw-r--r--   0        0        0     5066 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/utilities.py
--rw-r--r--   0        0        0     2310 2023-05-03 16:37:48.808743 ensembleperturbation-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3723 2023-05-03 16:37:49.861170 ensembleperturbation-1.2.1/setup.py
--rw-r--r--   0        0        0     3731 2023-05-03 16:37:49.861724 ensembleperturbation-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-06-26 13:45:23.157278 ensembleperturbation-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1554 2023-06-26 13:45:23.157278 ensembleperturbation-1.2.2/README.md
+-rw-r--r--   0        0        0        3 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/__init__.py
+-rw-r--r--   0        0        0     3803 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/combine_results.py
+-rw-r--r--   0        0        0     1952 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/make_storm_ensemble.py
+-rw-r--r--   0        0        0     5792 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/perturb_tracks.py
+-rw-r--r--   0        0        0     2566 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/plot_results.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/__init__.py
+-rw-r--r--   0        0        0    32929 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/adcirc.py
+-rw-r--r--   0        0        0    24828 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/comparison.py
+-rw-r--r--   0        0        0    46714 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/schism.py
+-rw-r--r--   0        0        0      545 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/utilities.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/perturbation/__init__.py
+-rw-r--r--   0        0        0    75293 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/perturbation/atcf.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/__init__.py
+-rw-r--r--   0        0        0    10510 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/gdal_dataset.py
+-rw-r--r--   0        0        0     5453 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/geometry.py
+-rw-r--r--   0        0        0     1590 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/map.py
+-rw-r--r--   0        0        0     9135 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/nodes.py
+-rw-r--r--   0        0        0    14013 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/perturbation.py
+-rw-r--r--   0        0        0    20101 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/surrogate.py
+-rw-r--r--   0        0        0     4623 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/taylor_diagram.py
+-rw-r--r--   0        0        0      908 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/utilities.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/__init__.py
+-rw-r--r--   0        0        0     2663 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py
+-rw-r--r--   0        0        0    11112 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
+-rw-r--r--   0        0        0     5332 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
+-rw-r--r--   0        0        0    23410 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/surrogate.py
+-rw-r--r--   0        0        0     5066 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/utilities.py
+-rw-r--r--   0        0        0     2326 2023-06-26 13:45:30.097446 ensembleperturbation-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3723 2023-06-26 13:45:31.101437 ensembleperturbation-1.2.2/setup.py
+-rw-r--r--   0        0        0     3731 2023-06-26 13:45:31.101974 ensembleperturbation-1.2.2/PKG-INFO
```

### Comparing `ensembleperturbation-1.2.1/LICENSE` & `ensembleperturbation-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/README.md` & `ensembleperturbation-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/client/combine_results.py` & `ensembleperturbation-1.2.2/ensembleperturbation/client/combine_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/client/make_storm_ensemble.py` & `ensembleperturbation-1.2.2/ensembleperturbation/client/make_storm_ensemble.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/client/perturb_tracks.py` & `ensembleperturbation-1.2.2/ensembleperturbation/client/perturb_tracks.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/client/plot_results.py` & `ensembleperturbation-1.2.2/ensembleperturbation/client/plot_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/parsing/adcirc.py` & `ensembleperturbation-1.2.2/ensembleperturbation/parsing/adcirc.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/parsing/comparison.py` & `ensembleperturbation-1.2.2/ensembleperturbation/parsing/comparison.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/parsing/schism.py` & `ensembleperturbation-1.2.2/ensembleperturbation/parsing/schism.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/parsing/utilities.py` & `ensembleperturbation-1.2.2/ensembleperturbation/parsing/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/perturbation/atcf.py` & `ensembleperturbation-1.2.2/ensembleperturbation/perturbation/atcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1097,37 +1097,44 @@
         track = VortexTrack.from_file(
             filename,
             start_date=start_date,
             end_date=end_date,
             file_deck=file_deck,
             advisories=advisories,
         )
+        if file_deck in ['a', ATCF_FileDeck('a')]:
+            track.forecast_time = (
+                track.data.track_start_time.min() if start_date is None else start_date
+            )
         instance = VortexPerturber.from_track(track)
         instance.__filename = filename
         return instance
 
     @classmethod
     def from_track(cls, track: VortexTrack) -> 'VortexPerturber':
         """
         build storm perturber from an existing `VortexTrack` object
 
         :param track: `VortexTrack` object
         """
 
+        start_date = track.start_date
+        if track.forecast_time is not None:
+            start_date = track.forecast_time
         instance = cls(
             track.nhc_code,
-            start_date=track.start_date,
+            start_date=start_date,
             end_date=track.end_date,
             file_deck=track.file_deck,
             advisories=track.advisories,
         )
         instance.track = track
         instance.__previous_configuration = {
             'storm': track.nhc_code,
-            'start_date': track.start_date,
+            'start_date': start_date,
             'end_date': track.end_date,
             'file_deck': track.file_deck,
             'advisories': track.advisories,
         }
         return instance
 
     @property
@@ -1187,19 +1194,27 @@
             else:
                 is_equal = True
 
         if not is_equal:
             if self.__filename is not None and self.__filename.exists():
                 self.__track = VortexTrack.from_file(
                     self.__filename,
+                    file_deck=configuration['file_deck'],
+                    advisories=configuration['advisories'],
                     start_date=configuration['start_date'],
                     end_date=configuration['end_date'],
                 )
             else:
                 self.__track = VortexTrack(**configuration)
+            if configuration['file_deck'] in ['a', ATCF_FileDeck('a')]:
+                self.__track.forecast_time = (
+                    self.__track.data.track_start_time.min()
+                    if configuration['start_date'] is None
+                    else configuration['start_date']
+                )
             self.__previous_configuration = configuration
 
         if self.__track.nhc_code is not None:
             self.storm = self.__track.nhc_code
 
         return self.__track
```

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/gdal_dataset.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/geometry.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/geometry.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/map.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/map.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/nodes.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/nodes.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/perturbation.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/perturbation.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from matplotlib import pyplot
 from matplotlib.cm import get_cmap
 from matplotlib.collections import LineCollection
 from matplotlib.colors import LogNorm, Normalize
 from matplotlib.patches import Patch
 import numpy
 from stormevents.nhc import VortexTrack
+from stormevents.nhc.atcf import ATCF_FileDeck
 import xarray
 
 from ensembleperturbation.plotting.surrogate import comparison_plot_grid
 from ensembleperturbation.plotting.utilities import colorbar_axis
 from ensembleperturbation.utilities import encode_categorical_values
 
 
@@ -241,15 +242,19 @@
             if output_directory is not None:
                 figure.savefig(
                     output_directory / 'storm_tracks.png', dpi=200, bbox_inches='tight',
                 )
 
 
 def plot_track_perturbations(
-    perturbations: dict, storm_name: str = None, output_directory: PathLike = None,
+    perturbations: dict,
+    storm_name: str = None,
+    output_directory: PathLike = None,
+    file_deck: ATCF_FileDeck = None,
+    advisories: List[str] = None,
 ):
 
     num_perturbations = len(perturbations)
     perturbation_keys = list(perturbations.keys())
     perturbation_types = ['ensemble'] * num_perturbations
     if 'original' in perturbation_keys:
         num_perturbations = num_perturbations - 1
@@ -272,15 +277,19 @@
     )
     linear_normalization = Normalize()
     colors = get_cmap('jet')(linear_normalization(encoded_perturbation_types))
 
     bounds = numpy.array([None, None, None, None])
     for index, run in enumerate(perturbation_keys):
         pkey = list(perturbations[run].keys())
-        storm = VortexTrack.from_file(perturbations[run][pkey[0]]['fort22_filename']).data
+        storm = VortexTrack.from_file(
+            perturbations[run][pkey[0]]['fort22_filename'],
+            file_deck=file_deck,
+            advisories=advisories,
+        ).data
 
         # Track
         points = storm.loc[:, ['longitude', 'latitude']].values.reshape(-1, 1, 2)
         segments = numpy.concatenate([points[:-1], points[1:]], axis=1)
         line_collection = LineCollection(
             segments,
             linewidths=numpy.concatenate(
```

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/surrogate.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/taylor_diagram.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/plotting/utilities.py` & `ensembleperturbation-1.2.2/ensembleperturbation/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/ensemble_array.py` & `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py` & `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py` & `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/surrogate.py` & `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/ensembleperturbation/utilities.py` & `ensembleperturbation-1.2.2/ensembleperturbation/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.1/pyproject.toml` & `ensembleperturbation-1.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'ensembleperturbation'
-version = "1.2.1"
+version = "1.2.2"
 description = 'perturbation of coupled model input over a space of input variables'
 authors = ['Zach Burnett <zachary.burnett@noaa.gov>']
 license = 'CC0-1.0'
 readme = 'README.md'
 repository = 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git'
 documentation = 'https://ensembleperturbation.readthedocs.io'
 
@@ -40,15 +40,15 @@
 pyproj = '>=2.6'
 tables = '*'
 typepigeon = '*'
 python-dateutil = '*'
 requests = '*'
 shapely = '*'
 scikit-learn = '*'
-stormevents = '>=2.1.4'
+stormevents = '>=2.2.1' # Forecast time
 isort = { version = '*', optional = true }
 oitnb = { version = '*', optional = true }
 pytest = { version = '*', optional = true }
 pytest-cov = { version = '*', optional = true }
 pytest-xdist = { version = '*', optional = true }
 wget = { version = '*', optional = true }
 m2r2 = { version = '*', optional = true }
```

### Comparing `ensembleperturbation-1.2.1/setup.py` & `ensembleperturbation-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'pint-pandas',
  'pint<0.20',
  'pyproj>=2.6',
  'python-dateutil',
  'requests',
  'scikit-learn',
  'shapely',
- 'stormevents>=2.1.4',
+ 'stormevents>=2.2.1',
  'tables',
  'typepigeon']
 
 extras_require = \
 {'development': ['isort', 'oitnb'],
  'documentation': ['m2r2',
                    'sphinx',
@@ -54,15 +54,15 @@
                      'perturb_tracks = '
                      'ensembleperturbation.client.perturb_tracks:main',
                      'plot_results = '
                      'ensembleperturbation.client.plot_results:main']}
 
 setup_kwargs = {
     'name': 'ensembleperturbation',
-    'version': '1.2.1',
+    'version': '1.2.2',
     'description': 'perturbation of coupled model input over a space of input variables',
     'long_description': '# Ensemble Perturbation\n\n[![tests](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/tests/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Atests)\n[![codecov](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation/branch/main/graph/badge.svg?token=4DwZePHp18)](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation)\n[![build](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/build/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Abuild)\n[![version](https://img.shields.io/pypi/v/EnsemblePerturbation)](https://pypi.org/project/EnsemblePerturbation)\n[![license](https://img.shields.io/github/license/noaa-ocs-modeling/EnsemblePerturbation)](https://creativecommons.org/share-your-work/public-domain/cc0)\n[![style](https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw)](https://sourceforge.net/p/oitnb/code)\n[![documentation](https://readthedocs.org/projects/ensembleperturbation/badge/?version=latest)](https://ensembleperturbation.readthedocs.io/en/latest/?badge=latest)\n\nPython library for perturbing coupled model inputs into ensemble runs. Provides\nperturbation and results comparison.\n\n```bash\npip install ensembleperturbation\n```\n\nDocumentation can be found at https://ensembleperturbation.readthedocs.io\n\n## Command-line interface\n\n`ensembleperturbation` exposes the following CLI commands:\n\n- `make_storm_ensemble`\n- `perturb_tracks`\n- `combine_results`\n- `plot_results`\n',
     'author': 'Zach Burnett',
     'author_email': 'zachary.burnett@noaa.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git',
```

### Comparing `ensembleperturbation-1.2.1/PKG-INFO` & `ensembleperturbation-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembleperturbation
-Version: 1.2.1
+Version: 1.2.2
 Summary: perturbation of coupled model input over a space of input variables
 Home-page: https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 License: CC0-1.0
 Author: Zach Burnett
 Author-email: zachary.burnett@noaa.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
@@ -44,15 +44,15 @@
 Requires-Dist: requests
 Requires-Dist: scikit-learn
 Requires-Dist: shapely
 Requires-Dist: sphinx-rtd-theme; extra == "documentation"
 Requires-Dist: sphinx; extra == "documentation"
 Requires-Dist: sphinxcontrib-bibtex; extra == "documentation"
 Requires-Dist: sphinxcontrib-programoutput; extra == "documentation"
-Requires-Dist: stormevents (>=2.1.4)
+Requires-Dist: stormevents (>=2.2.1)
 Requires-Dist: tables
 Requires-Dist: typepigeon
 Requires-Dist: wget; extra == "testing"
 Project-URL: Documentation, https://ensembleperturbation.readthedocs.io
 Project-URL: Repository, https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 Description-Content-Type: text/markdown
```

