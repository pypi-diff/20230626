# Comparing `tmp/geonomics-1.3.8.tar.gz` & `tmp/geonomics-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonomics-1.3.8.tar", last modified: Wed Feb 15 16:17:43 2023, max compression
+gzip compressed data, was "geonomics-1.3.9.tar", last modified: Thu Apr 13 16:57:12 2023, max compression
```

## Comparing `geonomics-1.3.8.tar` & `geonomics-1.3.9.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.968258 geonomics-1.3.8/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2021-12-01 11:42:45.000000 geonomics-1.3.8/LICENSE.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.3.8/MANIFEST.in
--rw-rw-r--   0 deth      (1000) deth      (1000)     9440 2023-02-15 16:17:43.968258 geonomics-1.3.8/PKG-INFO
--rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.3.8/README.rst
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.924258 geonomics-1.3.8/geonomics/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.3.8/geonomics/__init__.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.920258 geonomics-1.3.8/geonomics/data/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.932258 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/MMRR.R
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3514 2022-09-11 23:56:38.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/MMRR.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.932258 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/__pycache__/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/env.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/gen.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/geo.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/IBD_IBE_demo/run_mantel.R
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.932258 geonomics-1.3.8/geonomics/data/default_models/
--rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.3.8/geonomics/data/default_models/selection_params.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.936258 geonomics-1.3.8/geonomics/data/yosemite_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.936258 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.940258 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.948258 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.952258 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.956258 geonomics-1.3.8/geonomics/demos/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.3.8/geonomics/demos/_IBD_IBE.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/demos/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.3.8/geonomics/demos/_simult_select.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.3.8/geonomics/demos/_yosemite.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.956258 geonomics-1.3.8/geonomics/help/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/help/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/help/_memory_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/help/_param_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    38124 2022-01-01 17:50:11.000000 geonomics-1.3.8/geonomics/main.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.960258 geonomics-1.3.8/geonomics/ops/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/ops/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/ops/change.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    13079 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/ops/demography.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.3.8/geonomics/ops/mating.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.3.8/geonomics/ops/movement.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     7761 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/ops/mutation.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/ops/selection.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.964258 geonomics-1.3.8/geonomics/sim/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/sim/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/sim/burnin.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.3.8/geonomics/sim/data.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   132048 2023-02-15 16:08:40.000000 geonomics-1.3.8/geonomics/sim/model.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    45641 2022-12-26 20:55:09.000000 geonomics-1.3.8/geonomics/sim/params.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19969 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/sim/stats.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.964258 geonomics-1.3.8/geonomics/structs/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/structs/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5433 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/structs/community.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    63099 2022-09-04 20:07:18.000000 geonomics-1.3.8/geonomics/structs/genome.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8672 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/structs/individual.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    32817 2021-07-09 03:11:40.000000 geonomics-1.3.8/geonomics/structs/landscape.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   120572 2023-02-15 14:34:17.000000 geonomics-1.3.8/geonomics/structs/species.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.968258 geonomics-1.3.8/geonomics/utils/
--rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/utils/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.3.8/geonomics/utils/_str_repr_.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10533 2021-03-24 04:15:29.000000 geonomics-1.3.8/geonomics/utils/io.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.3.8/geonomics/utils/spatial.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.3.8/geonomics/utils/viz.py
--rw-rw-r--   0 deth      (1000) deth      (1000)       22 2023-02-15 16:13:38.000000 geonomics-1.3.8/geonomics/version.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-02-15 16:17:43.924258 geonomics-1.3.8/geonomics.egg-info/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     9440 2023-02-15 16:17:43.000000 geonomics-1.3.8/geonomics.egg-info/PKG-INFO
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2023-02-15 16:17:43.000000 geonomics-1.3.8/geonomics.egg-info/SOURCES.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2023-02-15 16:17:43.000000 geonomics-1.3.8/geonomics.egg-info/dependency_links.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2023-02-15 16:17:43.000000 geonomics-1.3.8/geonomics.egg-info/requires.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2023-02-15 16:17:43.000000 geonomics-1.3.8/geonomics.egg-info/top_level.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2023-02-15 16:17:43.968258 geonomics-1.3.8/setup.cfg
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2680 2022-01-01 17:57:19.000000 geonomics-1.3.8/setup.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.940418 geonomics-1.3.9/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2021-12-01 11:42:45.000000 geonomics-1.3.9/LICENSE.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.3.9/MANIFEST.in
+-rw-rw-r--   0 deth      (1000) deth      (1000)     9440 2023-04-13 16:57:12.940418 geonomics-1.3.9/PKG-INFO
+-rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.3.9/README.rst
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.896418 geonomics-1.3.9/geonomics/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.3.9/geonomics/__init__.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.896418 geonomics-1.3.9/geonomics/data/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.904418 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/MMRR.R
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3514 2022-09-11 23:56:38.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/MMRR.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.908418 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/__pycache__/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/env.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/gen.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/geo.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/IBD_IBE_demo/run_mantel.R
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.908418 geonomics-1.3.9/geonomics/data/default_models/
+-rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.3.9/geonomics/data/default_models/selection_params.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.908418 geonomics-1.3.9/geonomics/data/yosemite_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.908418 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.916418 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.920418 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.928418 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.928418 geonomics-1.3.9/geonomics/demos/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.3.9/geonomics/demos/_IBD_IBE.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/demos/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.3.9/geonomics/demos/_simult_select.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.3.9/geonomics/demos/_yosemite.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.932418 geonomics-1.3.9/geonomics/help/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/help/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/help/_memory_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/help/_param_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    38124 2022-01-01 17:50:11.000000 geonomics-1.3.9/geonomics/main.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.936418 geonomics-1.3.9/geonomics/ops/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/ops/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/ops/change.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    13079 2023-03-19 21:57:12.000000 geonomics-1.3.9/geonomics/ops/demography.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.3.9/geonomics/ops/mating.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.3.9/geonomics/ops/movement.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     7761 2021-07-09 03:11:40.000000 geonomics-1.3.9/geonomics/ops/mutation.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.3.9/geonomics/ops/selection.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.936418 geonomics-1.3.9/geonomics/sim/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/sim/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/sim/burnin.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.3.9/geonomics/sim/data.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   132048 2023-02-15 16:08:40.000000 geonomics-1.3.9/geonomics/sim/model.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    45641 2022-12-26 20:55:09.000000 geonomics-1.3.9/geonomics/sim/params.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2023-04-13 16:46:44.000000 geonomics-1.3.9/geonomics/sim/stats.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.940418 geonomics-1.3.9/geonomics/structs/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/structs/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5433 2021-07-09 03:11:40.000000 geonomics-1.3.9/geonomics/structs/community.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    63099 2022-09-04 20:07:18.000000 geonomics-1.3.9/geonomics/structs/genome.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     8672 2021-07-09 03:11:40.000000 geonomics-1.3.9/geonomics/structs/individual.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    32817 2021-07-09 03:11:40.000000 geonomics-1.3.9/geonomics/structs/landscape.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   120572 2023-02-15 14:34:17.000000 geonomics-1.3.9/geonomics/structs/species.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.940418 geonomics-1.3.9/geonomics/utils/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/utils/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.3.9/geonomics/utils/_str_repr_.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10807 2023-04-13 16:46:40.000000 geonomics-1.3.9/geonomics/utils/io.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.3.9/geonomics/utils/spatial.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.3.9/geonomics/utils/viz.py
+-rw-rw-r--   0 deth      (1000) deth      (1000)       22 2023-04-13 16:54:23.000000 geonomics-1.3.9/geonomics/version.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2023-04-13 16:57:12.896418 geonomics-1.3.9/geonomics.egg-info/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9440 2023-04-13 16:57:12.000000 geonomics-1.3.9/geonomics.egg-info/PKG-INFO
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2023-04-13 16:57:12.000000 geonomics-1.3.9/geonomics.egg-info/SOURCES.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2023-04-13 16:57:12.000000 geonomics-1.3.9/geonomics.egg-info/dependency_links.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2023-04-13 16:57:12.000000 geonomics-1.3.9/geonomics.egg-info/requires.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2023-04-13 16:57:12.000000 geonomics-1.3.9/geonomics.egg-info/top_level.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2023-04-13 16:57:12.940418 geonomics-1.3.9/setup.cfg
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2680 2022-01-01 17:57:19.000000 geonomics-1.3.9/setup.py
```

### Comparing `geonomics-1.3.8/LICENSE.txt` & `geonomics-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/PKG-INFO` & `geonomics-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.3.8
+Version: 1.3.9
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.3.8.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.3.9.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geonomics-1.3.8/README.rst` & `geonomics-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/MMRR.R` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/MMRR.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/MMRR.py` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/MMRR.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/env.csv` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/env.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/gen.csv` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/gen.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/geo.csv` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/geo.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/IBD_IBE_demo/run_mantel.R` & `geonomics-1.3.9/geonomics/data/IBD_IBE_demo/run_mantel.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/default_models/selection_params.py` & `geonomics-1.3.9/geonomics/data/default_models/selection_params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif` & `geonomics-1.3.9/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/demos/_IBD_IBE.py` & `geonomics-1.3.9/geonomics/demos/_IBD_IBE.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/demos/_simult_select.py` & `geonomics-1.3.9/geonomics/demos/_simult_select.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/demos/_yosemite.py` & `geonomics-1.3.9/geonomics/demos/_yosemite.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/help/__init__.py` & `geonomics-1.3.9/geonomics/help/__init__.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/help/_memory_help.py` & `geonomics-1.3.9/geonomics/help/_memory_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/help/_param_help.py` & `geonomics-1.3.9/geonomics/help/_param_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/main.py` & `geonomics-1.3.9/geonomics/main.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/change.py` & `geonomics-1.3.9/geonomics/ops/change.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/demography.py` & `geonomics-1.3.9/geonomics/ops/demography.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/mating.py` & `geonomics-1.3.9/geonomics/ops/mating.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/movement.py` & `geonomics-1.3.9/geonomics/ops/movement.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/mutation.py` & `geonomics-1.3.9/geonomics/ops/mutation.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/ops/selection.py` & `geonomics-1.3.9/geonomics/ops/selection.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/sim/burnin.py` & `geonomics-1.3.9/geonomics/sim/burnin.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/sim/data.py` & `geonomics-1.3.9/geonomics/sim/data.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/sim/model.py` & `geonomics-1.3.9/geonomics/sim/model.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/sim/params.py` & `geonomics-1.3.9/geonomics/sim/params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/sim/stats.py` & `geonomics-1.3.9/geonomics/sim/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
     N = len(spp)
     #get the speciome
     speciome = spp._get_genotypes()
     #calculate the frequency of heterozygotes, locus-wise
     het = np.sum(np.mean(speciome, axis = 2) == 0.5, axis = 0)/N
     #get the mean heterozygosity, if mean argument is True
     if mean:
-        het = mean(het)
+        het = np.mean(het)
     return(het)
 
 #function to calculate the locus-wise minor allele frequency of the species
 def _calc_maf(spp):
     #get two times the pop size
     two_N = 2*len(spp)
     #get the speciome
```

### Comparing `geonomics-1.3.8/geonomics/structs/community.py` & `geonomics-1.3.9/geonomics/structs/community.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/structs/genome.py` & `geonomics-1.3.9/geonomics/structs/genome.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/structs/individual.py` & `geonomics-1.3.9/geonomics/structs/individual.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/structs/landscape.py` & `geonomics-1.3.9/geonomics/structs/landscape.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/structs/species.py` & `geonomics-1.3.9/geonomics/structs/species.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/utils/_str_repr_.py` & `geonomics-1.3.9/geonomics/utils/_str_repr_.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/utils/io.py` & `geonomics-1.3.9/geonomics/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,19 @@
     with open(filepath, 'a') as f:
         f.write(tmp_txt)
     os.remove(tmp_filename)
 
 
 # append a row of data to a CSV file
 def _append_row_to_csv(filepath, locuswise_array1d, t):
+    if (not isinstance(locuswise_array1d, list) and
+        not isinstance(locuswise_array1d, np.ndarray)):
+        assert (isinstance(locuswise_array1d, float) or
+                isinstance(locuswise_array1d, int))
+        locuswise_array1d = np.array([locuswise_array1d])
     data_dict = dict(zip(range(locuswise_array1d.size), locuswise_array1d))
     write_header = not os.path.exists(filepath)
     with open(filepath, 'a') as f:
         dict_writer = csv.DictWriter(f, ['t'] + [*data_dict.keys()])
         if write_header:
             dict_writer.writeheader()
         dict_writer.writerow({'t': t, **data_dict})
```

### Comparing `geonomics-1.3.8/geonomics/utils/spatial.py` & `geonomics-1.3.9/geonomics/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics/utils/viz.py` & `geonomics-1.3.9/geonomics/utils/viz.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/geonomics.egg-info/PKG-INFO` & `geonomics-1.3.9/geonomics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.3.8
+Version: 1.3.9
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.3.8.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.3.9.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geonomics-1.3.8/geonomics.egg-info/SOURCES.txt` & `geonomics-1.3.9/geonomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.3.8/setup.py` & `geonomics-1.3.9/setup.py`

 * *Files identical despite different names*

