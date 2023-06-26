# Comparing `tmp/m23-1.8.7.tar.gz` & `tmp/m23-1.8.8.tar.gz`

## Comparing `m23-1.8.7.tar` & `m23-1.8.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.7/.flake8
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 m23-1.8.7/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.7/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.7/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.7/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.7/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.7/renormalize.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.7/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.7/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.7/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.7/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.7/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.7/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.7/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.7/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.8/.flake8
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 m23-1.8.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.8/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.8/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.8/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.8/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.8/renormalize.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.8/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.8/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.8/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15888 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.8/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.8/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.8/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.8/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.8/PKG-INFO
```

### Comparing `m23-1.8.7/CHANGELOG.md` & `m23-1.8.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.8 (2023-06-26)
+
+### Fix
+
+* Catch any exception encoutered during processing a night, log it and move to next ([`3fca7cb`](https://github.com/LutherAstrophysics/m23/commit/3fca7cbefe3942c17210e0b25d3cca4cebdcf908))
+
 ## v1.8.7 (2023-06-26)
 
 ### Fix
 
 * Catch exception during internight normalization ([`4988a5c`](https://github.com/LutherAstrophysics/m23/commit/4988a5c082e899eb946e9cbf6e8f693f9ed34771))
 
 ## v1.8.6 (2023-06-25)
```

### Comparing `m23-1.8.7/brown.toml` & `m23-1.8.8/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/mf.toml` & `m23-1.8.8/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/nights_csv.toml` & `m23-1.8.8/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/rainbow.toml` & `m23-1.8.8/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/requirements.txt` & `m23-1.8.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/.github/workflows/python-publish.yml` & `m23-1.8.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/.vscode/settings.json` & `m23-1.8.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/__main__.py` & `m23-1.8.8/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/constants.py` & `m23-1.8.8/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/align/__init__.py` & `m23-1.8.8/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/calibrate/calibration.py` & `m23-1.8.8/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/calibrate/master_calibrate.py` & `m23-1.8.8/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/charts/__init__.py` & `m23-1.8.8/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/combine/__init__.py` & `m23-1.8.8/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/extract/__init__.py` & `m23-1.8.8/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/__init__.py` & `m23-1.8.8/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/aligned_combined_file.py` & `m23-1.8.8/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/alignment_stats_file.py` & `m23-1.8.8/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/color_normalized_file.py` & `m23-1.8.8/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/flux_log_combined_file.py` & `m23-1.8.8/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/log_file_combined_file.py` & `m23-1.8.8/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/masterflat_file.py` & `m23-1.8.8/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/normfactor_file.py` & `m23-1.8.8/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/raw_image_file.py` & `m23-1.8.8/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/reference_log_file.py` & `m23-1.8.8/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/ri_color_file.py` & `m23-1.8.8/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/file/sky_bg_file.py` & `m23-1.8.8/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/internight_normalize/__init__.py` & `m23-1.8.8/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/matrix/fill.py` & `m23-1.8.8/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/norm/__init__.py` & `m23-1.8.8/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/norm/get_line.py` & `m23-1.8.8/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/align_combined_extract.py` & `m23-1.8.8/src/m23/processor/align_combined_extract.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/config_loader.py` & `m23-1.8.8/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/generate_masterflat.py` & `m23-1.8.8/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.8.8/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/nights_csv.py` & `m23-1.8.8/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/nights_csv_config_loader.py` & `m23-1.8.8/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/processor/process_nights.py` & `m23-1.8.8/src/m23/processor/process_nights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import shutil
 import sys
+import traceback
 from datetime import date
 from pathlib import Path
 from typing import Iterable, List
 
 import multiprocess as mp
 import toml
 from astropy.io.fits import getdata
@@ -330,39 +331,51 @@
     # Create a file for storing alignment transformation
     alignment_stats_file_name = AlignmentStatsFile.generate_file_name(night_date)
     alignment_stats_file = AlignmentStatsFile(output / alignment_stats_file_name)
     alignment_stats_file.create_file_and_write_header()
 
     log_files_to_normalize: List[LogFileCombinedFile] = []
     for nth_combined_image in range(no_of_combined_images):
-        align_combined_extract(
-            config,
-            night,
-            output,
-            night_date,
-            nth_combined_image,
-            raw_images,
-            master_dark_data,
-            master_flat_data,
-            alignment_stats_file,
-            image_duration,
-            log_files_to_normalize,
-        )
+        try:
+            align_combined_extract(
+                config,
+                night,
+                output,
+                night_date,
+                nth_combined_image,
+                raw_images,
+                master_dark_data,
+                master_flat_data,
+                alignment_stats_file,
+                image_duration,
+                log_files_to_normalize,
+            )
+        except Exception:
+            tb = traceback.format_exc()
+            logger.error("Exception during alignment combination extraction")
+            logger.debug(tb)
+            return
 
     # Intranight + Internight Normalization
-    normalization_helper(
-        radii_of_extraction,
-        reference_log_file,
-        log_files_to_normalize,
-        image_duration,
-        night_date,
-        color_ref_file_path,
-        output,
-        logfile_combined_reference_logfile,
-    )
+    try:
+        normalization_helper(
+            radii_of_extraction,
+            reference_log_file,
+            log_files_to_normalize,
+            image_duration,
+            night_date,
+            color_ref_file_path,
+            output,
+            logfile_combined_reference_logfile,
+        )
+    except Exception:
+        tb = traceback.format_exc()
+        logger.error("Exception during normalization/sky_bg generation")
+        logger.debug(tb)
+        return
 
 
 def start_data_processing_auxiliary(config: Config):
     """
     This function processes (one or more) nights defined in config dict by
     putting together various functionalities like calibration, alignment,
     extraction, and normalization together.
```

### Comparing `m23-1.8.7/src/m23/processor/renormalize.py` & `m23-1.8.8/src/m23/processor/renormalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import sys
+import traceback
 from pathlib import Path
 
 import multiprocess as mp
 
 from m23 import __version__
 from m23.constants import FLUX_LOGS_COMBINED_FOLDER_NAME
 from m23.file.log_file_combined_file import LogFileCombinedFile
@@ -56,24 +57,30 @@
         # Ensure color ref file path is str
         color_ref_file_path = str(renormalize_dict["reference"]["color"])
 
         log_files_to_use = [LogFileCombinedFile(file) for file in night["files_to_use"]]
         img_duration = log_files_to_use[0].img_duration()
 
         # Perform intranight normalization then internight normalization
-        normalization_helper(
-            radii_of_extraction,
-            reference_log_file,
-            log_files_to_use,
-            img_duration,
-            night_date,
-            color_ref_file_path,
-            NIGHT_FOLDER,
-            logfile_combined_reference_logfile,
-        )
+        try:
+            normalization_helper(
+                radii_of_extraction,
+                reference_log_file,
+                log_files_to_use,
+                img_duration,
+                night_date,
+                color_ref_file_path,
+                NIGHT_FOLDER,
+                logfile_combined_reference_logfile,
+            )
+        except Exception:
+            tb = traceback.format_exc()
+            logger.error("Exception during normalization/sky_bg generation")
+            logger.debug(tb)
+            return
 
     with mp.Pool(int(os.cpu_count() * 0.75)) as p:  # Use 75% CPU
         p.map(night_renorm_mapper, renormalize_dict["input"]["nights"])
 
 
 def renormalize(file_path: str):
     """
```

### Comparing `m23-1.8.7/src/m23/processor/renormalize_config_loader.py` & `m23-1.8.8/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.8.8/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/reference/MeanRI100.txt` & `m23-1.8.8/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/reference/README.md` & `m23-1.8.8/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/reference/m23_3.5_071.fit` & `m23-1.8.8/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.8.8/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/sky/__init__.py` & `m23-1.8.8/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/sky/moon/__init__.py` & `m23-1.8.8/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/utils/__init__.py` & `m23-1.8.8/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/utils/date.py` & `m23-1.8.8/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/src/m23/utils/rename.py` & `m23-1.8.8/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/.gitignore` & `m23-1.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/README.md` & `m23-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.7/pyproject.toml` & `m23-1.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.8.7"
+version = "1.8.8"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.8.7/PKG-INFO` & `m23-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.8.7
+Version: 1.8.8
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
```

