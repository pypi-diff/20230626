# Comparing `tmp/m23-1.8.8.tar.gz` & `tmp/m23-1.9.0.tar.gz`

## Comparing `m23-1.8.8.tar` & `m23-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.8/.flake8
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 m23-1.8.8/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.8/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.8/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.8/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.8/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.8/renormalize.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.8/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.8/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.8/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15888 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.8/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.8/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.8/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.8/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.8/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.9.0/.flake8
+-rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 m23-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.9.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.9.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.9.0/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.9.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.9.0/renormalize.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.9.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.9.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.9.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.9.0/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.9.0/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.9.0/PKG-INFO
```

### Comparing `m23-1.8.8/CHANGELOG.md` & `m23-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.0 (2023-06-26)
+
+### Feature
+
+* Use extensive logging ([`60afdaf`](https://github.com/LutherAstrophysics/m23/commit/60afdaf00e3bbea2f14265912b0d7d1cf61d3688))
+
 ## v1.8.8 (2023-06-26)
 
 ### Fix
 
 * Catch any exception encoutered during processing a night, log it and move to next ([`3fca7cb`](https://github.com/LutherAstrophysics/m23/commit/3fca7cbefe3942c17210e0b25d3cca4cebdcf908))
 
 ## v1.8.7 (2023-06-26)
```

### Comparing `m23-1.8.8/brown.toml` & `m23-1.9.0/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/mf.toml` & `m23-1.9.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/nights_csv.toml` & `m23-1.9.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/rainbow.toml` & `m23-1.9.0/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/requirements.txt` & `m23-1.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/.github/workflows/python-publish.yml` & `m23-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/.vscode/settings.json` & `m23-1.9.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/__main__.py` & `m23-1.9.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/constants.py` & `m23-1.9.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/align/__init__.py` & `m23-1.9.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/calibrate/calibration.py` & `m23-1.9.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/calibrate/master_calibrate.py` & `m23-1.9.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/charts/__init__.py` & `m23-1.9.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/combine/__init__.py` & `m23-1.9.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/extract/__init__.py` & `m23-1.9.0/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/__init__.py` & `m23-1.9.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/aligned_combined_file.py` & `m23-1.9.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/alignment_stats_file.py` & `m23-1.9.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/color_normalized_file.py` & `m23-1.9.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/flux_log_combined_file.py` & `m23-1.9.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/log_file_combined_file.py` & `m23-1.9.0/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/masterflat_file.py` & `m23-1.9.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/normfactor_file.py` & `m23-1.9.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/raw_image_file.py` & `m23-1.9.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/reference_log_file.py` & `m23-1.9.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/ri_color_file.py` & `m23-1.9.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/file/sky_bg_file.py` & `m23-1.9.0/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/internight_normalize/__init__.py` & `m23-1.9.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/matrix/fill.py` & `m23-1.9.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/norm/__init__.py` & `m23-1.9.0/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/norm/get_line.py` & `m23-1.9.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/align_combined_extract.py` & `m23-1.9.0/src/m23/processor/align_combined_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     from_index = nth_combined_image * no_of_images_to_combine
     # Note the to_index is exclusive
     to_index = (nth_combined_image + 1) * no_of_images_to_combine
 
     # NOTE
     # It's very easy to get confused between no_of_combined_images
-    # and the no_of_images_to_combine. THe later is the number of raw images
+    # and the no_of_images_to_combine. The later is the number of raw images
     # that are combined together to form on aligned combined image
 
     images_data = [raw_image_file.data() for raw_image_file in raw_images[from_index:to_index]]
     # Ensure that image dimensions are as specified by rows and cols
     # If there's extra noise cols or rows, we crop them
     images_data = [crop(matrix, rows, cols) for matrix in images_data]
 
@@ -120,69 +120,86 @@
             )
 
             if save_aligned_images:
                 aligned_image.create_file(aligned_data.astype("int32"), raw_image_to_align)
 
             alignment_stats_file.add_record(raw_image_to_align_name, statistics)
             logger.info(f"Aligned {raw_image_to_align_name}")
-        except CouldNotAlignException:
+        except CouldNotAlignException as e:
             logger.error(f"Could not align image {raw_image_to_align}")
             logger.error(f"Skipping combination {from_index}-{to_index}")
+            logger.error(f"{e}")
+            break
+        except Exception as e:
+            logger.error(f"Could not align image {raw_image_to_align}")
+            logger.error(f"Skipping combination {from_index}-{to_index}")
+            logger.error(f"{e}")
             break
 
     # We proceed to next set of images if the alignment wasn't successful for any one
     # image in the combination set. We now this by checking no of aligned images.
     if len(aligned_images_data) < no_of_images_to_combine:
+        logger.warning(
+            f"Length of aligned images {len(aligned_images_data)}. No of images to combined: {no_of_images_to_combine}"  # noqa
+        )
+        logger.warning("Skipping align-combine-extract")
         return
 
     # Combination
     combined_images_data = np.sum(aligned_images_data, axis=0)
+    logger.info("Combined")
 
     # We take the middle image from the combination as the sample This is
     # the image whose header will be copied to the combined image fit file
     midpoint_index = from_index + no_of_images_to_combine // 2
     sample_raw_image_file = raw_images[midpoint_index]
+    logger.info(f"Using {sample_raw_image_file} as sample")
 
     aligned_combined_image_number = to_index // no_of_images_to_combine
+    logger.info(f"Aligned combined image number {aligned_combined_image_number}")
     aligned_combined_file_name = AlignedCombinedFile.generate_file_name(
         image_duration, aligned_combined_image_number
     )
+    logger.info(f"Aligned combined image name {aligned_combined_file_name}")
     aligned_combined_file = AlignedCombinedFile(
         ALIGNED_COMBINED_OUTPUT_FOLDER / aligned_combined_file_name
     )
     # Image viewing softwares like Astromagic and Fits Liberator don't work
     # if the image data type is float, for some reason that we don't know.
     # So we're setting the datatype to int32 which has enough precision for
     # us.
     aligned_combined_file.create_file(combined_images_data.astype("int32"), sample_raw_image_file)
+    logger.info(f"Set {aligned_combined_file_name} dtype to int32")
     logger.info(f"Combined images {from_index}-{to_index}")
 
     # Extraction
     log_file_combined_file_name = LogFileCombinedFile.generate_file_name(
         night_date, aligned_combined_image_number, image_duration
     )
     log_file_combined_file = LogFileCombinedFile(
         LOG_FILES_COMBINED_OUTPUT_FOLDER / log_file_combined_file_name
     )
 
     date_time_to_use = get_datetime_to_use(
         aligned_combined_file, night, no_of_images_to_combine, NIGHT_INPUT_IMAGES_FOLDER
     )
+    logger.info(f"Using datetime {date_time_to_use} for extraction")
 
     extract_stars(
         combined_images_data,
         reference_log_file,
         radii_of_extraction,
         log_file_combined_file,
         aligned_combined_file,
         date_time_to_use,
     )
 
-    log_files_to_normalize.append(log_file_combined_file)
     logger.info(f"Extraction from combination {from_index}-{to_index} completed")
+    log_files_to_normalize.append(log_file_combined_file)
+    logger.info(f"Adding logfile {log_files_to_normalize} to the list of log files to use")
 
 
 def get_datetime_to_use(
     aligned_combined: AlignedCombinedFile,
     night_config: ConfigInputNight,
     no_of_raw_images_in_one_combination: int,
     raw_images_folder: Path,
```

### Comparing `m23-1.8.8/src/m23/processor/config_loader.py` & `m23-1.9.0/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/generate_masterflat.py` & `m23-1.9.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.9.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/nights_csv.py` & `m23-1.9.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/nights_csv_config_loader.py` & `m23-1.9.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/processor/process_nights.py` & `m23-1.9.0/src/m23/processor/process_nights.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,14 +216,15 @@
 
 
 def process_night(night: ConfigInputNight, config: Config, output: Path, night_date: date):  # noqa
     """
     Processes a given night of data based on the settings provided in `config` dict
     """
     # Save the config file used to do the current data processing
+    print("GODDAMN")
     CONFIG_PATH = output / CONFIG_FILE_NAME
     with CONFIG_PATH.open("w+") as fd:
         toml.dump(config, fd)
 
     # Number of expected rows and columns in all raw images
     rows, cols = config["image"]["rows"], config["image"]["columns"]
     radii_of_extraction = config["processing"]["radii_of_extraction"]
@@ -231,15 +232,15 @@
     log_file_path = output / get_log_file_name(night_date)
     # Clear file contents if exists, so that reprocessing a night wipes out
     # contents instead of appending to it
     if log_file_path.exists():
         log_file_path.unlink()
 
     logger = logging.getLogger("LOGGER_" + str(night_date))
-    logger.setLevel(logging.INFO)
+    logger.setLevel(logging.DEBUG)
     formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     ch = logging.FileHandler(log_file_path)
     ch.setFormatter(formatter)
     logger.addHandler(ch)
     # Write to std out in addition to writing to a logfile
     ch2 = logging.StreamHandler(sys.stdout)
     ch2.setFormatter(formatter)
@@ -328,14 +329,15 @@
     # Note the subtle typing difference between no_of_combined_images and no_of_images_to_combine
     no_of_combined_images = len(raw_images) // no_of_images_to_combine
 
     # Create a file for storing alignment transformation
     alignment_stats_file_name = AlignmentStatsFile.generate_file_name(night_date)
     alignment_stats_file = AlignmentStatsFile(output / alignment_stats_file_name)
     alignment_stats_file.create_file_and_write_header()
+    logger.info("Created alignment stats file")
 
     log_files_to_normalize: List[LogFileCombinedFile] = []
     for nth_combined_image in range(no_of_combined_images):
         try:
             align_combined_extract(
                 config,
                 night,
@@ -345,35 +347,37 @@
                 raw_images,
                 master_dark_data,
                 master_flat_data,
                 alignment_stats_file,
                 image_duration,
                 log_files_to_normalize,
             )
-        except Exception:
+        except Exception as e:
             tb = traceback.format_exc()
             logger.error("Exception during alignment combination extraction")
-            logger.debug(tb)
+            logger.error(e)
+            logger.error(tb)
             return
 
     # Intranight + Internight Normalization
     try:
         normalization_helper(
             radii_of_extraction,
             reference_log_file,
             log_files_to_normalize,
             image_duration,
             night_date,
             color_ref_file_path,
             output,
             logfile_combined_reference_logfile,
         )
-    except Exception:
+    except Exception as e:
         tb = traceback.format_exc()
         logger.error("Exception during normalization/sky_bg generation")
+        logger.error(e)
         logger.debug(tb)
         return
 
 
 def start_data_processing_auxiliary(config: Config):
     """
     This function processes (one or more) nights defined in config dict by
```

### Comparing `m23-1.8.8/src/m23/processor/renormalize.py` & `m23-1.9.0/src/m23/processor/renormalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def night_renorm_mapper(night):
         NIGHT_FOLDER = night["path"]
         night_date = get_date_from_input_night_folder_name(NIGHT_FOLDER.name)
         log_file_path = NIGHT_FOLDER / get_log_file_name(night_date)
         radii_of_extraction = renormalize_dict["processing"]["radii_of_extraction"]
 
         logger = logging.getLogger("LOGGER_" + str(night_date))
-        logger.setLevel(logging.INFO)
+        logger.setLevel(logging.DEBUG)
         formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         ch = logging.FileHandler(log_file_path)
         ch.setFormatter(formatter)
         logger.addHandler(ch)
         # Write to std out in addition to writing to a logfile
         ch2 = logging.StreamHandler(sys.stdout)
         ch2.setFormatter(formatter)
```

### Comparing `m23-1.8.8/src/m23/processor/renormalize_config_loader.py` & `m23-1.9.0/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.9.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/reference/MeanRI100.txt` & `m23-1.9.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/reference/README.md` & `m23-1.9.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/reference/m23_3.5_071.fit` & `m23-1.9.0/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.9.0/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/sky/__init__.py` & `m23-1.9.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/sky/moon/__init__.py` & `m23-1.9.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/utils/__init__.py` & `m23-1.9.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/utils/date.py` & `m23-1.9.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/src/m23/utils/rename.py` & `m23-1.9.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/.gitignore` & `m23-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/README.md` & `m23-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.8/pyproject.toml` & `m23-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.8.8"
+version = "1.9.0"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.8.8/PKG-INFO` & `m23-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.8.8
+Version: 1.9.0
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
```

