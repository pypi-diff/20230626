# Comparing `tmp/m23-1.8.4.tar.gz` & `tmp/m23-1.8.5.tar.gz`

## Comparing `m23-1.8.4.tar` & `m23-1.8.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.4/.flake8
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 m23-1.8.4/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.4/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.4/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.4/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.4/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.4/renormalize.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.4/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.4/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.4/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.4/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.4/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.4/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.4/README.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 m23-1.8.4/pyproject.toml
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 m23-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.5/.flake8
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 m23-1.8.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.5/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.5/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.5/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.5/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.5/renormalize.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 m23-1.8.5/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.5/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.5/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.5/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.5/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.5/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.5/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.5/PKG-INFO
```

### Comparing `m23-1.8.4/CHANGELOG.md` & `m23-1.8.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.5 (2023-06-25)
+
+### Fix
+
+* Use multiprocessing to use different CPUs to process different nights ([`f761a5b`](https://github.com/LutherAstrophysics/m23/commit/f761a5b797416f45c30b6d3591dd25d2a3c2b2af))
+
 ## v1.8.4 (2023-06-25)
 
 ### Fix
 
 * Multiprocessing logging in windows ([`4851295`](https://github.com/LutherAstrophysics/m23/commit/4851295a6a5b008779ecc904fc3b33c572124cd7))
 * Enhance windows logging support for multiprocessing ([`524cdbb`](https://github.com/LutherAstrophysics/m23/commit/524cdbbf419e1bfa959475999f05e27ede7bb667))
```

### Comparing `m23-1.8.4/brown.toml` & `m23-1.8.5/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/mf.toml` & `m23-1.8.5/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/nights_csv.toml` & `m23-1.8.5/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/rainbow.toml` & `m23-1.8.5/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/requirements.txt` & `m23-1.8.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/.github/workflows/python-publish.yml` & `m23-1.8.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/.vscode/settings.json` & `m23-1.8.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/__main__.py` & `m23-1.8.5/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/constants.py` & `m23-1.8.5/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/align/__init__.py` & `m23-1.8.5/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/calibrate/calibration.py` & `m23-1.8.5/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/calibrate/master_calibrate.py` & `m23-1.8.5/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/charts/__init__.py` & `m23-1.8.5/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/combine/__init__.py` & `m23-1.8.5/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/extract/__init__.py` & `m23-1.8.5/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/__init__.py` & `m23-1.8.5/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/aligned_combined_file.py` & `m23-1.8.5/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/alignment_stats_file.py` & `m23-1.8.5/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/color_normalized_file.py` & `m23-1.8.5/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/flux_log_combined_file.py` & `m23-1.8.5/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/log_file_combined_file.py` & `m23-1.8.5/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/masterflat_file.py` & `m23-1.8.5/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/normfactor_file.py` & `m23-1.8.5/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/raw_image_file.py` & `m23-1.8.5/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/reference_log_file.py` & `m23-1.8.5/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/ri_color_file.py` & `m23-1.8.5/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/file/sky_bg_file.py` & `m23-1.8.5/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/internight_normalize/__init__.py` & `m23-1.8.5/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/matrix/fill.py` & `m23-1.8.5/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/norm/__init__.py` & `m23-1.8.5/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/norm/get_line.py` & `m23-1.8.5/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/align_combined_extract.py` & `m23-1.8.5/src/m23/processor/align_combined_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import logging
 from datetime import timedelta
 from pathlib import Path
 
 import numpy as np
-from logger_tt import setup_logging
+
 from m23.align import image_alignment
 from m23.calibrate.calibration import calibrateImages
-from m23.constants import (ALIGNED_COMBINED_FOLDER_NAME, ALIGNED_FOLDER_NAME,
-                           LOG_FILES_COMBINED_FOLDER_NAME,
-                           M23_RAW_IMAGES_FOLDER_NAME,
-                           RAW_CALIBRATED_FOLDER_NAME)
+from m23.constants import (
+    ALIGNED_COMBINED_FOLDER_NAME,
+    ALIGNED_FOLDER_NAME,
+    LOG_FILES_COMBINED_FOLDER_NAME,
+    M23_RAW_IMAGES_FOLDER_NAME,
+    RAW_CALIBRATED_FOLDER_NAME,
+)
 from m23.exceptions import CouldNotAlignException
 from m23.extract import extract_stars
 from m23.file.aligned_combined_file import AlignedCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.raw_image_file import RawImageFile
 from m23.file.reference_log_file import ReferenceLogFile
 from m23.matrix import crop
 from m23.matrix.fill import fillMatrix
 from m23.processor.config_loader import Config, ConfigInputNight
 from m23.utils import time_taken_to_capture_and_save_a_raw_file
 
-setup_logging(use_multiprocessing=True)
 
 def align_combined_extract(
     config: Config,
     night: ConfigInputNight,
     output: Path,
     night_date,
     nth_combined_image,
     raw_images,
     master_dark_data,
     master_flat_data,
     alignment_stats_file,
     image_duration,
-    log_files_to_normalize_queue,
+    log_files_to_normalize,
 ):
     logger = logging.getLogger("LOGGER_" + str(night_date))
 
     # Define relevant input folders for the night being processed
     NIGHT_INPUT_FOLDER: Path = night["path"]
     NIGHT_INPUT_IMAGES_FOLDER = NIGHT_INPUT_FOLDER / M23_RAW_IMAGES_FOLDER_NAME
 
@@ -171,15 +173,15 @@
         reference_log_file,
         radii_of_extraction,
         log_file_combined_file,
         aligned_combined_file,
         date_time_to_use,
     )
 
-    log_files_to_normalize_queue.put(log_file_combined_file)
+    log_files_to_normalize.append(log_file_combined_file)
     logger.info(f"Extraction from combination {from_index}-{to_index} completed")
 
 
 def get_datetime_to_use(
     aligned_combined: AlignedCombinedFile,
     night_config: ConfigInputNight,
     no_of_raw_images_in_one_combination: int,
```

### Comparing `m23-1.8.4/src/m23/processor/config_loader.py` & `m23-1.8.5/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/generate_masterflat.py` & `m23-1.8.5/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.8.5/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/nights_csv.py` & `m23-1.8.5/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/nights_csv_config_loader.py` & `m23-1.8.5/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/process_nights.py` & `m23-1.8.5/src/m23/processor/process_nights.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,40 +310,29 @@
     no_of_combined_images = len(raw_images) // no_of_images_to_combine
 
     # Create a file for storing alignment transformation
     alignment_stats_file_name = AlignmentStatsFile.generate_file_name(night_date)
     alignment_stats_file = AlignmentStatsFile(output / alignment_stats_file_name)
     alignment_stats_file.create_file_and_write_header()
 
-    # We use multiprocessing to run alignment/combination/extraction in parallel
-    with mp.Manager() as manager:
-        log_files_to_normalize_queue = manager.Queue()
-        with mp.Pool() as p:
-
-            def align_combine_extract_mapper(nth_combined_image):
-                align_combined_extract(
-                    config,
-                    night,
-                    output,
-                    night_date,
-                    nth_combined_image,
-                    raw_images,
-                    master_dark_data,
-                    master_flat_data,
-                    alignment_stats_file,
-                    image_duration,
-                    log_files_to_normalize_queue,
-                )
-
-            p.map(align_combine_extract_mapper, range(no_of_combined_images))
-
-        log_files_to_normalize: List[LogFileCombinedFile] = []
-        while not log_files_to_normalize_queue.empty():
-            log_file: LogFileCombinedFile = log_files_to_normalize_queue.get()
-            log_files_to_normalize.append(log_file)
+    log_files_to_normalize: List[LogFileCombinedFile] = []
+    for nth_combined_image in range(no_of_combined_images):
+        align_combined_extract(
+            config,
+            night,
+            output,
+            night_date,
+            nth_combined_image,
+            raw_images,
+            master_dark_data,
+            master_flat_data,
+            alignment_stats_file,
+            image_duration,
+            log_files_to_normalize,
+        )
 
     # Intranight + Internight Normalization
     normalization_helper(
         radii_of_extraction,
         reference_log_file,
         log_files_to_normalize,
         image_duration,
@@ -360,23 +349,26 @@
     putting together various functionalities like calibration, alignment,
     extraction, and normalization together.
     """
 
     OUTPUT_PATH: Path = config["output"]["path"]
     # If directory doesn't exist create directory including necessary parent directories.
     OUTPUT_PATH.mkdir(parents=True, exist_ok=True)
-
-    for night in config["input"]["nights"]:
+    
+    def process_nights_mapper(night):
         night_path: Path = night["path"]
         night_date = get_date_from_input_night_folder_name(night_path.name)
         OUTPUT_NIGHT_FOLDER = OUTPUT_PATH / get_output_folder_name_from_night_date(night_date)
         # Create output folder for the night, if it doesn't already exist
         OUTPUT_NIGHT_FOLDER.mkdir(exist_ok=True)
         process_night(night, config, OUTPUT_NIGHT_FOLDER, night_date)
 
+    with mp.Pool() as p:
+        p.map(process_nights_mapper, config["input"]["nights"])
+
 
 def start_data_processing(file_path: str):
     """
     Starts data processing with the configuration file `file_path` provided as the argument.
     Calls auxiliary function `start_data_processing_auxiliary` if the configuration is valid.
     """
     validate_file(Path(file_path), on_success=start_data_processing_auxiliary)
```

### Comparing `m23-1.8.4/src/m23/processor/renormalize.py` & `m23-1.8.5/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/processor/renormalize_config_loader.py` & `m23-1.8.5/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.8.5/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/reference/MeanRI100.txt` & `m23-1.8.5/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/reference/README.md` & `m23-1.8.5/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/reference/m23_3.5_071.fit` & `m23-1.8.5/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.8.5/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/sky/__init__.py` & `m23-1.8.5/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/sky/moon/__init__.py` & `m23-1.8.5/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/utils/__init__.py` & `m23-1.8.5/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/utils/date.py` & `m23-1.8.5/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/src/m23/utils/rename.py` & `m23-1.8.5/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/.gitignore` & `m23-1.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/README.md` & `m23-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.4/pyproject.toml` & `m23-1.8.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.8.4"
+version = "1.8.5"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
     'matplotlib==3.7.0',
     'ephem==4.1.4',
-    'multiprocess==0.70.14',
-    'logger-tt==1.7.3'
+    'multiprocess==0.70.14'
 ]
 
 [tool.semantic_release]
 branch = "main"
 version_variable = "src/m23/__init__.py:__version__"
 version_toml = "pyproject.toml:project.version"
 version_source = "tag"
```

### Comparing `m23-1.8.4/PKG-INFO` & `m23-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.8.4
+Version: 1.8.5
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
-Requires-Dist: logger-tt==1.7.3
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing-extensions==4.4.0
 Description-Content-Type: text/markdown
```

