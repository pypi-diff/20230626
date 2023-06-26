# Comparing `tmp/m23-1.9.3.tar.gz` & `tmp/m23-1.9.4.tar.gz`

## Comparing `m23-1.9.3.tar` & `m23-1.9.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.9.3/.flake8
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 m23-1.9.3/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.9.3/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.9.3/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.9.3/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.9.3/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.9.3/renormalize.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.9.3/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.9.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.9.3/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.9.3/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15998 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.9.3/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.9.3/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.9.3/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.9.3/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.9.3/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.9.4/.flake8
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 m23-1.9.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.9.4/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.9.4/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.9.4/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.9.4/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.9.4/renormalize.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.9.4/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.9.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.9.4/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.9.4/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15997 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.9.4/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.9.4/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.9.4/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.9.4/PKG-INFO
```

### Comparing `m23-1.9.3/CHANGELOG.md` & `m23-1.9.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.4 (2023-06-26)
+
+### Fix
+
+* Set appropriate log level ([`8ad5bbd`](https://github.com/LutherAstrophysics/m23/commit/8ad5bbdd0b6488140a44e0e2dcc8b298d8ef5a85))
+
 ## v1.9.3 (2023-06-26)
 
 ### Performance
 
 * Decrease processor usage ([`33b6443`](https://github.com/LutherAstrophysics/m23/commit/33b6443ab9586475d1f5cc14f5004d213e224c43))
 
 ## v1.9.2 (2023-06-26)
```

### Comparing `m23-1.9.3/brown.toml` & `m23-1.9.4/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/mf.toml` & `m23-1.9.4/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/nights_csv.toml` & `m23-1.9.4/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/rainbow.toml` & `m23-1.9.4/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/requirements.txt` & `m23-1.9.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/.github/workflows/python-publish.yml` & `m23-1.9.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/.vscode/settings.json` & `m23-1.9.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/__main__.py` & `m23-1.9.4/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/constants.py` & `m23-1.9.4/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/align/__init__.py` & `m23-1.9.4/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/calibrate/calibration.py` & `m23-1.9.4/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/calibrate/master_calibrate.py` & `m23-1.9.4/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/charts/__init__.py` & `m23-1.9.4/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/combine/__init__.py` & `m23-1.9.4/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/extract/__init__.py` & `m23-1.9.4/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/__init__.py` & `m23-1.9.4/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/aligned_combined_file.py` & `m23-1.9.4/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/alignment_stats_file.py` & `m23-1.9.4/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/color_normalized_file.py` & `m23-1.9.4/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/flux_log_combined_file.py` & `m23-1.9.4/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/log_file_combined_file.py` & `m23-1.9.4/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/masterflat_file.py` & `m23-1.9.4/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/normfactor_file.py` & `m23-1.9.4/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/raw_image_file.py` & `m23-1.9.4/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/reference_log_file.py` & `m23-1.9.4/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/ri_color_file.py` & `m23-1.9.4/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/file/sky_bg_file.py` & `m23-1.9.4/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/internight_normalize/__init__.py` & `m23-1.9.4/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/matrix/fill.py` & `m23-1.9.4/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/norm/__init__.py` & `m23-1.9.4/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/norm/get_line.py` & `m23-1.9.4/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/align_combined_extract.py` & `m23-1.9.4/src/m23/processor/align_combined_extract.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/config_loader.py` & `m23-1.9.4/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/generate_masterflat.py` & `m23-1.9.4/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.9.4/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/nights_csv.py` & `m23-1.9.4/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/nights_csv_config_loader.py` & `m23-1.9.4/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/processor/process_nights.py` & `m23-1.9.4/src/m23/processor/process_nights.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     log_file_path = output / get_log_file_name(night_date)
     # Clear file contents if exists, so that reprocessing a night wipes out
     # contents instead of appending to it
     if log_file_path.exists():
         log_file_path.unlink()
 
     logger = logging.getLogger("LOGGER_" + str(night_date))
-    logger.setLevel(logging.DEBUG)
+    logger.setLevel(logging.INFO)
     formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     ch = logging.FileHandler(log_file_path)
     ch.setFormatter(formatter)
     logger.addHandler(ch)
     # Write to std out in addition to writing to a logfile
     ch2 = logging.StreamHandler(sys.stdout)
     ch2.setFormatter(formatter)
```

### Comparing `m23-1.9.3/src/m23/processor/renormalize.py` & `m23-1.9.4/src/m23/processor/renormalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def night_renorm_mapper(night):
         NIGHT_FOLDER = night["path"]
         night_date = get_date_from_input_night_folder_name(NIGHT_FOLDER.name)
         log_file_path = NIGHT_FOLDER / get_log_file_name(night_date)
         radii_of_extraction = renormalize_dict["processing"]["radii_of_extraction"]
 
         logger = logging.getLogger("LOGGER_" + str(night_date))
-        logger.setLevel(logging.DEBUG)
+        logger.setLevel(logging.INFO)
         formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         ch = logging.FileHandler(log_file_path)
         ch.setFormatter(formatter)
         logger.addHandler(ch)
         # Write to std out in addition to writing to a logfile
         ch2 = logging.StreamHandler(sys.stdout)
         ch2.setFormatter(formatter)
```

### Comparing `m23-1.9.3/src/m23/processor/renormalize_config_loader.py` & `m23-1.9.4/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.9.4/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/reference/MeanRI100.txt` & `m23-1.9.4/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/reference/README.md` & `m23-1.9.4/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/reference/m23_3.5_071.fit` & `m23-1.9.4/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.9.4/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/sky/__init__.py` & `m23-1.9.4/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/sky/moon/__init__.py` & `m23-1.9.4/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/utils/__init__.py` & `m23-1.9.4/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/utils/date.py` & `m23-1.9.4/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/src/m23/utils/rename.py` & `m23-1.9.4/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/.gitignore` & `m23-1.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/README.md` & `m23-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.9.3/pyproject.toml` & `m23-1.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.9.3"
+version = "1.9.4"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.9.3/PKG-INFO` & `m23-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.9.3
+Version: 1.9.4
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
```

