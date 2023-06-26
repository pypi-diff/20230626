# Comparing `tmp/liiatools-0.1.5.2.tar.gz` & `tmp/liiatools-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liiatools-0.1.5.2.tar", max compression
+gzip compressed data, was "liiatools-0.1.5.3.tar", max compression
```

## Comparing `liiatools-0.1.5.2.tar` & `liiatools-0.1.5.3.tar`

### file list

```diff
@@ -1,143 +1,141 @@
--rw-r--r--   0        0        0     1084 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/__init__.py
--rw-r--r--   0        0        0      434 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/__main__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/__init__.py
--rw-r--r--   0        0        0     4364 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/filters.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/__init__.py
--rw-r--r--   0        0        0      280 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/stream.py
--rw-r--r--   0        0        0     1640 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/xml.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/__init__.py
--rw-r--r--   0        0        0      131 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/README.md
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/annex_a_cli.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
--rw-r--r--   0        0        0     4908 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
--rw-r--r--   0        0        0    11751 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
--rw-r--r--   0        0        0      451 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
--rw-r--r--   0        0        0     1381 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
--rw-r--r--   0        0        0     5122 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
--rw-r--r--   0        0        0    12608 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
--rw-r--r--   0        0        0      772 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
--rw-r--r--   0        0        0      885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
--rw-r--r--   0        0        0     3052 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
--rw-r--r--   0        0        0     2894 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
--rw-r--r--   0        0        0     2066 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/__init__.py
--rw-r--r--   0        0        0    12206 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/cin_cli.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
--rw-r--r--   0        0        0     6065 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
--rw-r--r--   0        0        0     2644 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
--rw-r--r--   0        0        0      811 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/converter.py
--rw-r--r--   0        0        0     2757 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
--rw-r--r--   0        0        0     6012 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/logger.py
--rw-r--r--   0        0        0      405 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/schema.py
--rw-r--r--   0        0        0     3860 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/validator.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
--rw-r--r--   0        0        0     2487 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
--rw-r--r--   0        0        0    10532 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
--rw-r--r--   0        0        0    10132 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/columns.py
--rw-r--r--   0        0        0     5126 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
--rw-r--r--   0        0        0     1612 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/converters.py
--rw-r--r--   0        0        0     1248 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
--rw-r--r--   0        0        0     2993 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
--rw-r--r--   0        0        0     3184 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/filters.py
--rw-r--r--   0        0        0     8547 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/logger.py
--rw-r--r--   0        0        0     1189 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/parse.py
--rw-r--r--   0        0        0     1749 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/populate.py
--rw-r--r--   0        0        0     5080 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/prep.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
--rw-r--r--   0        0        0     2425 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
--rw-r--r--   0        0        0     1482 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
--rw-r--r--   0        0        0     2491 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
--rw-r--r--   0        0        0     1078 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
--rw-r--r--   0        0        0     4704 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/s903_cli.py
--rw-r--r--   0        0        0     7475 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/s903_main_functions.py
--rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/__init__.py
--rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/lds_school_clean/__init__.py
--rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
--rw-r--r--   0        0        0     8213 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/shared_functions/common.py
--rw-r--r--   0        0        0     1827 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/shared_functions/converters.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/__init__.py
--rw-r--r--   0        0        0      778 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py
--rw-r--r--   0        0        0      778 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py
--rw-r--r--   0        0        0      851 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py
--rw-r--r--   0        0        0      745 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py
--rw-r--r--   0        0        0     2508 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py
--rw-r--r--   0        0        0     2842 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py
--rw-r--r--   0        0        0     3204 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/__init__.py
--rw-r--r--   0        0        0     5395 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py
--rw-r--r--   0        0        0     7134 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/__init__.py
--rw-r--r--   0        0        0      980 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py
--rw-r--r--   0        0        0     7796 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py
--rw-r--r--   0        0        0       24 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/env
--rw-r--r--   0        0        0     1628 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/main.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/spec/__init__.py
--rw-r--r--   0        0        0    23265 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd
--rw-r--r--   0        0        0     4771 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/__init__.py
--rw-r--r--   0        0        0     2268 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/__init__.py
--rw-r--r--   0        0        0      829 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_cli.py
--rw-r--r--   0        0        0      839 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_main_functions.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_clean/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_la_agg/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_pan_agg/__init__.py
--rw-r--r--   0        0        0     9774 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/sample_data.py
--rw-r--r--   0        0        0      470 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/schema.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/__init__.py
--rw-r--r--   0        0        0    11870 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/annex-a-merge.yml
--rw-r--r--   0        0        0    45318 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/data-map.yml
--rw-r--r--   0        0        0    10542 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/la-agg.yml
--rw-r--r--   0        0        0     1757 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/pan-agg.yml
--rw-r--r--   0        0        0    27319 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/annex_a/samples/Annex_A.xlsx
--rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2017.xsd
--rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2018.xsd
--rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2019.xsd
--rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2020.xsd
--rw-r--r--   0        0        0    31267 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2021.xsd
--rw-r--r--   0        0        0    31909 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2022.xsd
--rw-r--r--   0        0        0    32229 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2023.xsd
--rw-r--r--   0        0        0    32229 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2024.xsd
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/__init__.py
--rw-r--r--   0        0        0      711 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/agg.yml
--rw-r--r--   0        0        0     3423 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/samples/cin-2022.xml
--rw-r--r--   0        0        0      739 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/common/LA-codes.yml
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/common/__init__.py
--rw-r--r--   0        0        0    11211 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2017.yml
--rw-r--r--   0        0        0    11211 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2018.yml
--rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2019.yml
--rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2020.yml
--rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2021.yml
--rw-r--r--   0        0        0    11322 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2022.yml
--rw-r--r--   0        0        0    11322 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2023.yml
--rw-r--r--   0        0        0    11977 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2024.yml
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/__init__.py
--rw-r--r--   0        0        0     3339 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/la-agg.yml
--rw-r--r--   0        0        0     1792 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/pan-agg.yml
--rw-r--r--   0        0        0      459 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
--rw-r--r--   0        0        0     1585 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/sufficiency.yml
--rw-r--r--   0        0        0        1 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/school_census/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/__init__.py
--rw-r--r--   0        0        0     3716 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml
--rw-r--r--   0        0        0    17431 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
--rw-r--r--   0        0        0     1049 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 liiatools-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/datasets/cincensus/__init__.py
+-rw-r--r--   0        0        0     4364 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/datasets/cincensus/filters.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/util/__init__.py
+-rw-r--r--   0        0        0      280 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/util/stream.py
+-rw-r--r--   0        0        0     1640 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/csdatatools/util/xml.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/__init__.py
+-rw-r--r--   0        0        0      131 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/__init__.py
+-rw-r--r--   0        0        0     7047 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/annex_a_cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
+-rw-r--r--   0        0        0     4908 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
+-rw-r--r--   0        0        0    11751 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
+-rw-r--r--   0        0        0      451 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
+-rw-r--r--   0        0        0     1381 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
+-rw-r--r--   0        0        0     5122 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
+-rw-r--r--   0        0        0    12608 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
+-rw-r--r--   0        0        0      772 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
+-rw-r--r--   0        0        0      885 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
+-rw-r--r--   0        0        0     2495 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
+-rw-r--r--   0        0        0     3052 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2894 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
+-rw-r--r--   0        0        0     2066 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/__init__.py
+-rw-r--r--   0        0        0    12206 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/cin_cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
+-rw-r--r--   0        0        0     6065 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
+-rw-r--r--   0        0        0     2644 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
+-rw-r--r--   0        0        0      811 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/converter.py
+-rw-r--r--   0        0        0     2757 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
+-rw-r--r--   0        0        0     6012 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/logger.py
+-rw-r--r--   0        0        0      405 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/schema.py
+-rw-r--r--   0        0        0     3860 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/validator.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
+-rw-r--r--   0        0        0     2487 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
+-rw-r--r--   0        0        0    10532 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
+-rw-r--r--   0        0        0    10132 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/columns.py
+-rw-r--r--   0        0        0     5126 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
+-rw-r--r--   0        0        0     1612 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/converters.py
+-rw-r--r--   0        0        0     1248 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
+-rw-r--r--   0        0        0     3025 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
+-rw-r--r--   0        0        0     3184 2023-06-26 07:59:48.205162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/filters.py
+-rw-r--r--   0        0        0     8547 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/logger.py
+-rw-r--r--   0        0        0     1189 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/parse.py
+-rw-r--r--   0        0        0     1750 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/populate.py
+-rw-r--r--   0        0        0     5080 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/prep.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
+-rw-r--r--   0        0        0     2486 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
+-rw-r--r--   0        0        0     3029 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
+-rw-r--r--   0        0        0     1482 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
+-rw-r--r--   0        0        0     2491 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
+-rw-r--r--   0        0        0     1078 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
+-rw-r--r--   0        0        0     4705 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/s903_cli.py
+-rw-r--r--   0        0        0     7633 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/s903/s903_main_functions.py
+-rw-r--r--   0        0        0        1 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/school_census/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/school_census/lds_school_clean/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
+-rw-r--r--   0        0        0     8213 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/shared_functions/common.py
+-rw-r--r--   0        0        0     1827 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/shared_functions/converters.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/__init__.py
+-rw-r--r--   0        0        0     1455 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/__init__.py
+-rw-r--r--   0        0        0     2336 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py
+-rw-r--r--   0        0        0      898 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py
+-rw-r--r--   0        0        0     7922 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/__init__.py
+-rw-r--r--   0        0        0     5644 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py
+-rw-r--r--   0        0        0     7672 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/__init__.py
+-rw-r--r--   0        0        0      975 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py
+-rw-r--r--   0        0        0     8656 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py
+-rw-r--r--   0        0        0       24 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/env
+-rw-r--r--   0        0        0     1764 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/main.py
+-rw-r--r--   0        0        0     5138 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/util/__init__.py
+-rw-r--r--   0        0        0     2479 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0      829 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/csww_cli.py
+-rw-r--r--   0        0        0      839 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/csww_main_functions.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/lds_csww_clean/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/lds_csww_la_agg/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/lds_csww_pan_agg/__init__.py
+-rw-r--r--   0        0        0     9774 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/sample_data.py
+-rw-r--r--   0        0        0      470 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/schema.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/__init__.py
+-rw-r--r--   0        0        0    11870 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/annex-a-merge.yml
+-rw-r--r--   0        0        0    45318 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/data-map.yml
+-rw-r--r--   0        0        0    10542 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/la-agg.yml
+-rw-r--r--   0        0        0     1757 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/pan-agg.yml
+-rw-r--r--   0        0        0    27319 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/annex_a/samples/Annex_A.xlsx
+-rw-r--r--   0        0        0    30559 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2017.xsd
+-rw-r--r--   0        0        0    30559 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2018.xsd
+-rw-r--r--   0        0        0    30559 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2019.xsd
+-rw-r--r--   0        0        0    30559 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2020.xsd
+-rw-r--r--   0        0        0    31267 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2021.xsd
+-rw-r--r--   0        0        0    31909 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2022.xsd
+-rw-r--r--   0        0        0    32229 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2023.xsd
+-rw-r--r--   0        0        0    32229 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2024.xsd
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/agg.yml
+-rw-r--r--   0        0        0     3423 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/cin_census/samples/cin-2022.xml
+-rw-r--r--   0        0        0      739 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/common/LA-codes.yml
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/common/__init__.py
+-rw-r--r--   0        0        0    11211 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2017.yml
+-rw-r--r--   0        0        0    11211 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2018.yml
+-rw-r--r--   0        0        0    11280 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2019.yml
+-rw-r--r--   0        0        0    11280 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2020.yml
+-rw-r--r--   0        0        0    11280 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2021.yml
+-rw-r--r--   0        0        0    11322 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2022.yml
+-rw-r--r--   0        0        0    11322 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2023.yml
+-rw-r--r--   0        0        0    11977 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2024.yml
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/__init__.py
+-rw-r--r--   0        0        0     3339 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/la-agg.yml
+-rw-r--r--   0        0        0     1792 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/pan-agg.yml
+-rw-r--r--   0        0        0      459 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
+-rw-r--r--   0        0        0     1585 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/s903/sufficiency.yml
+-rw-r--r--   0        0        0        1 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/school_census/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.209162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0    18158 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/samples/csww/BAD/social_work_workforce_2022.xml
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/samples/flatfiles/BAD/la_log/blank.txt
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/samples/log_files/blank.txt
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/samples/outputs/blank.txt
+-rw-r--r--   0        0        0        0 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/samples/request/blank.txt
+-rw-r--r--   0        0        0    17431 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
+-rw-r--r--   0        0        0     1074 2023-06-26 07:59:48.213162 liiatools-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 liiatools-0.1.5.3/PKG-INFO
```

### Comparing `liiatools-0.1.5.2/LICENSE` & `liiatools-0.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/filters.py` & `liiatools-0.1.5.3/liiatools/csdatatools/datasets/cincensus/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/csdatatools/util/xml.py` & `liiatools-0.1.5.3/liiatools/csdatatools/util/xml.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/annex_a_cli.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/annex_a_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/logger.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/populate.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/populate.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/regex.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_clean/regex.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/cin_cli.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/cin_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/converter.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/converter.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/logger.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/validator.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_clean/validator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/columns.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/columns.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/converters.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/degrade.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         elif isinstance(event, events.EndTable):
             yield event
             yield TableEvent.from_event(event, data=data)
             data = None
         elif data is not None and isinstance(event, RowEvent):
             try:
                 data.append(event.row + [la_name, event.year])
-            except AttributeError:  # raised in case event.year is missing so data is not added
+            except (
+                AttributeError
+            ):  # raised in case event.year is missing so data is not added
                 pass
         yield event
 
 
 def save_tables(stream, output):
     """
     Save the data events as csv files in the Outputs directory
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/filters.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/logger.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/parse.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/parse.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/populate.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/populate.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             yield event
             year = None
         elif isinstance(event, events.EndRow) and year is not None:
             yield event.from_event(event, year=year)
         else:
             yield event
 
+
 @streamfilter(check=lambda x: x.get("header") in ["CHILD"], fail_function=pass_event)
 def create_la_child_id(event, la_code):
     """
     Creates an identifier from a combination of the Child Unique ID and Local Authority so matching child IDs
     are not removed in the merging a de-duping steps
 
     :param event: A filtered list of event objects
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/prep.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_clean/prep.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,69 +19,35 @@
     Matches the columns in the DataFrame against one of the 10 SSDA903 file types
     """
     for table_name, expected_columns in column_names.items():
         if set(s903_df.columns) == set(expected_columns):
             return table_name
 
 
-def merge_la_files(output, s903_df, table_name):
+def _merge_dfs(s903_df, old_df, la_name):
     """
-    Looks for existing file of the same type and merges with new file if found
+    Deletes existing data for new LA from pan file
+    Merges new LA data to pan file
     """
-    old_file = Path(output, f"SSDA903_{table_name}_merged.csv")
-    if old_file.is_file():
-        old_df = pd.read_csv(old_file, index_col=None)
-        merged_df = pd.concat([s903_df, old_df], axis=0)
-    else:
-        merged_df = s903_df
-    return merged_df
-
-
-def convert_datetimes(s903_df, dates, table_name):
-    """
-    Ensures that all date fields have been parsed as dates
-    """
-    for date_field in dates[table_name]:
-        s903_df[date_field] = pd.to_datetime(s903_df[date_field], format="%Y/%m/%d")
-    return s903_df
-
-
-def deduplicate(s903_df, table_name, sort_order, dedup):
-    """
-    Sorts and removes duplicate records from merged files following schema
-    """
-    s903_df = s903_df.sort_values(
-        sort_order[table_name], ascending=False, ignore_index=True
-    )
-    s903_df = s903_df.drop_duplicates(subset=dedup[table_name], keep="first")
-    return s903_df
-
-
-def remove_old_data(s903_df, years):
-    """
-    Removes data older than a specified number of years
-    """
-    year = pd.to_datetime("today").year
-    month = pd.to_datetime("today").month
-    if month <= 6:
-        year = year - 1
-    s903_df = s903_df[s903_df["YEAR"] >= year - years]
+    old_df = old_df.drop(old_df[old_df["LA"] == la_name].index)
+    s903_df = pd.concat([s903_df, old_df], axis=0, ignore_index=True)
     return s903_df
 
 
-def convert_dates(s903_df, dates, table_name):
+def merge_agg_files(output, table_name, s903_df, la_name):
     """
-    Ensures that all date fields have been parsed as dates
+    Checks if pan file exists
+    Passes old and new file to function to be merged
     """
-    for date_field in dates[table_name]:
-        s903_df[date_field] = pd.to_datetime(
-            s903_df[date_field], format="%Y/%m/%d"
-        ).dt.date
+    output_file = Path(output, f"pan_London_SSDA903_{table_name}.csv")
+    if output_file.is_file():
+        old_df = pd.read_csv(output_file, index_col=None)
+        s903_df = _merge_dfs(s903_df, old_df, la_name)
     return s903_df
 
 
-def export_la_file(output, table_name, s903_df):
+def export_pan_file(output, table_name, s903_df):
     """
-    Writes the output as a csv
+    Writes file to output directory
     """
-    output_path = Path(output, f"SSDA903_{table_name}_merged.csv")
+    output_path = Path(output, f"pan_London_SSDA903_{table_name}.csv")
     s903_df.to_csv(output_path, index=False)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,35 +19,22 @@
     Matches the columns in the DataFrame against one of the 10 SSDA903 file types
     """
     for table_name, expected_columns in column_names.items():
         if set(s903_df.columns) == set(expected_columns):
             return table_name
 
 
-def _merge_dfs(s903_df, old_df, la_name):
+def data_min(s903_df, minimise, table_name):
     """
-    Deletes existing data for new LA from pan file
-    Merges new LA data to pan file
+    Performs additional data minimisation for pan-London sufficiency analysis in line with schema
     """
-    old_df = old_df.drop(old_df[old_df["LA"] == la_name].index)
-    s903_df = pd.concat([s903_df, old_df], axis=0, ignore_index=True)
+    if table_name in minimise.keys():
+        s903_df = s903_df.drop(columns=minimise[table_name], axis=1)
     return s903_df
 
 
-def merge_agg_files(output, table_name, s903_df, la_name):
-    """
-    Checks if pan file exists
-    Passes old and new file to function to be merged
-    """
-    output_file = Path(output, f"pan_London_SSDA903_{table_name}.csv")
-    if output_file.is_file():
-        old_df = pd.read_csv(output_file, index_col=None)
-        s903_df = _merge_dfs(s903_df, old_df, la_name)
-    return s903_df
-
-
-def export_pan_file(output, table_name, s903_df):
+def export_suff_file(output, table_name, s903_df):
     """
     Writes file to output directory
     """
     output_path = Path(output, f"pan_London_SSDA903_{table_name}.csv")
     s903_df.to_csv(output_path, index=False)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/s903_cli.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/s903_cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,8 @@
 def sufficiency_output(input, output):
     """
     Applies data minimisation to data from aggregated SSDA903 file (output of pan-agg()) and outputs to Sufficiency analysis folder
     :param input: should specify the input file location, including file name and suffix, and be usable by a Path function
     :param output: should specify the path to the output folder
     :return: None
     """
-    s903_main_functions.sufficiency_output(input, output)
+    s903_main_functions.sufficiency_output(input, output)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/s903/s903_main_functions.py` & `liiatools-0.1.5.3/liiatools/datasets/s903/s903_main_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,27 @@
 from liiatools.datasets.shared_functions.common import (
     flip_dict,
     check_file_type,
     supported_file_types,
     check_year,
     save_year_error,
     save_incorrect_year_error,
-    check_year_within_range
+    check_year_within_range,
 )
 
 log = logging.getLogger()
 click_log.basic_config(log)
 
 COMMON_CONFIG_DIR = Path(common_asset_dir.__file__).parent
 # Get all the possible LA codes that could be used
 with open(f"{COMMON_CONFIG_DIR}/LA-codes.yml") as las:
     la_list = list(yaml.full_load(las)["data_codes"].values())
+YEARS_TO_GO_BACK = 7
+YEAR_START_MONTH = 1
+REFERENCE_DATE = datetime.now()
 
 
 def cleanfile(input, la_code, la_log_dir, output):
     """
     Cleans input SSDA903 csv files according to config and outputs cleaned csv files.
     :param input: should specify the input file location, including file name and suffix, and be usable by a Path function
     :param la_code: should be a three-letter string for the local authority depositing the file
@@ -80,19 +83,21 @@
     # Configuration
     try:
         filename = str(Path(input).resolve().stem)
         year = check_year(filename)
     except (AttributeError, ValueError):
         save_year_error(input, la_log_dir)
         return
-    
-    years_to_go_back = 6
-    year_start_month = 6
-    reference_date = datetime.now()
-    if check_year_within_range(year, years_to_go_back, year_start_month, reference_date) is False:
+
+    if (
+        check_year_within_range(
+            year, YEARS_TO_GO_BACK, YEAR_START_MONTH, REFERENCE_DATE
+        )
+        is False
+    ):
         save_incorrect_year_error(input, la_log_dir)
         return
 
     config = clean_config.Config(year)
     la_name = flip_dict(config["data_codes"])[la_code]
     if (
         check_file_type(
@@ -145,15 +150,20 @@
 
     # De-duplicate and remove old data according to schema
     dates = config["dates"]
     s903_df = agg_process.convert_datetimes(s903_df, dates, table_name)
     sort_order = config["sort_order"]
     dedup = config["dedup"]
     s903_df = agg_process.deduplicate(s903_df, table_name, sort_order, dedup)
-    s903_df = agg_process.remove_old_data(s903_df, years=6)
+    s903_df = agg_process.remove_old_data(
+        s903_df,
+        num_of_years=YEARS_TO_GO_BACK,
+        new_year_start_month=YEAR_START_MONTH,
+        as_at_date=REFERENCE_DATE,
+    )
 
     # If file still has data, after removing old data: re-format and export merged file
     if len(s903_df) > 0:
         s903_df = agg_process.convert_dates(s903_df, dates, table_name)
         agg_process.export_la_file(output, table_name, s903_df)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/shared_functions/common.py` & `liiatools-0.1.5.3/liiatools/datasets/shared_functions/common.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/shared_functions/converters.py` & `liiatools-0.1.5.3/liiatools/datasets/shared_functions/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,69 @@
+"""
+  Growth rate table and Population growth table: 2020 to 2026
+"""
+
 import os
 import pandas as pd
-import numpy as np
-import work_path
-
-'''
-  Growth rate table and Population growth table: 2020 to 2026
-'''
+import liiatools.datasets.social_work_workforce.SWFtools.util.work_path as work_path
 
 
 def growth_tables():
-
-    growth_rate_df = {'LEAName': ['Havering', 'Barking and Dagenham', 'Redbridge', 'Newham', 'Tower Hamlets', 'Waltham Forest'],
-                      '2020': [0.0118, 0.0121, 0.0129, 0.0195, 0.0144, 0.0197],
-                      '2021': [0.3639, 0.0136, 0.0249, 0.0090, 0.0115, 0.0086],
-                      '2022': [0.0309, 0.0111, 0.0247, 0.0117, 0.0107, 0.0100],
-                      '2023': [0.0248, 0.0120, 0.0301, 0.0073, 0.0114, 0.0091],
-                      '2024': [0.0254, 0.0137, 0.0261, 0.0118, 0.0115, 0.0087],
-                      '2025': [0.0227, 0.0113, 0.0208, 0.0095, 0.0100, 0.0102],
-                      '2026': [0.023, 0.0107, 0.0243, 0.0093, 0.0118, 0.0058]
-                      }
+    growth_rate_df = {
+        "LEAName": [
+            "Havering",
+            "Barking and Dagenham",
+            "Redbridge",
+            "Newham",
+            "Tower Hamlets",
+            "Waltham Forest",
+        ],
+        "2020": [0.0118, 0.0121, 0.0129, 0.0195, 0.0144, 0.0197],
+        "2021": [0.3639, 0.0136, 0.0249, 0.0090, 0.0115, 0.0086],
+        "2022": [0.0309, 0.0111, 0.0247, 0.0117, 0.0107, 0.0100],
+        "2023": [0.0248, 0.0120, 0.0301, 0.0073, 0.0114, 0.0091],
+        "2024": [0.0254, 0.0137, 0.0261, 0.0118, 0.0115, 0.0087],
+        "2025": [0.0227, 0.0113, 0.0208, 0.0095, 0.0100, 0.0102],
+        "2026": [0.023, 0.0107, 0.0243, 0.0093, 0.0118, 0.0058],
+    }
 
     growth_rate_table = pd.DataFrame(growth_rate_df)
 
-    # print(growth_rate_table)
-
     # ===== Save and export file ===== #
-    fileOutN = 'growth_rate_table.xlsx'
+    fileOutN = "growth_rate_table.xlsx"
     requestPath = work_path.request
     fileOut = os.path.join(requestPath, fileOutN)
     growth_rate_table.to_excel(fileOut, index=False)
 
     print("Auxiliary table: ", fileOutN, " Created")
 
-    '''
+    """
       Population growth table: 2020 to 2026
-    '''
+    """
 
-    population_growth_df = {'LEAName': ['Barking and Dagenham', 'Havering', 'Newham', 'Redbridge', 'Tower Hamlets', 'Waltham Forest'],
-                            '2020': [320128, 161409, 461239, 215230, 529399, 383747],
-                            '2021': [324487, 220150, 465409, 220598, 535487, 387033],
-                            '2022': [328104, 226948, 470857, 226048, 541209, 390895],
-                            '2023': [332057, 232581, 474304, 232857, 547400, 394462],
-                            '2024': [336590, 238498, 479905, 238942, 553698, 397877],
-                            '2025': [340410, 243909, 484480, 243909, 559221, 401948],
-                            '2026': [344040, 249520, 488977, 249844, 565820, 404285]
-                            }
+    population_growth_df = {
+        "LEAName": [
+            "Barking and Dagenham",
+            "Havering",
+            "Newham",
+            "Redbridge",
+            "Tower Hamlets",
+            "Waltham Forest",
+        ],
+        "2020": [320128, 161409, 461239, 215230, 529399, 383747],
+        "2021": [324487, 220150, 465409, 220598, 535487, 387033],
+        "2022": [328104, 226948, 470857, 226048, 541209, 390895],
+        "2023": [332057, 232581, 474304, 232857, 547400, 394462],
+        "2024": [336590, 238498, 479905, 238942, 553698, 397877],
+        "2025": [340410, 243909, 484480, 243909, 559221, 401948],
+        "2026": [344040, 249520, 488977, 249844, 565820, 404285],
+    }
 
     population_growth_table = pd.DataFrame(population_growth_df)
 
-    # print(population_growth_table)
-
     # ===== Save and export file ===== #
-    fileOutN = 'population_growth_table.xlsx'
+    fileOutN = "population_growth_table.xlsx"
     requestPath = work_path.request
     fileOut = os.path.join(requestPath, fileOutN)
     population_growth_table.to_excel(fileOut, index=False)
 
     print("Auxiliary table: ", fileOutN, " Created")
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import os
-import pandas as pd
-import numpy as np
-import work_path
-
-'''
-   Spreadsheet generation with columns ordered by: YearCensus, LEAName, Gender, Ethinicity_Compact. 
+"""
+   Spreadsheet generation with columns ordered by: YearCensus, LEAName, Gender, Ethnicity_Compact. 
    And with the sum columns: FTESum. 
    And the employee count: SWENo_Count
-'''
+"""
+import os
+import pandas as pd
+import liiatools.datasets.social_work_workforce.SWFtools.util.work_path as work_path
 
 
 def pivotGen():
-
     # ===== Read file ===== #
-    file = 'merged_modified.csv'
+    file = "merged_modified.csv"
     path = work_path.flatfile_folder
     requestPath = work_path.request
     pathFile = os.path.join(path, file)
     df = pd.read_csv(pathFile)
 
-
-    pivotTable = df.groupby(['YearCensus', 'LEAName', 'Gender', 'Ethinicity_Compact'])\
-        .agg(FTESum=('FTE', 'sum'), SWENo_Count=('SWENo', 'count'))
-
+    pivotTable = df.groupby(
+        ["YearCensus", "LEAName", "Gender", "Ethnicity_Compact"]
+    ).agg(FTESum=("FTE", "sum"), SWENo_Count=("SWENo", "count"))
 
     # ===== Save and export file ===== #
-    fileOutN = 'pivotTable.xlsx'
+    fileOutN = "pivotTable.xlsx"
     requestPath = work_path.request
     fileOut = os.path.join(requestPath, fileOutN)
     pivotTable.to_excel(fileOut, merge_cells=False)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""This file contains constants and functions used in converting and merging XML data from CIN folder"""
+"""This file contains constants and functions used in converting and merging XML data from CSWW folder"""
 
+import hashlib
+import datetime as dt
 from typing import Final, Dict, List
 from decouple import config
 
-import hashlib
-import datetime as dt
 
 # === CONSTANTS === #
 LEA_DICT: Final[Dict[str, str]] = {
-    '301': "Barking and Dagenham",
-    '316': "Newham",
-    '317': "Redbridge",
-    '211': "Tower Hamlets",
-    '311': "Havering",
-    '320': "Waltham Forest"
+    "301": "Barking and Dagenham",
+    "316": "Newham",
+    "317": "Redbridge",
+    "211": "Tower Hamlets",
+    "311": "Havering",
+    "320": "Waltham Forest",
 }
 
 ETHNICITY_GROUP_DICT: Final[Dict[str, str]] = {
     "WBRI": "White - British",
     "WIRI": "White - Irish",
     "WOTH": "Any Other White Background",
     "MWBC": "White and Black Caribbean",
@@ -30,15 +30,15 @@
     "AOTH": "Any Other Asian Background",
     "BCRB": "Black Caribbean",
     "BAFR": "Black African",
     "BOTH": "Any Other Black Background",
     "CHNE": "Chinese",
     "OOTH": "Any Other Ethnic Group",
     "REFU": "Declared not stated or Refused",
-    "NOBT": "Information Not Yet Obtained"
+    "NOBT": "Information Not Yet Obtained",
 }
 
 ETHNICITY_DICT: Final[Dict[str, str]] = {
     "WBRI": "White - British",
     "WIRI": "White - Irish",
     "WOTH": "Any Other White Background",
     "MWBC": "White and Black Caribbean",
@@ -51,123 +51,137 @@
     "AOTH": "Any Other Asian Background",
     "BCRB": "Black Caribbean",
     "BAFR": "Black African",
     "BOTH": "Any Other Black Background",
     "CHNE": "Chinese",
     "OOTH": "Any Other Ethnic Group",
     "REFU": "Declared not stated or Refused",
-    "NOBT": "Information Not Yet Obtained"
+    "NOBT": "Information Not Yet Obtained",
 }
 
 GENDER_DICT: Final[Dict[str, str]] = {
-    '0': "Not known (gender has not been recorded)",
-    '1': "male",
-    '2': "female",
-    '9': "not specified (indeterminate; unable to be classified as either male or female)"
+    "0": "Not known (gender has not been recorded)",
+    "1": "male",
+    "2": "female",
+    "9": "not specified (indeterminate; unable to be classified as either male or female)",
 }
 
 ORG_ROLE_DICT: Final[Dict[str, str]] = {
-    '1': "Senior Manager",
-    '2': "Middle Manager",
-    '3': "First Line Manager",
-    '4': "Senior Practitioner",
-    '5': "Case Holder",
-    '6': "Qualified without cases"
+    "1": "Senior Manager",
+    "2": "Middle Manager",
+    "3": "First Line Manager",
+    "4": "Senior Practitioner",
+    "5": "Case Holder",
+    "6": "Qualified without cases",
+}
+
+SENIORITY_CODE_DICT: Final[Dict[str, str]] = {
+    "1": "Newly qualified",
+    "2": "Early career",
+    "3": "Experienced",
+    "4": "Senior",
+    "5": "Agency",
 }
 
 QUAL_LEVEL_DICT: Final[Dict[str, str]] = {
-    '1': "Undergraduate",
-    '2': "Postgraduate",
-    '3': "Other (for example any other qualification)"
+    "1": "Undergraduate",
+    "2": "Postgraduate",
+    "3": "Other (for example any other qualification)",
 }
 
 
 # === FUNCTIONS === #
 def swe_hash(worker: Dict[str, str]):
     """
     Converts the **SWENo** field to a hash code represented in HEX
     :param worker: A dictionary containing worker data
     :return: None
     """
-    swe_num = worker['SWENo']
+    swe_num = worker["SWENo"]
 
-    private_string = config('sec_str', default='')
+    private_string = config("sec_str", default="")
 
     private_key = swe_num + private_string
 
     # Preparing plain text (SWENo) to hash it
     plaintext = private_key.encode()
 
     hash_algorithm = hashlib.sha3_256(plaintext)
 
-    worker['SWENo'] = hash_algorithm.hexdigest()
+    worker["SWENo"] = hash_algorithm.hexdigest()
 
 
 def convert_dates(worker: Dict[str, str]):
     """
     This function will:
     1) Add and compute the value for the following columns: **Age**, **RoleStartDate**, **RoleEndDate**, **DoB_year**
     (all of these values contain only their respective year, not the full date)
     2) Remove the **PersonBirthDate** field inside each worker dictionary
     :param worker: A dictionary containing worker data
     :return: None
     """
-    date_format = '%Y-%m-%d'
-
-    if 'PersonBirthDate' in worker:
-        birth_date = worker['PersonBirthDate']
-        worker['DoB_year'] = str(dt.datetime.strptime(birth_date, date_format).year)
-        worker['Age'] = str(dt.datetime.today().year - dt.datetime.strptime(birth_date, date_format).year)
-
-        del worker['PersonBirthDate']
+    date_format = "%Y-%m-%d"
 
-    if 'RoleStartDate' in worker:
-        worker['RoleStartDate'] = str(dt.datetime.strptime(worker['RoleStartDate'], date_format).year)
-
-    if 'RoleEndDate' in worker:
-        worker['RoleEndDate'] = str(dt.datetime.strptime(worker['RoleEndDate'], date_format).year)
+    if "PersonBirthDate" in worker:
+        birth_date = worker["PersonBirthDate"]
+        worker["DoB_year"] = str(dt.datetime.strptime(birth_date, date_format).year)
+        worker["Age"] = str(
+            dt.datetime.today().year
+            - dt.datetime.strptime(birth_date, date_format).year
+        )
+
+        del worker["PersonBirthDate"]
+
+    if "RoleStartDate" in worker:
+        worker["RoleStartDate"] = str(
+            dt.datetime.strptime(worker["RoleStartDate"], date_format).year
+        )
+
+    if "RoleEndDate" in worker:
+        worker["RoleEndDate"] = str(
+            dt.datetime.strptime(worker["RoleEndDate"], date_format).year
+        )
 
 
 def column_transfer(workers: List[Dict[str, str]], lea: str, year_census: str):
     """
     Adds new columns to the table.
     :param workers: A list of dictionaries containing worker data
     :param lea: Local Authority code
     :param year_census: Census year
     :return: None
     """
     for worker in workers:
-
         if lea in LEA_DICT:
-            worker['LEAName'] = LEA_DICT[lea]
+            worker["LEAName"] = LEA_DICT[lea]
         else:
-            worker['LEAName'] = ''
+            worker["LEAName"] = ""
 
         # Adding ethnicity extra columns
-        if 'Ethnicity' in worker:
-            ethnicity = worker['Ethnicity']
-            worker['Ethnicity_Group'] = ETHNICITY_GROUP_DICT[ethnicity]
-            worker['Ethnicity_Compact'] = ETHNICITY_DICT[ethnicity]
+        if "Ethnicity" in worker:
+            ethnicity = worker["Ethnicity"]
+            worker["Ethnicity_Group"] = ETHNICITY_GROUP_DICT[ethnicity]
+            worker["Ethnicity_Compact"] = ETHNICITY_DICT[ethnicity]
         else:
-            worker['Ethnicity_Group'] = ''
-            worker['Ethnicity_Compact'] = ''
+            worker["Ethnicity_Group"] = ""
+            worker["Ethnicity_Compact"] = ""
 
         # Adding gender extra column
-        if 'GenderCurrent' in worker:
-            worker['Gender'] = GENDER_DICT[worker['GenderCurrent']]
+        if "GenderCurrent" in worker:
+            worker["Gender"] = GENDER_DICT[worker["GenderCurrent"]]
         else:
-            worker['Gender'] = ''
+            worker["Gender"] = ""
 
         # Organisation role extra column
-        if 'OrgRole' in worker:
-            worker['OrgRoleName'] = ORG_ROLE_DICT[worker['OrgRole']]
+        if "OrgRole" in worker:
+            worker["OrgRoleName"] = ORG_ROLE_DICT[worker["OrgRole"]]
         else:
-            worker['OrgRoleName'] = ''
+            worker["OrgRoleName"] = ""
 
         # Qualification level
-        if 'QualLevel' in worker:
-            worker['QualLevelName'] = QUAL_LEVEL_DICT[worker['QualLevel']]
+        if "QualLevel" in worker:
+            worker["QualLevelName"] = QUAL_LEVEL_DICT[worker["QualLevel"]]
         else:
-            worker['QualLevelNAme'] = ''
+            worker["QualLevelNAme"] = ""
 
-        worker['YearCensus'] = year_census
-        worker['LEA'] = lea
+        worker["YearCensus"] = year_census
+        worker["LEA"] = lea
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,149 +3,230 @@
 import os
 from pathlib import Path
 from typing import List, Dict, Final
 
 import lxml.etree as etree
 from pandas import DataFrame
 
-import SWFtools.util.AppLogs as AppLog
-import SWFtools.dataprocessing.validation.validator as validator
-import SWFtools.dataprocessing.converter as converter
-from SWFtools.util.work_path import la_directories, flatfile_folder
-
-COLUMNS: Final[List[str]] = ["YearCensus", "LEA", "AgencyWorker", "SWENo", "FTE", "DoB_year", "Age", "GenderCurrent",
-                             "Ethnicity", "QualInst", "QualLevel", "StepUpGrad", "OrgRole", "RoleStartDate", "StartOrigin",
-                             "RoleEndDate", "LeaverDestination", "FTE30", "Cases30", "ContractWeeks", "FrontlineGrad",
-                             "CFKSSstatus"]
-
-COLUMNS_MERGED_FILE: Final[List[str]] = ["YearCensus", "LEA", "LEAName", "AgencyWorker", "SWENo", "FTE", "DoB_year", "Age",
-                                         "GenderCurrent", "Gender", "Ethnicity", "Ethnicity_Group", "Ethnicity_Compact",
-                                         "QualInst", "QualLevel", "QualLevelName", "StepUpGrad", "OrgRole", "OrgRoleName",
-                                         "RoleStartDate", "StartOrigin", "RoleEndDate", "LeaverDestination", "FTE30",
-                                         "Cases30", "ContractWeeks", "FrontlineGrad", "CFKSSstatus"]
+import liiatools.datasets.social_work_workforce.SWFtools.util.AppLogs as AppLog
+import liiatools.datasets.social_work_workforce.SWFtools.dataprocessing.validation.validator as validator
+import liiatools.datasets.social_work_workforce.SWFtools.dataprocessing.converter as converter
+from liiatools.datasets.social_work_workforce.SWFtools.util.work_path import (
+    la_directories,
+    flatfile_folder,
+)
+
+COLUMNS: Final[List[str]] = [
+    "YearCensus",
+    "LEA",
+    "AgencyWorker",
+    "SWENo",
+    "FTE",
+    "DoB_year",
+    "Age",
+    "GenderCurrent",
+    "Ethnicity",
+    "QualInst",
+    "QualLevel",
+    "StepUpGrad",
+    "OrgRole",
+    "RoleStartDate",
+    "StartOrigin",
+    "RoleEndDate",
+    "LeaverDestination",
+    "FTE30",
+    "Cases30",
+    "ContractWeeks",
+    "FrontlineGrad",
+    "CFKSSstatus",
+]
+
+COLUMNS_MERGED_FILE: Final[List[str]] = [
+    "YearCensus",
+    "LEA",
+    "LEAName",
+    "AgencyWorker",
+    "SWENo",
+    "FTE",
+    "DoB_year",
+    "Age",
+    "GenderCurrent",
+    "Gender",
+    "Ethnicity",
+    "Ethnicity_Group",
+    "Ethnicity_Compact",
+    "QualInst",
+    "QualLevel",
+    "QualLevelName",
+    "StepUpGrad",
+    "OrgRole",
+    "OrgRoleName",
+    "RoleStartDate",
+    "StartOrigin",
+    "RoleEndDate",
+    "LeaverDestination",
+    "FTE30",
+    "Cases30",
+    "ContractWeeks",
+    "FrontlineGrad",
+    "CFKSSstatus",
+]
 
 
 def get_xml_files_from(directory: os.DirEntry) -> List[str]:
     """
     A function that returns a list of XML files that are directly inside the specified directory.
     :param directory: The directory that contains XML files. This is the LA directory
     :return: A list containing the names of the XML files. Each entry has the format: 'filename.xml'
     """
-    directory_files = [file for file in os.listdir(directory) if os.path.isfile(os.path.join(directory, file))]
-    xml_files = [file for file in directory_files if file.endswith('.xml')]
+    directory_files = [
+        file
+        for file in os.listdir(directory)
+        if os.path.isfile(os.path.join(directory, file))
+    ]
+    xml_files = [file for file in directory_files if file.endswith(".xml")]
 
     return xml_files
 
 
-def parse_and_validate(la_directory: os.DirEntry, xml_file: str) -> List[Dict[str, str]] | None:
+def parse_and_validate(
+    la_directory: os.DirEntry, xml_file: str
+) -> List[Dict[str, str]] | None:
     """
     Parses an XML file, validates it and adds **'LEA'** and **'YearCensus'** common fields.
     :param la_directory: The directory that contains the XML file.
     :param xml_file: The name of the XML file. Format: 'filename.xml'
     :return: Returns a list of dictionaries containing valid worker data. If the file failed validation it returns None
     """
     # === PARSING DATA === #
-    AppLog.log(f'Parsing \'{xml_file}\'...')
+    AppLog.log(f"Parsing '{xml_file}'...")
     parsed_xml = etree.parse(os.path.join(la_directory, xml_file))
 
     # === VALIDATING DATA === #
     validation_errors = []
 
-    AppLog.log(f'Validating \'{xml_file}\'...',console_output=True)
-    AppLog.log(f'Validating \'{xml_file}\'', la_directory.name)
+    AppLog.log(f"Validating '{xml_file}'...", console_output=True)
+    AppLog.log(f"Validating '{xml_file}'", la_directory.name)
 
     # Validation failed, continue with next file
     if not validator.is_acceptable(parsed_xml, validation_errors):
-        message = f'The file \'{xml_file}\' failed validation:'
+        message = f"The file '{xml_file}' failed validation:"
         AppLog.log(message, console_output=True)
         AppLog.log(message, la_directory.name)
         AppLog.log(validation_errors, la_directory.name)
         return None
 
-    AppLog.log(f'The file \'{xml_file}\' passed minimum validation requirement', console_output=True)
-    AppLog.log(f'Validating worker data...', console_output=True)
+    AppLog.log(
+        f"The file '{xml_file}' passed minimum validation requirement",
+        console_output=True,
+    )
+    AppLog.log(f"Validating worker data...", console_output=True)
 
     # May contain 'None' values where worker data failed validation
-    workers = [validator.get_valid_worker_data(worker, validation_errors) for worker in parsed_xml.iter('CSWWWorker')]
+    workers = [
+        validator.get_valid_worker_data(worker, validation_errors)
+        for worker in parsed_xml.iter("CSWWWorker")
+    ]
 
     # Validation summary data
     total_workers = len(workers)
     valid_count = sum(1 for worker in workers if worker is not None)
     validation_error_count = len(validation_errors)
 
     # Filter out the 'None' entries
     workers = [worker for worker in workers if worker is not None]
 
     # Print validation errors if there are any (worker validation)
     if validation_error_count != 0:
-        AppLog.log('Worker validation errors: ', la_directory.name)
+        AppLog.log("Worker validation errors: ", la_directory.name)
         AppLog.log(validation_errors, la_directory.name)
 
     # Print validation summary to LA and application log (runtime)
-    messages = [f'{valid_count} out of {total_workers} worker records passed validation',
-                f'{validation_error_count} worker validation errors.']
+    messages = [
+        f"{valid_count} out of {total_workers} worker records passed validation",
+        f"{validation_error_count} worker validation errors.",
+    ]
     AppLog.log(messages, la_directory.name)
     AppLog.log(messages, console_output=True)
 
     # === ADDING EXTENDED FIELDS === #
     # Pre-computed fields for conversion process
-    lea = parsed_xml.xpath('//LEA')[0].text
-    year_census = parsed_xml.xpath('//Year')[0].text
+    lea = parsed_xml.xpath("//LEA")[0].text
+    year_census = parsed_xml.xpath("//Year")[0].text
 
     converter.column_transfer(workers, lea, year_census)
 
     return workers
 
 
 def process_all_input_files():
     """
     Validates XML files, processes worker data, and merges all validated XMLs.
     :return: None
     """
-    AppLog.log_section_header('Processing all XML files inside CIN folder', console_output=True)
+    AppLog.log_section_header(
+        "Processing all XML files inside CIN folder", console_output=True
+    )
 
     processed_files_count = 0
-    path_merged_file = os.path.join(flatfile_folder, 'merged_LA_files.csv')
-    path_modified_merged_file = os.path.join(flatfile_folder, 'merged_modified.csv')
+    path_merged_file = os.path.join(flatfile_folder, "merged_LA_files.csv")
+    path_modified_merged_file = os.path.join(flatfile_folder, "merged_modified.csv")
 
     for la_directory in la_directories:
-        AppLog.log(f'Processing XML files inside: {la_directory.path}')
+        AppLog.log(f"Processing XML files inside: {la_directory.path}")
 
         xml_files = get_xml_files_from(la_directory)
 
         for xml_file in xml_files:
-
             workers = parse_and_validate(la_directory, xml_file)
 
             if workers is None:
                 continue
 
             # === PROCESSING WORKER DATA === #
-            AppLog.log('Processing worker data...', console_output=True)
-            AppLog.log('Processing worker data...', la_directory.name)
+            AppLog.log("Processing worker data...", console_output=True)
+            AppLog.log("Processing worker data...", la_directory.name)
             for worker in workers:
                 converter.swe_hash(worker)
                 converter.convert_dates(worker)
 
             # === WRITING TO CSV === #
-            path_file = os.path.join(flatfile_folder, la_directory.name, Path(xml_file).stem + '.csv')
+            path_file = os.path.join(
+                flatfile_folder, la_directory.name, Path(xml_file).stem + ".csv"
+            )
             data_frame = DataFrame(workers, columns=COLUMNS_MERGED_FILE)
 
             # Write single file
             data_frame.to_csv(path_file, index=False, columns=COLUMNS)
 
             # Write to common file (merged records file)
             # Either append data to existing file or write to file if it's the first file to be processed
             if processed_files_count != 0:
                 # header = False (do not append column names again)
                 # columns = COLUMNS | COLUMNS_MERGED_FILE (what columns/fields to write)
                 # mode is the same as Python file modes ('w' write is default)
-                data_frame.to_csv(path_merged_file, index=False, header=False, columns=COLUMNS, mode='a')
-                data_frame.to_csv(path_modified_merged_file, index=False, header=False, columns=COLUMNS_MERGED_FILE, mode='a')
+                data_frame.to_csv(
+                    path_merged_file,
+                    index=False,
+                    header=False,
+                    columns=COLUMNS,
+                    mode="a",
+                )
+                data_frame.to_csv(
+                    path_modified_merged_file,
+                    index=False,
+                    header=False,
+                    columns=COLUMNS_MERGED_FILE,
+                    mode="a",
+                )
             else:
                 data_frame.to_csv(path_merged_file, index=False, columns=COLUMNS)
-                data_frame.to_csv(path_modified_merged_file, index=False, columns=COLUMNS_MERGED_FILE)
+                data_frame.to_csv(
+                    path_modified_merged_file, index=False, columns=COLUMNS_MERGED_FILE
+                )
 
             processed_files_count = processed_files_count + 1
 
-    AppLog.log(f'Finished processing {processed_files_count} files in {len(la_directories)} directories.',
-               console_output=True)
+    AppLog.log(
+        f"Finished processing {processed_files_count} files in {len(la_directories)} directories.",
+        console_output=True,
+    )
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,36 @@
 
 from typing import List, Dict, Final
 
 import lxml.etree as etree
 
 import xmlschema
 from xmlschema import XMLSchemaValidationError
-from SWFtools.util.work_path import XML_SCHEMA
+from liiatools.datasets.social_work_workforce.SWFtools.util.work_path import XML_SCHEMA
 
-from SWFtools.dataprocessing.validation.validation_error import ValidationError, ERROR_CAUSE
+from liiatools.datasets.social_work_workforce.SWFtools.dataprocessing.validation.validation_error import (
+    ValidationError,
+    ERROR_CAUSE,
+)
 
 CIN_XML_SCHEMA: Final = xmlschema.XMLSchema11(XML_SCHEMA)
-WORKER_SCHEMA: Final = CIN_XML_SCHEMA.find('//CSWWWorker')
-NON_AGENCY_MANDATORY_TAG: Final = ['PersonBirthDate', 'GenderCurrent', 'Ethnicity', 'QualInst', 'StepUpGrad',
-                                    'OrgRole', 'RoleStartDate', 'StartOrigin', 'FTE30', 'WorkingDaysLost', 'FrontlineGrad']
+WORKER_SCHEMA: Final = CIN_XML_SCHEMA.find("//CSWWWorker")
+NON_AGENCY_MANDATORY_TAG: Final = [
+    "PersonBirthDate",
+    "GenderCurrent",
+    "Ethnicity",
+    "QualInst",
+    "StepUpGrad",
+    "OrgRole",
+    "RoleStartDate",
+    "StartOrigin",
+    "FTE30",
+    "WorkingDaysLost",
+    "FrontlineGrad",
+]
 
 
 def convert_schema_error(schema_error: XMLSchemaValidationError) -> ValidationError:
     """
     Converts an **XMLSchemaValidationError** to a custom validation error. See *'validation_error.py'*
     """
 
@@ -36,37 +50,55 @@
         # The tag of the read element
         read_tag = schema_error.elem[schema_error.args[2]].tag
 
         # The tag of the expected element
         expected_tag = schema_error.args[3].name
 
         if read_tag != expected_tag:
-            return ValidationError(ERROR_CAUSE.GROUP_FORMAT, schema_error.elem.tag, schema_error.sourceline)
+            return ValidationError(
+                ERROR_CAUSE.GROUP_FORMAT, schema_error.elem.tag, schema_error.sourceline
+            )
         elif occurs < occurs_range[0]:
-            return ValidationError(ERROR_CAUSE.MISSING_TAG, schema_error.elem.tag, schema_error.sourceline)
+            return ValidationError(
+                ERROR_CAUSE.MISSING_TAG, schema_error.elem.tag, schema_error.sourceline
+            )
         elif occurs > occurs_range[1]:
-            return ValidationError(ERROR_CAUSE.TOO_MANY_TAGS, schema_error.elem.tag, schema_error.sourceline)
+            return ValidationError(
+                ERROR_CAUSE.TOO_MANY_TAGS,
+                schema_error.elem.tag,
+                schema_error.sourceline,
+            )
         else:
-            print(f'UNEXPECTED ERROR!\n{schema_error}')
+            print(f"UNEXPECTED ERROR!\n{schema_error}")
             return None
     # Value does not match to any enumerated value
     elif schema_error.validator.__class__ == xmlschema.validators.XsdEnumerationFacets:
-        return ValidationError(ERROR_CAUSE.VALUE, schema_error.elem.tag, schema_error.sourceline)
+        return ValidationError(
+            ERROR_CAUSE.VALUE, schema_error.elem.tag, schema_error.sourceline
+        )
     # Value does not match pattern specified
     elif schema_error.validator.__class__ == xmlschema.validators.XsdPatternFacets:
-        return ValidationError(ERROR_CAUSE.VALUE, schema_error.elem.tag, schema_error.sourceline)
+        return ValidationError(
+            ERROR_CAUSE.VALUE, schema_error.elem.tag, schema_error.sourceline
+        )
     # Value is of unexpected type
     elif schema_error.validator.__class__ == xmlschema.validators.XsdAtomicBuiltin:
-        return ValidationError(ERROR_CAUSE.TYPE, schema_error.elem.tag, schema_error.sourceline)
+        return ValidationError(
+            ERROR_CAUSE.TYPE, schema_error.elem.tag, schema_error.sourceline
+        )
     # Value is below accepted range minimum inclusive
     elif schema_error.validator.__class__ == xmlschema.validators.XsdMinInclusiveFacet:
-        return ValidationError(ERROR_CAUSE.MIN_RANGE, schema_error.elem.tag, schema_error.sourceline)
+        return ValidationError(
+            ERROR_CAUSE.MIN_RANGE, schema_error.elem.tag, schema_error.sourceline
+        )
     # Value is above accepted range maximum inclusive
     elif schema_error.validator.__class__ == xmlschema.validators.XsdMaxInclusiveFacet:
-        return ValidationError(ERROR_CAUSE.MAX_RANGE, schema_error.elem.tag, schema_error.sourceline)
+        return ValidationError(
+            ERROR_CAUSE.MAX_RANGE, schema_error.elem.tag, schema_error.sourceline
+        )
 
 
 def is_acceptable(parsed_xml: etree.Element, error_list: List[ValidationError]) -> bool:
     """
     Validates **'Header'** and **'LALevelVacancies'** tags then checks that the format of the message is correct:
     **'Header'**, **'LALevelVacancies'** followed by **'CSWWWorker'** n times
 
@@ -74,97 +106,134 @@
     :param error_list: A list where all validation errors are placed into.
     :return: Returns 'True' if the document can be further processed of 'False' otherwise.
     """
 
     if not __is_message_format_valid(parsed_xml, error_list):
         return False
 
-    la_vacancies_schema = CIN_XML_SCHEMA.find('//LALevelVacancies')
-    la_vacancies_xml = parsed_xml.xpath('//LALevelVacancies')[0]
+    la_vacancies_schema = CIN_XML_SCHEMA.find("//LALevelVacancies")
+    la_vacancies_xml = parsed_xml.xpath("//LALevelVacancies")[0]
 
-    header_schema = CIN_XML_SCHEMA.find('//Header')
-    header_xml = parsed_xml.xpath('//Header')[0]
+    header_schema = CIN_XML_SCHEMA.find("//Header")
+    header_xml = parsed_xml.xpath("//Header")[0]
 
-    verr = [convert_schema_error(error) for error in header_schema.iter_errors(header_xml)]
-    verr.extend([convert_schema_error(error) for error in la_vacancies_schema.iter_errors(la_vacancies_xml)])
+    verr = [
+        convert_schema_error(error) for error in header_schema.iter_errors(header_xml)
+    ]
+    verr.extend(
+        [
+            convert_schema_error(error)
+            for error in la_vacancies_schema.iter_errors(la_vacancies_xml)
+        ]
+    )
 
     if len(verr) != 0:
         error_list.extend(verr)
         return False
 
     return True
 
 
 # Shallow validation of 'Header', 'LALevelVacancies', and 'CSWWWorker' tags
-def __is_message_format_valid(parsed_xml: etree.ElementTree, error_list: List[ValidationError]) -> bool:
+def __is_message_format_valid(
+    parsed_xml: etree.ElementTree, error_list: List[ValidationError]
+) -> bool:
     can_continue = True
 
     for error in CIN_XML_SCHEMA.iter_errors(parsed_xml, max_depth=1):
         va = convert_schema_error(error)
 
         # A group format means that the Header, LAVacancies and CSWWWorker tags are just out of order, can still proceed
         if va is not None and va.cause != ERROR_CAUSE.GROUP_FORMAT:
             can_continue = False
 
         error_list.append(va)
 
     return can_continue
 
 
-def get_valid_worker_data(worker_element: etree.Element, error_list: List[ValidationError]) -> Dict[str, str]:
+def get_valid_worker_data(
+    worker_element: etree.Element, error_list: List[ValidationError]
+) -> Dict[str, str]:
     """
     Takes in a worker element (lxml.etree), validates it and returns the worker data as a dictionary
     or **'None'** if the worker data is invalid.
 
     :param worker_element: A tree element (lxml.etree) that has the tag 'CSWWWorker' .
     :param error_list: A list where all validation errors are placed into.
     :return: A dictionary that contains the worker data. Child tags are the keys and
     their value as the dictionary's value
     """
 
     # === XML SCHEMA VALIDATION ===
-    va: List[ValidationError] = list(map(convert_schema_error, WORKER_SCHEMA.iter_errors(worker_element)))
+    va: List[ValidationError] = list(
+        map(convert_schema_error, WORKER_SCHEMA.iter_errors(worker_element))
+    )
 
     # === BUILDING WORKER DATA SET; FURTHER VALIDATION ===
     worker_data = {}
 
     for elem in worker_element:
         worker_data[elem.tag] = elem.text
 
-    is_agency_worker = worker_data['AgencyWorker'] == '1'
-    is_leaver = 'RoleEndDate' in worker_data
-    is_starter = 'RoleStartDate' in worker_data
+    is_agency_worker = worker_data["AgencyWorker"] == "1"
+    is_leaver = "RoleEndDate" in worker_data
+    is_starter = "RoleStartDate" in worker_data
 
     # Validation rules if the worker is a non-agency worker
     if not is_agency_worker:
         # If a worker is a non-agency worker, check that mandatory tags are present
         for tag in NON_AGENCY_MANDATORY_TAG:
             if tag not in worker_data:
-                va.append(ValidationError(ERROR_CAUSE.NON_AGENCY_MANDATORY_MISSING, tag, worker_element.sourceline))
+                va.append(
+                    ValidationError(
+                        ERROR_CAUSE.NON_AGENCY_MANDATORY_MISSING,
+                        tag,
+                        worker_element.sourceline,
+                    )
+                )
 
     # Validation rules if the worker is a starter (condition checked via eXclusive OR)
-    if is_starter ^ ('StartOrigin' in worker_data):
-        va.append(ValidationError(ERROR_CAUSE.MISSING_TAG, 'StartOrigin', worker_element.sourceline))
+    if is_starter ^ ("StartOrigin" in worker_data):
+        va.append(
+            ValidationError(
+                ERROR_CAUSE.MISSING_TAG, "StartOrigin", worker_element.sourceline
+            )
+        )
 
     # Validation rules if the worker is a leaver
-    if is_leaver and worker_data['FTE'] != '0':
-        sourceline = worker_element.xpath('//FTE')[0].sourceline
-        va.append(ValidationError(ERROR_CAUSE.LEAVER_FTE, 'FTE', sourceline))
+    if is_leaver and worker_data["FTE"] != "0":
+        sourceline = worker_element.xpath("//FTE")[0].sourceline
+        va.append(ValidationError(ERROR_CAUSE.LEAVER_FTE, "FTE", sourceline))
 
-    if is_leaver ^ ('ReasonLeave' in worker_data):
+    if is_leaver ^ ("ReasonLeave" in worker_data):
         if is_leaver:
-            va.append(ERROR_CAUSE.MISSING_TAG, 'ReasonLeave', worker_element.sourceline)
+            va.append(ERROR_CAUSE.MISSING_TAG, "ReasonLeave", worker_element.sourceline)
         else:
-            va.append(ValidationError(ERROR_CAUSE.LEAVER_UNEXPECTED, 'ReasonLeave', worker_element.sourceline))
+            va.append(
+                ValidationError(
+                    ERROR_CAUSE.LEAVER_UNEXPECTED,
+                    "ReasonLeave",
+                    worker_element.sourceline,
+                )
+            )
 
-    if is_leaver ^ ('LeaverDestination' in worker_data):
+    if is_leaver ^ ("LeaverDestination" in worker_data):
         if is_leaver:
-            va.append(ERROR_CAUSE.MISSING_TAG, 'LeaverDestination', worker_element.sourceline)
+            va.append(
+                ERROR_CAUSE.MISSING_TAG, "LeaverDestination", worker_element.sourceline
+            )
         else:
-            va.append(ValidationError(ERROR_CAUSE.LEAVER_UNEXPECTED, 'LeaverDestination', worker_element.sourceline))
+            va.append(
+                ValidationError(
+                    ERROR_CAUSE.LEAVER_UNEXPECTED,
+                    "LeaverDestination",
+                    worker_element.sourceline,
+                )
+            )
 
     # If there are any errors the element is invalid, return None and move on
     if len(va) != 0:
         error_list.extend(va)
         return None
 
     return worker_data
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/main.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-# ===== Main script where all the others will be called =====
+"""Main script where all the others will be called"""
 
 import time
-import SWFtools.util.AppLogs as AppLog
-import SWFtools.util.work_path as work_path
-import SWFtools.dataprocessing.file_operations as fop
-from SWFtools.analysis.growth_tables import growth_tables
-from SWFtools.analysis.pivotGen import pivotGen
-from SWFtools.analysis.seniority import seniority
-from SWFtools.analysis.progressed import progressed
-from SWFtools.analysis.seniority_forecast_5c import seniority_forecast_5c
-from SWFtools.analysis.seniority_forecast_04 import seniority_forecast_04
-from SWFtools.analysis.FTESum import FTESum
-from SWFtools.analysis.FTESum_2020 import FTESum_2020
+import liiatools.datasets.social_work_workforce.SWFtools.util.AppLogs as AppLog
+import liiatools.datasets.social_work_workforce.SWFtools.util.work_path as work_path
+import liiatools.datasets.social_work_workforce.SWFtools.dataprocessing.file_operations as fop
+from liiatools.datasets.social_work_workforce.SWFtools.analysis.growth_tables import (
+    growth_tables,
+)
+from liiatools.datasets.social_work_workforce.SWFtools.analysis.pivotGen import pivotGen
+from liiatools.datasets.social_work_workforce.SWFtools.analysis.seniority import (
+    seniority,
+    progressed,
+    seniority_forecast_5c,
+    seniority_forecast_04,
+)
+from liiatools.datasets.social_work_workforce.SWFtools.analysis.FTESum import (
+    FTESum,
+    FTESum_2020,
+)
 
 start = time.time()
 
 # Initialising logger (present throughout the program)
 AppLog.initialise()
 
 # CONVERSION STEPS
-#Recreate all folders present in 'cin' into 'flatfiles' adding a 'la_log' folder to store all runtime logs
+# Recreate all folders present in 'cin' into 'flatfiles' adding a 'la_log' folder to store all runtime logs
 work_path.check_flatfiles_folder()
 
 # Validate, process, and convert all XML files found in LA directories to CSV then merge them
 fop.process_all_input_files()
 
-""" For creating spreadsheets, tables and other files that will be stored in the request folder """
+# For creating spreadsheets, tables and other files that will be stored in the request folder
 
 
 # Outputs a file of extension 'xlsx' named 'growth_tables' (does not process any file, contains hardcoded values)
 growth_tables()
 # Creates a pivot table grouping data on Census year, age, gender, and LEA name; and summing on FTE and SWE
 pivotGen()
 
@@ -37,13 +43,13 @@
 progressed()
 seniority_forecast_5c()
 FTESum()
 FTESum_2020()
 seniority_forecast_04()
 
 end = time.time()
-total_time = round(end-start, 3)
+total_time = round(end - start, 3)
 
 print()
 print("Execution Time:", total_time)
 
 AppLog.log_footer(total_time)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import platform
 import sys
 import datetime
 from pathlib import Path
 from typing import List, Final, Dict
 
-import SWFtools.util.work_path as work_path
+import liiatools.datasets.social_work_workforce.SWFtools.util.work_path as work_path
 
 log_paths: Dict[str, str] = {}
 
 TIME_FORMAT_FILE_NAME: Final[str] = "%d_%m_%Y_%H_%M_%S"
 TIME_FORMAT_LOG_ENTRY: Final[str] = "%d/%m/%Y at %H:%M:%S"
 
 OPERATING_SYSTEM: Final = platform.uname().system
@@ -19,37 +19,49 @@
 
 # Creates a log file for runtime logs and writes a log header into the file
 def initialise():
     time_start = datetime.datetime.now()
 
     # The log file will be stored in a dictionary for later use
     runtime_log_file_name = time_start.strftime(TIME_FORMAT_FILE_NAME) + ".txt"
-    log_paths["runtime"] = os.path.join(work_path.runtime_log_files, runtime_log_file_name)
+    log_paths["runtime"] = os.path.join(
+        work_path.runtime_log_files, runtime_log_file_name
+    )
 
     try:
         with open(log_paths["runtime"], "w") as file:
-            file.write("=" * 20 + '\n')
-            file.write(f'Log file created on: {time_start.strftime(TIME_FORMAT_LOG_ENTRY)}\n')
-            file.write(f'Operating System: {OPERATING_SYSTEM}\n')
-            file.write("=" * 20 + '\n')
+            file.write("=" * 20 + "\n")
+            file.write(
+                f"Log file created on: {time_start.strftime(TIME_FORMAT_LOG_ENTRY)}\n"
+            )
+            file.write(f"Operating System: {OPERATING_SYSTEM}\n")
+            file.write("=" * 20 + "\n")
     except Exception as e:
-        print("A critical error occurred when attempting to create and write into runtime log file.\nError message:\n")
+        print(
+            "A critical error occurred when attempting to create and write into runtime log file.\nError message:\n"
+        )
         print(e)
-        print('')
+        print("")
         sys.exit("The program closed after error occurred at runtime.")
 
 
-def log_section_header(log_text: str, log_dir_name: str = "runtime", console_output: bool = False):
-    thick_line = '=' * 5
-    log_text = f'# {thick_line} {log_text} {thick_line} #'
+def log_section_header(
+    log_text: str, log_dir_name: str = "runtime", console_output: bool = False
+):
+    thick_line = "=" * 5
+    log_text = f"# {thick_line} {log_text} {thick_line} #"
     log(log_text, log_dir_name, console_output)
 
 
 # Writes text into a log file that corresponds to the log id passed
-def log(log_text: str | List[str], log_dir_name: str = "runtime", console_output: bool = False):
+def log(
+    log_text: str | List[str],
+    log_dir_name: str = "runtime",
+    console_output: bool = False,
+):
     """
     Writes text into the log file of an LA or to the application's runtime log file.
     :param log_text: A line or list of lines of text that will be written in the log file.
     :param log_dir_name: Directory name of the LA as it appears in the CIN folder. This will be used as a log id.
     If no value is passed it will write to the applications log file ('runtime')
 
     :param console_output: If it is set to 'True' then the passed text will also be printed to console. 'False' by default.
@@ -58,60 +70,81 @@
     time_stamp = datetime.datetime.now()
     entry_time_stamp = time_stamp.strftime(TIME_FORMAT_LOG_ENTRY)
 
     try:
         # If a log file was created then it's id can be found inside log_files dictionary as a key
         if log_dir_name in log_paths:
             if console_output:
-                __write_to_log_file_verbose(log_text, entry_time_stamp, 'a', log_paths[log_dir_name])
+                __write_to_log_file_verbose(
+                    log_text, entry_time_stamp, "a", log_paths[log_dir_name]
+                )
             else:
-                __write_to_log_file(log_text, entry_time_stamp, 'a', log_paths[log_dir_name])
+                __write_to_log_file(
+                    log_text, entry_time_stamp, "a", log_paths[log_dir_name]
+                )
 
         # If log_id was not found in log_files dictionary, check if it matches to any LA directories and create
         # it in its respective directory
         elif work_path.is_la_directory(log_dir_name):
-            file_path = os.path.join(work_path.flatfile_folder, log_dir_name, 'la_log',
-                                     time_stamp.strftime(TIME_FORMAT_FILE_NAME) + ".txt")
+            file_path = os.path.join(
+                work_path.flatfile_folder,
+                log_dir_name,
+                "la_log",
+                time_stamp.strftime(TIME_FORMAT_FILE_NAME) + ".txt",
+            )
             log_paths[log_dir_name] = file_path
 
             if console_output:
-                __write_to_log_file_verbose(log_text, entry_time_stamp, 'w', log_paths[log_dir_name])
+                __write_to_log_file_verbose(
+                    log_text, entry_time_stamp, "w", log_paths[log_dir_name]
+                )
             else:
-                __write_to_log_file(log_text, entry_time_stamp, 'w', log_paths[log_dir_name])
+                __write_to_log_file(
+                    log_text, entry_time_stamp, "w", log_paths[log_dir_name]
+                )
 
     except Exception as e:
         print("An error occurred when writing into the log file.\nError message:\n")
         print(e)
 
 
-def __write_to_log_file(log_text: str | List[str], entry_time_stamp: str, mode: str, path: str):
+def __write_to_log_file(
+    log_text: str | List[str], entry_time_stamp: str, mode: str, path: str
+):
     multiple_lines = type(log_text) is list
 
     with open(path, mode) as file:
         if multiple_lines:
             for line in log_text:
-                file.write(f'[{entry_time_stamp}]: {line}\n')
+                file.write(f"[{entry_time_stamp}]: {line}\n")
         else:
-            file.write(f'[{entry_time_stamp}]: {log_text}\n')
+            file.write(f"[{entry_time_stamp}]: {log_text}\n")
 
 
-def __write_to_log_file_verbose(log_text: str | List[str], entry_time_stamp: str, mode: str, path: str):
+def __write_to_log_file_verbose(
+    log_text: str | List[str], entry_time_stamp: str, mode: str, path: str
+):
     multiple_lines = type(log_text) is list
 
     with open(path, mode) as file:
         if multiple_lines:
             for line in log_text:
-                file.write(f'[{entry_time_stamp}]: {line}\n')
-                print(f'[{entry_time_stamp}]: {line}')
+                file.write(f"[{entry_time_stamp}]: {line}\n")
+                print(f"[{entry_time_stamp}]: {line}")
         else:
-            file.write(f'[{entry_time_stamp}]: {log_text}\n')
-            print(f'[{entry_time_stamp}]: {log_text}')
+            file.write(f"[{entry_time_stamp}]: {log_text}\n")
+            print(f"[{entry_time_stamp}]: {log_text}")
 
 
 def log_footer(total_time: float):
     log_file_path = log_paths["runtime"]
 
-    text = ["=" * 20, 'Process executed successfully.',
-            f'Total time spent in seconds: {total_time}', f'Log file saved to: {log_file_path}',
-            f'File name: {Path(log_file_path).stem}', "="*20]
+    text = [
+        "=" * 20,
+        "Process executed successfully.",
+        f"Total time spent in seconds: {total_time}",
+        f"Log file saved to: {log_file_path}",
+        f"File name: {Path(log_file_path).stem}",
+        "=" * 20,
+    ]
 
     log(text)
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 import sys
+import os
+import liiatools.datasets.social_work_workforce.SWFtools.util.AppLogs as AppLogs
 
-import SWFtools.util.AppLogs as AppLogs
 # Setting the paths to work and executing and using the scripts
 
-import os
-
 # Define filepaths
-main_folder = r'/file_directories/'
+main_folder = r"/workspaces/liia-tools/liiatools/spec/social_work_workforce"
 
-# CIN Census files must be in one "LA" folder per LA, in the cin_folder
-cin_folder = os.path.join(main_folder, 'cin')
+# CSWW files must be in one "LA" folder per LA, in the cssw_folder
+csww_folder = os.path.join(main_folder, "samples/csww")
+# print (f"csww_folder is {csww_folder}")
 
 # Flat files
-flatfile_folder = os.path.join(main_folder, 'flatfiles')
+flatfile_folder = os.path.join(main_folder, "samples/flatfiles")
 
 # Outputs
-output_folder = os.path.join(main_folder, 'outputs')
+output_folder = os.path.join(main_folder, "samples/outputs")
 
 # Chris requests folder
-request = os.path.join(main_folder, 'request')
+request = os.path.join(main_folder, "samples/request")
 
 # Workforce XML schema
-XML_SCHEMA = os.path.join('spec', 'wf_xmlschema.xsd')
+XML_SCHEMA = os.path.join(main_folder, "social_work_workforce_2022.xsd")
 
 # Runtime log files
-runtime_log_files = os.path.join(main_folder, 'log_files')
+runtime_log_files = os.path.join(main_folder, "samples/log_files")
 
 # Local Authority directories
-la_directories = [folder for folder in os.scandir(cin_folder) if os.path.isdir(folder)]
+la_directories = [folder for folder in os.scandir(csww_folder) if os.path.isdir(folder)]
 
 
 def check_flatfiles_folder():
     """
-    Checks that the 'flatfiles' folder contains all directories that are present in 'cin' folder and creates them if
+    Checks that the 'flatfiles' folder contains all directories that are present in 'csww' folder and creates them if
     they are not present.
     :return: None
     """
     total_dirs = len(la_directories)
     checked_dirs = 0
-    AppLogs.log(f'Checking {total_dirs} directories...', console_output=True)
+    AppLogs.log(f"Checking {total_dirs} directories...", console_output=True)
 
     for directory in la_directories:
         la_flat_files_directory = os.path.join(flatfile_folder, directory.name)
 
         if os.path.exists(la_flat_files_directory):
-            AppLogs.log(f'{directory.name} - Directory already exists', console_output=True)
+            AppLogs.log(
+                f"{directory.name} - Directory already exists", console_output=True
+            )
         # If the folder does not exist, create it and add a log folder called 'la_log'
         else:
             try:
                 os.mkdir(la_flat_files_directory)
 
                 la_log_file_directory = os.path.join(la_flat_files_directory, "la_log")
                 os.mkdir(la_log_file_directory)
 
-                AppLogs.log(f'Created directory: {directory}', console_output=True)
+                AppLogs.log(f"Created directory: {directory}", console_output=True)
             except PermissionError as pe:
-                AppLogs.log(f'PERMISSION ERROR!\n{pe}', console_output=True)
+                AppLogs.log(f"PERMISSION ERROR!\n{pe}", console_output=True)
 
-                print('')
+                print("")
                 sys.exit("The program closed after error occurred at runtime.")
 
         checked_dirs = checked_dirs + 1
-        AppLogs.log(f'Checked {checked_dirs} of {total_dirs} directories.')
+        AppLogs.log(f"Checked {checked_dirs} of {total_dirs} directories.")
 
 
 def is_la_directory(name: str) -> bool:
     for d in la_directories:
         if d.name == name:
             return True
```

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_cli.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/csww_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_main_functions.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/csww_main_functions.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/sample_data.py` & `liiatools-0.1.5.3/liiatools/datasets/social_work_workforce/sample_data.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/annex_a/annex-a-merge.yml` & `liiatools-0.1.5.3/liiatools/spec/annex_a/annex-a-merge.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/annex_a/data-map.yml` & `liiatools-0.1.5.3/liiatools/spec/annex_a/data-map.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/annex_a/la-agg.yml` & `liiatools-0.1.5.3/liiatools/spec/annex_a/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/annex_a/pan-agg.yml` & `liiatools-0.1.5.3/liiatools/spec/annex_a/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/annex_a/samples/Annex_A.xlsx` & `liiatools-0.1.5.3/liiatools/spec/annex_a/samples/Annex_A.xlsx`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2017.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2017.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2018.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2018.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2019.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2019.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2020.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2020.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2021.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2021.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2022.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2022.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2023.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2023.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2024.xsd` & `liiatools-0.1.5.3/liiatools/spec/cin_census/CIN_schema_2024.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/agg.yml` & `liiatools-0.1.5.3/liiatools/spec/cin_census/agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/cin_census/samples/cin-2022.xml` & `liiatools-0.1.5.3/liiatools/spec/cin_census/samples/cin-2022.xml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/common/LA-codes.yml` & `liiatools-0.1.5.3/liiatools/spec/common/LA-codes.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2017.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2017.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2018.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2018.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2019.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2019.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2020.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2020.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2021.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2021.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2022.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2022.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2023.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2023.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2024.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/SSDA903_schema_2024.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/la-agg.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/pan-agg.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/s903/sufficiency.yml` & `liiatools-0.1.5.3/liiatools/spec/s903/sufficiency.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd` & `liiatools-0.1.5.3/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.2/pyproject.toml` & `liiatools-0.1.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liiatools"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance"
 authors = [
     "Michael Hanks <michael.hanks@socialfinance.org.uk>",
     "Patrick Troy <patrick.troy@socialfinance.org.uk>",
     "Céline Gross <celine.m.gross@gmail.com>",
     "Kaj Siebert <kaj@k-si.com>",
     "Matthew Pugh <matthew.pugh@socialfinance.org.uk>"
@@ -24,14 +24,15 @@
 dacite = "^1.6.0"
 XlsxWriter = "^3.0.3"
 pandas = "^1.4.2"
 openpyxl = "^3.0.9"
 xlrd = "^2.0.1"
 click-log = "^0.4.0"
 cchardet = "2.1.7"
+python-decouple = "^3.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 coverage = "^6.3.2"
 safety = "^1.10.3"
 black = "^22.1.0"
 flake8 = "^4.0.1"
```

### Comparing `liiatools-0.1.5.2/PKG-INFO` & `liiatools-0.1.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liiatools
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance
 License: MIT
 Author: Michael Hanks
 Author-email: michael.hanks@socialfinance.org.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,12 +17,13 @@
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: more-itertools (>=8.12.0,<9.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
+Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: regex (>=2022.4.24,<2023.0.0)
 Requires-Dist: sfdata-stream-parser (==0.4.1)
 Requires-Dist: tablib[cli,xlsx] (>=3.2.0,<4.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Requires-Dist: xmlschema (>=1.10.0,<2.0.0)
```

