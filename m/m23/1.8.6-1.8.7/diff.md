# Comparing `tmp/m23-1.8.6.tar.gz` & `tmp/m23-1.8.7.tar.gz`

## Comparing `m23-1.8.6.tar` & `m23-1.8.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.6/.flake8
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 m23-1.8.6/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.6/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.6/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.6/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.6/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.6/renormalize.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.6/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.6/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.6/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15187 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.6/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.6/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.6/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.6/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.6/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.7/.flake8
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 m23-1.8.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.7/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.7/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.7/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.7/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.7/renormalize.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.7/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.7/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.7/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.7/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.7/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.7/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.7/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.7/PKG-INFO
```

### Comparing `m23-1.8.6/CHANGELOG.md` & `m23-1.8.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.7 (2023-06-26)
+
+### Fix
+
+* Catch exception during internight normalization ([`4988a5c`](https://github.com/LutherAstrophysics/m23/commit/4988a5c082e899eb946e9cbf6e8f693f9ed34771))
+
 ## v1.8.6 (2023-06-25)
 
 ### Fix
 
 * Use 75% of CPU at max ([`fb8cdc7`](https://github.com/LutherAstrophysics/m23/commit/fb8cdc7e8ca5af9d48498dd8cc3a49002ec84523))
 
 ## v1.8.5 (2023-06-25)
```

### Comparing `m23-1.8.6/brown.toml` & `m23-1.8.7/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/mf.toml` & `m23-1.8.7/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/nights_csv.toml` & `m23-1.8.7/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/rainbow.toml` & `m23-1.8.7/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/requirements.txt` & `m23-1.8.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/.github/workflows/python-publish.yml` & `m23-1.8.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/.vscode/settings.json` & `m23-1.8.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/__main__.py` & `m23-1.8.7/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/constants.py` & `m23-1.8.7/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/align/__init__.py` & `m23-1.8.7/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/calibrate/calibration.py` & `m23-1.8.7/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/calibrate/master_calibrate.py` & `m23-1.8.7/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/charts/__init__.py` & `m23-1.8.7/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/combine/__init__.py` & `m23-1.8.7/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/extract/__init__.py` & `m23-1.8.7/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/__init__.py` & `m23-1.8.7/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/aligned_combined_file.py` & `m23-1.8.7/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/alignment_stats_file.py` & `m23-1.8.7/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/color_normalized_file.py` & `m23-1.8.7/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/flux_log_combined_file.py` & `m23-1.8.7/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/log_file_combined_file.py` & `m23-1.8.7/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/masterflat_file.py` & `m23-1.8.7/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/normfactor_file.py` & `m23-1.8.7/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/raw_image_file.py` & `m23-1.8.7/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/reference_log_file.py` & `m23-1.8.7/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/ri_color_file.py` & `m23-1.8.7/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/file/sky_bg_file.py` & `m23-1.8.7/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/internight_normalize/__init__.py` & `m23-1.8.7/src/m23/internight_normalize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
+import traceback
 from pathlib import Path
 from typing import Callable, Dict, List, TypedDict
 
 import numpy as np
 from scipy.optimize import curve_fit
 
 from m23.charts import draw_internight_brightness_chart, draw_internight_color_chart
 from m23.constants import COLOR_NORMALIZED_FOLDER_NAME, FLUX_LOGS_COMBINED_FOLDER_NAME
+from m23.exceptions import InternightException
 from m23.file.color_normalized_file import ColorNormalizedFile
 from m23.file.flux_log_combined_file import FluxLogCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.ri_color_file import RIColorFile
 from m23.utils import (
     customMedian,
     get_date_from_input_night_folder_name,
@@ -272,17 +274,24 @@
         y_differences += section_data[section_number]["y_differences"]
 
     y_diff_std = np.std(y_differences, ddof=1)
     y_diff_mean = np.mean(y_differences)
     y_diff_min = y_diff_mean - 5 * y_diff_std
     y_diff_max = y_diff_mean + 5 * y_diff_std
     y_no_of_bins = 10  # We want to use 10 bins, like IDL code
-    bin_frequencies, bins_edges = np.histogram(
-        y_differences, range=[y_diff_min, y_diff_max], bins=y_no_of_bins
-    )
+    try:
+        bin_frequencies, bins_edges = np.histogram(
+            y_differences, range=[y_diff_min, y_diff_max], bins=y_no_of_bins
+        )
+    except ValueError:
+        tb = traceback.format_exc()
+        logger.error("Internight norm encountered exception in making histogram of residuals")
+        logger.debug(tb)
+        raise InternightException
+
     bins_mid_values = []
     for index, current_value in enumerate(bins_edges[:-1]):
         next_value = bins_edges[index + 1]
         bins_mid_values.append((current_value + next_value) / 2)
     fit_coefficients, _ = curve_fit(
         n_term_3_gauss_fit, bins_mid_values, bin_frequencies, maxfev=5000
     )
```

### Comparing `m23-1.8.6/src/m23/matrix/fill.py` & `m23-1.8.7/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/norm/__init__.py` & `m23-1.8.7/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/norm/get_line.py` & `m23-1.8.7/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/align_combined_extract.py` & `m23-1.8.7/src/m23/processor/align_combined_extract.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/config_loader.py` & `m23-1.8.7/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/generate_masterflat.py` & `m23-1.8.7/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.8.7/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/nights_csv.py` & `m23-1.8.7/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/nights_csv_config_loader.py` & `m23-1.8.7/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/process_nights.py` & `m23-1.8.7/src/m23/processor/process_nights.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     M23_RAW_IMAGES_FOLDER_NAME,
     MASTER_DARK_NAME,
     OUTPUT_CALIBRATION_FOLDER_NAME,
     RAW_CALIBRATED_FOLDER_NAME,
     SKY_BG_BOX_REGION_SIZE,
     SKY_BG_FOLDER_NAME,
 )
+from m23.exceptions import InternightException
 from m23.extract import sky_bg_average_for_all_regions
 from m23.file.aligned_combined_file import AlignedCombinedFile
 from m23.file.alignment_stats_file import AlignmentStatsFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.masterflat_file import MasterflatFile
 from m23.file.raw_image_file import RawImageFile
 from m23.file.reference_log_file import ReferenceLogFile
@@ -49,15 +50,15 @@
     get_output_folder_name_from_night_date,
     get_radius_folder_name,
     get_raw_images,
     sorted_by_number,
 )
 
 
-def normalization_helper(
+def normalization_helper(  # noqa
     radii_of_extraction: List[int],
     reference_log_file: ReferenceLogFile,
     log_files_to_use: List[LogFileCombinedFile],
     img_duration: float,
     night_date: date,
     color_ref_file_path: Path,
     output: Path,
@@ -97,20 +98,24 @@
         log_files_to_use, FLUX_LOGS_COMBINED_OUTPUT_FOLDER.parent, radii_of_extraction
     )
 
     # Generate sky bg file
     sky_bg_filename = output / SKY_BG_FOLDER_NAME / SkyBgFile.generate_file_name(night_date)
 
     # Internight normalization
-    normfactors = internight_normalize(
-        output,
-        logfile_combined_reference_logfile,
-        color_ref_file_path,
-        radii_of_extraction,
-    )
+    try:
+        normfactors = internight_normalize(
+            output,
+            logfile_combined_reference_logfile,
+            color_ref_file_path,
+            radii_of_extraction,
+        )
+    except InternightException:
+        logger.error("Returning in middle of internight normalization")
+        return
 
     # Create folder if it doesn't exist
     sky_bg_filename.parent.mkdir(parents=True, exist_ok=True)
     color_normfactors = {
         radius: normfactors[radius]["color"].items() for radius in radii_of_extraction
     }
     brightness_normfactors = {
```

### Comparing `m23-1.8.6/src/m23/processor/renormalize.py` & `m23-1.8.7/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/processor/renormalize_config_loader.py` & `m23-1.8.7/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.8.7/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/reference/MeanRI100.txt` & `m23-1.8.7/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/reference/README.md` & `m23-1.8.7/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/reference/m23_3.5_071.fit` & `m23-1.8.7/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.8.7/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/sky/__init__.py` & `m23-1.8.7/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/sky/moon/__init__.py` & `m23-1.8.7/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/utils/__init__.py` & `m23-1.8.7/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/utils/date.py` & `m23-1.8.7/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/src/m23/utils/rename.py` & `m23-1.8.7/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/.gitignore` & `m23-1.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/README.md` & `m23-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.6/pyproject.toml` & `m23-1.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.8.6"
+version = "1.8.7"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.8.6/PKG-INFO` & `m23-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.8.6
+Version: 1.8.7
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
```

