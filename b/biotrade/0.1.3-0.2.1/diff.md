# Comparing `tmp/biotrade-0.1.3.tar.gz` & `tmp/biotrade-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotrade-0.1.3.tar", last modified: Wed May 10 17:22:40 2023, max compression
+gzip compressed data, was "biotrade-0.2.1.tar", last modified: Mon Jun 26 14:06:54 2023, max compression
```

## Comparing `biotrade-0.1.3.tar` & `biotrade-0.2.1.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/
--rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.1.3/LICENCE.md
--rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.1.3/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.1.3/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     8487 2023-05-10 17:22:40.643249 biotrade-0.1.3/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7729 2023-05-10 17:21:49.000000 biotrade-0.1.3/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/biotrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     1419 2023-05-10 17:21:49.000000 biotrade-0.1.3/biotrade/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.635249 biotrade-0.1.3/biotrade/common/
--rw-r--r--   0 paul      (1000) paul      (1000)    12946 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/common/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.1.3/biotrade/common/compare.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/logger.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/sanitize.py
--rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/time_series.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.1.3/biotrade/common/update.py
--rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.1.3/biotrade/common/url_request_header.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.635249 biotrade-0.1.3/biotrade/comtrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3507 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.1.3/biotrade/comtrade/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/comtrade/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    16659 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6521 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/dump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    43893 2023-04-28 17:19:21.000000 biotrade-0.1.3/biotrade/comtrade/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/quality.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/config_data/
--rw-r--r--   0 paul      (1000) paul      (1000)     2995 2022-11-14 08:51:12.000000 biotrade-0.1.3/biotrade/config_data/column_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6686 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/config_data/comtrade_faostat_product_mapping.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.1.3/biotrade/config_data/comtrade_hs_2d.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.1.3/biotrade/config_data/comtrade_hs_product_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.1.3/biotrade/config_data/comtrade_reporters.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/faostat_commodity_tree.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    43326 2023-05-10 16:55:49.000000 biotrade-0.1.3/biotrade/config_data/faostat_country_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_trade_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/faostat_products_name_code_shortname.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/regulation_front_end_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   233587 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/config_data/regulation_products.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.1.3/biotrade/config_data/wood_product_aggregates.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/eurostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.1.3/biotrade/eurostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4473 2022-05-09 10:14:29.000000 biotrade-0.1.3/biotrade/eurostat/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/faostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.1.3/biotrade/faostat/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.1.3/biotrade/faostat/coefficients.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/convert.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-05-10 13:26:24.000000 biotrade-0.1.3/biotrade/faostat/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.1.3/biotrade/faostat/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4132 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/faostat/mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.1.3/biotrade/faostat/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/quality.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/share_coefficients.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/hwp/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.1.3/biotrade/hwp/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/hwp/country.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/biotrade/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/tests/test_aggregate.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/biotrade/world_bank/
--rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/world_bank/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/world_bank/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8964 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/world_bank/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/biotrade.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     8487 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     2627 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       76 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       36 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/scripts/front_end/
--rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/DEPRECATED_reporter_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2391 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/annual_variation_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/annual_variation_trade_quantity_value.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3335 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/average_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/average_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.1.3/scripts/front_end/db_scheduler.py
--rw-r--r--   0 paul      (1000) paul      (1000)    27233 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/functions.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/product_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/trends_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.1.3/scripts/front_end/trends_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.1.3/scripts/front_end/update_db.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/scripts/quality/
--rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.1.3/scripts/quality/faostat_compare_aggregates_to_constituents.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-05-10 17:22:40.643249 biotrade-0.1.3/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1554 2023-05-10 17:21:49.000000 biotrade-0.1.3/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.126624 biotrade-0.2.1/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.2.1/LICENCE.md
+-rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.2.1/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.2.1/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-06-26 14:06:54.126624 biotrade-0.2.1/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7600 2023-06-26 14:05:44.000000 biotrade-0.2.1/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.114624 biotrade-0.2.1/biotrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3634 2023-06-26 14:05:44.000000 biotrade-0.2.1/biotrade/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.118624 biotrade-0.2.1/biotrade/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)    13743 2023-06-26 13:47:11.000000 biotrade-0.2.1/biotrade/common/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.2.1/biotrade/common/compare.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/logger.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3921 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/common/reallocate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/sanitize.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/common/time_series.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.2.1/biotrade/common/update.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.2.1/biotrade/common/url_request_header.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.118624 biotrade-0.2.1/biotrade/comtrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/comtrade/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.2.1/biotrade/comtrade/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.2.1/biotrade/comtrade/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20253 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/comtrade/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6819 2023-06-26 13:47:11.000000 biotrade-0.2.1/biotrade/comtrade/dump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/comtrade/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    46862 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/comtrade/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/comtrade/quality.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.118624 biotrade-0.2.1/biotrade/config_data/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3860 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/config_data/column_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6719 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/config_data/comtrade_faostat_product_mapping.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.2.1/biotrade/config_data/comtrade_hs_2d.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.2.1/biotrade/config_data/comtrade_hs_product_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.2.1/biotrade/config_data/comtrade_reporters.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.2.1/biotrade/config_data/faostat_commodity_tree.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    43339 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/config_data/faostat_country_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.2.1/biotrade/config_data/faostat_forestry_production_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.2.1/biotrade/config_data/faostat_forestry_production_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.2.1/biotrade/config_data/faostat_forestry_trade_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.2.1/biotrade/config_data/faostat_products_name_code_shortname.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.2.1/biotrade/config_data/regulation_front_end_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   233668 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/config_data/regulation_products.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.2.1/biotrade/config_data/wood_product_aggregates.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.122624 biotrade-0.2.1/biotrade/eurostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.2.1/biotrade/eurostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4632 2023-06-26 14:05:44.000000 biotrade-0.2.1/biotrade/eurostat/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.122624 biotrade-0.2.1/biotrade/faostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.2.1/biotrade/faostat/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.2.1/biotrade/faostat/coefficients.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/convert.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:47:11.000000 biotrade-0.2.1/biotrade/faostat/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.2.1/biotrade/faostat/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4179 2023-06-08 08:14:15.000000 biotrade-0.2.1/biotrade/faostat/mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.2.1/biotrade/faostat/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/quality.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/faostat/share_coefficients.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.122624 biotrade-0.2.1/biotrade/hwp/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.2.1/biotrade/hwp/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/hwp/country.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.122624 biotrade-0.2.1/biotrade/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/tests/test_aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3469 2023-06-26 13:50:21.000000 biotrade-0.2.1/biotrade/tests/test_front_end.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      837 2023-05-15 17:30:05.000000 biotrade-0.2.1/biotrade/tests/test_mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3145 2023-06-26 13:47:11.000000 biotrade-0.2.1/biotrade/tests/test_reallocate.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.122624 biotrade-0.2.1/biotrade/world_bank/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/world_bank/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.2.1/biotrade/world_bank/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9162 2023-05-15 15:21:01.000000 biotrade-0.2.1/biotrade/world_bank/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.114624 biotrade-0.2.1/biotrade.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-06-26 14:06:54.000000 biotrade-0.2.1/biotrade.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     2754 2023-06-26 14:06:54.000000 biotrade-0.2.1/biotrade.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-06-26 14:06:54.000000 biotrade-0.2.1/biotrade.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      123 2023-06-26 14:06:54.000000 biotrade-0.2.1/biotrade.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2023-06-26 14:06:54.000000 biotrade-0.2.1/biotrade.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.114624 biotrade-0.2.1/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.126624 biotrade-0.2.1/scripts/front_end/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.2.1/scripts/front_end/DEPRECATED_reporter_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2583 2023-06-26 13:50:21.000000 biotrade-0.2.1/scripts/front_end/annual_variation_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.2.1/scripts/front_end/annual_variation_trade_quantity_value.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3571 2023-06-26 13:50:21.000000 biotrade-0.2.1/scripts/front_end/average_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.2.1/scripts/front_end/average_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.2.1/scripts/front_end/db_scheduler.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    27701 2023-06-26 13:50:21.000000 biotrade-0.2.1/scripts/front_end/functions.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.2.1/scripts/front_end/product_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.2.1/scripts/front_end/trends_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.2.1/scripts/front_end/trends_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.2.1/scripts/front_end/update_db.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 14:06:54.126624 biotrade-0.2.1/scripts/quality/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.2.1/scripts/quality/faostat_compare_aggregates_to_constituents.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-06-26 14:06:54.126624 biotrade-0.2.1/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1644 2023-06-26 14:05:44.000000 biotrade-0.2.1/setup.py
```

### Comparing `biotrade-0.1.3/LICENCE.md` & `biotrade-0.2.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/NOTICE.txt` & `biotrade-0.2.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/PKG-INFO` & `biotrade-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.1.3
+Version: 0.2.1
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
@@ -22,14 +22,20 @@
 
 The `biotrade` package analyses international trade of bio-based products. It focuses on
 the agriculture and forestry sectors, from primary production to secondary products
 transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
+# Documentation
+
+The documentation is available at:
+https://bioeconomy.gitlab.io/forobs/biotrade/
+
+
 # Installation
 
 ## Base installation
 
 Install the biotrade package from the python package index with pip:
 
     python -m pip install biotrade
@@ -212,16 +218,14 @@
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
 
 # Similar projects
 
-- The python package [pandas-datareader](https://pydata.github.io/pandas-datareader/)
-
 - The R packages FAOSTAT and WDI
 
 
 # Tests
 
 This package uses pytest for unit testing. Run the test suite with
 
@@ -239,11 +243,9 @@
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
 The authors would like to acknowledge ideas and feedback received from the following
-persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
-
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
-inspiration to load Eurostat data from the bulk download repository.
+persons: Giovanni Bausano, Noemi Cazzaniga, Mirco Migliavacca, Roberto Pilli, Lucas
+Sinclair.
```

### Comparing `biotrade-0.1.3/README.md` & `biotrade-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 The `biotrade` package analyses international trade of bio-based products. It focuses on
 the agriculture and forestry sectors, from primary production to secondary products
 transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
+# Documentation
+
+The documentation is available at:
+https://bioeconomy.gitlab.io/forobs/biotrade/
+
+
 # Installation
 
 ## Base installation
 
 Install the biotrade package from the python package index with pip:
 
     python -m pip install biotrade
@@ -190,16 +196,14 @@
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
 
 # Similar projects
 
-- The python package [pandas-datareader](https://pydata.github.io/pandas-datareader/)
-
 - The R packages FAOSTAT and WDI
 
 
 # Tests
 
 This package uses pytest for unit testing. Run the test suite with
 
@@ -217,11 +221,9 @@
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
 The authors would like to acknowledge ideas and feedback received from the following
-persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
-
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
-inspiration to load Eurostat data from the bulk download repository.
+persons: Giovanni Bausano, Noemi Cazzaniga, Mirco Migliavacca, Roberto Pilli, Lucas
+Sinclair.
```

### Comparing `biotrade-0.1.3/biotrade/common/aggregate.py` & `biotrade-0.2.1/biotrade/common/aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,27 @@
         >>> swdoak = comtrade.db.select(table="yearly", product_code="440791")
         >>> # Display interesting columns
         >>> swdoak[["reporter", "partner", "year", 'unit', 'quantity', 'net_weight','trade_value']]
         >>> # Aggregate to EU and ROW
         >>> swdoak_agg = agg_trade_eu_row(swdoak, drop_index_col=["flag"],
         >>>                               value_col=['quantity', 'net_weight','trade_value'])
 
+    Select Yearly soy trade from Comtrade then aggregate over EU and Rest of the World
+
+        >>> from biotrade.comtrade import comtrade
+        >>> from biotrade.common.aggregate import agg_trade_eu_row
+        >>> df = comtrade.db.select("yearly", product_code_start="1507", partner="Brazil")
+        >>> cols_of_interest = ['classification', 'year',
+        >>>        'flow_code', 'flow', 'reporter_code',
+        >>>        'reporter', 'partner_code', 'partner', 'partner_iso',
+        >>>        'product_code', 'unit_code', 'unit', 'quantity', 'net_weight', 'trade_value' ]
+        >>> dfeurow = agg_trade_eu_row(df[cols_of_interest],
+        >>>                         grouping_side = "reporter",
+        >>>                         value_col=['quantity', 'net_weight','trade_value'])
+
     """
     # Make a copy of the data frame so that it will not be modified in place
     df = df.copy()
 
     # Default argument values
     if drop_index_col is None:
         drop_index_col = ["flag"]
```

### Comparing `biotrade-0.1.3/biotrade/common/compare.py` & `biotrade-0.2.1/biotrade/common/compare.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/country.py` & `biotrade-0.2.1/biotrade/common/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/database.py` & `biotrade-0.2.1/biotrade/common/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/logger.py` & `biotrade-0.2.1/biotrade/common/logger.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/products.py` & `biotrade-0.2.1/biotrade/common/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/sanitize.py` & `biotrade-0.2.1/biotrade/common/sanitize.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/time_series.py` & `biotrade-0.2.1/biotrade/common/time_series.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/update.py` & `biotrade-0.2.1/biotrade/common/update.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/common/url_request_header.py` & `biotrade-0.2.1/biotrade/common/url_request_header.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/comtrade/__init__.py` & `biotrade-0.2.1/biotrade/comtrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 
     # Location of module configuration data
     config_data_dir = module_dir / "config_data"
 
     # Load a mapping table used to rename columns
     df = pandas.read_csv(config_data_dir / "column_names.csv")
     # Select only relevant columns and remove incomplete mappings
-    df = df[["biotrade", "comtrade_machine", "comtrade_human"]]
-    column_names = df[df.isna().sum(axis=1) == 0]
+    df = df[
+        ["biotrade", "comtrade_machine", "comtrade_human", "comtrade_apicall"]
+    ]
+    column_names = df
 
     def __init__(self):
         # Location of the data
         self.data_dir = data_dir / "comtrade"
         if not self.data_dir.exists():
             self.data_dir.mkdir()
```

### Comparing `biotrade-0.1.3/biotrade/comtrade/aggregate.py` & `biotrade-0.2.1/biotrade/comtrade/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/comtrade/country_groups.py` & `biotrade-0.2.1/biotrade/comtrade/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/comtrade/database.py` & `biotrade-0.2.1/biotrade/comtrade/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 """
 # First party modules
 import logging
 import pandas
 import re
 
 # Third party modules
+import comtradeapicall
 from sqlalchemy import Integer, Float, Text, UniqueConstraint
 from sqlalchemy import Table, Column, MetaData, and_, or_
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.schema import CreateSchema
 
 # Internal modules
 from biotrade import data_dir, database_url
@@ -119,14 +120,16 @@
         """
         table = Table(
             name,
             self.metadata,
             Column("product_code", Text),
             Column("product_description", Text),
             Column("parent", Text),
+            Column("is_leaf", Integer),
+            Column("aggregate_level", Integer),
             UniqueConstraint(
                 "product_code",
             ),
             schema=self.schema,
         )
         return table
 
@@ -149,44 +152,44 @@
         Note the "product" column is left empty, removed from the data frame
         before it is stored in the database because it would be too large. The
         text description of a product (commodity) is available in the product table.
         """
         table = Table(
             name,
             self.metadata,
+            Column("dataset_code", Text),
+            Column("classification_search_code", Text),
             Column("classification", Text),
+            Column("is_original_classification", Integer),
+            Column("frequency", Text),
+            Column("ref_date", Integer),
             Column("year", Integer),
+            Column("month", Integer),
             Column("period", Integer),
-            Column("period_description", Text),
-            Column("aggregate_level", Integer),
-            Column("is_leaf", Integer),
-            Column("flow_code", Integer),
-            Column("flow", Text),
+            Column("is_reported", Integer),
+            Column("is_aggregated", Integer),
+            Column("flow_code", Text),
             Column("reporter_code", Integer, index=True),
-            Column("reporter", Text),
-            Column("reporter_iso", Text),
             Column("partner_code", Integer, index=True),
-            Column("partner", Text),
-            Column("partner_iso", Text),
-            Column("partner_2_code", Text),
-            Column("partner_2", Text),
-            Column("partner_2_iso", Text),
+            Column("partner_2_code", Integer),
             Column("customs_proc_code", Text),
-            Column("customs", Text),
-            Column("mode_of_transport_code", Text),
-            Column("mode_of_transport", Text),
+            Column("mode_of_supply_code", Text),
+            Column("mode_of_transport_code", Integer),
             Column("product_code", Text, index=True),
+            Column("product_type", Text),
             Column("unit_code", Integer),
-            Column("unit", Text),
             Column("quantity", Float),
-            Column("alt_qty_unit_code", Text),
-            Column("alt_qty_unit", Text),
+            Column("is_quantity_estimated", Integer),
+            Column("alt_qty_unit_code", Integer),
             Column("alt_qty", Float),
+            Column("is_alt_quantity_estimated", Integer),
             Column("net_weight", Float),
+            Column("is_net_weight_estimated", Integer),
             Column("gross_weight", Float),
+            Column("is_gross_weight_estimated", Integer),
             Column("trade_value", Float),
             Column("cif_value", Float),
             Column("fob_value", Float),
             Column("flag", Integer),
             UniqueConstraint(
                 "period",
                 "flow_code",
@@ -315,16 +318,14 @@
     ):
         """
         Select comtrade trade data for the given arguments
 
         :param str table: name of the database table to select from
         :param list or str reporter: list of reporter names
         :param list or str partner: list of partner names
-        :param list or str flow: list of flow directions
-            ['Imports', 'Exports', 'Re-imports', 'Re-exports']
         :param list or int reporter_code: list of reporter codes
         :param list or int partner_code: list of partner codes
         :param list or int product_code: list of product codes
             Exact matches of product codes
         :param list or int product_code_start: list of product codes
             Partial matches of all products that start with this code
         :param list or str flow: list of flow, for example "import", "export"
@@ -341,48 +342,135 @@
         table = self.tables[table]
         # Change character or integer arguments to lists suitable for a
         # column.in_() clause or for a list comprehension.
         if isinstance(reporter, str):
             reporter = [reporter]
         if isinstance(partner, str):
             partner = [partner]
-        if isinstance(reporter_code, (int, str)):
+        if isinstance(reporter_code, int):
             reporter_code = [reporter_code]
-        if isinstance(partner_code, (int, str)):
+        if isinstance(partner_code, int):
             partner_code = [partner_code]
-        if isinstance(product_code, (int, str)):
+        if isinstance(product_code, str):
             product_code = [product_code]
-        if isinstance(product_code_start, (int, str)):
+        if isinstance(product_code_start, str):
             product_code_start = [product_code_start]
         if isinstance(flow, str):
             flow = [flow]
         # Build the select statement
         stmt = table.select()
+        # Define complementary data and columns to be selected and renamed
+        column_dict = {
+            "reporterCode": "reporter_code",
+            "reporterDesc": "reporter",
+            "reporterCodeIsoAlpha3": "reporter_iso",
+            "PartnerCode": "partner_code",
+            "PartnerDesc": "partner",
+            "PartnerCodeIsoAlpha3": "partner_iso",
+            "qtyCode": "unit_code",
+            "qtyDescription": "unit",
+        }
+        # reporter data
+        reporter_data = comtradeapicall.getReference("reporter")[
+            ["reporterCode", "reporterDesc", "reporterCodeIsoAlpha3"]
+        ].rename(columns=column_dict)
+        # partner data
+        partner_data = comtradeapicall.getReference("partner")[
+            ["PartnerCode", "PartnerDesc", "PartnerCodeIsoAlpha3"]
+        ].rename(columns=column_dict)
+        # quantity data
+        quantity_data = comtradeapicall.getReference("qtyunit")[
+            ["qtyCode", "qtyDescription"]
+        ].rename(columns=column_dict)
+        # define a compiled regex
+        regex_pat = re.compile(r"\W+")
+        # flow data
+        flow_data = comtradeapicall.getReference("flow")[["id", "text"]].rename(
+            columns={"id": "flow_code", "text": "flow"}
+        )
+        # rename flow column content to snake case using the compiled regex
+        flow_data["flow"] = (
+            flow_data["flow"]
+            .str.replace(regex_pat, "_", regex=True)
+            .str.lower()
+        )
+        # mode of transport data
+        mot_data = (
+            comtradeapicall.getReference("mot")[["id", "text"]]
+            .astype({"id": int})
+            .rename(
+                columns={
+                    "id": "mode_of_transport_code",
+                    "text": "mode_of_transport",
+                }
+            )
+        )
+        # custom procedure data
+        customs_data = comtradeapicall.getReference("customs")[
+            ["id", "text"]
+        ].rename(
+            columns={
+                "id": "customs_proc_code",
+                "text": "customs",
+            }
+        )
         if reporter is not None:
-            stmt = stmt.where(table.c.reporter.in_(reporter))
+            # Obtain codes from reporter data
+            reporter = reporter_data[
+                reporter_data.reporter.isin(reporter)
+            ].reporter_code.tolist()
+            # Add already defined reporter codes
+            if isinstance(reporter_code, list):
+                reporter_code += reporter
+            else:
+                reporter_code = reporter
         if partner is not None:
-            stmt = stmt.where(table.c.partner.in_(partner))
+            # Obtain codes from partner data
+            partner = partner_data[
+                partner_data.partner.isin(partner)
+            ].partner_code.tolist()
+            # Add already defined reporter codes
+            if isinstance(partner_code, list):
+                partner_code += partner
+            else:
+                partner_code = partner
         if reporter_code is not None:
             stmt = stmt.where(table.c.reporter_code.in_(reporter_code))
         if partner_code is not None:
             stmt = stmt.where(table.c.partner_code.in_(partner_code))
         if product_code is not None:
             stmt = stmt.where(table.c.product_code.in_(product_code))
         if product_code_start is not None:
             stmt = stmt.where(
-                or_(table.c.product_code.ilike(f"{c}%") for c in product_code_start)
+                or_(
+                    table.c.product_code.ilike(f"{c}%")
+                    for c in product_code_start
+                )
             )
         if flow is not None:
-            stmt = stmt.where(table.c.flow.in_(flow))
+            # Rename flow list to snake case using the compiled regex
+            flow = [regex_pat.sub("_", item).lower() for item in flow]
+            # Obtain codes from flow data
+            flow_code = flow_data[flow_data.flow.isin(flow)].flow_code.tolist()
+            stmt = stmt.where(table.c.flow_code.in_(flow_code))
         if period_start is not None:
             stmt = stmt.where(table.c.period >= period_start)
         if period_end is not None:
             stmt = stmt.where(table.c.period <= period_end)
         # Query the database and return a data frame
         df = pandas.read_sql_query(stmt, self.engine)
+        # Merge with complementary data
+        df = (
+            df.merge(reporter_data, on="reporter_code", how="left")
+            .merge(partner_data, on="partner_code", how="left")
+            .merge(quantity_data, on="unit_code", how="left")
+            .merge(flow_data, on="flow_code", how="left")
+            .merge(mot_data, on="mode_of_transport_code", how="left")
+            .merge(customs_data, on="customs_proc_code", how="left")
+        )
         return df
 
     def select_long(self, *args, **kwargs):
         """Same as select but in long format with an element column and where
         the empty columns have been removed.
 
         Example:
@@ -396,15 +484,17 @@
         # Remove empty columns
         not_empty = [col for col in df.columns if not all(df[col].isna())]
         df = df[not_empty]
         # This can be removed once this is dealt with in comtrade/pump.py
         # Rename column content to snake case using a compiled regex
         regex_pat = re.compile(r"\W+")
         if "flow" in df.columns:
-            df["flow"] = df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
+            df["flow"] = (
+                df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
+            )
             # Remove the plural "s"
             df["flow"] = df["flow"].str.replace("s", "", regex=True)
         # TODO: Change period to a date time object
         # Reshape to long format
         value_cols = ["net_weight", "trade_value"]
         index = set(df.columns) - set(value_cols)
         df_long = df.melt(
```

### Comparing `biotrade-0.1.3/biotrade/comtrade/dump.py` & `biotrade-0.2.1/biotrade/comtrade/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         :param int chunk_size number of rows to read from the database at a time, to avoid memory errors
 
         If a list of product codes is given, store one file for each 2 digit code.
 
         For example save monthly "Animal Or Vegetable Fats And Oil" data which starts with 15:
 
             >>> from biotrade.comtrade import comtrade
-            >>> comtrade.dump.store_2d_csv("monthly", 15, chunk_size=10**4)
+            >>> comtrade.dump.store_2d_csv("monthly", 15)
 
         Dump all bioeconomy related products
 
             >>> hs2d = comtrade.products.hs2d.query("bioeconomy == 1")
             >>> for this_code in hs2d["product_code"]:
             >>>     comtrade.dump.store_2d_csv("monthly", this_code)
 
@@ -133,14 +133,20 @@
 
     def load_2d_csv(self, table, file_path):
         """Load a dump into the given database table
 
         :param (str) table, name of the database table
         :param (str or file object) file_path, path to the file from which to save the data
 
+        TODO: current version requires the user to manually delete the data
+        from the database before an update
+
+                psql $BIOTRADE_DATABASE_URL
+                DELETE FROM raw_comtrade.monthly WHERE product_code like '44%';
+
         If data is already present in the database for that product code, the
         user will be asked to confirm deletion. To avoid this confirmation
         message when processing many dump files automatically, delete all table
         content before calling this function.
 
         For information, in case the data is not deleted and if the new data causes
         duplications the database unique constraint will raise an error:
@@ -167,10 +173,11 @@
         )
         # Check that the name of the file contains the unique product code in the data
 
         # Delete existing data for the corresponding product code
         # TODO: uptate the db.delete method so that it can deal with product_code.
         # This should be possible if the where statements can be concatenated
         # Or create the statement here to delete at the HS 2 to level.
+        self.logger.info("Reading into a data frame:\n %s", file_path)
 
         # Write to the database
         self.db.append(df, table)
```

### Comparing `biotrade-0.1.3/biotrade/comtrade/products.py` & `biotrade-0.2.1/biotrade/comtrade/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/comtrade/pump.py` & `biotrade-0.2.1/biotrade/comtrade/pump.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,34 @@
 import shutil
 from zipfile import ZipFile
 import datetime
 import pytz
 import os
 import re
 import time
-import requests
-import gzip
+
+try:
+    import requests
+except Exception as e:
+    msg = "Failed to import requests, you will not be able to load data from Comtrade,"
+    msg += "but you can still use other methods.\n"
+    print(msg, str(e))
 
 # Third party modules
 import json
 import logging
 import pandas
-import comtradeapicall
+import numpy as np
+
+try:
+    import comtradeapicall
+except Exception as e:
+    msg = "Failed to import comtradeapicall package, you will not be able to load data from there,"
+    msg += "but you can still use other methods.\n"
+    print(msg, str(e))
 
 # Internal modules
 from biotrade.common.url_request_header import HEADER
 
 
 class Pump:
     """
@@ -133,25 +145,87 @@
         df.rename(columns=lambda x: re.sub(r"[()\.]", "", x), inplace=True)
         # Replace $ sign by d, used only for human readable dataset
         df.rename(columns=lambda x: re.sub(r"\$", "d", x), inplace=True)
         # Rename columns using the naming convention defined in self.column_names
         mapping = self.column_names.set_index(renaming_from).to_dict()[
             renaming_to
         ]
+        # Discard nan keys of mapping dictionary
+        mapping.pop(np.nan, None)
         df.rename(columns=mapping, inplace=True)
         # Rename column content to snake case using a compiled regex
         regex_pat = re.compile(r"\W+")
         if "flow" in df.columns:
             df["flow"] = (
                 df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
             )
             # Remove the plural "s"
             df["flow"] = df["flow"].str.replace("s", "", regex=True)
         return df
 
+    def download_bulk_gz(self, period, frequency):
+        """
+        Method of Pump class to download bulk data from comtradeapicall package, which returns country gz files
+        stored into a temporary directory
+
+        :param (int) period, as year or year+month
+        :param (str) frequency, as "A" yearly or "M" monthly
+        :output (path) temp_dir, directory path which contains the gz files
+        :output (int) response_code, response status of the comtradeapicall
+
+        For example monthly bilateral trade gz files for all products in November
+        2021 can be downloaded into a temporary directory as:
+
+            >>> from biotrade.comtrade import comtrade
+            >>> temp_dir, resp_code = comtrade.pump.download_bulk_gz(202111, "M")
+        """
+
+        # Temporary folder creation
+        temp_dir = Path(tempfile.mkdtemp())
+        self.logger.info(
+            "Downloading %s data for period %s from:\n %s.%s",
+            "yearly" if frequency == "A" else "monthly",
+            period,
+            comtradeapicall.__name__,
+            comtradeapicall.bulkDownloadFinalFile.__name__,
+        )
+        # Variable for checking successful gz download
+        download_successful = False
+        # Default sleep time before downloading gz files
+        sleep_time = 5
+        # Send the request: if successful put the gz files into the temporary
+        # folder else retry and double the wait time at each try
+        # If the wait raises to more than 1 hour the loop stops.
+        while not download_successful and sleep_time < 3600:
+            time.sleep(sleep_time)
+            try:
+                # Create a request
+                comtradeapicall.bulkDownloadFinalFile(
+                    self.token,
+                    temp_dir,
+                    typeCode="C",
+                    freqCode=frequency,
+                    clCode="HS",
+                    period=period,
+                    decompress=False,
+                )
+                response_code = 200
+                download_successful = True
+                # No data available
+                if len(os.listdir(temp_dir)) == 0:
+                    response_code = 404
+            except Exception as error:
+                response_code = error
+            # To avoid system exit exception
+            except BaseException as base_error:
+                response_code = base_error
+            sleep_time *= 2
+            self.logger.info(f"HTTP response code: {response_code}")
+        return temp_dir, response_code
+
     def download_bulk_csv(self, period, frequency):
         """
         Method of Pump class to download bulk data from API
         https://comtrade.un.org/data/doc/api/bulk/ which returns a zip file
         stored into a temporary directory
 
         :param (int) period, as year or year+month
@@ -204,92 +278,120 @@
                     download_successful = True
             except requests.exceptions.RequestException as error:
                 response_code = error
             sleep_time *= 2
             self.logger.info(f"HTTP response code: {response_code}")
         return temp_dir, response_code
 
-    def gz_transfer_db(
+    def transfer_gz_files(
         self,
         temp_dir,
         table_name,
         bioeconomy_tuple,
         check_data_presence,
         api_period,
     ):
         """
-        Pump method to transfer large csv file to db using dataframe.
-        500k data frame rows ~ 500 MB of memory usage
-        2 millions data frame rows ~ 2 GB of memory usage
+        Pump method to transfer gz files to db using dataframe.
+        500k data frame rows ~ 350 MB of memory usage
+        4 millions data frame rows ~ 2.8 GB of memory usage
 
-        :param (path) temp_file, path of the zip file containing the csv file
+        :param (path) temp_dir, path of the folder containing the gz files
             to copy into db
         :param (str) table_name, table name of the db
         :param (tuple) bioeconomy_tuple, commodity codes to store data
         :param (bool) check_data_presence, to delete data in case of existing
             rows into db
         :param (int) api_period, period to delete existing data
-        :param (int) chunk_size, splitting csv to transfer to df default is 10**6
+        :return (int) records_transferred, rows uploaded to db
         """
-        # Number of records transferred from csv file
-        records_downloaded_csv = 0
         # List of chunk rows
         chunk_list = []
-        # Open the zip file
+        # Preallocate a dataframe
+        df = pandas.DataFrame()
+        # Read the gz files
         for temp_file in os.listdir(temp_dir):
-            # Loop on csv files and upload them
-            df = pandas.read_csv(
-                temp_dir / temp_file,
-                sep="\t",
-                dtype={"cmdCode": str},
-            )
+            # Loop on gz files and upload them
+            try:
+                df = pandas.read_csv(
+                    temp_dir / temp_file,
+                    sep="\t",
+                    dtype={"datasetCode": str, "cmdCode": str, "mosCode": str},
+                )
+            # Continue with the next file
+            except Exception as error_gz:
+                self.logger.warning(
+                    f"Unable to load data from {temp_file} for period {api_period} due to\n {error_gz}"
+                )
+                continue
             # If length is > 0 select rows
             if not df.empty:
+                # Remove potential white spaces between tab delimiter in string columns
+                strip_cols = df.select_dtypes(["object"]).columns
+                df[strip_cols] = df[strip_cols].apply(lambda x: x.str.strip())
+                nrow_before = len(df)
+                memory_before = round(
+                    df.memory_usage(deep=True).sum() / (1024**2), 2
+                )
+                selector = (
+                    (df["customsCode"] == "C00")
+                    & (df["motCode"] == 0)
+                    & (df["mosCode"] == "0")
+                    & (df["partner2Code"] == 0)
+                    & (df["flowCode"].isin(["M", "X", "RM", "RX"]))
+                )
                 if table_name in ("monthly", "yearly"):
-                    # Store codes with bioeconomy label and 6 digits, not differentiating modality of transport and procedures
-                    df = df[
-                        (df["cmdCode"].str.startswith(bioeconomy_tuple))
+                    # Store codes with bioeconomy label and 6 digits, not differentiating modality of transport (0), supply ("0"), 2nd partner (0)  and procedures ("C00")
+                    # only (re)exported and (re)imported data
+                    selector_6d = (
+                        selector
+                        & df["cmdCode"].str.startswith(bioeconomy_tuple)
                         & (df["cmdCode"].str.len() == 6)
-                        & (df["customsCode"] == "C00")
-                        & (df["motCode"] == 0)
-                    ]
+                    )
+                    df = df[selector_6d]
                 elif table_name == "yearly_hs2":
-                    # Store codes with bioeconomy label and 2 digits, not differentiating modality of transport and procedures
-                    df = df[
-                        (df["cmdCode"].isin(bioeconomy_tuple))
-                        & (df["customsCode"] == "C00")
-                        & (df["motCode"] == 0)
-                    ]
+                    # Store codes with bioeconomy label and 2 digits, not differentiating modality of transport (0), supply ("0"), 2nd partner (0)  and procedures ("C00")
+                    # only (re)exported and (re)imported data
+                    selector_2d = selector & df["cmdCode"].isin(
+                        bioeconomy_tuple
+                    )
+                    df = df[selector_2d]
+                msg = f"Before filtering {temp_file[:-3]} file, the dataframe occupies {memory_before} MB and number of rows are {nrow_before}, after {round(df.memory_usage(deep=True).sum() / (1024**2), 2)} MB with {len(df)} rows"
+                print(msg)
                 # Append rows
                 chunk_list.append(df)
         # Construct the final df to upload to db
-        df = pandas.concat(chunk_list)
-        self.logger.info(
-            "Memory usage:\n%s GB",
-            round(df.memory_usage(deep=True).sum() / (1024**3), 2),
-        )
+        if chunk_list:
+            df = pandas.concat(chunk_list)
+            self.logger.info(
+                "Memory usage of the filtered dataframe corresponding to period %s:\n%s GB",
+                api_period,
+                round(df.memory_usage(deep=True).sum() / (1024**3), 2),
+            )
         if not df.empty:
-            # TODO add new sanitized columns
             # Call method to rename column names
             df = self.sanitize_variable_names(
-                df, renaming_from="comtrade_human", renaming_to="biotrade"
+                df, renaming_from="comtrade_apicall", renaming_to="biotrade"
             )
-            # TODO uncomment delete and upload of data
-            # # Delete already existing data
-            # if check_data_presence:
-            #     self.db.delete_data(
-            #         table_name,
-            #         api_period,
-            #         api_period,
-            #     )
-            # # Append data to db
-            # self.db.append(df, table_name)
-        # Keep track of the the length of the data in the log file
-        records_downloaded_csv += len(df)
-        return records_downloaded_csv
+            # Delete already existing data
+            if check_data_presence:
+                self.db.delete_data(
+                    table_name,
+                    api_period,
+                    api_period,
+                )
+            # Append data to db
+            self.db.append(df, table_name)
+        else:
+            self.logger.warning(
+                f"Dataframe for period {api_period} is empty. Previous data in the db are not deleted."
+            )
+        # Keep track of the length of the transferred data in the log file
+        records_transferred = len(df)
+        return records_transferred
 
     def transfer_csv_chunk(
         self,
         temp_file,
         table_name,
         bioeconomy_tuple,
         check_data_presence,
@@ -384,48 +486,51 @@
     def transfer_bulk_csv(
         self,
         table_name,
         start_year,
         end_year,
         frequency,
         check_data_presence,
-        use_package=False,
     ):
         """
-        Pump method to transfer bulk csv file of Comtrade API requests to
+        Pump method to transfer bulk files of Comtrade API requests/package to
         Comtrade db.
         Performance with Intel(R) Core(TM) i7-1065G7 CPU @ 1.30GHz:
         ~ 1.5 hours to upload db monthly data for 1 year
         ~ 9 hours to upload db monthly data for 6 years
 
         :param (str) table_name, name of the db table to store data
         :param (int) start_year, year from the download should start
         :param (int) start_year, year from the download should end
         :param (str) frequency, as "A" yearly or "M" monthly
         :param (bool) check_data_presence, if data already exists into db
 
         Example for uploading data from 2016 to 2017 with monthly data into
         "monthly" comtrade table:
 
-        First check if data already exists into db.
+        First check if data already exists into db
+
             >>> from biotrade.comtrade import comtrade
             >>> data_check = comtrade.db.check_data_presence(
-                    table = "monthly"
-                    start_year = 2016,
-                    end_year = 2017,
-                    frequency = "M",
-                )
+            >>>     table = "monthly",
+            >>>     start_year = 2016,
+            >>>     end_year = 2017,
+            >>>     frequency = "M",
+            >>> )
+
         Upload data to db
+
             >>> comtrade.pump.transfer_bulk_csv(
-                    table_name = "monthly",
-                    start_year = 2016,
-                    end_year = 2017,
-                    frequency = "M",
-                    check_data_presence = data_check,
-                )
+            >>>     table_name = "monthly",
+            >>>     start_year = 2016,
+            >>>     end_year = 2017,
+            >>>     frequency = "M",
+            >>>     check_data_presence = data_check,
+            >>> )
+
         """
         # Adjust frequency parameter in case it is wrong provided
         if table_name in ("yearly", "yearly_hs2"):
             frequency = "A"
         elif table_name == "monthly":
             frequency = "M"
         # Period list of downloads failed
@@ -477,98 +582,63 @@
                         datetime.datetime(period, int(month), 1).date()
                         > current_date
                     ):
                         break
                 # Construct the period to pass to transfer_csv_chunk method
                 api_period = int(str(period) + month)
                 # Use the new Comtrade API package
-                if use_package:
-                    temp_dir = Path(tempfile.mkdtemp())
+                # Store gz data into the temporary directory
+                temp_dir, response_code = self.download_bulk_gz(
+                    api_period,
+                    frequency,
+                )
+                # If data are downloaded (response = 200) copy data into a pandas data frame and upload it to the db
+                if response_code == 200:
+                    # Store into the database
                     try:
-                        # TODO add a recursive function for download and remove hard coded parts to the download function
-                        # Save csv files for each reporter in the temp folder
-                        comtradeapicall.bulkDownloadFinalFile(
-                            self.token,
-                            temp_dir,
-                            typeCode="C",
-                            freqCode="M",
-                            clCode="HS",
-                            period="202302",
-                            decompress=False,
-                        )
-                        # Upload data into the database
-                        records_downloaded = self.gz_transfer_db(
+                        # Transfer gz files to db
+                        records_downloaded = self.transfer_gz_files(
                             temp_dir,
                             table_name,
                             bioeconomy_tuple,
                             check_data_presence,
                             api_period,
                         )
-                    except Exception as e:
+                        # Total number of records
+                        total_records += records_downloaded
+                        self.logger.info(
+                            f"Updated database table {table_name} for period"
+                            + f" {api_period}\n"
+                            + f"{total_records} records uploaded in total."
+                        )
+                    # Failed to store data into db
+                    except Exception as error_db:
                         self.logger.warning(
-                            "Failed to upload data from API request for"
-                            + f" period {api_period} due to {e}"
+                            "Failed to store data into the database for table"
+                            + f" {table_name} and period {api_period}\n"
+                            + f"{error_db}"
                         )
                         period_list_failed.append(api_period)
-                # Use the old Comtrade APIs
+                # Data not downloaded from API requests/package
                 else:
-                    # Store zip data into the temporary directory
-                    temp_dir, response_code = self.download_bulk_csv(
-                        api_period,
-                        frequency,
+                    self.logger.warning(
+                        "Failed to download from API request for"
+                        + f" period {api_period} due to HTTP/URL error"
                     )
-                    # If data are downloaded (response = 200) copy the csv of
-                    # the zip file into a pandas data frame
-                    if response_code == 200:
-                        # Temporary zip file path
-                        temp_file = temp_dir / os.listdir(temp_dir)[0]
-                        # Store into the database
-                        try:
-                            # Transfer large csv files into chunks
-                            records_downloaded = self.transfer_csv_chunk(
-                                temp_file,
-                                table_name,
-                                bioeconomy_tuple,
-                                check_data_presence,
-                                api_period,
-                            )
-                            # Total number of records
-                            total_records += records_downloaded
-                            self.logger.info(
-                                f"Update database table {table_name} for period"
-                                + f" {api_period}\n"
-                                + f"{total_records} records uploaded in total."
-                            )
-                        # Failed to store data into db
-                        except Exception as error_db:
-                            self.logger.info(
-                                "Failed to store data into the database for table"
-                                + f" {table_name} and period {api_period}\n"
-                                + f"{error_db}"
-                            )
-                            period_list_failed.append(api_period)
-                    # Data not downloaded from API requests
-                    else:
-                        self.logger.info(
-                            "Failed to dowload from API request for"
-                            + f" period {api_period} due to HTTP/URL error"
-                        )
-                        period_list_failed.append(api_period)
+                    period_list_failed.append(api_period)
                 # Remove temporary directory
                 shutil.rmtree(temp_dir)
         # Log info if some periods failed to be uploaded into db
         if len(period_list_failed):
             self.logger.warning(
                 "List of failed download periods for table"
                 + f" {table_name}: {period_list_failed}"
             )
 
-    def update_db(
-        self, table_name, frequency, start_year=None, use_package=False
-    ):
+    def update_db(self, table_name, frequency, start_year=None):
         """
         Pump method to update db. If data from 2016 are already present,
         it updates data of the last and current year, otherwise it uploads
         data from 2016.
 
         :param (string) table_name, name of Comtrade db table
         :param (string) frequency, "M" for monthly data or "A" for annual
@@ -606,15 +676,14 @@
         # Transfer from api bulk requests to db
         self.transfer_bulk_csv(
             table_name,
             start_year,
             current_year,
             frequency,
             data_present,
-            use_package,
         )
 
     def download_df(
         self,
         max="500",
         type="C",
         freq="A",
@@ -729,25 +798,31 @@
         Usage:
 
             >>> from biotrade.comtrade import comtrade
             >>> comtrade.pump.update_db_parameter()
 
         """
         # Reload the data from Comtrade
-        hs = self.get_parameter_list("classificationHS.json")
+        hs = comtradeapicall.getReference("cmd:HS")
         hs = hs.rename(
-            columns={"id": "product_code", "text": "product_description"}
+            columns={
+                "id": "product_code",
+                "text": "product_description",
+                "isLeaf": "is_leaf",
+                "aggrLevel": "aggregate_level",
+            }
         )
         duplicated = hs.duplicated("product_code")
         if any(duplicated):
             self.logger.info(
                 "Dropping the following duplicated rows:\n %s", hs[duplicated]
             )
             hs = hs[~duplicated]
         # Delete existing data in the database
+        self.logger.info("Dropping existing product table rows.")
         self.db.tables["product"].delete().execute()
         # Store the data in the database
         self.db.append(hs, "product", drop_description=False)
         self.logger.info("The product table has been updated.")
 
     def write_log(
         self,
@@ -855,15 +930,14 @@
             )
         """
         records_downloaded = 0
         reporters = self.parent.country_groups.reporters
         # list of years
         years = [str(i) for i in range(start_year, end_year + 1)]
         for reporter_code in reporters.id:
-
             reporter_name = reporters.text[
                 reporters.id == reporter_code
             ].to_string(index=False)
             # https://comtrade.un.org/data/doc/api
             # "1 request every second (per IP address or authenticated user)."
             time.sleep(2)
```

### Comparing `biotrade-0.1.3/biotrade/comtrade/quality.py` & `biotrade-0.2.1/biotrade/comtrade/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/comtrade_faostat_product_mapping.csv` & `biotrade-0.2.1/biotrade/config_data/comtrade_faostat_product_mapping.csv`

 * *Files 1% similar despite different names*

```diff
@@ -449,18 +449,21 @@
 382319,1276
 400110,836
 400121,837
 400122,837
 400129,837
 400130,839
 410110,928
+410120,928
 410121,920
 410122,920
 410129,920
 410130,919
+410150,920
+410190,920
 410221,998
 411520,1217
 430110,1195
 430130,1002
 430160,1195
 430190,1195
 500100,1185
```

### Comparing `biotrade-0.1.3/biotrade/config_data/comtrade_hs_2d.csv` & `biotrade-0.2.1/biotrade/config_data/comtrade_hs_2d.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/comtrade_hs_product_short_names.csv` & `biotrade-0.2.1/biotrade/config_data/comtrade_hs_product_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/comtrade_reporters.csv` & `biotrade-0.2.1/biotrade/config_data/comtrade_reporters.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_commodity_tree.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_commodity_tree.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_country_groups.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_country_groups.csv`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 35,47,CV,CV,CPV,CPV,132,member,Cabo Verde,the Republic of Cabo Verde,Cabo Verde,Cabo Verde,1975,,World,Africa,5100,Western Africa,5105,Developing,0,
 36,48,KY,KY,CYM,CYM,136,areas and territories,Cayman Islands,Cayman Islands,Cayman Islands,Islas Caimán,1960,,World,Americas,5200,Caribbean,5206,Developing,0,
 37,49,CF,CF,CAF,CAF,140,member,Central African Republic,the Central African Republic,Central African Republic,República Centroafricana,1960,,World,Africa,5100,Middle Africa,5102,Developing,0,
 39,50,TD,TD,TCD,TCD,148,member,Chad,the Republic of Chad,Chad,Chad,1960,,World,Africa,5100,Middle Africa,5102,Developing,0,
 259,,,JG,CHI,CHI,830,areas and territories,Channel Islands,Channel Islands,Channel Islands,Channel Islands,,,,,,,,,0,
 40,51,CL,CL,CHL,CHL,152,member,Chile,the Republic of Chile,Chile,Chile,1945,,World,Americas,5200,South America,5207,Developing,0,
 351,,,,,,,member,China,"China (China mainland, Hong Kong SAR, Macao SAR, Taiwan)",China,China,1945,,World,Asia,5300,Eastern Asia,5302,Developing,0,
-41,53,,,,,1248,areas and territories,"China, mainland",the People's Republic of China,China mainland,China,,,World,Asia,5300,Eastern Asia,5302,Developing,0,
-357,,CN,CN,CHN,CHN,156,areas and territories,China mainland and Taiwan,"China (China mainland, Taiwan)",China mainland and Taiwan,China,,,World,Asia,5300,Eastern Asia,5302,Developing,0,
+41,53,CN,CN,CHN,CHN,156,areas and territories,"China, mainland",the People's Republic of China,China mainland,China,,,World,Asia,5300,Eastern Asia,5302,Developing,0,
+357,,,,,,,areas and territories,China mainland and Taiwan,"China (China mainland, Taiwan)",China mainland and Taiwan,China,,,World,Asia,5300,Eastern Asia,5302,Developing,0,
 96,33364,HK,HK,HKG,HKG,344,areas and territories,"China, Hong Kong SAR","China, Hong Kong Special Administrative Region",Hong Kong,"China, RAE de Hong Kong",,,World,Asia,5300,Eastern Asia,5302,Developing,0,
 128,149,MO,MO,MAC,MAC,446,areas and territories,"China, Macao SAR","China, Macao Special Administrative Region",Macao,"China, RAE de Macao",,,World,Asia,5300,Eastern Asia,5302,Developing,0,
 42,54,CX,CX,CXR,CXR,162,areas and territories,Christmas Island,Christmas Island,Christmas Island,Isla Christmas,,,,,,,,,0,
 ,55,,,,,,areas and territories,Clipperton Island,Clipperton Island,Clipperton Island,Isla de Clipperton,,,,,,,,,0,
 43,56,CC,CC,CCK,CCK,166,areas and territories,Cocos (Keeling) Islands,Cocos (Keeling) Islands,Cocos (Keeling) Islands,Islas Cocos (Keeling),,,,,,,,,0,
 44,57,CO,CO,COL,COL,170,member,Colombia,the Republic of Colombia,Colombia,Colombia,1945,,World,Americas,5200,South America,5207,Developing,0,
 45,58,KM,KM,COM,COM,174,member,Comoros,the Union of the Comoros,Comoros,Comoras,1975,,World,Africa,5100,Eastern Africa,5101,Developing,0,
@@ -122,15 +122,15 @@
 100,115,IN,IN,IND,IND,699,member,India,the Republic of India,India,India,1945,,World,Asia,5300,Southern Asia,5303,Developing,0,
 101,116,ID,ID,IDN,IDN,360,member,Indonesia,the Republic of Indonesia,Indonesia,Indonesia,1950,,World,Asia,5300,South-Eastern Asia,5304,Developing,0,
 102,117,IR,IR,IRN,IRN,364,member,Iran (Islamic Republic of),the Islamic Republic of Iran,Iran (Islamic Republic of),Irán (República Islámica del),1945,,World,Asia,5300,Southern Asia,5303,Developing,0,
 103,118,IQ,IQ,IRQ,IRQ,368,member,Iraq,the Republic of Iraq,Iraq,Iraq,1945,,World,Asia,5300,Western Asia,5305,Developing,0,
 104,119,IE,IE,IRL,IRL,372,member,Ireland,Ireland,Ireland,Irlanda,1955,,World,Europe,5400,Northern Europe,5402,Developed,1,Western Europe
 264,120,IM,IM,IMN,IMY,833,areas and territories,Isle of Man,Isle of Man,Isle of Man,Isla de Man,,,World,Europe,5400,Northern Europe,5402,Developed,0,
 105,121,IL,IL,ISR,ISR,376,member,Israel,the State of Israel,Israel,Israel,1949,,World,Asia,5300,Western Asia,5305,Developing,0,
-106,122,IT,IT,ITA,ITA,381,member,Italy,the Republic of Italy,Italy,Italia,1955,,World,Europe,5400,Southern Europe,5403,Developed,1,Southern Europe
+106,122,IT,IT,ITA,ITA,380,member,Italy,the Republic of Italy,Italy,Italia,1955,,World,Europe,5400,Southern Europe,5403,Developed,1,Southern Europe
 109,123,JM,JM,JAM,JAM,388,member,Jamaica,Jamaica,Jamaica,Jamaica,1962,,World,Americas,5200,Caribbean,5206,Developing,0,
 110,126,JP,JP,JPN,JPN,392,member,Japan,Japan,Japan,Japón,1956,,World,Asia,5300,Eastern Asia,5302,Developed,0,
 ,127,,,,,,areas and territories,Jarvis Island,Jarvis Island,Jarvis Island,Isla Jarvis,,,,,,,,,0,
 283,128,JE,JE,JEY,JEY,832,areas and territories,Jersey,Bailiwick of Jersey,Jersey,Jersey,,,World,Europe,5400,Northern Europe,5402,Developed,0,
 111,129,,,,,,areas and territories,Johnston Island,Johnston Island,Johnston Island,Isla Johnston,,,,,,,,,0,
 112,130,JO,JO,JOR,JOR,400,member,Jordan,the Hashemite Kingdom of Jordan,Jordan,Jordania,1955,,World,Asia,5300,Western Asia,5305,Developing,0,
 108,132,KZ,KZ,KAZ,KAZ,398,member,Kazakhstan,the Republic of Kazakhstan,Kazakhstan,Kasajstán,1992,,World,Asia,5300,Central Asia,5301,Developing,0,
@@ -169,15 +169,15 @@
 142,168,MS,MS,MSR,MSR,500,areas and territories,Montserrat,Montserrat,Montserrat,Montserrat,,,World,Americas,5200,Caribbean,5206,Developing,0,
 143,169,MA,MA,MAR,MAR,504,member,Morocco,the Kingdom of Morocco,Morocco,Marruecos,1956,,World,Africa,5100,Northern Africa,5103,Developing,0,
 144,170,MZ,MZ,MOZ,MOZ,508,member,Mozambique,the Republic of Mozambique,Mozambique,Mozambique,1975,,World,Africa,5100,Eastern Africa,5101,Developing,0,
 28,171,MM,MM,MMR,MMR,104,member,Myanmar,the Republic of the Union of Myanmar,Myanmar,Myanmar,1948,,World,Asia,5300,South-Eastern Asia,5304,Developing,0,
 147,172,NA,NA,NAM,NAM,516,member,Namibia,the Republic of Namibia,Namibia,Namibia,1990,,World,Africa,5100,Southern Africa,5104,Developing,0,
 148,173,NR,NR,NRU,NRU,520,member,Nauru,the Republic of Nauru,Nauru,Nauru,1999,,World,Oceania,5500,Micronesia,5503,Developing,0,
 149,175,NP,NP,NPL,NPL,524,member,Nepal,the Federal Democratic Republic of Nepal,Nepal,Nepal,1955,,World,Asia,5300,Southern Asia,5303,Developing,0,
-150,177,NL,NL,NLD,NLD,528,member,Netherlands,the Kingdom of the Netherlands,Netherlands,Países Bajos,1945,,World,Europe,5400,Western Europe,5404,Developed,1,Western Europe
+150,177,NL,NL,NLD,NLD,528,member,Netherlands (Kingdom of the),the Kingdom of the Netherlands,Netherlands,Países Bajos,1945,,World,Europe,5400,Western Europe,5404,Developed,1,Western Europe
 151,176,AN,AN,ANT,ANT,530,old,Netherlands Antilles (former),Netherlands Antilles,Netherlands Antilles,Netherlands Antilles,1986,2009,World,Americas,5200,Caribbean,5206,Developing,0,
 ,,,,,,532,old,Netherlands Antilles,Netherlands Antilles,Netherlands Antilles,Netherlands Antilles,1945,1985,,,,,,,0,
 152,,,,,,,areas and territories,Neutral Zone,Neutral Zone,Neutral Zone,Zona Neutral,,,,,,,,,0,
 153,178,NC,NC,NCL,NCL,540,areas and territories,New Caledonia,New Caledonia,New Caledonia,Nueva Caledonia,,,World,Oceania,5500,Melanesia,5502,Developing,0,
 156,179,NZ,NZ,NZL,NZL,554,member,New Zealand,New Zealand,New Zealand,Nueva Zelandia,1945,,World,Oceania,5500,Australia and New Zealand,5501,Developed,0,
 157,180,NI,NI,NIC,NIC,558,member,Nicaragua,the Republic of Nicaragua,Nicaragua,Nicaragua,1945,,World,Americas,5200,Central America,5204,Developing,0,
 158,181,NE,NE,NER,NER,562,member,Niger,the Republic of the Niger,Niger,Níger,1960,,World,Africa,5100,Western Africa,5105,Developing,0,
```

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_groups.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_forestry_production_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_short_names.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_forestry_production_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_forestry_trade_groups.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_forestry_trade_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/faostat_products_name_code_shortname.csv` & `biotrade-0.2.1/biotrade/config_data/faostat_products_name_code_shortname.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/regulation_front_end_groups.csv` & `biotrade-0.2.1/biotrade/config_data/regulation_front_end_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/config_data/regulation_products.csv` & `biotrade-0.2.1/biotrade/config_data/regulation_products.csv`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 "0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020220","Meat; of bovine animals, cuts with bone in (excluding carcasses and half-carcasses), frozen","867","Meat of cattle with the bone; fresh or chilled","0","866","866","1","partial"
 "0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020230","Meat; of bovine animals, boneless cuts, frozen","870","Meat of cattle boneless; fresh or chilled","1","867","866","1","partial"
 "020610","Edible offal of cattle, fresh or chilled","Fresh edible offal of cattle","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020610","Offal, edible; of bovine animals, fresh or chilled","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "020622","Edible cattle livers, frozen","Frozen edible cattle livers","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020622","Offal, edible; of bovine animals, livers, frozen","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "020629","Edible cattle offal (excluding tongues and livers), frozen","Frozen edible cattle offal (excluding tongues and livers)","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020629","Offal, edible; of bovine animals, (other than tongues and livers), frozen","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "160250","Other prepared or preserved meat, meat offal, blood of bovine animals","Other prepared meat of bovine animals","Cattle","1602","Prepared or preserved meat, meat offal, blood or insects","160250","Meat preparations; of bovine animals, meat or meat offal, prepared or preserved (excluding livers and homogenised preparations)","875","Beef and veal preparations nes","0","867","866","1","total"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410110","Hides and skins; raw, whole, of bovine animals, weight per skin not exceeding 8kg when simply dried, 10kg when dry-salted or 14kg when fresh, wet-salted or otherwise preserved","928","Skins; wet-salted of calves","0","919","866","1","partial"
-"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410120","Raw hides and skins; whole, unsplit, of bovine or equine animals, of a weight per skin not exceeding 8kg when simply dried, 10kg when dry-salted or 16kg when fresh, wet-salted or otherwise preserved","NA","NA","NA","NA","NA","0","missing"
+"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410120","Raw hides and skins; whole, unsplit, of bovine or equine animals, of a weight per skin not exceeding 8kg when simply dried, 10kg when dry-salted or 16kg when fresh, wet-salted or otherwise preserved","928","Skins; wet-salted of calves","0","919","866","1","partial"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410121","Hides and skins; raw, whole, of bovine animals, fresh or wet-salted, weight per skin exceeding 14kg","920","Hides; wet-salted of cattle","0","919","866","1","partial"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410122","Hides and skins; raw, of bovine animals, fresh or wet-salted, butts and bends","920","Hides; wet-salted of cattle","0","919","866","1","partial"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410129","Hides and skins; raw, of bovine animals, fresh or wet-salted, other than whole, but not butts or bends","920","Hides; wet-salted of cattle","0","919","866","1","partial"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410130","Hides and skins; raw, of bovine animals, preserved in ways n.e.s. in heading no. 4101","919","Raw hides and skins of cattle","0","866","866","1","partial"
-"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410150","Hides and skins; raw, whole, of bovine or equine animals, of a weight per skin exceeding 16 kg","NA","NA","NA","NA","NA","0","missing"
-"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410190","Hides and skins; other than whole, but including butts, bends and bellies, of bovine (including. buffalo) and equine animals, fresh, salted or preserved, but not tanned, parchment dressed or further prepared, whether or not dehaired or split","NA","NA","NA","NA","NA","0","missing"
+"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410150","Hides and skins; raw, whole, of bovine or equine animals, of a weight per skin exceeding 16 kg","920","Hides; wet-salted of cattle","0","919","866","1","partial"
+"4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410190","Hides and skins; other than whole, but including butts, bends and bellies, of bovine (including. buffalo) and equine animals, fresh, salted or preserved, but not tanned, parchment dressed or further prepared, whether or not dehaired or split","920","Hides; wet-salted of cattle","0","919","866","1","partial"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410410","Leather; whole bovine skin, without hair on, of a unit surface area not exceeding 28 square feet (2.6m2), excluding leather of heading no. 4108 and 4109","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410411","Tanned or crust hides and skins; without hair on, bovine or equine, in the wet state (including wet-blue), full grains, unsplit; grain splits","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410419","Tanned or crust hides and skins; bovine or equine, without hair on, in the wet state (including wet-blue), excluding full grains, unsplit; grain splits","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410421","Leather; bovine, without hair on, vegetable pre-tanned, (but not further prepared), whether or not split, excluding leather of heading no. 4108 and 4109","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410422","Leather; bovine, without hair on, pre-tanned, (not vegetable pre-tanned), but not further prepared, whether or not split, excluding leather of heading no. 4108 and 4109","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410429","Leather; bovine and equine n.e.s. in heading no. 4104, without hair on, tanned or retanned but not further prepared, whether or not split, excluding leather of heading no. 4108 and 4109","NA","NA","NA","NA","NA","0","missing"
 "4104","Tanned or crust hides and skins of cattle, without hair on, whether or not split, but not further prepared","Tanned or crust hides and skins of cattle","Cattle","4104","Tanned or crust hides and skins of bovine (including buffalo) or equine animals, without hair on, whether or not split, but not further prepared","410431","Leather; bovine and equine, without hair on, parchment-dressed or prepared after tanning, full grains and grain splits, excluding leather of heading no. 4108 and 4109","NA","NA","NA","NA","NA","0","missing"
```

### Comparing `biotrade-0.1.3/biotrade/config_data/wood_product_aggregates.csv` & `biotrade-0.2.1/biotrade/config_data/wood_product_aggregates.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/eurostat/__init__.py` & `biotrade-0.2.1/biotrade/eurostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/eurostat/pump.py` & `biotrade-0.2.1/biotrade/eurostat/pump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Download data from the Eurostat bulk download facility.
 
+Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was
+taken as an inspiration to load Eurostat data from the bulk download
+repository.
+
 """
 # Standard imports
 import logging
 import re
 
 # Third party libraries
 import numpy as np
```

### Comparing `biotrade-0.1.3/biotrade/faostat/__init__.py` & `biotrade-0.2.1/biotrade/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/aggregate.py` & `biotrade-0.2.1/biotrade/faostat/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/convert.py` & `biotrade-0.2.1/biotrade/faostat/convert.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/country.py` & `biotrade-0.2.1/biotrade/faostat/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/country_groups.py` & `biotrade-0.2.1/biotrade/faostat/country_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,18 @@
         and partner countries.
 
         >>> from biotrade.faostat import faostat
         >>> db = faostat.db
         >>> df_soy = db.select(table="crop_trade", product = "soy")
         >>> df_continents = faostat.country_groups.continents
         >>> df_soy_merge = df_soy.merge(df_continents, how='left',
-                left_on = 'reporter_code', right_on = 'faost_code')
+        >>>     left_on = 'reporter_code', right_on = 'faost_code')
         >>> df_soy_merge = df_soy_merge.merge(df_continents, how='left',
-                left_on = 'partner_code', right_on = 'faost_code',
-                suffixes=('_reporter','_partner'))
+        >>>     left_on = 'partner_code', right_on = 'faost_code',
+        >>>     suffixes=('_reporter','_partner'))
         """
         return self.df[["faost_code", "continent", "sub_continent"]]
 
     def search_name(self, pattern: str) -> pandas.DataFrame:
         """Search for a country name in the country groups table"""
         if isinstance(pattern, str):
             pattern = [pattern]
```

### Comparing `biotrade-0.1.3/biotrade/faostat/database.py` & `biotrade-0.2.1/biotrade/faostat/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/mirror.py` & `biotrade-0.2.1/biotrade/faostat/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Functions to analyse mirror flows.
 """
-import warnings
+import logging
+
+logger = logging.getLogger("biotrade.faostat")
 
 
 def put_mirror_beside(df, drop_index_col=None):
     """Merge mirror flows to obtain a value column and a value_mirror column
     for the corresponding mirror flow.
 
     :param data frame df: bilateral trade flows in faostat compatible format,
@@ -84,10 +86,10 @@
         df_m.drop(columns="element_code", inplace=True)
     # Build the aggregation index based on all columns in df_m
     # Removing the "value" and the drop_index_col columns
     index = df_m.columns.to_list()
     for col in drop_index_col + ["value"]:
         if col in df.columns:
             index.remove(col)
-    warnings.warn(f"\nMerging mirror flows on the following index:\n {index}")
+    logger.info("\nMerging mirror flows on the following index:\n %s", index)
     # Merge with the original data frame
-    return df.merge(df_m, on=index, how="left", suffixes=("", "_mirror"))
+    return df.merge(df_m, on=index, how="outer", suffixes=("", "_mirror"))
```

### Comparing `biotrade-0.1.3/biotrade/faostat/products.py` & `biotrade-0.2.1/biotrade/faostat/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/pump.py` & `biotrade-0.2.1/biotrade/faostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/quality.py` & `biotrade-0.2.1/biotrade/faostat/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/faostat/share_coefficients.py` & `biotrade-0.2.1/biotrade/faostat/share_coefficients.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/hwp/country.py` & `biotrade-0.2.1/biotrade/hwp/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/tests/test_aggregate.py` & `biotrade-0.2.1/biotrade/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/world_bank/__init__.py` & `biotrade-0.2.1/biotrade/world_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/world_bank/database.py` & `biotrade-0.2.1/biotrade/world_bank/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/biotrade/world_bank/pump.py` & `biotrade-0.2.1/biotrade/world_bank/pump.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     >>> world_bank.pump.update(["indicator", "indicator_name"])
 
 """
 from pathlib import Path
 from zipfile import ZipFile
 import tempfile
 import logging
-import requests
+
+try:
+    import requests
+except Exception as e:
+    msg = "Failed to import requests, you will not be able to load data from World Bank,"
+    msg += "but you can still use other methods.\n"
+    print(msg, str(e))
 import shutil
 import pandas as pd
 import csv
 
 # Internal modules
 from biotrade.common.url_request_header import HEADER
 from biotrade.common.sanitize import sanitize_variable_names
```

### Comparing `biotrade-0.1.3/biotrade.egg-info/PKG-INFO` & `biotrade-0.2.1/biotrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.1.3
+Version: 0.2.1
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
@@ -22,14 +22,20 @@
 
 The `biotrade` package analyses international trade of bio-based products. It focuses on
 the agriculture and forestry sectors, from primary production to secondary products
 transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
+# Documentation
+
+The documentation is available at:
+https://bioeconomy.gitlab.io/forobs/biotrade/
+
+
 # Installation
 
 ## Base installation
 
 Install the biotrade package from the python package index with pip:
 
     python -m pip install biotrade
@@ -212,16 +218,14 @@
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
 
 # Similar projects
 
-- The python package [pandas-datareader](https://pydata.github.io/pandas-datareader/)
-
 - The R packages FAOSTAT and WDI
 
 
 # Tests
 
 This package uses pytest for unit testing. Run the test suite with
 
@@ -239,11 +243,9 @@
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
 The authors would like to acknowledge ideas and feedback received from the following
-persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
-
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
-inspiration to load Eurostat data from the bulk download repository.
+persons: Giovanni Bausano, Noemi Cazzaniga, Mirco Migliavacca, Roberto Pilli, Lucas
+Sinclair.
```

### Comparing `biotrade-0.1.3/biotrade.egg-info/SOURCES.txt` & `biotrade-0.2.1/biotrade.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 biotrade.egg-info/top_level.txt
 biotrade/common/aggregate.py
 biotrade/common/compare.py
 biotrade/common/country.py
 biotrade/common/database.py
 biotrade/common/logger.py
 biotrade/common/products.py
+biotrade/common/reallocate.py
 biotrade/common/sanitize.py
 biotrade/common/time_series.py
 biotrade/common/update.py
 biotrade/common/url_request_header.py
 biotrade/comtrade/__init__.py
 biotrade/comtrade/aggregate.py
 biotrade/comtrade/country_groups.py
@@ -54,14 +55,17 @@
 biotrade/faostat/products.py
 biotrade/faostat/pump.py
 biotrade/faostat/quality.py
 biotrade/faostat/share_coefficients.py
 biotrade/hwp/__init__.py
 biotrade/hwp/country.py
 biotrade/tests/test_aggregate.py
+biotrade/tests/test_front_end.py
+biotrade/tests/test_mirror.py
+biotrade/tests/test_reallocate.py
 biotrade/world_bank/__init__.py
 biotrade/world_bank/database.py
 biotrade/world_bank/pump.py
 scripts/front_end/DEPRECATED_reporter_list.py
 scripts/front_end/annual_variation_harvested_area_production.py
 scripts/front_end/annual_variation_trade_quantity_value.py
 scripts/front_end/average_harvested_area_production.py
```

### Comparing `biotrade-0.1.3/scripts/front_end/DEPRECATED_reporter_list.py` & `biotrade-0.2.1/scripts/front_end/DEPRECATED_reporter_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/annual_variation_harvested_area_production.py` & `biotrade-0.2.1/scripts/front_end/annual_variation_harvested_area_production.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 
 """
 
 
 def main():
     from scripts.front_end.functions import (
         main_product_list,
-        consistency_check_china_data,
+        aggregated_data,
         reporter_iso_codes,
         replace_zero_with_nan_values,
         save_file,
     )
     from biotrade.faostat import faostat
     import pandas as pd
 
     # Obtain the main product codes
-    main_product_list = main_product_list(["crop_production", "forestry_production"])
+    main_product_list = main_product_list(
+        ["crop_production", "forestry_production"]
+    )
     # Select quantities from Faostat db for crop data for all countries (code < 1000)
     crop_data = faostat.db.select(
         table="crop_production",
         product_code=main_product_list,
         element=["production", "area_harvested", "stocks"],
     )
     # Select wood production data
@@ -33,32 +35,39 @@
         table="forestry_production",
         product_code=main_product_list,
         element=["production"],
     )
     # Merge data
     crop_data = pd.concat([crop_data, wood_data], ignore_index=True)
     crop_data = crop_data[crop_data["reporter_code"] < 1000]
-    # China Mainland + Taiwan data
-    df_china = consistency_check_china_data(crop_data)
-    # Add China data to crop_data (exclude Taiwan data)
-    crop_data = pd.concat(
-        [crop_data[~(crop_data["reporter_code"] == 214)], df_china],
-        ignore_index=True,
+    # Aggregate french territories values to France and add them to the dataframe
+    code_list = [68, 69, 87, 135, 182, 270, 281]
+    agg_country_code = 68
+    agg_country_name = faostat.country_groups.df
+    agg_country_name = agg_country_name[
+        agg_country_name.faost_code == agg_country_code
+    ].fao_table_name.values[0]
+    crop_data = aggregated_data(
+        crop_data, code_list, agg_country_code, agg_country_name
     )
     # Substitute faostat codes with iso3 codes
     crop_data = reporter_iso_codes(crop_data)
     # Columns to be retained
     column_list = ["reporter_code", "product_code", "period", "value", "unit"]
     # Harvested area data
     dropna_col = ["value"]
     crop_data = replace_zero_with_nan_values(crop_data, dropna_col)
     crop_data = crop_data.dropna(subset=dropna_col)
-    harvested_area = crop_data[crop_data["element"] == "area_harvested"][column_list]
+    harvested_area = crop_data[crop_data["element"] == "area_harvested"][
+        column_list
+    ]
     # Production data
-    production = crop_data[crop_data["element"].isin(["production", "stocks"])][column_list]
+    production = crop_data[crop_data["element"].isin(["production", "stocks"])][
+        column_list
+    ]
     # Save csv files to env variable path or into biotrade data folder
     save_file(harvested_area, "harvested_area_annual_variation.csv")
     save_file(production, "production_annual_variation.csv")
 
 
 # Needed to avoid running module when imported
 if __name__ == "__main__":
```

### Comparing `biotrade-0.1.3/scripts/front_end/annual_variation_trade_quantity_value.py` & `biotrade-0.2.1/scripts/front_end/annual_variation_trade_quantity_value.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/average_harvested_area_production.py` & `biotrade-0.2.1/scripts/front_end/average_harvested_area_production.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 def main():
     # Import internal dependencies
     import pandas as pd
     import numpy as np
     from biotrade.faostat import faostat
     from scripts.front_end.functions import COLUMN_PERC_SUFFIX
     from scripts.front_end.functions import (
-        consistency_check_china_data,
+        aggregated_data,
         main_product_list,
         average_results,
         reporter_iso_codes,
         replace_zero_with_nan_values,
         save_file,
     )
 
     # Obtain the main product codes
-    main_product_list = main_product_list(["crop_production", "forestry_production"])
+    main_product_list = main_product_list(
+        ["crop_production", "forestry_production"]
+    )
     # Query db to obtain data
     crop_df = faostat.db.select(
         table="crop_production",
         product_code=main_product_list,
         element=["production", "area_harvested", "stocks"],
     )
     # Select wood production data
@@ -38,18 +40,22 @@
         product_code=main_product_list,
         element=["production"],
     )
     # Merge data
     df = pd.concat([crop_df, wood_df], ignore_index=True)
     # Select only reporter with code lower than 1000
     df = df[df["reporter_code"] < 1000].reset_index(drop=True)
-    # China Mainland + Taiwan data
-    df_china = consistency_check_china_data(df)
-    # Add China data to df (exclude Taiwan data)
-    df = pd.concat([df[~(df["reporter_code"] == 214)], df_china], ignore_index=True)
+    # Aggregate french territories values to France and add them to the dataframe
+    code_list = [68, 69, 87, 135, 182, 270, 281]
+    agg_country_code = 68
+    agg_country_name = faostat.country_groups.df
+    agg_country_name = agg_country_name[
+        agg_country_name.faost_code == agg_country_code
+    ].fao_table_name.values[0]
+    df = aggregated_data(df, code_list, agg_country_code, agg_country_name)
     # Substitute faostat codes with iso3 codes
     df = reporter_iso_codes(df)
     # Define the columns and codes for the average calculations
     dict_list = [
         {
             "average_col": "reporter_code",
             "percentage_col": "product_code",
@@ -78,20 +84,26 @@
         intervals,
     )
     # Columns to keep
     drop_column = "element"
     column_list = df_final.columns.tolist()
     column_list.remove(drop_column)
     # Define dropna columns
-    dropna_col = [col for col in df_final.columns if col.endswith(COLUMN_PERC_SUFFIX)]
+    dropna_col = [
+        col for col in df_final.columns if col.endswith(COLUMN_PERC_SUFFIX)
+    ]
     df_final = replace_zero_with_nan_values(df_final, dropna_col)
     df_final = df_final.dropna(subset=dropna_col, how="all")
     # Save csv files to env variable path or into biotrade data folder
-    harvested_area = df_final[df_final["element"] == "area_harvested"][column_list]
+    harvested_area = df_final[df_final["element"] == "area_harvested"][
+        column_list
+    ]
     save_file(harvested_area, "harvested_area_average.csv")
-    production = df_final[df_final["element"].isin(["production", "stocks"])][column_list]
+    production = df_final[df_final["element"].isin(["production", "stocks"])][
+        column_list
+    ]
     save_file(production, "production_average.csv")
 
 
 # Needed to avoid running module when imported
 if __name__ == "__main__":
     main()
```

### Comparing `biotrade-0.1.3/scripts/front_end/average_trade_quantity.py` & `biotrade-0.2.1/scripts/front_end/average_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/db_scheduler.py` & `biotrade-0.2.1/scripts/front_end/db_scheduler.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/functions.py` & `biotrade-0.2.1/scripts/front_end/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,37 +143,30 @@
 
     """
     # Reporter codes
     reporter_file = faostat.config_data_dir / "faostat_country_groups.csv"
     reporter = pd.read_csv(reporter_file)
     # Obtain iso3 codes for reporters and partners
     df = df.merge(
-        reporter[["faost_code", "iso3_code", "fao_status_info"]],
+        reporter[["faost_code", "iso3_code"]],
         how="left",
         left_on="reporter_code",
         right_on="faost_code",
     )
     df["reporter_code"] = df["iso3_code"]
-    # Remove data of old reporters
-    df = df[df.fao_status_info != "old"]
-    subset_col = ["reporter_code"]
     if "partner_code" in df.columns:
-        df.drop(columns=["faost_code", "iso3_code", "fao_status_info"], inplace=True)
+        df.drop(columns=["faost_code", "iso3_code"], inplace=True)
         df = df.merge(
-            reporter[["faost_code", "iso3_code", "fao_status_info"]],
+            reporter[["faost_code", "iso3_code"]],
             how="left",
             left_on=["partner_code"],
             right_on=["faost_code"],
         )
         df["partner_code"] = df["iso3_code"]
-        # Remove data of old partners
-        df = df[df.fao_status_info != "old"]
-        subset_col.append("partner_code")
-    # Faostat code 41 (China mainland) and 351 (China mainland + Hong Kong + Macao + Taiwan ) are not mapped into ISO 3 Codes
-    df.dropna(subset=subset_col, inplace=True)
+    df.drop(columns=["faost_code", "iso3_code"], inplace=True)
     # Consider only data of official country codes by GISCO
     if os.environ.get("FRONT_END_SCRIPTS"):
         path = Path(os.environ["FRONT_END_SCRIPTS"])
     else:
         path = Path(os.getenv("PYTHONPATH")) / "scripts" / "front_end"
     country_codes = (
         pd.read_csv(
@@ -182,14 +175,18 @@
         )
         .ISO3_CODE.drop_duplicates()
         .to_list()
     )
     df = df[df.reporter_code.isin(country_codes)].reset_index(drop=True)
     if "partner_code" in df.columns:
         df = df[df.partner_code.isin(country_codes)].reset_index(drop=True)
+        # Remove free zones internal trade data
+        df = df[df["reporter_code"] != df["partner_code"]].reset_index(
+            drop=True
+        )
     return df
 
 
 def merge_faostat_comtrade_data(
     faostat_code=None,
     comtrade_regulation=None,
     aggregate=True,
@@ -306,19 +303,23 @@
         {
             "year": [most_recent_year, *years],
             "period_aggregation": [0, *periods],
         }
     )
     # Define the min year inside each period
     df_periods_min = (
-        df_periods.groupby(["period_aggregation"]).agg({"year": "min"}).reset_index()
+        df_periods.groupby(["period_aggregation"])
+        .agg({"year": "min"})
+        .reset_index()
     )
     # Define the max year inside each period
     df_periods_max = (
-        df_periods.groupby(["period_aggregation"]).agg({"year": "max"}).reset_index()
+        df_periods.groupby(["period_aggregation"])
+        .agg({"year": "max"})
+        .reset_index()
     )
     # Merge on the periods
     df_periods = df_periods.merge(
         df_periods_min,
         how="left",
         on="period_aggregation",
         suffixes=("", "_min"),
@@ -327,18 +328,22 @@
         df_periods_max,
         how="left",
         on="period_aggregation",
         suffixes=("", "_max"),
     )
     # Define the structure yyyy-yyyy for the period aggregation column
     df_periods["period_aggregation"] = (
-        df_periods["year_min"].astype(str) + "-" + df_periods["year_max"].astype(str)
+        df_periods["year_min"].astype(str)
+        + "-"
+        + df_periods["year_max"].astype(str)
     )
     # Assign the associated period to each data
-    df = df.merge(df_periods[["year", "period_aggregation"]], on="year", how="left")
+    df = df.merge(
+        df_periods[["year", "period_aggregation"]], on="year", how="left"
+    )
     df["period"] = df["period_aggregation"]
     # Default index list for aggregations + the adds from the arguments
     index_list = ["element", "period", "unit"]
     df_final = pd.DataFrame()
     column_drop = []
     # Load for each dict the aggregation column, the percentage column and the code for threshold values in order to compute calculations
     for dict in dict_list:
@@ -378,27 +383,31 @@
         )
         if value_col_name not in column_drop:
             column_drop.append(value_col_name)
         # Merge with mean and total values
         df_new = df_new.merge(df_mean, how="left", on=index_list_upd)
         df_new = df_new.merge(df_total, how="left", on=index_list_upd)
         # Percentage associated to the percentage column on a given aggregated period
-        df_new[percentage_col_name] = df_new["value"] / df_new[total_col_name] * 100
+        df_new[percentage_col_name] = (
+            df_new["value"] / df_new[total_col_name] * 100
+        )
         # Sort by percentage, compute the cumulative sum and shift it by one
         df_new.sort_values(
             by=[*index_list_upd, percentage_col_name],
             ascending=False,
             inplace=True,
             ignore_index=True,
         )
         # Skip nan values is True for cumsum by default
-        df_new["cumsum"] = df_new.groupby(index_list_upd)[percentage_col_name].cumsum()
-        df_new["cumsum_lag"] = df_new.groupby(index_list_upd)["cumsum"].transform(
-            "shift", fill_value=0
-        )
+        df_new["cumsum"] = df_new.groupby(index_list_upd)[
+            percentage_col_name
+        ].cumsum()
+        df_new["cumsum_lag"] = df_new.groupby(index_list_upd)[
+            "cumsum"
+        ].transform("shift", fill_value=0)
         # Create a grouping variable instead of the percentage column, which will be 'Others' for
         # values above the threshold
         df_new[dict["percentage_col"]] = df_new[dict["percentage_col"]].where(
             df_new["cumsum_lag"] < threshold, other_code
         )
         # Group the percentage column values which are in the 'Others' category and calculate their percentage
         df_new = (
@@ -408,15 +417,17 @@
                     "value": "sum",
                     average_col_name: "first",
                     total_col_name: "first",
                 }
             )
             .reset_index()
         )
-        df_new[percentage_col_name] = df_new["value"] / df_new[total_col_name] * 100
+        df_new[percentage_col_name] = (
+            df_new["value"] / df_new[total_col_name] * 100
+        )
         if df_final.empty:
             df_final = df_new
         else:
             # Merge or concatenate depending on the common columns in merge_col_list
             merge_col_list = [*index_list_upd, dict["percentage_col"]]
             if average_col_name in df_final.columns:
                 merge_col_list.append(average_col_name)
@@ -492,17 +503,23 @@
                     bins=bins,
                     labels=list(range(0, len(interval_array) - 1)),
                 )
                 df_key["interval_range"] = pd.cut(
                     df_key["avg_value"],
                     bins=bins,
                 )
-                key_legend["interval"] = df_key["interval"].cat.categories.values
-                key_legend["min_value"] = df_key["interval_range"].cat.categories.left
-                key_legend["max_value"] = df_key["interval_range"].cat.categories.right
+                key_legend["interval"] = df_key[
+                    "interval"
+                ].cat.categories.values
+                key_legend["min_value"] = df_key[
+                    "interval_range"
+                ].cat.categories.left
+                key_legend["max_value"] = df_key[
+                    "interval_range"
+                ].cat.categories.right
                 key_legend["product_code"] = key[0]
                 key_legend["element"] = key[1]
                 key_legend["unit"] = key[2]
             # Inconsistencies could be detected with the warning
             else:
                 faostat.db.logger.warning(
                     f"The dataset represented by {groupby_max_cols} = {key} tuple has not been included into the final csv file due to inconsistencies, please check the data."
@@ -518,45 +535,56 @@
                 ignore_index=True,
             )
         # Columns to keep in the legend dataframe
         drop_column = "element"
         column_list = df_legend.columns.tolist()
         column_list.remove(drop_column)
         # Save interval legends
-        harvested_area_legend = df_legend[df_legend["element"] == "area_harvested"][
-            column_list
-        ]
+        harvested_area_legend = df_legend[
+            df_legend["element"] == "area_harvested"
+        ][column_list]
         save_file(harvested_area_legend, "harvested_area_average_legend.csv")
         production_legend = df_legend[
             df_legend["element"].isin(["production", "stocks"])
         ][column_list]
         save_file(production_legend, "production_average_legend.csv")
     # Associate the avg productions (eventually with intervals) to the final dataframe
     df_final = df_final.merge(df_avg, on=groupby_avg_cols, how="left")
     return df_final
 
 
-def consistency_check_china_data(df):
+def aggregated_data(df, code_list, agg_country_code, agg_country_name):
     """
-    Script that aggregate China Mainland + Tawain data in order to overcome inconsistencies
+    Script that aggregates country data in order to overcome inconsistencies
 
-    :param df (DataFrame), which contains China data
-    :return df_china (DataFrame), with aggregate data for China Mainland + Taiwan
+    :param df (DataFrame), which contains production or trade data
+    :param code_list (list), country codes to be aggregated
+    :param agg_country_code (int), country code to be assigned for the aggregation
+    :param agg_country_name (string), country name to be assigned for the aggregation
+    :return df (DataFrame), with aggregated data
 
     """
     # Trade data
     if "partner_code" in df.columns:
-        # Define China data with isocode CHN and Faostat code 357 from China mainland (41) + Taiwan (214) data both from reporter and partner
-        df_china = df[df[["reporter_code", "partner_code"]].isin([41, 214]).any(axis=1)]
+        # Define aggregated data both for reporter and parnter
+        df_agg = df[
+            df[["reporter_code", "partner_code"]].isin(code_list).any(axis=1)
+        ]
         # Avoid counting internal trades
-        mask = (df_china.reporter_code.isin([41, 214])) & (df_china.partner_code.isin([41, 214]))
-        df_china = df_china[~mask]
+        mask = (df_agg.reporter_code.isin(code_list)) & (
+            df_agg.partner_code.isin(code_list)
+        )
+        df_agg = df_agg[~mask]
+        # Remove country code list data from df dataset
+        df = df[
+            ~(df[["reporter_code", "partner_code"]].isin(code_list)).any(axis=1)
+        ]
         # Aggregation on the reporter side
-        df_china_1 = (
-            df_china[df_china["reporter_code"].isin([41, 214])]
+        df_agg_1 = (
+            df_agg[df_agg["reporter_code"].isin(code_list)]
             .groupby(
                 [
                     "source",
                     "partner_code",
                     "partner",
                     "product_code",
                     "product",
@@ -566,24 +594,24 @@
                     "unit",
                 ]
             )
             # If all null values, do not return 0 but Nan
             .agg({"value": lambda x: x.sum(min_count=1)})
             .reset_index()
         )
-        df_china_1["reporter_code"] = 357
-        df_china_1["reporter"] = "China mainland and Taiwan"
-        # Concat with reporter codes not 41 either 214
-        df_china_1 = pd.concat(
-            [df_china[~df_china["reporter_code"].isin([41, 214])], df_china_1],
+        df_agg_1["reporter_code"] = agg_country_code
+        df_agg_1["reporter"] = agg_country_name
+        # Concat with reporter codes not in country code list
+        df_agg_1 = pd.concat(
+            [df_agg[~df_agg["reporter_code"].isin(code_list)], df_agg_1],
             ignore_index=True,
         )
         # Aggregation also on the partner side
-        df_china_2 = (
-            df_china_1[df_china_1["partner_code"].isin([41, 214])]
+        df_agg_2 = (
+            df_agg_1[df_agg_1["partner_code"].isin(code_list)]
             .groupby(
                 [
                     "source",
                     "reporter_code",
                     "reporter",
                     "product_code",
                     "product",
@@ -593,48 +621,55 @@
                     "unit",
                 ]
             )
             # If all null values, do not return 0 but Nan
             .agg({"value": lambda x: x.sum(min_count=1)})
             .reset_index()
         )
-        df_china_2["partner_code"] = 357
-        df_china_2["partner"] = "China mainland and Taiwan"
-        # Concat with partner codes not 41 and 214
-        df_china_2 = pd.concat(
+        df_agg_2["partner_code"] = agg_country_code
+        df_agg_2["partner"] = agg_country_name
+        # Concat with partner codes not in country code list
+        df_agg_2 = pd.concat(
             [
-                df_china_1[~df_china_1["partner_code"].isin([41, 214])],
-                df_china_2,
+                df_agg_1[~df_agg_1["partner_code"].isin(code_list)],
+                df_agg_2,
             ],
             ignore_index=True,
         )
-        df_china = df_china_2
+        df_agg = df_agg_2
     # Production data
     else:
-        # Produce China data with isocode CHN and Faostat code 357 from China mainland (41) + Taiwan (214) data
-        df_china = df[df["reporter_code"].isin([41, 214])]
-        df_china = (
-            df_china.groupby(
+        # Produce reporter aggregated data
+        df_agg = df[df["reporter_code"].isin(code_list)]
+        # Remove country code list data from df dataset
+        df = df[~(df["reporter_code"].isin(code_list))]
+        df_agg = (
+            df_agg.groupby(
                 [
                     "product_code",
                     "product",
                     "element_code",
                     "element",
                     "year",
                     "unit",
                 ]
             )
             # If all null values, do not return 0 but Nan
             .agg({"value": lambda x: x.sum(min_count=1)}).reset_index()
         )
-        df_china["reporter_code"] = 357
-        df_china["reporter"] = "China mainland and Taiwan"
+        df_agg["reporter_code"] = agg_country_code
+        df_agg["reporter"] = agg_country_name
     # Fill period column
-    df_china["period"] = df_china["year"]
-    return df_china
+    df_agg["period"] = df_agg["year"]
+    # Build the final dataset to return
+    df = pd.concat(
+        [df, df_agg],
+        ignore_index=True,
+    )
+    return df
 
 
 def trend_analysis(
     df_data, multi_process=False, groupby_column_list=[], value_column=None
 ):
     """
     Script which performs the trend analysis
```

### Comparing `biotrade-0.1.3/scripts/front_end/product_list.py` & `biotrade-0.2.1/scripts/front_end/product_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/trends_harvested_area_production.py` & `biotrade-0.2.1/scripts/front_end/trends_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/front_end/trends_trade_quantity.py` & `biotrade-0.2.1/scripts/front_end/trends_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/scripts/quality/faostat_compare_aggregates_to_constituents.py` & `biotrade-0.2.1/scripts/quality/faostat_compare_aggregates_to_constituents.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.3/setup.py` & `biotrade-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,34 +17,38 @@
 readme_path = path.join(this_dir, "README.md")
 with open(readme_path, encoding="utf-8") as handle:
     readme = handle.read()
 
 # Call setup #
 setup(
     name="biotrade",
-    version="0.1.3",
+    version="0.2.1",
     description="Agriculture and forestry statistics.",
     license="MIT",
     url="https://gitlab.com/bioeconomy/forobs/biotrade/",
     author="Paul Rougieux, Selene Patani",
     author_email="paul.rougieux@gmail.com",
     packages=find_namespace_packages(exclude=["notebooks", "scripts"]),
     install_requires=[
         "pandas",
         "sqlalchemy",
         "sqlalchemy_utils",
         "psycopg2",
         "requests",
+        "scipy",
+        "pymannkendall",
+        "matplotlib",
+        "comtradeapicall",
     ],
     extras_require={"api": ["fastapi", "uvicorn"]},
     python_requires=">=3.7",
     long_description=readme,
     long_description_content_type="text/markdown",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering",
```

