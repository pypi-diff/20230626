# Comparing `tmp/opensafely-cohort-extractor-1.85.0.tar.gz` & `tmp/opensafely-cohort-extractor-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensafely-cohort-extractor-1.85.0.tar", last modified: Mon Jun 26 12:17:35 2023, max compression
+gzip compressed data, was "dist/opensafely-cohort-extractor-1.9.0.tar", last modified: Tue Nov  3 15:43:23 2020, max compression
```

## Comparing `opensafely-cohort-extractor-1.85.0.tar` & `opensafely-cohort-extractor-1.9.0.tar`

### file list

```diff
@@ -1,75 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.081712 opensafely-cohort-extractor-1.85.0/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 12:17:35.081712 opensafely-cohort-extractor-1.85.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.073712 opensafely-cohort-extractor-1.85.0/cohortextractor/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/codelistlib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34188 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/cohortextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.073712 opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/date_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    67375 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/emis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/expectation_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/mssql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/ons_cis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   135816 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/patients.py
--rw-r--r--   0 runner    (1001) docker     (123)    36662 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/process_covariate_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/study_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/therapeutics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   150004 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/tpp_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/trino_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/uk_population_bands_2018.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/update_custom_medication_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/update_vmp_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/cohortextractor/validate_dummy_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.077712 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-26 12:17:35.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 12:17:34.000000 opensafely-cohort-extractor-1.85.0/opensafely_cohort_extractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:17:35.081712 opensafely-cohort-extractor-1.85.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.081712 opensafely-cohort-extractor-1.85.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:35.081712 opensafely-cohort-extractor-1.85.0/tests/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/emis_backend_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_codelistlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_cohortextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_date_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    95261 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_emis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    41331 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_expectation_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_study_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_therapeutics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   249861 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_tpp_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_trino_docker_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_trino_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_update_custom_medication_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_update_vmp_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/test_validate_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-06-26 12:17:30.000000 opensafely-cohort-extractor-1.85.0/tests/tpp_backend_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.723164 opensafely-cohort-extractor-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2020-11-03 15:43:23.723164 opensafely-cohort-extractor-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3037 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.719164 opensafely-cohort-extractor-1.9.0/cohortextractor/
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/VERSION
+-rw-r--r--   0 runner    (1001) docker     (116)      483 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2077 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/codelistlib.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    24712 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/cohortextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.719164 opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11195 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4473 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations_combine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4890 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations_extract.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7316 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/date_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42203 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/emis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5661 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/expectation_generators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6839 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1967 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/localrun.py
+-rw-r--r--   0 runner    (1001) docker     (116)      210 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/measure.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5165 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/mssql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22078 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/patients.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4111 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/presto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15501 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/process_covariate_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3184 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/remotejobs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13952 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/study_definition.py
+-rw-r--r--   0 runner    (1001) docker     (116)    72753 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/tpp_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)      290 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/cohortextractor/uk_population_bands_2018.csv
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.719164 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1626 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-11-03 15:43:23.000000 opensafely-cohort-extractor-1.9.0/opensafely_cohort_extractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-03 15:43:23.723164 opensafely-cohort-extractor-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      857 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.719164 opensafely-cohort-extractor-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      317 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:23.719164 opensafely-cohort-extractor-1.9.0/tests/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7261 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1568 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations_combine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5345 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations_extract.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7930 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/emis_backend_setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2277 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_codelistlib.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1115 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_cohortextractor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1234 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_date_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    53654 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_emis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27334 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_expectation_generators.py
+-rw-r--r--   0 runner    (1001) docker     (116)      840 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1666 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4547 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_study_definition.py
+-rw-r--r--   0 runner    (1001) docker     (116)   102187 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/test_tpp_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19469 2020-11-03 15:43:21.000000 opensafely-cohort-extractor-1.9.0/tests/tpp_backend_setup.py
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/cohortextractor.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/cohortextractor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 #!/usr/bin/env python3
 
 """A cross-platform script to build cohorts, run models, build and
 start a notebook, open a web browser on the correct port, and handle
 shutdowns gracefully
 """
-import base64
+import cohortextractor
+from collections import defaultdict
 import csv
-import datetime
+import glob
+import logging
 import importlib
 import os
-import pathlib
 import re
+import requests
 import sys
-import traceback
-from argparse import ArgumentParser
-from collections import defaultdict
-from io import BytesIO
 
+import base64
+from io import BytesIO
+from argparse import ArgumentParser
+from matplotlib import pyplot as plt
 import numpy as np
 import pandas
-import seaborn as sns
-import structlog
+from pandas.api.types import is_categorical_dtype
+from pandas.api.types import is_bool_dtype
+from pandas.api.types import is_datetime64_dtype
+from pandas.api.types import is_numeric_dtype
 import yaml
-from matplotlib import pyplot as plt
-from pandas.api.types import (
-    is_bool_dtype,
-    is_categorical_dtype,
-    is_datetime64_dtype,
-    is_numeric_dtype,
-)
 
-import cohortextractor
-from cohortextractor.exceptions import DummyDataValidationError, ValidationError
-from cohortextractor.update_custom_medication_dictionary import (
-    update_custom_medication_dictionary,
-)
-from cohortextractor.update_vmp_mapping import update_vmp_mapping
-
-from .log_utils import log_execution_time, log_stats
+import datetime
+import seaborn as sns
+from prettytable import PrettyTable
 
-logger = structlog.get_logger()
+from cohortextractor.localrun import localrun
 
 notebook_tag = "opencorona-research"
 target_dir = "/home/app/notebook"
 
 
-SUPPORTED_FILE_FORMATS = ["csv", "csv.gz", "feather", "dta", "dta.gz"]
-EXTENSION_REGEX = "|".join(map(re.escape, SUPPORTED_FILE_FORMATS))
-
-
 def show_exception_timestamp(*args):
     """
     Output a timestamp before any exception traceback which can be useful when
     debugging
     """
     timestamp = datetime.datetime.now(datetime.timezone.utc).strftime(
         "%Y-%m-%d %H:%M:%S UTC"
@@ -134,125 +122,66 @@
         msg = "This command expects the following relative paths to exist: {}"
         raise RuntimeError(msg.format(", ".join(missing_paths)))
 
 
 def generate_cohort(
     output_dir,
     expectations_population,
-    dummy_data_file,
     selected_study_name=None,
     index_date_range=None,
     skip_existing=False,
-    output_format=SUPPORTED_FILE_FORMATS[0],
-    output_name=None,
-    params=(),
 ):
     preflight_generation_check()
     study_definitions = list_study_definitions()
     if selected_study_name and selected_study_name != "all":
         for study_name, suffix in study_definitions:
             if study_name == selected_study_name:
                 study_definitions = [(study_name, suffix)]
                 break
-    if dummy_data_file and len(study_definitions) > 1:
-        msg = "You can only provide dummy data for a single study definition"
-        raise DummyDataValidationError(msg)
-    if output_name and len(study_definitions) > 1:
-        raise ValidationError(
-            "You can only use the --output-file argument with a single study definition"
-        )
     for study_name, suffix in study_definitions:
-        with log_execution_time(
-            logger,
-            description="generate_cohort",
-            study_definition=study_name,
-            index_date="all",
-        ):
-            _generate_cohort(
-                output_dir,
-                study_name,
-                suffix if not output_name else "",
-                expectations_population,
-                dummy_data_file,
-                index_date_range=index_date_range,
-                skip_existing=skip_existing,
-                output_format=output_format,
-                output_name=output_name or "input",
-                params=params,
-            )
+        print(f"Generating cohort for {study_name}...")
+        _generate_cohort(
+            output_dir,
+            study_name,
+            suffix,
+            expectations_population,
+            index_date_range=index_date_range,
+            skip_existing=skip_existing,
+        )
 
 
 def _generate_cohort(
     output_dir,
     study_name,
     suffix,
     expectations_population,
-    dummy_data_file,
     index_date_range=None,
     skip_existing=False,
-    output_format=SUPPORTED_FILE_FORMATS[0],
-    output_name="input",
-    params=(),
 ):
-    logger.info(
-        f"Generating cohort for {study_name} in {output_dir}",
-    )
-    logger.debug(
-        "args:",
-        suffix=suffix,
-        expectations_population=expectations_population,
-        dummy_data_file=dummy_data_file,
-        index_date_range=index_date_range,
-        skip_existing=skip_existing,
-        output_format=output_format,
-    )
-
-    study = load_study_definition(study_name, params=params)
+    print("Running. Please wait...")
+    study = load_study_definition(study_name)
 
     os.makedirs(output_dir, exist_ok=True)
-
-    index_dates = _generate_date_range(index_date_range)
-    log_stats(logger, index_date_count=len(index_dates) if index_date_range else 0)
-    if index_date_range:
-        log_stats(logger, min_index_date=index_dates[-1], max_index_date=index_dates[0])
-
-    # record if we've logged the SQL for this generate_cohort run
-    # For subsequent runs, we log the timing and the first line of the SQL only, since
-    # the only difference should be the index date
-    sql_logged = False
-    for index_date in index_dates:
-        log_kwargs = dict(description="generate_cohort", study_definition=study_name)
+    for index_date in _generate_date_range(index_date_range):
         if index_date is not None:
-            log_kwargs.update(index_date=index_date)
-        with log_execution_time(logger, **log_kwargs):
-            if index_date is not None:
-                logger.info(f"Setting index_date to {index_date}")
-                study.set_index_date(index_date)
-                if sql_logged:
-                    study.set_sql_logging(truncate=True)
-                date_suffix = f"_{index_date}"
-            else:
-                date_suffix = ""
-            # If this is changed then the regex in `_generate_measures()`
-            # must be updated
-            output_file = (
-                f"{output_dir}/{output_name}{suffix}{date_suffix}.{output_format}"
+            study.set_index_date(index_date)
+            date_suffix = f"_{index_date}"
+        else:
+            date_suffix = ""
+        # If this is changed then the glob pattern in `_generate_measures()`
+        # must be updated
+        output_file = f"{output_dir}/input{suffix}{date_suffix}.csv"
+        if skip_existing and os.path.exists(output_file):
+            print(f"Not regenerating pre-existing file at {output_file}")
+        else:
+            study.to_csv(
+                output_file,
+                expectations_population=expectations_population,
             )
-            if skip_existing and os.path.exists(output_file):
-                logger.info(f"Not regenerating pre-existing file at {output_file}")
-            else:
-                study.to_file(
-                    output_file,
-                    expectations_population=expectations_population,
-                    dummy_data_file=dummy_data_file,
-                )
-                logger.info(
-                    f"Successfully created cohort and covariates at {output_file}"
-                )
-                sql_logged = True
+            print(f"Successfully created cohort and covariates at {output_file}")
 
 
 def _generate_date_range(date_range_str):
     # Bail out with an "empty" range: this means we don't need separate
     # codepaths to handle the range, single date, and no date supplied cases
     if not date_range_str:
         return [None]
@@ -261,17 +190,14 @@
         raise ValueError(
             f"Invalid date range '{date_range_str}': end cannot be earlier than start"
         )
     dates = []
     while start <= end:
         dates.append(start.isoformat())
         start = _increment_date(start, period)
-    # The latest data is generally more interesting/useful so we may as well
-    # extract that first
-    dates.reverse()
     return dates
 
 
 def _parse_date_range(date_range_str):
     period = "month"
     if " to " in date_range_str:
         start, end = date_range_str.split(" to ", 1)
@@ -308,164 +234,100 @@
             return date.replace(month=date.month + 1)
         else:
             return date.replace(month=1, year=date.year + 1)
     else:
         raise ValueError(f"Unknown time period '{period}'")
 
 
-def generate_measures(
-    output_dir,
-    selected_study_name=None,
-    skip_existing=False,
-    params=(),
-):
+def generate_measures(output_dir, selected_study_name=None, skip_existing=False):
     preflight_generation_check()
     study_definitions = list_study_definitions()
     if selected_study_name and selected_study_name != "all":
         for study_name, suffix in study_definitions:
             if study_name == selected_study_name:
                 study_definitions = [(study_name, suffix)]
                 break
-
     for study_name, suffix in study_definitions:
-        with log_execution_time(
-            logger,
-            description="generate_measures",
-            study_definition=study_name,
-            input_file="all",
-        ):
-            _generate_measures(
-                output_dir,
-                study_name,
-                suffix,
-                skip_existing=skip_existing,
-                params=params,
-            )
+        print(f"Generating measure for {study_name}...")
+        _generate_measures(output_dir, study_name, suffix, skip_existing=skip_existing)
 
 
-def _generate_measures(
-    output_dir,
-    study_name,
-    suffix,
-    skip_existing=False,
-    params=(),
-):
-    logger.info(
-        f"Generating measure for {study_name} in {output_dir}",
-    )
-    logger.debug("args", suffix=suffix, skip_existing=skip_existing)
-    measures = load_study_definition(study_name, value="measures", params=params)
+def _generate_measures(output_dir, study_name, suffix, skip_existing=False):
+    print("Running. Please wait...")
+    measures = load_study_definition(study_name, value="measures")
     measure_outputs = defaultdict(list)
-    filename_re = re.compile(rf"^input{re.escape(suffix)}.+\.({EXTENSION_REGEX})$")
-
-    log_stats(logger, measures_count=len(measures))
-    for file in os.listdir(output_dir):
-        if not filename_re.match(file):
-            continue
+    for file in glob.glob(f"{output_dir}/input{suffix}*.csv"):
         date = _get_date_from_filename(file)
         if date is None:
             continue
-        filepath = os.path.join(output_dir, file)
-        logger.info(f"Calculating measures for {filepath}")
-        date_string_for_logs = date.strftime("%Y-%m-%d")
-        with log_execution_time(
-            logger,
-            description="generate_measures",
-            input_file=filepath,
-            date=date_string_for_logs,
-            study_definition=study_name,
-        ):
-            patient_df = None
-            for measure in measures:
-                logger.info(f"Calculating {measure.id}")
-                output_file = f"{output_dir}/measure_{measure.id}_{date}.csv"
-                measure_outputs[measure.id].append(output_file)
-                if skip_existing and os.path.exists(output_file):
-                    logger.info(f"Not generating pre-existing file {output_file}")
-                    continue
-                # We do this lazily so that if all corresponding output files
-                # already exist we can avoid loading the patient data entirely
-                if patient_df is None:
-                    logger.info(f"Loading patient data from {filepath}")
-                    with log_execution_time(
-                        logger,
-                        description="Load patient dataframe for measures",
-                        input_file=filepath,
-                        date=date_string_for_logs,
-                    ):
-                        patient_df = _load_dataframe_for_measures(filepath, measures)
-                        log_stats(
-                            logger,
-                            dataframe="patient_df",
-                            measure_id=measure.id,
-                            date=date_string_for_logs,
-                            memory=patient_df.memory_usage(deep=True).sum(),
-                        )
-                with log_execution_time(
-                    logger,
-                    description="Calculate measure",
-                    measure_id=measure.id,
-                    date=date_string_for_logs,
-                ):
-                    measure_df = measure.calculate(patient_df, _report)
-                log_stats(
-                    logger,
-                    dataframe="measure_df",
-                    measure_id=measure.id,
-                    date=date_string_for_logs,
-                    memory=measure_df.memory_usage(deep=True).sum(),
-                )
-                measure_df.to_csv(output_file, index=False)
-                logger.info(f"Created measure output at {output_file}")
+        patient_df = None
+        for measure in measures:
+            output_file = f"{output_dir}/measure_{measure.id}_{date}.csv"
+            measure_outputs[measure.id].append(output_file)
+            if skip_existing and os.path.exists(output_file):
+                print(f"Not generating pre-existing file {output_file}")
+                continue
+            # We do this lazily so that if all corresponding output files
+            # already exist we can avoid loading the patient data entirely
+            if patient_df is None:
+                patient_df = _load_csv_for_measures(file, measures)
+            measure_df = _calculate_measure_df(patient_df, measure)
+            measure_df.to_csv(output_file, index=False)
+            print(f"Created measure output at {output_file}")
     if not measure_outputs:
-        logger.warn(
+        print(
             "No matching output files found. You may need to first run:\n"
             "  cohortextractor generate_cohort --index-date-range ..."
         )
         return
     for measure in measures:
         output_file = f"{output_dir}/measure_{measure.id}.csv"
         _combine_csv_files_with_dates(output_file, measure_outputs[measure.id])
-        logger.info(f"Combined measure output for all dates in {output_file}")
+        print(f"Combined measure output for all dates in {output_file}")
+
+
+def _calculate_measure_df(patient_df, measure):
+    if measure.group_by:
+        measure_df = patient_df[
+            [measure.numerator, measure.denominator, measure.group_by]
+        ]
+        measure_df = measure_df.groupby(measure.group_by).sum()
+        measure_df = measure_df.reset_index()
+    else:
+        measure_df = patient_df[[measure.numerator, measure.denominator]]
+    measure_df["value"] = (
+        measure_df[measure.numerator] / measure_df[measure.denominator]
+    )
+    return measure_df
 
 
 def _get_date_from_filename(filename):
-    match = re.search(rf"_(\d\d\d\d\-\d\d\-\d\d)\.({EXTENSION_REGEX})$", filename)
+    match = re.search(r"_(\d\d\d\d\-\d\d\-\d\d)\.csv$", filename)
     return datetime.date.fromisoformat(match.group(1)) if match else None
 
 
-def _load_dataframe_for_measures(filename, measures):
+def _load_csv_for_measures(file, measures):
     """
-    Given a file name and a list of measures, load the file into a Pandas
+    Given a CSV file name and a list of measures, load the file into a Pandas
     dataframe with types as appropriate for the supplied measures
     """
-    filename = str(filename)
     numeric_columns = set()
     group_by_columns = set()
     for measure in measures:
         numeric_columns.update([measure.numerator, measure.denominator])
-        group_by_columns.update(measure.group_by)
+        if measure.group_by:
+            group_by_columns.add(measure.group_by)
     # This is a special column which we don't load from the CSV but whose value
     # is always set to 1 for every row
-    numeric_columns.discard(measure.POPULATION_COLUMN)
-    group_by_columns.discard(measure.POPULATION_COLUMN)
+    numeric_columns.discard("population")
     dtype = {col: "category" for col in group_by_columns}
     for col in numeric_columns:
         dtype[col] = "float64"
-    if filename.endswith(".csv") or filename.endswith(".csv.gz"):
-        df = pandas.read_csv(
-            filename, dtype=dtype, usecols=list(dtype.keys()), keep_default_na=False
-        )
-    elif filename.endswith(".feather"):
-        df = pandas.read_feather(filename, columns=list(dtype.keys()))
-    elif filename.endswith(".dta") or filename.endswith(".dta.gz"):
-        df = pandas.read_stata(filename, columns=list(dtype.keys()))
-    else:
-        raise RuntimeError(f"Unsupported file format: {filename}")
-    df[measure.POPULATION_COLUMN] = 1
+    df = pandas.read_csv(file, dtype=dtype, usecols=list(dtype.keys()))
+    df["population"] = 1
     return df
 
 
 def _combine_csv_files_with_dates(filename, input_files):
     """
     Takes a list of CSV files which have dates in their filenames and combines
     them into a single CSV file with an additional "date" column indicating the
@@ -486,24 +348,14 @@
                     raise RuntimeError(
                         f"Files {input_files[0]} and {file} have different headers"
                     )
                 for row in reader:
                     writer.writerow(row + [date])
 
 
-# Used for reporting events to users. We may introduce a dedicated
-# mechanism for this eventually, but for now it just uses the logging
-# system.
-reporter = structlog.get_logger("cohortextactor.reporter")
-
-
-def _report(msg):
-    reporter.info(msg)
-
-
 def make_cohort_report(input_dir, output_dir):
     for study_name, suffix in list_study_definitions():
         _make_cohort_report(input_dir, output_dir, study_name, suffix)
 
 
 def _make_cohort_report(input_dir, output_dir, study_name, suffix):
     study = load_study_definition(study_name)
@@ -532,14 +384,15 @@
                     make_chart(name, df[name] > 0, bool)
                 )
             )
         descriptives.loc["values", name] = main_chart
         descriptives.loc["nulls", name] = empty_values_chart
 
     with open(f"{output_dir}/descriptives{suffix}.html", "w") as f:
+
         f.write(
             """<html>
 <head>
   <style>
     table {
       text-align: left;
       position: relative;
@@ -562,35 +415,57 @@
   </style>
 </head>
 <body>"""
         )
 
         f.write(descriptives.to_html(escape=False, na_rep="", justify="left", border=0))
         f.write("</body></html>")
-    logger.info(f"Created cohort report at {output_dir}/descriptives{suffix}.html")
+    print(f"Created cohort report at {output_dir}/descriptives{suffix}.html")
+
 
+def update_codelists():
+    base_path = os.path.join(os.getcwd(), "codelists")
 
-def dump_cohort_sql(study_definition, params=()):
-    study = load_study_definition(study_definition, params=params)
+    # delete all existing codelists
+    for path in glob.glob(os.path.join(base_path, "*.csv")):
+        os.unlink(path)
+
+    with open(os.path.join(base_path, "codelists.txt")) as f:
+        for line in f:
+            line = line.strip()
+            if not line:
+                continue
+
+            print(line)
+            project_id, codelist_id, version = line.split("/")
+            url = f"https://codelists.opensafely.org/codelist/{project_id}/{codelist_id}/{version}/download.csv"
+
+            rsp = requests.get(url)
+            rsp.raise_for_status()
+
+            with open(
+                os.path.join(base_path, f"{project_id}-{codelist_id}.csv"), "w"
+            ) as f:
+                f.write(rsp.text)
+
+
+def dump_cohort_sql(study_definition):
+    study = load_study_definition(study_definition)
     print(study.to_sql())
 
 
-def dump_study_yaml(study_definition, params=()):
-    study = load_study_definition(study_definition, params=params)
+def dump_study_yaml(study_definition):
+    study = load_study_definition(study_definition)
     print(yaml.dump(study.to_data()))
 
 
-def load_study_definition(name, value="study", params=()):
+def load_study_definition(name, value="study"):
     sys.path.extend([relative_dir(), os.path.join(relative_dir(), "analysis")])
     # Avoid creating __pycache__ files in the analysis directory
     sys.dont_write_bytecode = True
-    # Set any supplied "<key>=<value>" parameters on the global `params` dict
-    cohortextractor.params.clear()
-    cohortextractor.params.update(params)
-    logger.info(f"Setting cohortextractor.params to: {cohortextractor.params}")
     return getattr(importlib.import_module(name), value)
 
 
 def list_study_definitions(ignore_errors=False):
     pattern = re.compile(r"^(study_definition(_\w+)?)\.py$")
     matches = []
     try:
@@ -607,29 +482,15 @@
             suffix = match.group(2) or ""
             matches.append((name, suffix))
     if not matches and not ignore_errors:
         raise RuntimeError(f"No study definitions found in {relative_dir()}")
     return matches
 
 
-def check_maintenance(current_mode):
-    # avoid circular imports
-    from cohortextractor.study_definition import StudyDefinition
-
-    db_url = os.environ["DATABASE_URL"]
-    backend_cls = StudyDefinition.get_backend_for_database_url(db_url)
-    backend = backend_cls(db_url, None)
-
-    if backend.in_maintenance_mode(current_mode):
-        # Note: logs are output on stderr, so this should be the only output on
-        # stdout
-        print("db-maintenance")
-
-
-def main(args=None):
+def main():
     parser = ArgumentParser(
         description="Generate cohorts and run models in openSAFELY framework. "
     )
     # Cohort parser options
     parser.add_argument("--version", help="Display version", action="store_true")
     parser.add_argument(
         "--verbose", help="Show extra logging info", action="store_true"
@@ -639,14 +500,54 @@
         "generate_cohort", help="Generate cohort"
     )
     generate_cohort_parser.set_defaults(which="generate_cohort")
     generate_measures_parser = subparsers.add_parser(
         "generate_measures", help="Generate measures from cohort data"
     )
     generate_measures_parser.set_defaults(which="generate_measures")
+    run_parser = subparsers.add_parser("run", help="Run action from project.yaml")
+    run_parser.set_defaults(which="run")
+
+    run_parser.add_argument(
+        "db",
+        help="Database to run against",
+        choices=["full", "slice", "dummy"],
+        type=str,
+    )
+    run_parser.add_argument(
+        "action",
+        help="Action to execute",
+        type=str,
+    )
+    run_parser.add_argument(
+        "backend",
+        help="Backend to execute against",
+        choices=["expectations", "tpp", "all"],
+        type=str,
+        default="all",
+    )
+
+    run_parser.add_argument(
+        "--medium-privacy-storage-base",
+        help="Location to store medium privacy data",
+    )
+    run_parser.add_argument(
+        "--high-privacy-storage-base",
+        help="Location to store high privacy data",
+    )
+    run_parser.add_argument(
+        "--force-run",
+        help="Force a new run for the action",
+        action="store_true",
+    )
+    run_parser.add_argument(
+        "--force-run-dependencies",
+        help="Force a new run for the action and all its dependencies (only when `--force-run` is also specified)",
+        action="store_true",
+    )
     cohort_report_parser = subparsers.add_parser(
         "cohort_report", help="Generate cohort report"
     )
     cohort_report_parser.set_defaults(which="cohort_report")
     cohort_report_parser.add_argument(
         "--input-dir",
         help="Location to look for input CSVs",
@@ -656,66 +557,40 @@
     cohort_report_parser.add_argument(
         "--output-dir",
         help="Location to store output CSVs",
         type=str,
         default="output",
     )
 
+    update_codelists_parser = subparsers.add_parser(
+        "update_codelists",
+        help="Update codelists, using specification at codelists/codelists.txt",
+    )
+    update_codelists_parser.set_defaults(which="update_codelists")
     dump_cohort_sql_parser = subparsers.add_parser(
         "dump_cohort_sql", help="Show SQL to generate cohort"
     )
     dump_cohort_sql_parser.add_argument(
         "--study-definition", help="Study definition name", type=str, required=True
     )
-    dump_cohort_sql_parser.add_argument(
-        "--param",
-        nargs="+",
-        action="append",
-        dest="params",
-        default=[],
-        help="Additional parameter to pass to study definition",
-    )
     dump_cohort_sql_parser.set_defaults(which="dump_cohort_sql")
     dump_study_yaml_parser = subparsers.add_parser(
         "dump_study_yaml", help="Show study definition as YAML"
     )
     dump_study_yaml_parser.set_defaults(which="dump_study_yaml")
     dump_study_yaml_parser.add_argument(
         "--study-definition", help="Study definition name", type=str, required=True
     )
-    dump_study_yaml_parser.add_argument(
-        "--param",
-        nargs="+",
-        action="append",
-        dest="params",
-        default=[],
-        help="Additional parameter to pass to study definition",
-    )
+
     # Cohort parser options
     generate_cohort_parser.add_argument(
         "--output-dir",
-        help="Location to store output files",
-        type=str,
-    )
-    generate_cohort_parser.add_argument(
-        "--output-format",
-        help=(
-            f"Output file format: {SUPPORTED_FILE_FORMATS[0]} (default),"
-            f" {', '.join(SUPPORTED_FILE_FORMATS[1:])}"
-        ),
+        help="Location to store output CSVs",
         type=str,
-        choices=SUPPORTED_FILE_FORMATS,
-    )
-    generate_cohort_parser.add_argument(
-        "--output-file",
-        help=(
-            f"Full path to output file, including directory and extension e.g. "
-            f"output/input.{SUPPORTED_FILE_FORMATS[0]}"
-        ),
-        type=pathlib.Path,
+        default="output",
     )
     generate_cohort_parser.add_argument(
         "--study-definition",
         help="Study definition to use",
         type=str,
         choices=["all"] + [x[0] for x in list_study_definitions(ignore_errors=True)],
         default="all",
@@ -733,48 +608,31 @@
         default="",
     )
     generate_cohort_parser.add_argument(
         "--skip-existing",
         help="Do not regenerate data if output file already exists",
         action="store_true",
     )
-    generate_cohort_parser.add_argument(
-        "--with-end-date-fix",
-        action="store_true",
-    )
-    generate_cohort_parser.add_argument(
-        "--param",
-        nargs="+",
-        action="append",
-        dest="params",
-        default=[],
-        help="Additional parameter to pass to study definition",
-    )
     cohort_method_group = generate_cohort_parser.add_mutually_exclusive_group()
     cohort_method_group.add_argument(
         "--expectations-population",
         help="Generate a dataframe from study expectations",
         type=int,
         default=0,
     )
     cohort_method_group.add_argument(
-        "--dummy-data-file",
-        help="Use dummy data from file",
-        type=pathlib.Path,
-    )
-    cohort_method_group.add_argument(
         "--database-url",
         help="Database URL to query (can be supplied as DATABASE_URL environment variable)",
         type=str,
     )
 
     # Measure generator parser options
     generate_measures_parser.add_argument(
         "--output-dir",
-        help="Location to store output files",
+        help="Location to store output CSVs",
         type=str,
         default="output",
     )
     generate_measures_parser.add_argument(
         "--study-definition",
         help="Study definition file containing measure definitions to use",
         type=str,
@@ -782,182 +640,82 @@
         default="all",
     )
     generate_measures_parser.add_argument(
         "--skip-existing",
         help="Do not regenerate measure if output file already exists",
         action="store_true",
     )
-    generate_measures_parser.add_argument(
-        "--param",
-        nargs="+",
-        action="append",
-        dest="params",
-        default=[],
-        help="Additional parameter to pass to study definition",
-    )
-
-    maintenance_parser = subparsers.add_parser(
-        "maintenance",
-        help="Report if backend db is currently performing maintenance",
-    )
-    maintenance_parser.set_defaults(which="maintenance")
-    maintenance_parser.add_argument(
-        "--database-url",
-        help="Database URL to query (can be supplied as DATABASE_URL environment variable)",
-    )
-    maintenance_parser.add_argument(
-        "--current-mode",
-        help="The current mode we think the database is in",
-        default="unknown",
-    )
-
-    update_vmp_mapping_parser = subparsers.add_parser(
-        "update_vmp_mapping",
-        help="Update VmpMapping table",
-    )
-    update_vmp_mapping_parser.set_defaults(which="update_vmp_mapping")
-
-    update_custom_medication_dictionary_parser = subparsers.add_parser(
-        "update_custom_medication_dictionary",
-        help="Update CustomMedicationDictionary table",
-    )
-    update_custom_medication_dictionary_parser.set_defaults(
-        which="update_custom_medication_dictionary"
-    )
-
-    options = parser.parse_args(sys.argv[1:] if args is None else args)
 
+    options = parser.parse_args()
+    if getattr(options, "force_run_dependencies", False) and not getattr(
+        options, "force_run", False
+    ):
+        parser.error("`--force-run-dependencies` requires `--force-run`")
     if options.version:
         print(f"v{cohortextractor.__version__}")
     elif not hasattr(options, "which"):
         parser.print_help()
     elif options.which == "generate_cohort":
         if options.database_url:
             os.environ["DATABASE_URL"] = options.database_url
         if options.temp_database_name:
             os.environ["TEMP_DATABASE_NAME"] = options.temp_database_name
-        if not (
-            options.expectations_population
-            or options.dummy_data_file
-            or os.environ.get("DATABASE_URL")
-        ):
+        if not options.expectations_population and not os.environ.get("DATABASE_URL"):
             parser.error(
                 "generate_cohort: error: one of the arguments "
-                "--expectations-population --dummy-data-file --database-url is required"
-            )
-        if options.output_file:
-            output_dir = options.output_file.parent
-            match = re.match(
-                rf"^(.+)\.({EXTENSION_REGEX})$", str(options.output_file.name)
-            )
-            if not match:
-                parser.error(
-                    f"generate_cohort: error: --output-file must have a supported "
-                    f"extension: {', '.join(SUPPORTED_FILE_FORMATS)}"
-                )
-            output_name = match.group(1)
-            output_format = match.group(2)
-            # It would be simpler if we could just insist that these other options
-            # weren't present, but job-runner adds `--output-dir` automatically so we
-            # can't do that.
-            if options.output_dir and options.output_dir != str(output_dir):
-                parser.error(
-                    f"generate_cohort: error: --output-dir '{options.output_dir}' "
-                    f"does not match directory in --output-file"
-                )
-            if options.output_format and options.output_format != output_format:
-                parser.error(
-                    f"generate_cohort: error: --output-format '{options.output_format}' "
-                    f"does not match format in --output-file"
-                )
-        else:
-            output_dir = options.output_dir or "output"
-            output_name = None
-            output_format = options.output_format or SUPPORTED_FILE_FORMATS[0]
-
-        try:
-            generate_cohort(
-                str(output_dir),
-                options.expectations_population,
-                options.dummy_data_file,
-                selected_study_name=options.study_definition,
-                index_date_range=options.index_date_range,
-                skip_existing=options.skip_existing,
-                output_format=output_format,
-                output_name=output_name,
-                params=dict_from_params(options.params),
+                "--expectations-population --database-url is required"
             )
-        except ValidationError as e:
-            print(f"{e.human_name}: {e}")
-            sys.exit(1)
-        except Exception as e:
-            # Checking for "DatabaseError" in the MRO means we can identify database errors without
-            # referencing a specific driver.  Both pymssql and presto/trino-python-client raise
-            # exceptions derived from a DatabaseError parent class
-
-            # Ignore errors which don't look like database errors
-            if "DatabaseError" not in str(e.__class__.mro()):
-                raise
-
-            traceback.print_exc()
-            # Exit with specific exit codes to help identify known issues
-            transient_errors = [
-                "Unexpected EOF from the server",
-                "DBPROCESS is dead or not enabled",
-            ]
-            if any(message in str(e) for message in transient_errors):
-                logger.error(f"Intermittent database error: {e}")
-                sys.exit(3)
-            if "Invalid object name 'CodedEvent_SNOMED'" in str(e):
-                logger.error(
-                    "CodedEvent_SNOMED table is currently not available.\n"
-                    "This is likely due to regular database maintenance."
-                )
-                sys.exit(4)
-            logger.error(f"Database error: {e}")
-            sys.exit(5)
-
+        generate_cohort(
+            options.output_dir,
+            options.expectations_population,
+            selected_study_name=options.study_definition,
+            index_date_range=options.index_date_range,
+            skip_existing=options.skip_existing,
+        )
     elif options.which == "generate_measures":
         generate_measures(
             options.output_dir,
             selected_study_name=options.study_definition,
             skip_existing=options.skip_existing,
-            params=dict_from_params(options.params),
         )
+    elif options.which == "run":
+        log_level = options.verbose and logging.DEBUG or logging.ERROR
+        result = localrun(
+            options.action,
+            options.backend,
+            options.db,
+            medium_privacy_storage_base=options.medium_privacy_storage_base,
+            high_privacy_storage_base=options.high_privacy_storage_base,
+            force_run=options.force_run,
+            force_run_dependencies=options.force_run_dependencies,
+            log_level=log_level,
+        )
+        if result:
+            print("Generated outputs:")
+            output = PrettyTable()
+            output.field_names = ["status", "path"]
+
+            for action in result:
+                for location in action["output_locations"]:
+                    output.add_row(
+                        [
+                            action["status_message"],
+                            location["relative_path"],
+                        ]
+                    )
+            print(output)
+        else:
+            print("Nothing to do")
+
     elif options.which == "cohort_report":
         make_cohort_report(options.input_dir, options.output_dir)
+    elif options.which == "update_codelists":
+        update_codelists()
+        print("Codelists updated. Don't forget to commit them to the repo")
     elif options.which == "dump_cohort_sql":
-        dump_cohort_sql(
-            options.study_definition, params=dict_from_params(options.params)
-        )
+        dump_cohort_sql(options.study_definition)
     elif options.which == "dump_study_yaml":
-        dump_study_yaml(
-            options.study_definition, params=dict_from_params(options.params)
-        )
-    elif options.which == "maintenance":
-        if options.database_url:
-            os.environ["DATABASE_URL"] = options.database_url
-        check_maintenance(options.current_mode)
-    elif options.which == "update_vmp_mapping":
-        update_vmp_mapping()
-    elif options.which == "update_custom_medication_dictionary":
-        update_custom_medication_dictionary()
-
-
-def dict_from_params(params):
-    # Arguments like this:
-    #
-    #     --param key1=value1 --param key2 = value2 --param key3= 'value 3'
-    #
-    # Are parsed by argpase into a list like this:
-    #
-    #     [["key1=value1"], ["key2", "=", "value2"], ["key3=", "value 3"]]
-    #
-    # We want to transform that into a dict like this:
-    #
-    #     {"key1": "value1", "key2": "value2", "key3: "value 3"}
-    #
-    return dict("".join(param_parts).partition("=")[::2] for param_parts in params)
+        dump_study_yaml(options.study_definition)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import csv
 import datetime
+from datetime import timedelta
 import os
 import random
 import tempfile
-from datetime import timedelta
 
 from cohortextractor.mssql_utils import mssql_dbapi_connection_from_url
-
-from .vaccinations_combine import add_patient_vaccination_dates
 from .vaccinations_extract import (
     patients_with_ages_and_practices_sql,
     vaccination_events_sql,
 )
+from .vaccinations_combine import add_patient_vaccination_dates
 
 
 class VaccinationsStudyDefinition:
     def __init__(
         self,
         #
         # This is the first date for which we need data. If the maximum age
@@ -97,16 +96,15 @@
         self.event_washout_period = event_washout_period
         self.vaccination_schedule = vaccination_schedule
         self.date_of_birth_range = self.get_date_of_birth_range(
             start_date, datetime.date.today(), get_registered_practice_at_months
         )
         self.database_url = os.environ.get("DATABASE_URL")
 
-    def to_file(self, filename, expectations_population=False):
-        assert str(filename).endswith(".csv")
+    def to_csv(self, filename, expectations_population=False):
         if expectations_population:
             self.write_dummy_data(filename, expectations_population)
         else:
             with tempfile.TemporaryDirectory() as tmpdir:
                 patients_filename = os.path.join(tmpdir, "patients.csv")
                 events_filename = os.path.join(tmpdir, "vaccination_events.csv")
                 self.extract_data(patients_filename, events_filename)
@@ -124,15 +122,15 @@
 
         -- -------------------------------------------------------------------
 
         -- Get vaccination events
         {events_sql};
         """
 
-    def to_dicts(self, convert_to_strings=True):
+    def to_dicts(self):
         raise NotImplementedError()
 
     def to_data(self):
         raise NotImplementedError()
 
     def get_date_of_birth_range(self, start_date, today, age_thresholds):
         """
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations_combine.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations_combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from collections import defaultdict
 import datetime
 import itertools
-from collections import defaultdict
 
 
 def add_patient_vaccination_dates(patients, vaccination_events, washout_period=0):
     patients_vaccinations = get_patient_vaccination_dates(
         vaccination_events, washout_period
     )
     joined = LeftJoinSortedRows(patients, patients_vaccinations, on="patient_id")
@@ -71,15 +71,15 @@
             vaccine2: [
               date_1,
               date_2,
               ...
             ],
         ]
     """
-    get_patient_id = lambda row: row["patient_id"]  # noqa
+    get_patient_id = lambda row: row["patient_id"]
     for patient_id, group in itertools.groupby(vaccination_events, key=get_patient_id):
         vaccine_dates = defaultdict(list)
         for row in group:
             vaccine_name = row["vaccine_name"]
             date_given = datetime.date.fromisoformat(row["date_given"])
             vaccine_dates[vaccine_name].append(date_given)
         yield patient_id, vaccine_dates.items()
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/dashboards/vaccinations_extract.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/dashboards/vaccinations_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cohortextractor.tpp_backend import codelist_to_sql, quote
+from cohortextractor.tpp_backend import quote, codelist_to_sql
 
 
 def patients_with_ages_and_practices_sql(date_of_birth_range, age_thresholds):
     """
     Retrieves patients with date of birth (rounded to start of month) plus the
     practice pseudo IDs to which they were registered in the months where they
     hit the defined age thresholds (measured in months).
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/emis_backend.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/tpp_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,302 +1,300 @@
 import datetime
-import math
+import enum
+import hashlib
 import os
 import re
 import uuid
 
-import structlog
-
-from .codelistlib import codelist
-from .csv_utils import is_csv_filename, write_rows_to_csv
-from .date_expressions import TrinoDateFormatter
 from .expressions import format_expression
-from .log_utils import LoggingDatabaseConnection, log_execution_time, log_stats
-from .pandas_utils import dataframe_from_rows, dataframe_to_file
-from .trino_utils import trino_connection_from_url
+from .mssql_utils import (
+    mssql_dbapi_connection_from_url,
+    mssql_connection_params_from_url,
+    mssql_table_to_csv,
+)
 
-logger = structlog.get_logger()
-sql_logger = structlog.get_logger("cohortextractor.sql")
 
 # Characters that are safe to interpolate into SQL (see
 # `placeholders_and_params` below)
 safe_punctation = r" _.-+/()"
 SAFE_CHARS_RE = re.compile(f"^[a-zA-Z0-9{re.escape(safe_punctation)}]+$")
 
-PATIENT_TABLE = "patient_all_orgs_v2"
-MEDICATION_TABLE = "medication_all_orgs_v2"
-OBSERVATION_TABLE = "observation_all_orgs_v2"
-IMMUNISATIONS_TABLE = "immunisation_all_orgs_v2"
-ICNARC_TABLE = "icnarc_view"
-ONS_TABLE = "ons_view"
-CPNS_TABLE = "cpns_view"
-# Sometimes a clinician will want to record that an event has happened at some
-# point in the past without knowing the specific date. In TPP such events are
-# given a date of 1900-01-01 and in EMIS they are given a date of NULL.
-# However, we already use NULL as a value to indicate that a patient had no
-# matching event at all, so we need another value to indicate "they had a
-# matching event but at an indeterminate time in the past". For consistency's
-# sake we use the same date as in TPP.
-EARLIEST_DATE = "1900-01-01"
-
 
-class EMISBackend:
+class TPPBackend:
     _db_connection = None
     _current_column_name = None
 
-    def __init__(
-        self,
-        database_url,
-        covariate_definitions,
-        temporary_database=None,
-        dummy_data=False,  # Ignored
-    ):
+    def __init__(self, database_url, covariate_definitions, temporary_database=None):
         self.database_url = database_url
         self.covariate_definitions = covariate_definitions
-        self.postprocess_covariate_definitions()
-        self.next_table_id = 1
-        self.temp_table_prefix = self.get_temp_table_prefix()
-        self.patient_no_duplicates_table = self.add_table_prefix("patient")
+        self.temporary_database = temporary_database
+        self.next_temp_table_id = 1
         self.queries = self.get_queries(self.covariate_definitions)
-        self.truncate_sql_logs = False
-        logger.info(
-            "Initialising EMISBackend", temp_table_prefix=self.temp_table_prefix
-        )
 
-    def postprocess_covariate_definitions(self):
-        """The pseudo_id field is an integer in TPP and a string in EMIS.  It is defined
-        as being an integer in process_covariate_definitions, so we override that here.
-        """
-
-        for name, (query_type, query_args) in self.covariate_definitions.items():
-            if query_args.get("returning") == "pseudo_id":
-                query_args["column_type"] = "str"
-
-    def to_file(self, filename):
-        result = self.execute_query()
-
-        # Wrap the results stream in a function which captures unique IDs,
-        # replaces them with sequential IDs and logs progress
-        unique_ids = set()
-        total_rows = 0
-
-        def replace_ids_and_log(result):
-            nonlocal total_rows
-            headers = [x[0] for x in result.description]
-            id_column_index = headers.index("patient_id")
-            # In production "patient_id" is a string (hex-encoded hash) but in
-            # test it's an int so we need to handle that correctly
-            if result.description[id_column_index][1] == "integer":
-                _truncate_patient_id = lambda x: x  # noqa
-            else:
-                _truncate_patient_id = truncate_patient_id
-
-            yield headers
-
-            for row in result:
-                # Reduce long EMIS patient IDs (see docstring)
-                patient_id = _truncate_patient_id(row[id_column_index])
-                row[id_column_index] = patient_id
-                unique_ids.add(patient_id)
-                total_rows += 1
-                if total_rows % 1000000 == 0:
-                    logger.info(f"Downloaded {total_rows} results")
-                yield row
-            logger.info(f"Downloaded {total_rows} results")
-
-        results = replace_ids_and_log(result)
-
-        # Special handling for CSV as we can stream this directly to disk
-        # without building a dataframe in memory
-        if is_csv_filename(filename):
-            with log_execution_time(
-                logger, description=f"write_rows_to_csv {filename}"
-            ):
-                write_rows_to_csv(results, filename)
-        else:
-            with log_execution_time(
-                logger, description=f"Create df and write dataframe_to_file {filename}"
-            ):
-                df = dataframe_from_rows(self.covariate_definitions, results)
-                dataframe_to_file(df, filename)
-
-        duplicates = total_rows - len(unique_ids)
-        if duplicates != 0:
-            raise RuntimeError(f"Duplicate IDs found ({duplicates} rows)")
+    def to_csv(self, filename):
+        queries = list(self.queries)
+        # If we have a temporary database available we write results to a table
+        # there, download them, and then delete the table. This allows us to
+        # resume in the case of a failed download without rerunning the whole
+        # query
+        if self.temporary_database:
+            output_table = self.save_results_to_temporary_db(queries)
+        else:
+            output_table = "#final_output"
+            queries[-1] = (
+                f"-- Writing results into {output_table}\n"
+                f"SELECT * INTO {output_table} FROM ({queries[-1]}) t"
+            )
+            queries.append(f"CREATE INDEX ix_patient_id ON {output_table} (patient_id)")
+            self.execute_queries(queries)
+        temp_filename = self._get_temp_filename(filename)
+        unique_check = UniqueCheck()
+
+        def record_patient_id_and_log(row):
+            unique_check.add(row[0])
+            if unique_check.count % 1000000 == 0:
+                self.log(f"Downloaded {unique_check.count} results")
+
+        # `batch_size` here was chosen through a bit of unscientific
+        # trial-and-error and some guesswork. It may well need changing in
+        # future.
+        mssql_table_to_csv(
+            temp_filename,
+            cursor=self.get_db_connection().cursor(),
+            table=output_table,
+            key_column="patient_id",
+            batch_size=32000,
+            row_callback=record_patient_id_and_log,
+            retries=2,
+            sleep=0.5,
+        )
+        self.log(f"Downloaded {unique_check.count} results")
+
+        self.execute_queries(
+            [f"-- Deleting '{output_table}'\nDROP TABLE {output_table}"]
+        )
+        unique_check.assert_unique_ids()
+        # If the extraction doesn't complete successfully we still want to keep
+        # the output file for debugging purposes, just under a name which makes
+        # it clear that it's not complete
+        os.rename(temp_filename, filename)
+
+    def _get_temp_filename(self, filename):
+        root, extension = os.path.splitext(filename)
+        timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
+        return f"{root}.partial.{timestamp}{extension}"
 
-    def to_dicts(self, convert_to_strings=True):
-        result = self.execute_query()
+    def to_dicts(self):
+        result = self.execute_queries(self.queries)
         keys = [x[0] for x in result.description]
-        if convert_to_strings:
-            # Convert all values to str as that's what will end in the CSV
-            output = [dict(zip(keys, map(str, row))) for row in result]
-        else:
-            output = [dict(zip(keys, row)) for row in result]
-
-        unique_ids = set(item["patient_id"] for item in output)
-        duplicates = len(output) - len(unique_ids)
-        if duplicates != 0:
-            raise RuntimeError(f"Duplicate IDs found ({duplicates} rows)")
-        for ix, row in enumerate(output):
-            row["patient_id"] = ix
+        # Convert all values to str as that's what will end in the CSV
+        output = [dict(zip(keys, map(str, row))) for row in result]
+        unique_check = UniqueCheck()
+        for item in output:
+            unique_check.add(item["patient_id"])
+        unique_check.assert_unique_ids()
         return output
 
     def to_sql(self):
         """
         Generate a single SQL string.
 
         Useful for debugging, optimising, etc.
         """
-        return "\n\n\n".join(f"{query};" for query in self.queries)
+        return "\nGO\n\n".join(self.queries)
+
+    def save_results_to_temporary_db(self, queries):
+        """
+        Sometimes there are glitches (network issues?) which occur when
+        downloading large result sets. To avoid having to recompute these each
+        time we can write the results to a table which we only delete once
+        we've fully downloaded its contents. If the download is interrupted
+        then subsequent runs will pick up the table and download it without
+        having to re-run all the queries.
+        """
+        assert self.temporary_database
+        # We're using the hash of all the queries and the database name as a
+        # cache key. Obviously this doesn't take into account the fact that the
+        # data itself may change, but for our purposes this doesn't matter:
+        # this is designed to be a very short-lived cache which is deleted as
+        # soon as the data is successfully downloaded. We need to include the
+        # database name because a single server may contain multiple databases
+        # (e.g full data and sample data) which share a single temporary
+        # database.
+        hash_elements = queries + [
+            mssql_connection_params_from_url(self.database_url)["database"]
+        ]
+        query_hash = hashlib.sha1("\n".join(hash_elements).encode("utf8")).hexdigest()
+        output_table = f"{self.temporary_database}..DataExtract_{query_hash}"
+        self.log(f"Checking for existing results in '{output_table}'")
+        if not self.table_exists(output_table):
+            self.log(
+                "No existing results found, running queries to generate new results"
+            )
+            # We want to raise an error now, rather than waiting until we've
+            # run all the other queries
+            self.assert_database_exists_and_is_writable(self.temporary_database)
+            queries = list(queries)
+            final_query = queries.pop()
+            self.execute_queries(queries)
+            # We need to run the final query in a transaction so that we don't end up
+            # with an empty output table in the event that the query fails. See:
+            # https://docs.microsoft.com/en-us/sql/t-sql/queries/select-into-clause-transact-sql?view=sql-server-ver15#remarks
+            conn = self.get_db_connection()
+            self.log(f"Writing results into temporary table '{output_table}'")
+            previous_autocommit = conn.autocommit
+            conn.autocommit = False
+            cursor = conn.cursor()
+            cursor.execute("BEGIN TRANSACTION")
+            cursor.execute(f"SELECT * INTO {output_table} FROM ({final_query}) t")
+            cursor.execute(f"CREATE INDEX ix_patient_id ON {output_table} (patient_id)")
+            cursor.execute("COMMIT")
+            conn.autocommit = previous_autocommit
+            self.log(f"Downloading results from '{output_table}'")
+        else:
+            self.log(f"Downloading results from previous run in '{output_table}'")
+        return output_table
+
+    def table_exists(self, table_name):
+        # We don't have access to sys.tables so this seems like the simplest
+        # way of testing for table existence
+        cursor = self.get_db_connection().cursor()
+        try:
+            cursor.execute(f"SELECT 1 FROM {table_name}")
+            list(cursor)
+            return True
+        # Because we don't want to depend on a specific database driver we
+        # can't catch a specific exception class here
+        except Exception as e:
+            if "Invalid object name" in str(e):
+                return False
+            else:
+                raise
+
+    def assert_database_exists_and_is_writable(self, db_name):
+        # As above, there's probably a better way of doing this
+        test_table = f"{db_name}..test_{uuid.uuid4().hex}"
+        cursor = self.get_db_connection().cursor()
+        try:
+            cursor.execute(f"SELECT 1 AS foo INTO {test_table}")
+            cursor.execute(f"DROP TABLE {test_table}")
+        # Because we don't want to depend on a specific database driver we
+        # can't catch a specific exception class here
+        except Exception as e:
+            if "Database does not exist" in str(e):
+                raise RuntimeError(f"Temporary database '{db_name}' does not exist")
+            else:
+                raise
+
+    def get_db_connection(self):
+        if self._db_connection:
+            return self._db_connection
+        self._db_connection = mssql_dbapi_connection_from_url(self.database_url)
+        return self._db_connection
+
+    def close(self):
+        if self._db_connection:
+            self._db_connection.close()
+        self._db_connection = None
 
     def get_queries(self, covariate_definitions):
         output_columns = {}
+        column_types = {}
+        is_hidden = {}
         table_queries = {}
         for name, (query_type, query_args) in covariate_definitions.items():
             # So we can safely mutate these below
             query_args = query_args.copy()
             # These arguments are not used in generating column data and the
             # corresponding functions do not accept them
             query_args.pop("return_expectations", None)
-            is_hidden = query_args.pop("hidden", False)
-            # Fixed values are the simplest case
-            if query_type == "fixed_value":
-                output_columns[name] = self.get_fixed_value_expression(**query_args)
+            is_hidden[name] = query_args.pop("hidden", False)
+            column_type = query_args.pop("column_type")
+            # Record the types of columns we've seen so far so that
+            # `categorised_as` expressions can use them if necessary
+            column_types[name] = column_type
             # `categorised_as` columns don't generate their own table query,
             # they're just a CASE expression over columns generated by other
             # queries
-            elif query_type == "categorised_as":
+            if query_type == "categorised_as":
                 output_columns[name] = self.get_case_expression(
-                    output_columns, **query_args
+                    column_types, output_columns, **query_args
                 )
             # `value_from` columns also don't generate a table, they just take
             # a value from another table
             elif query_type == "value_from":
                 assert query_args["source"] in table_queries
-                output_columns[name] = self.get_column_expression(**query_args)
+                output_columns[name] = self.get_column_expression(
+                    column_type, **query_args
+                )
             # As do `aggregate_of` columns
             elif query_type == "aggregate_of":
                 output_columns[name] = self.get_aggregate_expression(
-                    output_columns, **query_args
+                    column_type, output_columns, **query_args
                 )
             else:
-                column_args = pop_keys_from_dict(
-                    query_args, ["column_type", "date_format"]
-                )
-                sql_list = self.get_queries_for_column(
-                    name, query_type, query_args, output_columns
-                )
+                date_format_args = pop_keys_from_dict(query_args, ["date_format"])
+                sql_list = self.get_queries_for_column(name, query_type, query_args)
                 # Wrap the final SELECT query so that it writes its results
                 # into the appropriate temporary table
-                table_name = self.add_table_prefix(name)
-                sql_list[
-                    -1
-                ] = f"CREATE TABLE IF NOT EXISTS {table_name} AS ({sql_list[-1]})"
+                sql_list[-1] = (
+                    f"-- Query for {name}\n"
+                    f"SELECT * INTO #{name} FROM ({sql_list[-1]}) t"
+                )
                 table_queries[name] = sql_list
-
+                # The first column should always be patient_id so we can join on it
                 output_columns[name] = self.get_column_expression(
-                    source=name,
+                    column_type,
+                    name,
                     returning=query_args.get("returning", "value"),
-                    **column_args,
+                    **date_format_args,
                 )
-            output_columns[name].is_hidden = is_hidden
         # If the population query defines its own temporary table then we use
         # that as the primary table to query against and left join everything
-        # else against that. Otherwise, we use the `patient` table.
+        # else against that. Otherwise, we use the `Patient` table.
         if "population" in table_queries:
-            primary_table = self.add_table_prefix("population")
-            patient_id_expr = ColumnExpression(f"{primary_table}.registration_id")
+            primary_table = "#population"
+            patient_id_expr = "#population.patient_id"
         else:
-            primary_table = self.patient_no_duplicates_table
-            patient_id_expr = ColumnExpression(
-                f"{self.patient_no_duplicates_table}.registration_id"
-            )
+            primary_table = "Patient"
+            patient_id_expr = "Patient.Patient_ID"
         # Insert `patient_id` as the first column
         output_columns = dict(patient_id=patient_id_expr, **output_columns)
         output_columns_str = ",\n          ".join(
             f"{expr} AS {name}"
             for (name, expr) in output_columns.items()
-            if not expr.is_hidden and name != "population"
+            if not is_hidden.get(name) and name != "population"
         )
-        joins = []
-        for name in table_queries:
-            if name == "population":
-                continue
-            table_name = self.add_table_prefix(name)
-            joins.append(
-                f"LEFT JOIN {table_name} ON {table_name}.registration_id = {patient_id_expr}"
-            )
+        joins = [
+            f"LEFT JOIN #{name} ON #{name}.patient_id = {patient_id_expr}"
+            for name in table_queries
+            if name != "population"
+        ]
         joins_str = "\n          ".join(joins)
         joined_output_query = f"""
+        -- Join all columns for final output
         SELECT
           {output_columns_str}
         FROM
           {primary_table}
           {joins_str}
         WHERE {output_columns["population"]} = 1
         """
-
-        # patient_all_orgs_v2 contains a handful of duplicate registration IDs.  This
-        # causes problems: because of the way we build our final query with a series of
-        # N LEFT JOINs, a registration ID appearing twice in the patient table can
-        # appear up to 2^N times.
-        #
-        # EMIS have not yet fixed this, so our first query creates a temporary table
-        # which removes these duplicate registration IDs.  The number of duplicates is
-        # small enough that it doesn't matter that it causes us to lose a few patients,
-        # and in any case there is no way to choose between patients with duplicate
-        # registration IDs.
-        patient_no_duplicates_query = f"""
-        CREATE TABLE IF NOT EXISTS {self.patient_no_duplicates_table} AS (
-            SELECT *
-            FROM {PATIENT_TABLE}
-            WHERE registration_id NOT IN (
-                SELECT registration_id
-                FROM {PATIENT_TABLE}
-                GROUP BY registration_id
-                HAVING COUNT(*) > 1
-            )
-        )
-        """
-        all_queries = [patient_no_duplicates_query]
-
+        all_queries = []
         for sql_list in table_queries.values():
             all_queries.extend(sql_list)
         all_queries.append(joined_output_query)
-
-        log_stats(
-            logger,
-            output_column_count=len(output_columns),
-            table_count=len(table_queries),
-            table_joins_count=len(joins),
-        )
         return all_queries
 
     def get_column_expression(self, column_type, source, returning, date_format=None):
         default_value = self.get_default_value_for_type(column_type)
-        table_name = self.add_table_prefix(source)
-        column_expr = f"{table_name}.{returning}"
+        column_expr = f"#{source}.{returning}"
         if column_type == "date":
             column_expr = truncate_date(column_expr, date_format)
-        return ColumnExpression(
-            f"COALESCE({column_expr}, {quote(default_value)})",
-            type=column_type,
-            default_value=default_value,
-            source_tables=[table_name],
-            date_format=date_format,
-        )
-
-    def get_fixed_value_expression(self, value, column_type, date_format=None):
-        return ColumnExpression(
-            quote(value, reformat_dates=False),
-            type=column_type,
-            default_value=self.get_default_value_for_type(column_type),
-            source_tables=[],
-            date_format=date_format,
-        )
+        return f"ISNULL({column_expr}, {quote(default_value)})"
 
     def get_default_value_for_type(self, column_type):
         if column_type == "date":
             return ""
         elif column_type == "str":
             return ""
         elif column_type == "bool":
@@ -304,357 +302,139 @@
         elif column_type == "int":
             return 0
         elif column_type == "float":
             return 0.0
         else:
             raise ValueError(f"Unhandled column type: {column_type}")
 
-    def get_case_expression(
-        self, other_columns, column_type, category_definitions, date_format=None
-    ):
-        category_definitions = category_definitions.copy()
-        defaults = [k for (k, v) in category_definitions.items() if v == "DEFAULT"]
-        if len(defaults) > 1:
-            raise ValueError("At most one default category can be defined")
-        if len(defaults) == 1:
-            default_value = defaults[0]
-            category_definitions.pop(default_value)
-        else:
-            raise ValueError(
-                "At least one category must be given the definition 'DEFAULT'"
-            )
-        # For each column already defined, determine its corresponding "empty"
-        # value (i.e. the default value for that column's type). This allows us
-        # to support implicit boolean conversion because we know what the
-        # "falsey" value for each column should be.
-        empty_value_map = {
-            name: column.default_value for name, column in other_columns.items()
-        }
-        clauses = []
-        tables_used = set()
-        for category, expression in category_definitions.items():
-            # The column references in the supplied expression need to be
-            # rewritten to ensure they refer to the correct CTE. The formatting
-            # function also ensures that the expression matches the very
-            # limited subset of SQL we support here.
-            formatted_expression, names_used = format_expression(
-                expression, other_columns, empty_value_map=empty_value_map
-            )
-            clauses.append(f"WHEN ({formatted_expression}) THEN {quote(category)}")
-            # Record all the source tables used in evaluating the expression
-            for name in names_used:
-                tables_used.update(other_columns[name].source_tables)
-        return ColumnExpression(
-            f"CASE {' '.join(clauses)} ELSE {quote(default_value)} END",
-            type=column_type,
-            # Note, confusingly, this is not the same as the `default_value`
-            # used above. Above it refers to the value the case-expression will
-            # default to in case of no match. Below it refers to the "empty"
-            # value for the column type which is almost always the empty string
-            # apart from bools and ints where it's zero.
-            default_value=self.get_default_value_for_type(column_type),
-            source_tables=list(tables_used),
-        )
-
-    def get_aggregate_expression(
-        self, other_columns, column_type, column_names, aggregate_function
-    ):
-        """Return an expression that is used to find the maximum or minimum value across
-        a number of other given columns.
-
-        We cannot use Table Value Constructors as in the TPP backend (this gives a
-        cryptic error message: "Given correlated subquery is not supported").
-
-        Instead, we use GREATEST() or LEAST(), but we have to be careful to handle
-        correctly any arguments to GREATEST/LEAST that have replaced NULLs.  To do this,
-        we replace any occurences of the default value for the given column_type with
-        the most extreme value possible for the column_type.  (So when finding the
-        maximum, we replace the default value with a small value, and when finding the
-        minimum, with a large value.)
-
-        If all the arguments to GREATEST/LEAST have replaced NULLs, GREATEST/LEAST will
-        return the extreme value, so when that happens, we have to replace this with the
-        default value for the column type.
-
-        This gives us the result we want but it does mean we can't distinguish e.g. a
-        recorded value of 0.0 from a missing value.  This, however, is a general problem
-        with the way we handle NULLs in our system, and so we're not introducing any new
-        difficulty here.  (It's also unlikely to be a problem in practice.)
-        """
-
-        default_value = self.get_default_value_for_type(column_type)
-        function = {"MAX": "GREATEST", "MIN": "LEAST"}[aggregate_function]
-
-        if column_type in ["int", "float"]:
-            extreme_value_lookup = {"MAX": -(2**63), "MIN": 2 ** (63 - 1)}
-            extreme_value = [aggregate_function]
-        elif column_type == "date":
-            extreme_value_lookup = {"MAX": "'0001-01-01'", "MIN": "'9999-12-31'"}
-        else:
-            assert False, column_type
-        extreme_value = extreme_value_lookup[aggregate_function]
-
-        components = ", ".join(
-            f"""
-            CASE WHEN {other_columns[name]} = {quote(default_value)}
-                THEN {extreme_value}
-            ELSE {other_columns[name]} END"""
-            for name in column_names
-        )
-
-        # Keep track of all source tables used in evaluating this aggregate
-        tables_used = set()
-        for name in column_names:
-            tables_used.update(other_columns[name].source_tables)
-        return ColumnExpression(
-            f"""
-        CASE WHEN {function}({components}) = {extreme_value}
-            THEN {quote(default_value)}
-        ELSE {function}({components}) END""",
-            type=column_type,
-            default_value=default_value,
-            source_tables=list(tables_used),
-            # It's already been checked that date_format is consistent across
-            # the source columns, so we just grab the first one and use the
-            # date_format from that
-            date_format=other_columns[column_names[0]].date_format,
-        )
-
-    def execute_query(self):
+    def execute_queries(self, queries):
         cursor = self.get_db_connection().cursor()
-        queries = list(self.queries)
-        final_query = queries.pop()
-        run_analyze = bool(os.environ.get("RUN_ANALYZE"))
-        for sql in queries:
-            table_name = re.search(r"CREATE TABLE IF NOT EXISTS (\w+)", sql).groups()[0]
-            logger.info(f"Running query for {table_name}")
-            cursor.execute(sql, log_desc=f"Create table {table_name}")
-            if run_analyze:
-                cursor.execute(
-                    f"ANALYZE {table_name}", log_desc=f"Analyze table {table_name}"
-                )
-
-        output_table = self.get_output_table_name(os.environ.get("TEMP_DATABASE_NAME"))
-        if output_table:
-            logger.info(f"Running final query and writing output to '{output_table}'")
-            sql = f"CREATE TABLE IF NOT EXISTS {output_table} AS {final_query}"
-            cursor.execute(sql, log_desc="Create final query table")
-            logger.info(f"Downloading data from '{output_table}'")
-            cursor.execute(
-                f"SELECT * FROM {output_table}",
-                log_desc=f"Downloading data from '{output_table}'",
-            )
-        else:
-            logger.info(
-                "No TEMP_DATABASE_NAME defined in environment, downloading results "
-                "directly without writing to output table"
-            )
-            cursor.execute(
-                final_query, log_desc="Download results without writing to output table"
-            )
+        for query in queries:
+            comment_match = re.match(r"^\s*\-\-\s*(.+)\n", query)
+            if comment_match:
+                self.log(f"Running: {comment_match.group(1)}")
+            cursor.execute(query)
         return cursor
 
-    def get_output_table_name(self, temporary_database):
-        if not temporary_database:
-            return
+    def log(self, message):
         timestamp = datetime.datetime.now(datetime.timezone.utc).strftime(
-            "%Y%m%d_%H%M%S"
+            "%Y-%m-%d %H:%M:%S UTC"
         )
-        return f"{temporary_database}..Output_{timestamp}"
+        print(f"[{timestamp}] {message}", flush=True)
 
-    def get_temp_table_prefix(self):
-        if "TEMP_TABLE_PREFIX" in os.environ:
-            return os.environ["TEMP_TABLE_PREFIX"]
-        timestamp = datetime.datetime.now(datetime.timezone.utc).strftime(
-            "%Y%m%d_%H%M%S"
-        )
-        return f"_{timestamp}_{uuid.uuid4().hex[:4]}"
-
-    def add_table_prefix(self, name):
-        return f"{self.temp_table_prefix}_{name}"
-
-    def get_queries_for_column(
-        self, column_name, query_type, query_args, output_columns
-    ):
+    def get_queries_for_column(self, column_name, query_type, query_args):
         method_name = f"patients_{query_type}"
         method = getattr(self, method_name)
-        # We need to make available the SQL expression for each column in the
-        # output so far in case date expressions in the current column need to
-        # refer to these
-        self.output_columns = output_columns
         # Keep track of the current column name for debugging purposes
         self._current_column_name = column_name
         return_value = method(**query_args)
         self._current_column_name = None
         # We want to allow the query methods to return just a single SQL string
         # which we automatically wrap in a list
         if isinstance(return_value, str):
             return_value = [return_value]
-        for query in return_value:
-            assert (
-                "hashed_organisation" in query
-            ), f"SQL for `{column_name}` must contain 'hashed_organisation'"
         return return_value
 
-    def create_codelist_table(self, codelist):
+    def create_codelist_table(self, codelist, case_sensitive=True):
         table_name = self.get_temp_table_name("codelist")
-        cast = int if codelist.system in ("snomed", "snomedct", "dmd") else str
-        organisation_hash = quote(get_organisation_hash())
         if codelist.has_categories:
-            values = ", ".join(
-                f"({quote(cast(code))}, {quote(category)})"
-                for code, category in set(codelist)
-            )
-            queries = [
-                f"""
-                    CREATE TABLE IF NOT EXISTS {table_name} AS
-                    SELECT code, category, {organisation_hash} AS hashed_organisation FROM (
-                      VALUES {values}
-                    ) AS t (code, category)
-                    """
-            ]
+            values = list(codelist)
         else:
-            values = ", ".join(f"({quote(cast(code))})" for code in set(codelist))
-            queries = [
-                f"""
-                    CREATE TABLE IF NOT EXISTS {table_name} AS
-                    SELECT code, {organisation_hash} AS hashed_organisation FROM (
-                      VALUES {values}
-                    ) AS t (code)
-                    """
+            values = [(code, "") for code in codelist]
+        # Depending on the case-sensitivity of the code system the columns in question
+        # use different collations and we need to use a matching one here
+        collation = "Latin1_General_BIN" if case_sensitive else "Latin1_General_CI_AS"
+        max_code_len = max(len(code) for (code, category) in values)
+        queries = [
+            f"""
+            -- Uploading codelist for {self._current_column_name}
+            CREATE TABLE {table_name} (
+              code VARCHAR({max_code_len}) COLLATE {collation},
+              category VARCHAR(MAX)
+            )
+            """
+        ]
+        insert_sql = f"INSERT INTO {table_name} (code, category) VALUES"
+        # There's a limit on how many rows we can insert in one go using this method
+        # See: https://docs.microsoft.com/en-us/sql/t-sql/queries/table-value-constructor-transact-sql?view=sql-server-ver15#limitations-and-restrictions
+        batch_size = 999
+        for i in range(0, len(values), batch_size):
+            values_batch = values[i : i + batch_size]
+            values_sql_lines = [
+                "({}, {})".format(*map(quote, row)) for row in values_batch
             ]
+            values_sql = ",\n".join(values_sql_lines)
+            queries.append(f"{insert_sql}\n{values_sql}")
         return table_name, queries
 
     def get_temp_table_name(self, suffix):
-        table_name = f"{self.next_table_id}_"
-        self.next_table_id += 1
+        # The hash prefix indicates a temporary table
+        table_name = f"#tmp{self.next_temp_table_id}_"
+        self.next_temp_table_id += 1
         # We include the current column name if available for ease of debugging
         if self._current_column_name:
             table_name += f"{self._current_column_name}_"
         table_name += suffix
-        return self.add_table_prefix(table_name)
+        return table_name
 
-    def get_date_condition(self, table, date_expr, between):
-        """
-        Takes a table name, an SQL expression representing a date (which can
-        just be a column name on the table, or something more complicated) and
-        a date interval.
-        Returns two fragements of SQL: a "condition" and a "join"
-        The condition is SQL which evaluates true when `date_expr` is in the
-        supplied period.
-        The join provides the (possibly empty) JOINs which need to be appended
-        to "table" in order to evaluate the condition.
+    def patients_age_as_of(self, reference_date):
+        quoted_date = quote(reference_date)
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          CASE WHEN
+             dateadd(year, datediff (year, DateOfBirth, {quoted_date}), DateOfBirth) > {quoted_date}
+          THEN
+             datediff(year, DateOfBirth, {quoted_date}) - 1
+          ELSE
+             datediff(year, DateOfBirth, {quoted_date})
+          END AS value
+        FROM Patient
         """
-        if between is None:
-            between = (None, None)
-        min_date, max_date = between
-        min_date_expr, join_tables1 = self.date_ref_to_sql_expr(min_date)
-        max_date_expr, join_tables2 = self.date_ref_to_sql_expr(max_date)
-        date_expr = TrinoDateFormatter.cast_as_date(date_expr)
-        min_date_expr = TrinoDateFormatter.cast_as_date(min_date_expr)
-        max_date_expr = TrinoDateFormatter.cast_as_date(max_date_expr)
 
-        joins = [
-            f"LEFT JOIN {join_table}\n"
-            f"ON {join_table}.registration_id = {table}.registration_id"
-            for join_table in set(join_tables1 + join_tables2)
-        ]
-        join_str = "\n".join(joins)
-        if min_date_expr is not None and max_date_expr is not None:
-            return (
-                f"{date_expr} BETWEEN {min_date_expr} AND {max_date_expr}",
-                join_str,
-            )
-        elif min_date_expr is not None:
-            return f"{date_expr} >= {min_date_expr}", join_str
-        elif max_date_expr is not None:
-            return f"{date_expr} <= {max_date_expr}", join_str
-        else:
-            return "1=1", join_str
-
-    def get_date_sql(self, table, *date_expressions):
-        """
-        Given a table name and one or more date expressions return the
-        corresponding SQL expressions followed by a fragment of SQL supplying
-        any necessary JOINs
-        """
-        all_join_tables = set()
-        sql_expressions = []
-        for date_expression in date_expressions:
-            assert date_expression is not None
-            sql_expression, join_tables = self.date_ref_to_sql_expr(date_expression)
-            sql_expressions.append(sql_expression)
-            all_join_tables.update(join_tables)
-        joins = [
-            f"LEFT JOIN {join_table}\n"
-            f"ON {join_table}.registration_id = {table}.registration_id"
-            for join_table in all_join_tables
-        ]
-        join_str = "\n".join(joins)
-        return (*sql_expressions, join_str)
-
-    def date_ref_to_sql_expr(self, date):
-        """
-        Given a date reference return its corresponding SQL expression,
-        together with a list of any tables to which this expression refers
+    def patients_date_of_birth(self):
+        return """
+        SELECT Patient_ID AS patient_id, DateOfBirth AS value FROM Patient
         """
-        if date is None:
-            return None, []
-        # We don't yet handle any of the fancy cross-column references, just
-        # plain date literals
-        # Simple date literals
-        if is_iso_date(date):
-            return quote(date), []
-        # More complicated date expressions which reference other tables
-        formatter = TrinoDateFormatter(self.output_columns)
-        date_expr = formatter(date)
-        date_expr, column_name = formatter(date)
-        tables = self.output_columns[column_name].source_tables
-        return date_expr, tables
-
-    def patients_age_as_of(self, reference_date):
-        date_expr, date_joins = self.get_date_sql(
-            self.patient_no_duplicates_table, reference_date
-        )
-        return f"""
-            SELECT
-              registration_id,
-              hashed_organisation,
-              CASE WHEN
-                 date_add('year', date_diff('year', date_of_birth, {date_expr}), date_of_birth) > {date_expr}
-              THEN
-                 date_diff('year', date_of_birth, {date_expr}) - 1
-              ELSE
-                 date_diff('year', date_of_birth, {date_expr})
-              END AS value
-            FROM {self.patient_no_duplicates_table}
-            {date_joins}
-            """
 
     def patients_sex(self):
-        return f"""
-          SELECT
-            registration_id,
-            hashed_organisation,
-            CASE gender
-              -- See https://www.datadictionary.nhs.uk/data_dictionary/attributes/p/person/person_gender_code_de.asp?shownav=1
-              WHEN 1 THEN 'M'
-              WHEN 2 THEN 'F'
-              ELSE ''
-            END AS value
-          FROM {self.patient_no_duplicates_table}"""
+        return """
+        SELECT
+          Patient_ID AS patient_id,
+          Sex AS value
+        FROM Patient
+        """
 
     def patients_all(self):
         """
         All patients
         """
+        return """
+        SELECT Patient_ID AS patient_id, 1 AS value
+        FROM Patient
+        """
+
+    def patients_random_sample(self, percent):
+        """
+        A random sample of approximately `percent` patients
+        """
+        # See
+        # https://docs.microsoft.com/en-us/previous-versions/software-testing/cc441928(v=msdn.10)?redirectedfrom=MSDN
+        # A TABLESAMPLE clause is more efficient, but its
+        # approximations don't work with small numbers, and we might
+        # want to use this method for small numbers (and certainly do
+        # in the tests!)
+        assert percent, "Must specify a percentage greater than zero"
         return f"""
-            SELECT registration_id, hashed_organisation, 1 AS value
-            FROM {self.patient_no_duplicates_table}
-            """
+        SELECT Patient_ID, 1 AS value
+        FROM Patient
+        WHERE (ABS(CAST(
+        (BINARY_CHECKSUM(*) *
+        RAND()) as int)) % 100) < {quote(percent)}
+        """
 
     def patients_most_recent_bmi(
         self,
         # Set date limits
         between=None,
         minimum_age_at_measurement=16,
         # Add an additional column indicating when measurement was taken
@@ -675,255 +455,197 @@
         # From https://github.com/ebmdatalab/tpp-sql-notebook/issues/10:
         #
         # 1) BMI calculated from last recorded height and weight
         #
         # 2) If height and weight is not available, then take latest
         # recorded BMI. Both values must be recorded when the patient
         # is >=16, weight must be within the last 10 years
-        date_condition, date_joins = self.get_date_condition(
-            OBSERVATION_TABLE, "effective_date", between
-        )
+        date_condition = make_date_filter("ConsultationDate", between)
 
-        # TODO these codes need validating
-        bmi_code = 301331008  # Finding of body mass index (finding)
-        weight_codes = codelist(
-            [
-                "27113001",  # Body weight (observable entity)
-                "162763007",  # On examination - weight(finding)
-            ],
-            system="snomedct",
-        )
-        height_codes = codelist(
-            [
-                "271603002",  # Height / growth measure (observable entity)
-                "162755006",  # On examination - height (finding)
-            ],
-            system="snomedct",
-        )
+        bmi_code = "22K.."
+        # XXX these two sets of codes need validating. The final in
+        # each list is the canonical version according to TPP
+        weight_codes = [
+            "X76C7",  # Concept containing "body weight" terms:
+            "22A..",  # O/E weight
+        ]
+        height_codes = [
+            "XM01E",  # Concept containing height/length/stature/growth terms:
+            "229..",  # O/E height
+        ]
 
         bmi_cte = f"""
-        SELECT t.registration_id, t.value, t.effective_date
+        SELECT t.Patient_ID, t.BMI, t.ConsultationDate
         FROM (
-          SELECT {OBSERVATION_TABLE}.registration_id, "value_pq_1" AS value, effective_date,
+          SELECT Patient_ID, NumericValue AS BMI, ConsultationDate,
           ROW_NUMBER() OVER (
-            PARTITION BY {OBSERVATION_TABLE}.registration_id ORDER BY effective_date DESC
+            PARTITION BY Patient_ID ORDER BY ConsultationDate DESC, CodedEvent_ID
           ) AS rownum
-          FROM {OBSERVATION_TABLE}
-          WHERE snomed_concept_id = {quote(bmi_code)} AND {date_condition}
-          {date_joins}
+          FROM CodedEvent
+          WHERE CTV3Code = {quote(bmi_code)} AND {date_condition}
         ) t
         WHERE t.rownum = 1
         """
 
-        patients_cte = f"""
-           SELECT registration_id, hashed_organisation, date_of_birth
-           FROM {self.patient_no_duplicates_table}
+        patients_cte = """
+           SELECT Patient_ID, DateOfBirth
+           FROM Patient
         """
         weight_codes_sql = codelist_to_sql(weight_codes)
         weights_cte = f"""
-          SELECT t.registration_id, t.weight, t.effective_date
+          SELECT t.Patient_ID, t.weight, t.ConsultationDate
           FROM (
-            SELECT registration_id, "value_pq_1" AS weight, effective_date,
-            ROW_NUMBER() OVER (PARTITION BY registration_id ORDER BY effective_date DESC) AS rownum
-            FROM {OBSERVATION_TABLE}
-            WHERE snomed_concept_id IN ({weight_codes_sql}) AND {date_condition}
+            SELECT Patient_ID, NumericValue AS weight, ConsultationDate,
+              ROW_NUMBER() OVER (
+                PARTITION BY Patient_ID ORDER BY ConsultationDate DESC, CodedEvent_ID
+              ) AS rownum
+            FROM CodedEvent
+            WHERE CTV3Code IN ({weight_codes_sql}) AND {date_condition}
           ) t
           WHERE t.rownum = 1
         """
 
         height_codes_sql = codelist_to_sql(height_codes)
         # The height date restriction is different from the others. We don't
         # mind using old values as long as the patient was old enough when they
         # were taken.
-        height_date_condition, height_date_joins = self.get_date_condition(
-            OBSERVATION_TABLE,
-            "effective_date",
-            remove_lower_date_bound(between),
+        height_date_condition = make_date_filter(
+            "ConsultationDate",
+            between,
+            upper_bound_only=True,
         )
         heights_cte = f"""
-          SELECT t.registration_id, t.height, t.effective_date
+          SELECT t.Patient_ID, t.height, t.ConsultationDate
           FROM (
-            SELECT registration_id, "value_pq_1" AS height, effective_date,
-            ROW_NUMBER() OVER (PARTITION BY registration_id ORDER BY effective_date DESC) AS rownum
-            FROM {OBSERVATION_TABLE}
-            {height_date_joins}
-            WHERE snomed_concept_id IN ({height_codes_sql}) AND {height_date_condition}
+            SELECT Patient_ID, NumericValue AS height, ConsultationDate,
+            ROW_NUMBER() OVER (
+              PARTITION BY Patient_ID ORDER BY ConsultationDate DESC, CodedEvent_ID
+            ) AS rownum
+            FROM CodedEvent
+            WHERE CTV3Code IN ({height_codes_sql}) AND {height_date_condition}
           ) t
           WHERE t.rownum = 1
         """
 
         min_age = int(minimum_age_at_measurement)
 
         return f"""
         SELECT
-          patients.registration_id,
-          hashed_organisation,
-          CASE
-            WHEN height = 0 THEN NULL
-            ELSE ROUND(COALESCE(weight/(height*height), bmis.value), 1)
-          END AS value,
+          patients.Patient_ID AS patient_id,
+          ROUND(COALESCE(weight/SQUARE(NULLIF(height, 0)), bmis.BMI), 1) AS value,
           CASE
-            WHEN weight IS NULL OR height IS NULL THEN DATE(bmis.effective_date)
-            ELSE DATE(weights.effective_date)
+            WHEN weight IS NULL OR height IS NULL THEN bmis.ConsultationDate
+            ELSE weights.ConsultationDate
           END AS date
         FROM ({patients_cte}) AS patients
         LEFT JOIN ({weights_cte}) AS weights
-        ON weights.registration_id = patients.registration_id AND date_diff('year', patients.date_of_birth, weights.effective_date) >= {min_age}
+        ON weights.Patient_ID = patients.Patient_ID AND DATEDIFF(YEAR, patients.DateOfBirth, weights.ConsultationDate) >= {min_age}
         LEFT JOIN ({heights_cte}) AS heights
-        ON heights.registration_id = patients.registration_id AND date_diff('year', patients.date_of_birth, heights.effective_date) >= {min_age}
+        ON heights.Patient_ID = patients.Patient_ID AND DATEDIFF(YEAR, patients.DateOfBirth, heights.ConsultationDate) >= {min_age}
         LEFT JOIN ({bmi_cte}) AS bmis
-        ON bmis.registration_id = patients.registration_id AND date_diff('year', patients.date_of_birth, bmis.effective_date) >= {min_age}
+        ON bmis.Patient_ID = patients.Patient_ID AND DATEDIFF(YEAR, patients.DateOfBirth, bmis.ConsultationDate) >= {min_age}
         -- XXX maybe add a "WHERE NULL..." here
         """
 
-    def _summarised_recorded_value(
-        self,
-        codelist,
-        on_most_recent_day_of_measurement,
-        between,
-        include_date_of_match,
-        summary_function,
-    ):
-        date_condition, date_joins = self.get_date_condition(
-            OBSERVATION_TABLE, "effective_date", between
-        )
-        codelist_sql = codelist_to_sql(codelist)
-
-        if on_most_recent_day_of_measurement:
-            # The subquery finds, for each patient, the most recent day on which
-            # they've had a measurement. The outer query selects, for each patient,
-            # the mean value on that day.
-            # Note, there's a CAST in the JOIN condition but apparently SQL Server can still
-            # use an index for this. See: https://stackoverflow.com/a/25564539
-            return f"""
-            SELECT
-            days.registration_id,
-            days.hashed_organisation,
-            {summary_function}({OBSERVATION_TABLE}."value_pq_1") AS value,
-            days.date_measured AS date
-            FROM (
-                SELECT
-                    {OBSERVATION_TABLE}.registration_id,
-                    {OBSERVATION_TABLE}.hashed_organisation,
-                    CAST(MAX(effective_date) AS date) AS date_measured
-                FROM {OBSERVATION_TABLE}
-                {date_joins}
-                WHERE snomed_concept_id IN ({codelist_sql}) AND {date_condition}
-                GROUP BY {OBSERVATION_TABLE}.registration_id, {OBSERVATION_TABLE}.hashed_organisation
-            ) AS days
-            LEFT JOIN {OBSERVATION_TABLE}
-            ON (
-            {OBSERVATION_TABLE}.registration_id = days.registration_id
-            AND {OBSERVATION_TABLE}.snomed_concept_id IN ({codelist_sql})
-            AND CAST({OBSERVATION_TABLE}.effective_date AS date) = days.date_measured
-            )
-            GROUP BY days.registration_id, days.hashed_organisation, days.date_measured
-            """
-        else:
-            assert (
-                include_date_of_match is False
-            ), "Can only include measurement date if on_most_recent_day_of_measurement is True"
-
-            return f"""
-            SELECT
-                {OBSERVATION_TABLE}.registration_id,
-                {OBSERVATION_TABLE}.hashed_organisation,
-                {summary_function}({OBSERVATION_TABLE}."value_pq_1") AS value
-            FROM {OBSERVATION_TABLE}
-                {date_joins}
-            WHERE snomed_concept_id IN ({codelist_sql}) AND {date_condition}
-            GROUP BY {OBSERVATION_TABLE}.registration_id, {OBSERVATION_TABLE}.hashed_organisation
-            """
-
     def patients_mean_recorded_value(
         self,
         codelist,
-        # What period is the mean over?
-        on_most_recent_day_of_measurement=None,
-        # Set date limits
-        between=None,
-        # Add additional columns indicating when measurement was taken
-        include_date_of_match=False,
-    ):
-        return self._summarised_recorded_value(
-            codelist,
-            on_most_recent_day_of_measurement,
-            between,
-            include_date_of_match,
-            "AVG",
-        )
-
-    def patients_min_recorded_value(
-        self,
-        codelist,
-        # What period is the mean over?
+        # What period is the mean over? (Only one supported option for now)
         on_most_recent_day_of_measurement=None,
         # Set date limits
         between=None,
         # Add additional columns indicating when measurement was taken
         include_date_of_match=False,
     ):
-        return self._summarised_recorded_value(
-            codelist,
-            on_most_recent_day_of_measurement,
-            between,
-            include_date_of_match,
-            "MIN",
-        )
-
-    def patients_max_recorded_value(
-        self,
-        codelist,
-        # What period is the mean over?
-        on_most_recent_day_of_measurement=None,
-        # Set date limits
-        between=None,
-        # Add additional columns indicating when measurement was taken
-        include_date_of_match=False,
-    ):
-        return self._summarised_recorded_value(
-            codelist,
-            on_most_recent_day_of_measurement,
-            between,
-            include_date_of_match,
-            "MAX",
+        # We only support this option for now
+        assert on_most_recent_day_of_measurement
+        date_condition = make_date_filter("ConsultationDate", between)
+        codelist_sql = codelist_to_sql(codelist)
+        # The subquery finds, for each patient, the most recent day on which
+        # they've had a measurement. The outer query selects, for each patient,
+        # the mean value on that day.
+        # Note, there's a CAST in the JOIN condition but apparently SQL Server can still
+        # use an index for this. See: https://stackoverflow.com/a/25564539
+        return f"""
+        SELECT
+          days.Patient_ID AS patient_id,
+          AVG(CodedEvent.NumericValue) AS value,
+          days.date_measured AS date
+        FROM (
+            SELECT Patient_ID, CAST(MAX(ConsultationDate) AS date) AS date_measured
+            FROM CodedEvent
+            WHERE CTV3Code IN ({codelist_sql}) AND {date_condition}
+            GROUP BY Patient_ID
+        ) AS days
+        LEFT JOIN CodedEvent
+        ON (
+          CodedEvent.Patient_ID = days.Patient_ID
+          AND CodedEvent.CTV3Code IN ({codelist_sql})
+          AND CAST(CodedEvent.ConsultationDate AS date) = days.date_measured
         )
+        GROUP BY days.Patient_ID, days.date_measured
+        """
 
     def patients_registered_as_of(self, reference_date):
         """
         All patients registed on the given date
         """
         return self.patients_registered_with_one_practice_between(
             reference_date, reference_date
         )
 
-    def patients_registered_with_one_practice_between(self, start_date, end_date):
+    def patients_registered_with_one_practice_between(
+        self, start_date, end_date, practice_used_systm_one_throughout_period=False
+    ):
         """
         All patients registered with the same practice through the given period
         """
-        start_date_sql, end_date_sql, date_joins = self.get_date_sql(
-            self.patient_no_duplicates_table, start_date, end_date
-        )
+        # Note that current registrations are recorded with an EndDate
+        # of 9999-12-31
+        extra_condition = ""
+        if practice_used_systm_one_throughout_period:
+            # We only need to (and only can) check the date the practice
+            # *started* using SystmOne.  If they've stopped using it, then we
+            # won't have their data in the TPP database at all.
+            extra_condition = f"  AND Organisation.GoLiveDate <= {quote(start_date)}"
         return f"""
-            SELECT
-                {self.patient_no_duplicates_table}.registration_id,
-                {self.patient_no_duplicates_table}.hashed_organisation,
-                1 AS value
-            FROM {self.patient_no_duplicates_table}
-            {date_joins}
-            WHERE registered_date <= {start_date_sql}
-              AND (registration_end_date > {end_date_sql} OR registration_end_date IS NULL)
-            """
+        SELECT DISTINCT Patient.Patient_ID AS patient_id, 1 AS value
+        FROM Patient
+        INNER JOIN RegistrationHistory
+        ON RegistrationHistory.Patient_ID = Patient.Patient_ID
+        INNER JOIN Organisation
+        ON RegistrationHistory.Organisation_ID = Organisation.Organisation_ID
+        WHERE StartDate <= {quote(start_date)} AND EndDate > {quote(end_date)}
+        {extra_condition}
+        """
+
+    def patients_with_complete_history_between(self, start_date, end_date):
+        """
+        All patients for which we have a full set of records between the given
+        dates
+        """
+        # This should be do-able by checking for a contiguous set of
+        # RegistrationHistory entries covering the period. There's a further
+        # complication though which is that a practice might not have been
+        # using SystmOne at the point where the patient registered so we can
+        # only guarantee data from the point where the patient was registred
+        # *and* the practice was on SystmOne. Apparently the Organisation table
+        # now has a TPP go-live date which we can use for this purpose.
+        raise NotImplementedError()
 
     def patients_with_these_medications(self, **kwargs):
         """
         Patients who have been prescribed at least one of this list of
         medications in the defined period
         """
-        assert kwargs["codelist"].system in ("snomed", "snomedct")
+        # Note that we're using "ConsultationDate" for the date condition here,
+        # which is the date of prescription.  The MedicationIssue table also
+        # has StartDate (the date of issue) and EndDate (not exactly sure what
+        # this is).
+        assert kwargs["codelist"].system == "snomed"
         if kwargs["returning"] == "numeric_value":
             raise ValueError("Unsupported `returning` value: numeric_value")
         # This uses a special case function with a "fake it til you make it" API
         if kwargs["returning"] == "number_of_episodes":
             kwargs.pop("returning")
             # Remove unhandled arguments and check they are unused
             assert not kwargs.pop("find_first_match_in_period", None)
@@ -931,634 +653,533 @@
             assert not kwargs.pop("include_date_of_match", None)
             return self._number_of_episodes_by_medication(**kwargs)
         # This is the default code path for most queries
         else:
             # Remove unhandled arguments and check they are unused
             assert not kwargs.pop("episode_defined_as", None)
             return self._patients_with_events(
-                MEDICATION_TABLE,
-                "",
-                "snomed_concept_id",
+                "MedicationIssue",
+                """
+                INNER JOIN MedicationDictionary
+                ON MedicationIssue.MultilexDrug_ID = MedicationDictionary.MultilexDrug_ID
+                """,
+                "DMD_ID",
+                codes_are_case_sensitive=False,
                 **kwargs,
             )
 
     def patients_with_these_clinical_events(self, **kwargs):
         """
         Patients who have had at least one of these clinical events in the
         defined period
         """
-        assert kwargs["codelist"].system in ("snomed", "snomedct")
+        assert kwargs["codelist"].system == "ctv3"
         # This uses a special case function with a "fake it til you make it" API
         if kwargs["returning"] == "number_of_episodes":
             kwargs.pop("returning")
             # Remove unhandled arguments and check they are unused
             assert not kwargs.pop("find_first_match_in_period", None)
             assert not kwargs.pop("find_last_match_in_period", None)
             assert not kwargs.pop("include_date_of_match", None)
             return self._number_of_episodes_by_clinical_event(**kwargs)
         # This is the default code path for most queries
         else:
             assert not kwargs.pop("episode_defined_as", None)
             return self._patients_with_events(
-                OBSERVATION_TABLE,
-                "",
-                "snomed_concept_id",
-                **kwargs,
+                "CodedEvent", "", "CTV3Code", codes_are_case_sensitive=True, **kwargs
             )
 
     def _patients_with_events(
         self,
         from_table,
         additional_join,
         code_column,
+        codes_are_case_sensitive,
         codelist,
         # Allows us to say: find codes A and B, but only on days where X and Y
         # didn't happen
         ignore_days_where_these_codes_occur=None,
         # Set date limits
         between=None,
         # Matching rule
         find_first_match_in_period=None,
         find_last_match_in_period=None,
         # Set return type
         returning="binary_flag",
         include_date_of_match=False,
-        ignore_missing_values=False,
     ):
-        codelist_table, codelist_queries = self.create_codelist_table(codelist)
-        # Using COALESCE like this has the potential to produce very
-        # inefficient queries by scuppering use of indices. However, my
-        # understanding is there are no indicies anyway in the current Trino
-        # setup so this shouldn't actually make much difference
-        date_condition, date_joins = self.get_date_condition(
-            from_table, f"COALESCE(effective_date, {quote(EARLIEST_DATE)})", between
+        codelist_table, codelist_queries = self.create_codelist_table(
+            codelist, codes_are_case_sensitive
         )
+        date_condition = make_date_filter("ConsultationDate", between)
         ignored_day_condition, extra_queries = self._these_codes_occur_on_same_day(
-            from_table, ignore_days_where_these_codes_occur
-        )
-        missing_value_condition = (
-            "(value_pq_1 IS NOT NULL AND value_pq_1 != 0)"
-            if ignore_missing_values
-            else "1 = 1"
+            from_table, ignore_days_where_these_codes_occur, date_condition
         )
 
         # Result ordering
         if find_first_match_in_period:
-            ordering = "ASC NULLS FIRST"
+            ordering = "ASC"
             date_aggregate = "MIN"
         else:
-            ordering = "DESC NULLS LAST"
+            ordering = "DESC"
             date_aggregate = "MAX"
 
-        query_column = None
         column_name = returning
         if returning == "binary_flag" or returning == "date":
             column_name = "binary_flag"
             column_definition = "1"
             use_partition_query = False
         elif returning == "number_of_matches_in_period":
             column_definition = "COUNT(*)"
             use_partition_query = False
         elif returning == "numeric_value":
-            column_definition = '"value_pq_1"'
+            column_definition = "NumericValue"
             use_partition_query = True
         elif returning == "code":
-            column_definition = f"CAST({code_column} AS VARCHAR(18))"
-            query_column = code_column
+            column_definition = code_column
             use_partition_query = True
         elif returning == "category":
             if not codelist.has_categories:
                 raise ValueError(
                     "Cannot return categories because the supplied codelist does "
                     "not have any categories defined"
                 )
             column_definition = "category"
             use_partition_query = True
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
 
-        if query_column is None:
-            query_column = column_definition
-
         if use_partition_query:
             sql = f"""
             SELECT
-              registration_id,
-              hashed_organisation,
+              Patient_ID AS patient_id,
               {column_definition} AS {column_name},
-              COALESCE(DATE(effective_date), {quote(EARLIEST_DATE)}) AS date
+              ConsultationDate AS date
             FROM (
-              SELECT
-                {from_table}.registration_id,
-                {from_table}.hashed_organisation,
-                {query_column},
-                effective_date,
-                ROW_NUMBER() OVER (
-                  PARTITION BY {from_table}.registration_id
-                  ORDER BY effective_date {ordering}
-                ) AS rownum
+              SELECT Patient_ID, {column_definition}, ConsultationDate,
+              ROW_NUMBER() OVER (
+                PARTITION BY Patient_ID
+                ORDER BY ConsultationDate {ordering}, {from_table}_ID
+              ) AS rownum
               FROM {from_table}{additional_join}
               INNER JOIN {codelist_table}
               ON {code_column} = {codelist_table}.code
-              {date_joins}
-              WHERE {date_condition}
-                AND NOT {ignored_day_condition}
-                AND {missing_value_condition}
+              WHERE {date_condition} AND NOT {ignored_day_condition}
             ) t
             WHERE rownum = 1
             """
         else:
             sql = f"""
             SELECT
-              {from_table}.registration_id,
-              {from_table}.hashed_organisation,
+              Patient_ID AS patient_id,
               {column_definition} AS {column_name},
-              {date_aggregate}(COALESCE(DATE(effective_date), {quote(EARLIEST_DATE)})) AS date
+              {date_aggregate}(ConsultationDate) AS date
             FROM {from_table}{additional_join}
             INNER JOIN {codelist_table}
             ON {code_column} = {codelist_table}.code
-            {date_joins}
-            WHERE {date_condition}
-              AND NOT {ignored_day_condition}
-              AND {missing_value_condition}
-            GROUP BY {from_table}.registration_id, {from_table}.hashed_organisation
+            WHERE {date_condition} AND NOT {ignored_day_condition}
+            GROUP BY Patient_ID
             """
 
         return codelist_queries + extra_queries + [sql]
 
     def _number_of_episodes_by_medication(
         self,
         codelist,
         # Set date limits
         between=None,
         ignore_days_where_these_codes_occur=None,
         episode_defined_as=None,
     ):
-        codelist_table, codelist_queries = self.create_codelist_table(codelist)
-        date_condition, date_joins = self.get_date_condition(
-            MEDICATION_TABLE, "effective_date", between
+        codelist_table, codelist_queries = self.create_codelist_table(
+            codelist, case_sensitive=False
         )
+        date_condition = make_date_filter("ConsultationDate", between)
         ignored_day_condition, extra_queries = self._these_codes_occur_on_same_day(
-            MEDICATION_TABLE, ignore_days_where_these_codes_occur
+            "MedicationIssue", ignore_days_where_these_codes_occur, date_condition
         )
         if episode_defined_as is not None:
             pattern = r"^series of events each <= (\d+) days apart$"
             match = re.match(pattern, episode_defined_as)
             if not match:
                 raise ValueError(
                     f"Argument `episode_defined_as` must match " f"pattern: {pattern}"
                 )
             washout_period = int(match.group(1))
         else:
             washout_period = 0
 
         sql = f"""
         SELECT
-          registration_id,
-          hashed_organisation,
+          Patient_ID AS patient_id,
           SUM(is_new_episode) AS number_of_episodes
         FROM (
             SELECT
-              {MEDICATION_TABLE}.registration_id,
-              {MEDICATION_TABLE}.hashed_organisation,
+              Patient_ID,
               CASE
                 WHEN
-                  date_diff(
-                    'day',
-                    LAG(effective_date) OVER (
-                      PARTITION BY {MEDICATION_TABLE}.registration_id ORDER BY effective_date
-                    ),
-                    effective_date
+                  DATEDIFF(
+                    day,
+                    LAG(ConsultationDate) OVER (PARTITION BY Patient_ID ORDER BY ConsultationDate),
+                    ConsultationDate
                   ) <= {washout_period}
                 THEN 0
                 ELSE 1
               END AS is_new_episode
-            FROM {MEDICATION_TABLE}
+            FROM MedicationIssue
+            INNER JOIN MedicationDictionary
+            ON MedicationIssue.MultilexDrug_ID = MedicationDictionary.MultilexDrug_ID
             INNER JOIN {codelist_table}
-            ON snomed_concept_id = {codelist_table}.code
-            {date_joins}
+            ON DMD_ID = {codelist_table}.code
             WHERE {date_condition} AND NOT {ignored_day_condition}
         ) t
-        GROUP BY registration_id, hashed_organisation
+        GROUP BY Patient_ID
         """
         return codelist_queries + extra_queries + [sql]
 
     def _number_of_episodes_by_clinical_event(
         self,
         codelist,
         # Set date limits
         between=None,
         ignore_days_where_these_codes_occur=None,
         episode_defined_as=None,
-        ignore_missing_values=False,
     ):
-        codelist_table, codelist_queries = self.create_codelist_table(codelist)
-        date_condition, date_joins = self.get_date_condition(
-            OBSERVATION_TABLE, "effective_date", between
+        codelist_table, codelist_queries = self.create_codelist_table(
+            codelist, case_sensitive=True
         )
+        date_condition = make_date_filter("ConsultationDate", between)
         ignored_day_condition, extra_queries = self._these_codes_occur_on_same_day(
-            OBSERVATION_TABLE, ignore_days_where_these_codes_occur
+            "CodedEvent", ignore_days_where_these_codes_occur, date_condition
         )
-        missing_value_condition = (
-            "(value_pq_1 IS NOT NULL AND value_pq_1 != 0)"
-            if ignore_missing_values
-            else "1 = 1"
-        )
-
         if episode_defined_as is not None:
             pattern = r"^series of events each <= (\d+) days apart$"
             match = re.match(pattern, episode_defined_as)
             if not match:
                 raise ValueError(
                     f"Argument `episode_defined_as` must match " f"pattern: {pattern}"
                 )
             washout_period = int(match.group(1))
         else:
             washout_period = 0
 
         sql = f"""
         SELECT
-          registration_id,
-          hashed_organisation,
+          Patient_ID AS patient_id,
           SUM(is_new_episode) AS number_of_episodes
         FROM (
             SELECT
-              {OBSERVATION_TABLE}.registration_id,
-              {OBSERVATION_TABLE}.hashed_organisation,
+              Patient_ID,
               CASE
                 WHEN
-                  date_diff(
-                    'day',
-                    LAG(effective_date) OVER (
-                      PARTITION BY {OBSERVATION_TABLE}.registration_id ORDER BY effective_date
-                    ),
-                    effective_date
+                  DATEDIFF(
+                    day,
+                    LAG(ConsultationDate) OVER (PARTITION BY Patient_ID ORDER BY ConsultationDate),
+                    ConsultationDate
                   ) <= {washout_period}
                 THEN 0
                 ELSE 1
               END AS is_new_episode
-            FROM {OBSERVATION_TABLE}
+            FROM CodedEvent
             INNER JOIN {codelist_table}
-            ON snomed_concept_id = {codelist_table}.code
-            {date_joins}
-            WHERE {date_condition}
-              AND NOT {ignored_day_condition}
-              AND {missing_value_condition}
+            ON CTV3Code = {codelist_table}.code
+            WHERE {date_condition} AND NOT {ignored_day_condition}
         ) t
-        GROUP BY registration_id, hashed_organisation
+        GROUP BY Patient_ID
         """
         return codelist_queries + extra_queries + [sql]
 
-    def _these_codes_occur_on_same_day(self, joined_table, codelist):
+    def _these_codes_occur_on_same_day(self, joined_table, codelist, date_condition):
         """
         Generates a SQL condition that filters rows in `joined_table` so that
-        they only include events which happened on days where none of the codes
-        in `codelist` occur in the CodedEvents table.
+        they only include events which happened on days where one of the codes
+        in `codelist` occur in the CodedEvents table. Usually we negate this
+        condition in the surrounding query so that we only includes days where
+        *none* of the codes occured.
 
         We use this to support queries like "give me all the times a patient
         was prescribed this drug, but ignore any days on which they were having
         their annual COPD review".
         """
         if codelist is None:
             return "0 = 1", []
-        codelist_table, queries = self.create_codelist_table(codelist)
+        assert codelist.system == "ctv3"
+        codelist_table, queries = self.create_codelist_table(
+            codelist, case_sensitive=True
+        )
+        same_day_table = self.get_temp_table_name("same_day_events")
+        queries += [
+            f"""
+            SELECT Patient_ID, CAST(ConsultationDate AS date) AS day
+            INTO {same_day_table}
+            FROM CodedEvent
+            INNER JOIN {codelist_table}
+            ON CTV3Code = {codelist_table}.code
+            WHERE {date_condition}
+            """,
+            f"""
+            CREATE CLUSTERED INDEX ix ON {same_day_table} (Patient_ID, day)
+            """,
+        ]
         condition = f"""
         EXISTS (
-          SELECT * FROM {OBSERVATION_TABLE} AS sameday
-          INNER JOIN {codelist_table}
-          ON sameday.snomed_concept_id = {codelist_table}.code
+          SELECT 1 FROM {same_day_table}
           WHERE
-            sameday.registration_id = {joined_table}.registration_id
-            AND CAST(sameday.effective_date AS date) = CAST({joined_table}.effective_date AS date)
+            {joined_table}.Patient_ID = {same_day_table}.Patient_ID
+            AND CAST({joined_table}.ConsultationDate AS date) = {same_day_table}.day
         )
         """
         return condition, queries
 
     def patients_registered_practice_as_of(self, date, returning=None):
-        # At the moment we can only return current values for the fields in question.
-
         if returning == "stp_code":
-            column = "stp_code"
-        # "msoa" is the correct option here, "msoa_code" is supported for
-        # backwards compatibility
-        elif returning in ("msoa", "msoa_code"):
-            column = "msoa"
+            column = "STPCode"
+        elif returning == "msoa_code":
+            column = "MSOACode"
         elif returning == "nuts1_region_name":
-            column = "english_region_name"
+            column = "Region"
         elif returning == "pseudo_id":
-            column = "hashed_organisation"
+            column = "Organisation_ID"
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
-
-        return f"""
-            SELECT
-              registration_id,
-              hashed_organisation,
-              {column} AS {returning}
-            FROM
-              {self.patient_no_duplicates_table}
-            """
-
-    def patients_date_deregistered_from_all_supported_practices(self, between):
-        date_condition, date_joins = self.get_date_condition(
-            self.patient_no_duplicates_table, "registration_end_date", between
-        )
+        # Note that current registrations are recorded with an EndDate of
+        # 9999-12-31. Where registration periods overlap we use the one with
+        # the most recent start date. If there are several with the same start
+        # date we use the longest one (i.e. with the latest end date).
         return f"""
         SELECT
-          registration_id,
-          hashed_organisation,
-          registration_end_date AS value
-        FROM {self.patient_no_duplicates_table}
-        {date_joins}
-        WHERE {date_condition}
+          Patient_ID AS patient_id,
+          Organisation.{column} AS {returning}
+        FROM (
+          SELECT Patient_ID, Organisation_ID,
+          ROW_NUMBER() OVER (
+            PARTITION BY Patient_ID
+            ORDER BY StartDate DESC, EndDate DESC, Registration_ID
+          ) AS rownum
+          FROM RegistrationHistory
+          WHERE StartDate <= {quote(date)} AND EndDate > {quote(date)}
+        ) t
+        LEFT JOIN Organisation
+        ON Organisation.Organisation_ID = t.Organisation_ID
+        WHERE t.rownum = 1
         """
 
-    def patients_with_death_recorded_in_primary_care(
-        self,
-        # Set date limits
-        between=None,
-        # Set return type
-        returning="binary_flag",
-    ):
-        if returning == "binary_flag":
-            column = "1"
-        elif returning == "date_of_death":
-            column = "date_of_death"
-        else:
-            raise ValueError(f"Unsupported `returning` value: {returning}")
+    def patients_date_deregistered_from_all_supported_practices(self, between):
         if between is None:
             between = (None, None)
         min_date, max_date = between
+        # Registrations with no end date are recorded using an end date of
+        # 9999-12-31, so if no max date is supplied then we need to set a max
+        # date to something less than 9999-12-31 to filter out registrations
+        # which have no end date.
         if max_date is None:
-            max_date = "9999-12-31"  # Far enough in the future to catch everyone
+            max_date = "3000-01-01"
         if min_date is None:
-            min_date = "1900-01-01"  # Far enough in the path to catch everyone
+            min_date = "1900-01-01"
         return f"""
         SELECT
-          registration_id,
-          hashed_organisation,
-          {column} AS {returning}
+          Patient_ID AS patient_id,
+          CASE
+            WHEN
+              MAX(EndDate) BETWEEN {quote(min_date)} AND {quote(max_date)}
+            THEN
+              MAX(EndDate)
+          END AS value
         FROM
-          {self.patient_no_duplicates_table}
-        WHERE
-          date_of_death BETWEEN {quote(min_date)} AND {quote(max_date)}
-        """
-
-    def patients_with_vaccination_record(
-        self,
-        tpp,
-        emis,
-        # Set date limits
-        between=None,
-        # Set return type
-        returning="binary_flag",
-        # Matching rule
-        find_first_match_in_period=None,
-        find_last_match_in_period=None,
-    ):
-        product_codes = emis.get("product_codes")
-        procedure_codes = emis.get("procedure_codes")
-
-        if returning not in ("binary_flag", "date"):
-            raise ValueError(f"Unsupported `returning` value: {returning}")
-
-        if find_first_match_in_period:
-            date_aggregate = "MIN"
-            date_comparator = "<"
-        else:
-            date_aggregate = "MAX"
-            date_comparator = ">"
-
-        codelist_queries = []
-        if product_codes:
-            product_codes_table, codelist_query = self.create_codelist_table(
-                product_codes
-            )
-            codelist_queries.extend(codelist_query)
-        if procedure_codes:
-            procedure_codes_table, codelist_query = self.create_codelist_table(
-                procedure_codes
-            )
-            codelist_queries.extend(codelist_query)
-
-        if procedure_codes and product_codes:
-            date_condition, date_joins = self.get_date_condition("t", "t.date", between)
-
-            subquery = f"""
-            SELECT
-                t.registration_id,
-                t.hashed_organisation,
-                t.date
-            FROM (
-                SELECT
-                    m.registration_id,
-                    m.hashed_organisation,
-                    CASE
-                        WHEN m.effective_date {date_comparator} i.effective_date THEN m.effective_date
-                        ELSE i.effective_date
-                    END AS date
-                FROM {MEDICATION_TABLE} AS m
-                INNER JOIN {IMMUNISATIONS_TABLE} AS i
-                    ON m.registration_id = i.registration_id
-                INNER JOIN {product_codes_table}
-                    ON m.snomed_concept_id = {product_codes_table}.code
-                INNER JOIN {procedure_codes_table}
-                    ON i.snomed_concept_id = {procedure_codes_table}.code
-            ) t
-            {date_joins}
-            WHERE {date_condition}
-            """
-
-        elif procedure_codes:
-            assert not product_codes
-
-            date_condition, date_joins = self.get_date_condition(
-                "i", "effective_date", between
-            )
-
-            subquery = f"""
-                SELECT
-                    i.registration_id,
-                    i.hashed_organisation AS hashed_organisation,
-                    1 AS has_event,
-                    DATE(i.effective_date) AS date
-                FROM {IMMUNISATIONS_TABLE} AS i
-                INNER JOIN {procedure_codes_table}
-                    ON i.snomed_concept_id = {procedure_codes_table}.code
-                {date_joins}
-                WHERE {date_condition}
-            """
-
-        elif product_codes:
-            assert not procedure_codes
-
-            date_condition, date_joins = self.get_date_condition(
-                "m", "effective_date", between
-            )
-
-            subquery = f"""
-                SELECT
-                    m.registration_id,
-                    m.hashed_organisation AS hashed_organisation,
-                    1 AS has_event,
-                    DATE(m.effective_date) AS date
-                FROM {MEDICATION_TABLE} AS m
-                INNER JOIN {product_codes_table}
-                    ON m.snomed_concept_id = {product_codes_table}.code
-                {date_joins}
-                WHERE {date_condition}
-            """
-
-        else:
-            raise ValueError(
-                "Provide at least one of `product_codes` or `procedure_codes`"
-            )
-
-        sql = f"""
-        SELECT
-            s.registration_id,
-            s.hashed_organisation,
-            1 AS binary_flag,
-            {date_aggregate}(DATE(s.date)) AS date
-        FROM ({subquery}) s
-        GROUP BY s.registration_id, s.hashed_organisation
+          RegistrationHistory
+        GROUP BY
+          Patient_ID
         """
 
-        return codelist_queries + [sql]
-
     def patients_address_as_of(self, date, returning=None, round_to_nearest=None):
-        # At the moment we can only return current values for the fields in question.
-
+        # N.B. A value of -1 indicates no postcode recorded on the
+        # record, an invalid postcode, or no fixed abode.
+        #
+        # Related, there is a column in the address table to indicate
+        # NP for no postcode or NFA for no fixed abode
         if returning == "index_of_multiple_deprivation":
             assert round_to_nearest == 100
-            column = "imd_rank"
+            column = "ImdRankRounded"
         elif returning == "rural_urban_classification":
             assert round_to_nearest is None
-            column = "rural_urban"
+            column = "RuralUrbanClassificationCode"
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
+        # Note that current addresses are recorded with an EndDate of
+        # 9999-12-31. Where address periods overlap we use the one with the
+        # most recent start date. If there are several with the same start date
+        # we use the longest one (i.e. with the latest end date). We then
+        # prefer addresses which are not marked "NPC" for "No Postcode" and
+        # finally we use the address ID as a tie-breaker.
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          {column} AS {returning}
+        FROM (
+          SELECT Patient_ID, {column},
+          ROW_NUMBER() OVER (
+            PARTITION BY Patient_ID
+            ORDER BY
+              StartDate DESC,
+              EndDate DESC,
+              IIF(MSOACode = 'NPC', 1, 0),
+              PatientAddress_ID
+          ) AS rownum
+          FROM PatientAddress
+          WHERE StartDate <= {quote(date)} AND EndDate > {quote(date)}
+        ) t
+        WHERE rownum = 1
+        """
 
+    def patients_care_home_status_as_of(self, date, categorised_as):
+        # These are the columns to which the categorisation expression is
+        # allowed to refer
+        allowed_columns = {
+            "IsPotentialCareHome": "ISNULL(PotentialCareHomeAddressID, 0)",
+            "LocationRequiresNursing": "LocationRequiresNursing",
+            "LocationDoesNotRequireNursing": "LocationDoesNotRequireNursing",
+        }
+        allowed_column_types = {
+            "IsPotentialCareHome": "int",
+            "LocationRequiresNursing": "str",
+            "LocationDoesNotRequireNursing": "str",
+        }
+        case_expression = self.get_case_expression(
+            allowed_column_types, allowed_columns, categorised_as
+        )
+        # See `patients_address_as_of` above for details of the ordering used
+        # here
         return f"""
-            SELECT
-              registration_id,
-              hashed_organisation,
-              {column} AS {returning}
-            FROM
-              {self.patient_no_duplicates_table}
-            """
+        SELECT
+          Patient_ID AS patient_id,
+          {case_expression} AS value
+        FROM (
+          SELECT
+            PatientAddress.Patient_ID AS Patient_ID,
+            PotentialCareHomeAddress.PatientAddress_ID AS PotentialCareHomeAddressID,
+            LocationRequiresNursing,
+            LocationDoesNotRequireNursing,
+            ROW_NUMBER() OVER (
+              PARTITION BY PatientAddress.Patient_ID
+              ORDER BY
+                StartDate DESC,
+                EndDate DESC,
+                IIF(MSOACode = 'NPC', 1, 0),
+                PatientAddress.PatientAddress_ID
+              ) AS rownum
+          FROM PatientAddress
+          LEFT JOIN PotentialCareHomeAddress
+          ON PatientAddress.PatientAddress_ID = PotentialCareHomeAddress.PatientAddress_ID
+          WHERE StartDate <= {quote(date)} AND EndDate > {quote(date)}
+        ) t
+        WHERE rownum = 1
+        """
 
     # https://github.com/ebmdatalab/tpp-sql-notebook/issues/72
     def patients_admitted_to_icu(
         self,
         between=None,
         find_first_match_in_period=None,
         find_last_match_in_period=None,
         returning="binary_flag",
     ):
-        date_expression = """
+        if find_first_match_in_period:
+            date_aggregate = "MIN"
+        else:
+            date_aggregate = "MAX"
+        date_expression = f"""
+        {date_aggregate}(
         CASE
         WHEN
-          COALESCE(date_format(icuadmissiondatetime, '%Y-%m-%d'), '9999-01-01')
-            < COALESCE(date_format(originalicuadmissiondate, '%Y-%m-%d'), '9999-01-01')
+          COALESCE(IcuAdmissionDateTime, '9999-01-01') < COALESCE(OriginalIcuAdmissionDate, '9999-01-01')
         THEN
-          DATE(icuadmissiondatetime)
+          IcuAdmissionDateTime
         ELSE
-          DATE(originalicuadmissiondate)
-        END"""
-        date_condition, date_joins = self.get_date_condition(
-            ICNARC_TABLE, date_expression, between
-        )
+          OriginalIcuAdmissionDate
+        END)"""
+        date_condition = make_date_filter(date_expression, between)
 
         greater_than_zero_expr = "CASE WHEN {} > 0 THEN 1 ELSE 0 END"
 
         if returning == "date_admitted":
-            if find_first_match_in_period:
-                column_definition = f"MIN({date_expression})"
-            else:
-                column_definition = f"MAX({date_expression})"
+            column_definition = date_expression
         elif returning == "binary_flag":
             column_definition = 1
         elif returning == "had_respiratory_support":
             column_definition = greater_than_zero_expr.format(
-                "SUM(basicdays_respiratorysupport) + SUM(advanceddays_respiratorysupport)"
+                "SUM(BasicDays_RespiratorySupport) + SUM(AdvancedDays_RespiratorySupport)"
             )
         elif returning == "had_basic_respiratory_support":
             column_definition = greater_than_zero_expr.format(
-                "SUM(basicdays_respiratorysupport)"
+                "SUM(BasicDays_RespiratorySupport)"
             )
         elif returning == "had_advanced_respiratory_support":
             column_definition = greater_than_zero_expr.format(
-                "SUM(advanceddays_respiratorysupport)"
+                "SUM(AdvancedDays_RespiratorySupport)"
             )
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
-
         return f"""
         SELECT
-          {ICNARC_TABLE}.registration_id AS registration_id,
-          {ICNARC_TABLE}.hashed_organisation AS hashed_organisation,
+          Patient_ID AS patient_id,
           {column_definition} AS {returning}
         FROM
-          {ICNARC_TABLE}
-        {date_joins}
-        WHERE {date_condition}
-        GROUP BY {ICNARC_TABLE}.registration_id, {ICNARC_TABLE}.hashed_organisation
+          ICNARC
+        GROUP BY Patient_ID
+        HAVING {date_condition}
         """
 
     def patients_with_these_codes_on_death_certificate(
         self,
         codelist=None,
         # Set date limits
         between=None,
         # Matching rules
         match_only_underlying_cause=False,
         # Set return type
         returning="binary_flag",
     ):
-        date_condition, date_joins = self.get_date_condition(
-            "p",
-            "date_parse(CAST(o.reg_stat_dod AS VARCHAR), '%Y%m%d')",
-            between,
-        )
+        date_condition = make_date_filter("dod", between)
         if codelist is not None:
             assert codelist.system == "icd10"
             codelist_sql = codelist_to_sql(codelist)
             code_columns = ["icd10u"]
             if not match_only_underlying_cause:
-                code_columns.extend([f"icd10{i:03d}" for i in range(1, 16)])
+                code_columns.extend([f"ICD10{i:03d}" for i in range(1, 16)])
             code_conditions = " OR ".join(
                 f"{column} IN ({codelist_sql})" for column in code_columns
             )
         else:
             code_conditions = "1 = 1"
         if returning == "binary_flag":
             column_definition = "1"
         elif returning == "date_of_death":
-            # Yes, we're converting an integer to a string to a timestamp to a date.
-            column_definition = (
-                "CAST(date_parse(CAST(o.reg_stat_dod AS VARCHAR), '%Y%m%d') AS date)"
-            )
+            column_definition = "dod"
+            # Quick fix: a patient appears twice in the ONS data with different
+            # dates of death (offset by one day). This results in an error when
+            # running the extract.  As we need to extract this cohort urgently
+            # we're going to use the minimum date for now, pending a full
+            # discussion of how best to handle this kind of inconsistency.
+            return f"""
+            SELECT Patient_ID as patient_id, MIN(dod) AS {returning}
+            FROM ONS_Deaths
+            WHERE ({code_conditions}) AND {date_condition}
+            GROUP BY patient_id
+            """
         elif returning == "underlying_cause_of_death":
-            column_definition = "o.icd10u"
+            column_definition = "icd10u"
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
-        # ONS_TABLE is updated with each release of data from ONS, so we need to
-        # filter for just the records which match the most recent upload_date
+        # The SELECT DISTINCT is because completely duplicate rows have previously appeared
+        # in the underlying dataset.
         return f"""
-            SELECT
-                p.registration_id,
-                p.hashed_organisation as hashed_organisation,
-                {column_definition} AS {returning}
-            FROM {ONS_TABLE} o
-            JOIN {self.patient_no_duplicates_table} p ON o.pseudonhsnumber = p.nhs_no
-            {date_joins}
-            WHERE ({code_conditions})
-                AND {date_condition}
-                AND o.upload_date = (SELECT MAX(upload_date) FROM {ONS_TABLE})
-            """
+        SELECT DISTINCT Patient_ID as patient_id, {column_definition} AS {returning}
+        FROM ONS_Deaths
+        WHERE ({code_conditions}) AND {date_condition}
+        """
 
     def patients_died_from_any_cause(
         self,
         # Set date limits
         between=None,
         # Set return type
         returning="binary_flag",
@@ -1572,147 +1193,646 @@
     def patients_with_death_recorded_in_cpns(
         self,
         # Set date limits
         between=None,
         # Set return type
         returning="binary_flag",
     ):
-        date_condition, date_joins = self.get_date_condition(
-            CPNS_TABLE, "dateofdeath", between
-        )
+        date_condition = make_date_filter("DateOfDeath", between)
         if returning == "binary_flag":
             column_definition = "1"
         elif returning == "date_of_death":
-            column_definition = "MAX(dateofdeath)"
+            column_definition = "MAX(DateOfDeath)"
         else:
             raise ValueError(f"Unsupported `returning` value: {returning}")
         return f"""
-            SELECT
-              {CPNS_TABLE}.registration_id,
-              {CPNS_TABLE}.hashed_organisation,
-              {column_definition} AS {returning},
-              -- Crude error check so we blow up in the case of inconsistent dates
-              1 / CASE WHEN MAX(dateofdeath) = MIN(dateofdeath) THEN 1 ELSE 0 END AS _e
-            FROM {CPNS_TABLE}
-            {date_joins}
-            WHERE {date_condition}
-            GROUP BY {CPNS_TABLE}.registration_id, {CPNS_TABLE}.hashed_organisation
-            """
+        SELECT
+          Patient_ID as patient_id,
+          {column_definition} AS {returning},
+          -- Crude error check so we blow up in the case of inconsistent dates
+          1 / CASE WHEN MAX(DateOfDeath) = MIN(DateOfDeath) THEN 1 ELSE 0 END AS _e
+        FROM CPNS
+        WHERE {date_condition}
+        GROUP BY Patient_ID
+        """
 
-    def get_db_connection(self):
-        if self._db_connection:
-            return self._db_connection
-        self._db_connection = LoggingDatabaseConnection(
-            logger,
-            trino_connection_from_url(self.database_url),
-            truncate=self.truncate_sql_logs,
+    def patients_with_death_recorded_in_primary_care(
+        self,
+        # Set date limits
+        between=None,
+        # Set return type
+        returning="binary_flag",
+    ):
+        if returning == "binary_flag":
+            column = "1"
+        elif returning == "date_of_death":
+            column = "DateOfDeath"
+        else:
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+        if between is None:
+            between = (None, None)
+        min_date, max_date = between
+        # Patients with no date of death (i.e. alive ones) are recorded using a
+        # death date of 9999-12-31, so if no max date is supplied then we need
+        # to set a max date to something less than 9999-12-31 to filter these
+        # out
+        if max_date is None:
+            max_date = "3000-01-01"
+        if min_date is None:
+            min_date = "1900-01-01"
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          {column} AS {returning}
+        FROM
+          Patient
+        WHERE
+          DateOfDeath BETWEEN {quote(min_date)} AND {quote(max_date)}
+        """
+
+    def patients_with_tpp_vaccination_record(
+        self,
+        target_disease_matches=None,
+        product_name_matches=None,
+        # Set date limits
+        between=None,
+        # Set return type
+        returning="binary_flag",
+        # Matching rule
+        find_first_match_in_period=None,
+        find_last_match_in_period=None,
+        include_date_of_match=False,
+    ):
+        conditions = [make_date_filter("VaccinationDate", between)]
+        target_disease_matches = to_list(target_disease_matches)
+        if target_disease_matches:
+            content_codes = codelist_to_sql(target_disease_matches)
+            conditions.append(f"ref.VaccinationContent IN ({content_codes})")
+
+        product_name_matches = to_list(product_name_matches)
+        if product_name_matches:
+            product_name_codes = codelist_to_sql(product_name_matches)
+            conditions.append(f"ref.VaccinationName IN ({product_name_codes})")
+
+        conditions_str = " AND ".join(conditions)
+
+        # Result ordering
+        if find_first_match_in_period:
+            date_aggregate = "MIN"
+        else:
+            date_aggregate = "MAX"
+
+        if returning not in ("binary_flag", "date"):
+            # Because each Vaccination row can potentially map to multiple
+            # VaccinationReference rows (one for each disease targeted by the
+            # vaccine) anything beyond a simple binary flag or a date is going to
+            # require more thought.
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          1 AS binary_flag,
+          {date_aggregate}(VaccinationDate) AS date
+        FROM Vaccination
+        INNER JOIN VaccinationReference AS ref
+        ON ref.VaccinationName_ID = Vaccination.VaccinationName_ID
+        WHERE {conditions_str}
+        GROUP BY Patient_ID
+        """
+
+    def patients_with_gp_consultations(
+        self,
+        # Set date limits
+        between=None,
+        # Matching rule
+        find_first_match_in_period=None,
+        find_last_match_in_period=None,
+        # Set return type
+        returning="binary_flag",
+        include_date_of_match=False,
+    ):
+        if returning == "binary_flag" or returning == "date":
+            column_name = "binary_flag"
+            column_definition = "1"
+        elif returning == "number_of_matches_in_period":
+            column_name = returning
+            column_definition = "COUNT(*)"
+        else:
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+
+        valid_states = [
+            AppointmentStatus.ARRIVED,
+            AppointmentStatus.WAITING,
+            AppointmentStatus.IN_PROGRESS,
+            AppointmentStatus.FINISHED,
+            AppointmentStatus.PATIENT_WALKED_OUT,
+            AppointmentStatus.VISIT,
+        ]
+        valid_states_str = codelist_to_sql(map(int, valid_states))
+
+        date_condition = make_date_filter("SeenDate", between)
+        # Result ordering
+        date_aggregate = "MIN" if find_first_match_in_period else "MAX"
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          {column_definition} AS {column_name},
+          {date_aggregate}(SeenDate) AS date
+        FROM Appointment
+        WHERE Status IN ({valid_states_str}) AND {date_condition}
+        GROUP BY Patient_ID
+        """
+
+    def patients_with_complete_gp_consultation_history_between(
+        self, start_date, end_date
+    ):
+        """
+        In this context this should mean patients who have been continuously
+        registered with TPP-using practices throughout this period. However,
+        for now we restrict this to just patients who have been registered with
+        a single practice throughout this period.  As this is a more
+        restrictive condition this is fine for our purposes, however once we
+        get an implementation for `patients_with_complete_history_between` we
+        should switch to using this.
+        """
+        return self.patients_registered_with_one_practice_between(
+            start_date, end_date, practice_used_systm_one_throughout_period=True
         )
-        return self._db_connection
 
-    def close(self):
-        if self._db_connection:
-            self._db_connection.close()
-        self._db_connection = None
+    def patients_with_test_result_in_sgss(
+        self,
+        pathogen=None,
+        test_result=None,
+        # Set date limits
+        between=None,
+        # Matching rule
+        find_first_match_in_period=None,
+        find_last_match_in_period=None,
+        # Set return type
+        returning="binary_flag",
+        include_date_of_match=False,
+    ):
+        assert pathogen == "SARS-CoV-2"
+        assert test_result in ("positive", "negative", "any")
+        if returning not in ("binary_flag", "date"):
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+
+        date_condition = make_date_filter("date", between)
+        date_aggregate = "MIN" if find_first_match_in_period else "MAX"
+        if test_result == "any":
+            result_condition = "1 = 1"
+        else:
+            flag = 1 if test_result == "positive" else 0
+            result_condition = f"test_result = {quote(flag)}"
+
+        # These are the values we're expecting in our SGSS tables. If we ever
+        # get anything other than these we should throw an error rather than
+        # blindly continuing.
+        positive_descr = "SARS-CoV-2 CORONAVIRUS (Covid-19)"
+        negative_descr = "NEGATIVE SARS-CoV-2 (COVID-19)"
 
+        return f"""
+        SELECT
+          patient_id,
+          1 AS binary_flag,
+          {date_aggregate}(date) AS date,
+          -- We have to calculate something over the error check field
+          -- otherwise it never gets computed
+          MAX(_e) AS _e
+        FROM (
+          SELECT
+            1 AS test_result,
+            Patient_ID AS patient_id,
+            Earliest_Specimen_Date AS date,
+            -- Crude error check so we blow up in the case of unexpected data
+            1 / CASE WHEN Organism_Species_Name = '{positive_descr}' THEN 1 ELSE 0 END AS _e
+          FROM SGSS_Positive
+          UNION ALL
+          SELECT
+            0 AS test_result,
+            Patient_ID AS patient_id,
+            Earliest_Specimen_Date AS date,
+            -- Crude error check so we blow up in the case of unexpected data
+            1 / CASE WHEN Organism_Species_Name = '{negative_descr}' THEN 1 ELSE 0 END AS _e
+          FROM SGSS_Negative
+        ) t
+        WHERE {date_condition} AND {result_condition}
+        GROUP BY patient_id
+        """
 
-class ColumnExpression:
-    def __init__(
+    def patients_household_as_of(self, reference_date, returning):
+        if reference_date != "2020-02-01":
+            raise ValueError("Household data only currently available for 2020-02-01")
+        if returning == "pseudo_id":
+            column = "Household.Household_ID"
+        elif returning == "household_size":
+            column = "Household.HouseholdSize"
+        elif returning == "is_prison":
+            column = "CASE Household.Prison WHEN 'TRUE' THEN 1 ELSE 0 END"
+        elif returning == "has_members_in_other_ehr_systems":
+            column = (
+                "CASE Household.MixedSoftwareHousehold WHEN 'TRUE' THEN 1 ELSE 0 END"
+            )
+        elif returning == "percentage_of_members_with_data_in_this_backend":
+            column = "Household.TppPercentage"
+        elif returning == "msoa":
+            column = "Household.MSOA"
+        else:
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+        return f"""
+        SELECT
+          Patient_ID AS patient_id,
+          {column} AS {returning}
+        FROM HouseholdMember
+        INNER JOIN Household
+        ON HouseholdMember.Household_ID = Household.Household_ID
+        WHERE Household.NFA_Unknown != 1
+        """
+
+    def patients_attended_emergency_care(
         self,
-        # SQL fragment
-        expression,
-        # The column type returned by the above expression
-        type=None,
-        # The default value of the expression for missing values
-        default_value=None,
-        # The names of all tables used in evaluating the expression
-        source_tables=(),
-        # Indicates whether the column is included in the output
-        is_hidden=False,
-        # Only relevant for columns of type "date": records the format in which
-        # the date is represented
-        date_format=None,
+        between=None,
+        returning=None,
+        find_first_match_in_period=None,
+        find_last_match_in_period=None,
+        with_these_diagnoses=None,
+        discharged_to=None,
     ):
-        self.expression = expression
-        self.type = type
-        self.default_value = default_value
-        self.source_tables = source_tables
-        self.is_hidden = is_hidden
-        self.date_format = date_format
+        if find_first_match_in_period:
+            ordering = "ASC"
+            date_aggregate = "MIN"
+        else:
+            ordering = "DESC"
+            date_aggregate = "MAX"
+
+        if returning == "binary_flag":
+            column = "1"
+            use_partition_query = False
+        elif returning == "date_arrived":
+            column = f"{date_aggregate}(Arrival_Date)"
+            use_partition_query = False
+        elif returning == "number_of_matches_in_period":
+            column = "COUNT(*)"
+            use_partition_query = False
+        elif returning == "discharge_destination":
+            column = "Discharge_Destination_SNOMED_CT"
+            use_partition_query = True
+        else:
+            assert False
 
-    def __str__(self):
-        return self.expression
+        conditions = [make_date_filter("Arrival_Date", between)]
 
+        if with_these_diagnoses:
+            assert isinstance(with_these_diagnoses, list)
+            assert isinstance(with_these_diagnoses[0], str)
+            codes = ", ".join(map(quote, with_these_diagnoses))
+            fragments = [f"EC_Diagnosis_{ix:02} IN ({codes})" for ix in range(1, 25)]
+            conditions.append("(" + " OR ".join(fragments) + ")")
+
+        if discharged_to:
+            assert isinstance(discharged_to, list)
+            assert isinstance(discharged_to[0], str)
+            codes = ", ".join(map(quote, discharged_to))
+            conditions.append(f"Discharge_Destination_SNOMED_CT IN ({codes})")
 
-def codelist_to_sql(codelist):
-    cast = int if codelist.system in ("snomed", "snomedct") else str
+        conditions = " AND ".join(conditions)
+
+        if use_partition_query:
+            # Note EC_Ident is not guaranteed unique by the database but I
+            # suspect it is intended to be unique by the source. Out of ~20m
+            # rows currently there are only two duplicate EC_Idents and these
+            # are for rows identical in all respects apart from Patient_ID.
+            # Thus while using EC_Ident as the final sort column below doesn't
+            # absolutely *guaranteee* a deterministic sort order, I think it's
+            # good enough.
+            sql = f"""
+            SELECT
+              Patient_ID AS patient_id,
+              {column} AS {returning}
+            FROM (
+              SELECT EC.Patient_ID, {column},
+              ROW_NUMBER() OVER (
+                PARTITION BY EC.Patient_ID
+                ORDER BY Arrival_Date {ordering}, EC.EC_Ident
+              ) AS rownum
+              FROM EC
+              INNER JOIN EC_Diagnosis
+                ON EC.EC_Ident = EC_Diagnosis.EC_Ident
+              WHERE {conditions}
+            ) t
+            WHERE rownum = 1
+            """
+        else:
+            sql = f"""
+            SELECT
+              EC.Patient_ID AS patient_id,
+              {column} AS {returning}
+            FROM EC
+            INNER JOIN EC_Diagnosis
+              ON EC.EC_Ident = EC_Diagnosis.EC_Ident
+            WHERE {conditions}
+            GROUP BY EC.Patient_ID
+            """
+        return sql
+
+    def patients_admitted_to_hospital(
+        self,
+        between=None,
+        returning=None,
+        find_first_match_in_period=None,
+        find_last_match_in_period=None,
+        with_these_primary_diagnoses=None,
+        with_these_diagnoses=None,
+        with_these_procedures=None,
+    ):
+        if find_first_match_in_period:
+            ordering = "ASC"
+            date_aggregate = "MIN"
+        else:
+            ordering = "DESC"
+            date_aggregate = "MAX"
+
+        if returning == "binary_flag":
+            column = "1"
+            use_partition_query = False
+        elif returning == "date_admitted":
+            column = f"{date_aggregate}(Admission_Date)"
+            use_partition_query = False
+        elif returning == "date_discharged":
+            column = f"{date_aggregate}(Discharge_Date)"
+            use_partition_query = False
+        elif returning == "number_of_matches_in_period":
+            column = "COUNT(*)"
+            use_partition_query = False
+        elif returning == "primary_diagnosis":
+            column = "Spell_Primary_Diagnosis"
+            use_partition_query = True
+        else:
+            raise ValueError(f"Unsupported `returning` value: {returning}")
+
+        conditions = [make_date_filter("Admission_Date", between)]
+
+        if with_these_primary_diagnoses:
+            assert with_these_primary_diagnoses.system == "icd10"
+            codes_sql = codelist_to_sql(with_these_primary_diagnoses)
+            conditions.append(f"APCS_Der.Spell_Primary_Diagnosis IN ({codes_sql})")
+
+        if with_these_diagnoses:
+            assert with_these_diagnoses.system == "icd10"
+            fragments = [
+                f"Der_Diagnosis_All LIKE {pattern}"
+                for pattern in codelist_to_like_patterns(
+                    with_these_diagnoses, prefix="%[^A-Za-z0-9]", suffix="%"
+                )
+            ]
+            conditions.append("(" + " OR ".join(fragments) + ")")
+
+        if with_these_procedures:
+            assert with_these_procedures.system == "icd10"
+            fragments = [
+                f"Der_Procedure_All LIKE {pattern}"
+                for pattern in codelist_to_like_patterns(
+                    with_these_procedures, prefix="%[^A-Za-z0-9]", suffix="%"
+                )
+            ]
+            conditions.append("(" + " OR ".join(fragments) + ")")
+
+        conditions = " AND ".join(conditions)
+
+        if use_partition_query:
+            # Note APCS_Ident is not guaranteed unique by the database but I
+            # suspect it is intended to be unique by the source. For one thing,
+            # it seems to be used as a foreign key in the other ACDS tables.
+            # And out of ~3.5m rows currently there are only four duplicate
+            # APCS_Idents and these are for rows identical in all respects
+            # apart from Patient_ID.  Thus while using APCS_Ident as the final
+            # sort column below doesn't absolutely *guaranteee* a deterministic
+            # sort order, I think it's good enough.
+            sql = f"""
+            SELECT
+              Patient_ID AS patient_id,
+              {column} AS {returning}
+            FROM (
+              SELECT APCS.Patient_ID, {column},
+              ROW_NUMBER() OVER (
+                PARTITION BY APCS.Patient_ID
+                ORDER BY Admission_Date {ordering}, APCS.APCS_Ident
+              ) AS rownum
+              FROM APCS
+              INNER JOIN APCS_Der
+                ON APCS.APCS_Ident = APCS_Der.APCS_Ident
+              WHERE {conditions}
+            ) t
+            WHERE rownum = 1
+            """
+        else:
+            sql = f"""
+            SELECT
+              APCS.Patient_ID AS patient_id,
+              {column} AS {returning}
+            FROM APCS
+            INNER JOIN APCS_Der
+              ON APCS.APCS_Ident = APCS_Der.APCS_Ident
+            WHERE {conditions}
+            GROUP BY APCS.Patient_ID
+            """
+        return sql
+
+    def get_case_expression(
+        self, column_types, column_definitions, category_definitions
+    ):
+        category_definitions = category_definitions.copy()
+        defaults = [k for (k, v) in category_definitions.items() if v == "DEFAULT"]
+        if len(defaults) > 1:
+            raise ValueError("At most one default category can be defined")
+        if len(defaults) == 1:
+            default_value = defaults[0]
+            category_definitions.pop(default_value)
+        else:
+            raise ValueError(
+                "At least one category must be given the definition 'DEFAULT'"
+            )
+        # For each column already defined, determine its corresponding "empty"
+        # value (i.e. the default value for that column's type). This allows us
+        # to support implicit boolean conversion because we know what the
+        # "falsey" value for each column should be.
+        empty_value_map = {
+            name: self.get_default_value_for_type(column_type)
+            for name, column_type in column_types.items()
+        }
+        clauses = []
+        for category, expression in category_definitions.items():
+            # The column references in the supplied expression need to be
+            # rewritten to ensure they refer to the correct CTE. The formatting
+            # function also ensures that the expression matches the very
+            # limited subset of SQL we support here.
+            formatted_expression = format_expression(
+                expression, column_definitions, empty_value_map=empty_value_map
+            )
+            clauses.append(f"WHEN ({formatted_expression}) THEN {quote(category)}")
+        return f"CASE {' '.join(clauses)} ELSE {quote(default_value)} END"
+
+    def get_aggregate_expression(
+        self, column_type, column_definitions, column_names, aggregate_function
+    ):
+        assert aggregate_function in ("MIN", "MAX")
+        default_value = quote(self.get_default_value_for_type(column_type))
+        # In other databases we could use GREATEST/LEAST to aggregate over
+        # columns, but for MSSQL we need to use this Table Value Constructor
+        # trick: https://stackoverflow.com/a/6871572
+        components = ", ".join(f"({column_definitions[name]})" for name in column_names)
+        aggregate_expression = (
+            f"SELECT {aggregate_function}(value)"
+            f" FROM (VALUES {components}) AS _table(value)"
+            # This is slightly awkward: MIN and MAX ignore NULL values which is
+            # the behaviour we want here. For instance, given a column like:
+            #
+            #   minimum_of("covid_test_date", "hosptial_admission_date")
+            #
+            # We want this value to be equal to "covid_test_date" for patients
+            # which have not been admitted to hospital (i.e. patients for which
+            # "hospital_admission_date" is NULL).
+            #
+            # However, the values we have here have already been passed through
+            # the `ISNULL` function to replace NULLs with a default value
+            # (which for dates is the empty string). This means that if we just
+            # took the minimum over these values in the example above, we'd get
+            # the empty string from "hosptial_admission_date" rather than the
+            # value in "covid_test_date".
+            #
+            # To workaround this we add a WHERE clause to filter out any
+            # default values (essentially treating them as if they were NULL).
+            # This gives us the result we want but it does mean we can't
+            # distinguish e.g. a recorded value of 0.0 from a missing value.
+            # This, however, is a general problem with the way we handle NULLs
+            # in our system, and so we're not introducing any new difficulty
+            # here.  (It's also unlikely to be a problem in practice.)
+            f" WHERE value != {default_value}"
+        )
+        return f"ISNULL(({aggregate_expression}), {default_value})"
+
+
+def codelist_to_sql_list(codelist):
     if getattr(codelist, "has_categories", False):
-        values = [quote(cast(code)) for (code, category) in codelist]
+        return [quote(code) for (code, category) in codelist]
     else:
-        values = [quote(cast(code)) for code in codelist]
-    return ",".join(values)
+        return [quote(code) for code in codelist]
 
 
-def is_iso_date(value):
-    return bool(re.match(r"\d\d\d\d-\d\d-\d\d", value))
+def codelist_to_like_patterns(codelist, prefix="", suffix=""):
+    patterns = []
+    for quoted_code in codelist_to_sql_list(codelist):
+        assert quoted_code[0] == "'"
+        assert quoted_code[-1] == "'"
+        patterns.append(f"'{prefix}{quoted_code[1:-1]}{suffix}'")
+    return patterns
 
 
-def quote(value, reformat_dates=True):
-    if isinstance(value, (int, float)):
-        if math.isnan(value):
-            return "NULL"
-        else:
-            return str(value)
+def codelist_to_sql(codelist):
+    return ",".join(codelist_to_sql_list(codelist))
 
-    value = str(value)
-    if reformat_dates:
-        try:
-            datetime.datetime.strptime(value, "%Y-%m-%d")
-            return f"DATE('{value}')"
-        except ValueError:
-            pass
-
-    if not SAFE_CHARS_RE.match(value) and value != "":
-        raise ValueError(f"Value contains disallowed characters: {value}")
-    return f"'{value}'"
+
+def to_list(value):
+    if value is None:
+        return []
+    if not isinstance(value, (tuple, list)):
+        return [value]
+    return list(value)
 
 
-def remove_lower_date_bound(between):
-    if between is not None:
-        return (None, between[1])
+def standardise_if_date(value):
+    """For strings that look like ISO dates, format in a SQL-Server
+    friendly fashion
+
+    """
+
+    # ISO date strings with hyphens are unreliable in SQL Server:
+    # https://stackoverflow.com/a/25548626/559140
+    try:
+        date = datetime.datetime.strptime(value, "%Y-%m-%d")
+        value = date.strftime("%Y%m%d")
+    except ValueError:
+        pass
+    return value
+
+
+def quote(value):
+    if isinstance(value, (int, float)):
+        return str(value)
+    else:
+        value = str(value)
+        value = standardise_if_date(value)
+        if not SAFE_CHARS_RE.match(value) and value != "":
+            raise ValueError(f"Value contains disallowed characters: {value}")
+        return f"'{value}'"
+
+
+def make_date_filter(column, between, upper_bound_only=False):
+    if between is None:
+        between = (None, None)
+    min_date, max_date = between
+    if upper_bound_only:
+        min_date = None
+    if min_date is not None and max_date is not None:
+        return f"{column} BETWEEN {quote(min_date)} AND {quote(max_date)}"
+    elif min_date is not None:
+        return f"{column} >= {quote(min_date)}"
+    elif max_date is not None:
+        return f"{column} <= {quote(max_date)}"
+    else:
+        return "1=1"
 
 
 def truncate_date(column, date_format):
     if date_format == "YYYY" or date_format is None:
-        date_format = "%Y"
+        date_length = 4
     elif date_format == "YYYY-MM":
-        date_format = "%Y-%m"
+        date_length = 7
     elif date_format == "YYYY-MM-DD":
-        date_format = "%Y-%m-%d"
+        date_length = 10
     else:
         raise ValueError(f"Unhandled date format: {date_format}")
-    return f"date_format({column}, '{date_format}')"
+    # Style 23 below means YYYY-MM-DD format, see:
+    # https://docs.microsoft.com/en-us/sql/t-sql/functions/cast-and-convert-transact-sql?view=sql-server-ver15#date-and-time-styles
+    return f"CONVERT(VARCHAR({date_length}), {column}, 23)"
+
+
+class UniqueCheck:
+    def __init__(self):
+        self.count = 0
+        self.ids = set()
+
+    def add(self, item):
+        self.count += 1
+        self.ids.add(item)
+
+    def assert_unique_ids(self):
+        duplicates = self.count - len(self.ids)
+        if duplicates != 0:
+            raise RuntimeError(f"Duplicate IDs found ({duplicates} rows)")
 
 
 def pop_keys_from_dict(dictionary, keys):
     new_dict = {}
     for key in keys:
         if key in dictionary:
             new_dict[key] = dictionary.pop(key)
     return new_dict
 
 
-def get_organisation_hash():
-    return os.environ["EMIS_ORGANISATION_HASH"]
-
-
-def truncate_patient_id(patient_id):
-    """
-    EMIS patient IDs are 128 byte strings which significantly bloat our output
-    files. However, because they are actually hex-encoded SHA-512 hashes we can
-    get away with throwing away all but the first 63 bits and storing them as
-    int64s (63 bits so we can safely store them as signed int64s without
-    worrying about negative patient IDs, which might upset expectations
-    elsewhere). 63 bits still gives us plenty of entropy as sqrt(2^63) is about
-    2 billion so well above the threshold where we'd need to worry about
-    collisions with a population of a few tens of millions.
-    """
-    return int(patient_id[:16], 16) >> 1
+class AppointmentStatus(enum.IntEnum):
+    BOOKED = 0
+    ARRIVED = 1
+    DID_NOT_ATTEND = 2
+    IN_PROGRESS = 3
+    FINISHED = 4
+    REQUESTED = 5
+    BLOCKED = 6
+    VISIT = 8
+    WAITING = 9
+    CANCELLED_BY_PATIENT = 10
+    CANCELLED_BY_UNIT = 11
+    CANCELLED_BY_OTHER_SERVICE = 12
+    NO_ACCESS_VISIT = 14
+    CANCELLED_DUE_TO_DEATH = 15
+    PATIENT_WALKED_OUT = 16
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/expectation_generators.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/expectation_generators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import os
 from datetime import datetime
-
-import numpy as np
+from scipy.stats import expon
+from scipy.stats import rv_discrete
+from scipy.stats import norm
+from scipy.stats import uniform
 import pandas as pd
-from scipy.stats import expon, norm, poisson, rv_discrete, uniform
+import numpy as np
+import os
 
 
 def generate_ages(population, max_age=110):
     """Generate a population whose ages approximate UK population shape"""
 
     df = pd.read_csv(
         os.path.join(os.path.dirname(__file__), "uk_population_bands_2018.csv")
@@ -106,60 +108,40 @@
 
     int_ = kwargs.pop("int", None)
     if int_:
         if int_["distribution"] == "normal":
             mean = int_["mean"]
             stddev = int_["stddev"]
             df["int"] = norm.rvs(loc=mean, scale=stddev, size=population).astype("int")
-        elif int_["distribution"] == "poisson":
-            mean = int_["mean"]
-            df["int"] = poisson.rvs(mu=mean, size=population)
         elif int_["distribution"] == "population_ages":
             # A distribution that is something like a real UK population
             df["int"] = generate_ages(population)
         else:
             raise ValueError(
-                "Only `normal`, `poisson`, and `population_ages` distributions currently supported for ints"
+                "Only `normal` and `population_ages` distributions currently supported"
             )
     float_ = kwargs.pop("float", None)
     if float_:
         if float_["distribution"] == "normal":
             mean = float_["mean"]
             stddev = float_["stddev"]
             df["float"] = norm.rvs(loc=mean, scale=stddev, size=population)
         else:
             raise ValueError(
-                "Only `normal` distributions currently supported for floats"
+                "Only `normal` and `population_ages` distributions currently supported"
             )
 
     bool_ = kwargs.pop("bool", None)
     if bool_:
-        df["bool"] = 1
+        df["bool"] = True
 
     assert not kwargs, f"Encountered unexpected arguments: {kwargs}"
 
     if match_incidence is not None:
         # Remove rows to match the incidence of the passed-in series
-        set_empty_values(df, pd.isnull(match_incidence))
+        df.loc[pd.isnull(match_incidence), :] = None
     elif not universal:
         # Randomly remove rows to match incidence
-        set_empty_values(df, df.sample(n=int((1 - incidence) * population)).index)
+        df.loc[df.sample(n=int((1 - incidence) * population)).index, :] = None
     if date is None:
         df = df.drop("date", axis=1)
     return df
-
-
-def set_empty_values(df, row_selection):
-    empty_values = {
-        "bool": 0,
-        "int": 0,
-        "float": 0.0,
-        # Note this is intentionally `None` rather than `""` because at this
-        # point in the dummy data generation process these are DateTime objects
-        # not ISO strings and we can't mix types in the dataframe. When these
-        # get converted to strings during the CSV generation, the nulls become
-        # empty strings as expected.
-        "date": None,
-        "category": None,
-    }
-    for column in df.columns:
-        df.loc[row_selection, column] = empty_values.get(column, "")
```

### Comparing `opensafely-cohort-extractor-1.85.0/cohortextractor/expressions.py` & `opensafely-cohort-extractor-1.9.0/cohortextractor/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import re
 import sqlite3
 
 import sqlparse
 from sqlparse import tokens as ttypes
 
+
 IGNORE = object()
 
-# As well as alphanumeric, underscore, and space characters, which are generally used
-# for category names, we also have "comparator" categories for which we need to allow
-# the corresponding characters.
-SAFE_CHARS_RE = re.compile(r"^[a-zA-Z0-9_ <>=~]+$")
+SAFE_CHARS_RE = re.compile(r"^[a-zA-Z0-9_]+$")
 
 
 class InvalidExpressionError(ValueError):
     pass
 
 
 class UnknownColumnError(InvalidExpressionError):
     pass
 
 
 def format_expression(expression, name_map, empty_value_map):
     """
     Take an SQL expression (in a very limited dialect) and a column name
     mapping and return a reformatted expression with column references
-    rewritten using the supplied mapping, along with a set of all the names
-    used within the expression.
+    rewritten using the supplied mapping.
 
     `empty_value_map` is a dict giving the "empty" or falsey value appropriate
     to the type of each column. Any column references that are not involved in
     an explicit comparison are rewritten as `!= <empty value>`.
 
     For example, the expression
 
@@ -50,32 +47,29 @@
     tokens = list(tokens)
     try:
         validate_expression(tokens, empty_value_map)
     except InvalidExpressionError as e:
         raise InvalidExpressionError(
             f"Invalid SQL expression: {expression}\nError: {e}"
         )
-    names_referenced = set()
-    tokens = remap_names(tokens, name_map, names_referenced)
-    new_expression = " ".join(token.value for token in tokens)
-    return new_expression, names_referenced
+    tokens = remap_names(tokens, name_map)
+    return " ".join(token.value for token in tokens)
 
 
-def remap_names(tokens, name_map, names_referenced):
+def remap_names(tokens, name_map):
     """
     Takes an iterable of tokens and remaps any names found within using the
     `name_map` dictionary. Names not found in the map are an error.
     """
     for token in tokens:
         if token.ttype is ttypes.Name:
             try:
                 name = name_map[token.value]
             except KeyError:
                 raise UnknownColumnError(f"Unknown column: {token.value}")
-            names_referenced.add(token.value)
             yield sqlparse.sql.Token(ttypes.Name, name)
         else:
             yield token
 
 
 def filter_and_validate_tokens(tokens):
     """
@@ -95,20 +89,20 @@
         elif status is not IGNORE:
             raise RuntimeError(f"Invalid status return value: {status}")
 
 
 def validate_string(token):
     # Remove quotes
     value = token.value[1:-1]
-    if len(value) > 64:
-        raise ValueError(f"String literals must be 64 characters or less: {value}")
-    if not SAFE_CHARS_RE.match(value) and not value == "":
+    if len(value) > 16:
+        raise ValueError(f"String literals must be 16 characters or less: {value}")
+    if not SAFE_CHARS_RE.match(value):
         raise ValueError(
-            f"String literals can only contain alphanumeric characters, "
-            f"underscore and the comparators '<', '>', '=', and '~': {value}"
+            f"String literals can only contain alphanumeric characters and "
+            f"underscore: {value}"
         )
     return sqlparse.sql.Token(ttypes.Literal.String.Single, f"'{value}'")
 
 
 def is_allowed(token):
     """
     Does the supplied token match the limited range of allowed tokens or should
@@ -165,20 +159,18 @@
             yield token
         previous_ttype = token.ttype
 
 
 def token_for_value(value):
     if value == 0:
         return sqlparse.sql.Token(ttypes.Number.Integer, "0")
-    elif value == -1:
-        return sqlparse.sql.Token(ttypes.Number.Integer, "-1")
     elif value == "":
         return sqlparse.sql.Token(ttypes.Literal.String.Single, "''")
     else:
-        raise ValueError(f"Invalid empty value: {value}")
+        raise ValueError(f"Invalid empty value: f{value}")
 
 
 def validate_expression(tokens, empty_value_map):
     """
     Perform basic syntactic validation on the supplied expression
 
     This involves transforming it back into SQL and attempting to execute it
```

### Comparing `opensafely-cohort-extractor-1.85.0/setup.py` & `opensafely-cohort-extractor-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,32 @@
 import os
+from setuptools import setup, find_packages
 
-from setuptools import find_packages, setup
 
-try:
-    with open(os.path.join("cohortextractor", "VERSION")) as f:
-        version = f.read().strip()
-except Exception:
-    version = "99.99.99.dev1"
+with open(os.path.join("cohortextractor", "VERSION")) as f:
+    version = f.read().strip()
 
 setup(
     name="opensafely-cohort-extractor",
     version=version,
     packages=find_packages(),
     url="https://github.com/opensafely/cohort-extractor",
     author="OpenSAFELY",
     author_email="tech@opensafely.org",
     python_requires=">=3.7",
     install_requires=[
-        "lz4",  # implicit import for compressed feather files
-        "pyarrow",
+        "opensafely-jobrunner>=1.7.0",
         "pandas",
+        "prettytable",
         "pyyaml",
         "requests",
-        "retry",
         "seaborn",
+        "sqlalchemy",
         "sqlparse",
-        "structlog",
-        "tabulate",
+        "tinynetrc",
     ],
-    extras_require={
-        "drivers": [
-            # Used by the EMIS backend
-            "presto-python-client",
-            # Used by the TPP backend
-            "pymssql",
-        ]
-    },
     entry_points={
         "console_scripts": ["cohortextractor=cohortextractor.cohortextractor:main"]
     },
     include_package_data=True,
     classifiers=["License :: OSI Approved :: GNU General Public License v3 (GPLv3)"],
 )
```

### Comparing `opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations.py` & `opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import csv
 
-from cohortextractor import codelist
-from cohortextractor.dashboards.vaccinations import VaccinationsStudyDefinition
-from tests.test_tpp_backend import set_database_url, setup_function, setup_module
+from tests.test_tpp_backend import set_database_url, setup_module, setup_function
 from tests.tpp_backend_setup import (
-    CodedEvent,
-    MedicationDictionary,
-    MedicationIssue,
-    Organisation,
+    make_session,
     Patient,
     RegistrationHistory,
+    Organisation,
     Vaccination,
-    make_session,
+    MedicationIssue,
+    MedicationDictionary,
+    CodedEvent,
 )
 
+from cohortextractor import codelist
+from cohortextractor.dashboards.vaccinations import VaccinationsStudyDefinition
+
+
 # Reference these imported functions to keep pyflakes happy and to make it
 # clear these are functional pytest fixtures, not stray imports
 set_database_url
 setup_module
 setup_function
 
 
@@ -107,15 +109,15 @@
             "pcv_2",
             "mmr_1",
             "menb_3",
             "dtap_ipv_1",
             "mmr_2",
         ],
     )
-    study.to_file(tmp_path / "test.csv")
+    study.to_csv(tmp_path / "test.csv")
     with open(tmp_path / "test.csv", newline="") as f:
         reader = csv.DictReader(f)
         results = list(reader)
     assert results == [
         {
             "patient_id": "2",
             "date_of_birth": "2019-01-01",
@@ -196,15 +198,15 @@
             "pcv_2",
             "mmr_1",
             "menb_3",
             "dtap_ipv_1",
             "mmr_2",
         ],
     )
-    study.to_file(tmp_path / "dummy.csv", expectations_population=1000)
+    study.to_csv(tmp_path / "dummy.csv", expectations_population=1000)
     with open(tmp_path / "dummy.csv", newline="") as f:
         reader = csv.DictReader(f)
         results = list(reader)
     assert len(results) == 1000
     headers = list(results[0].keys())
     assert headers == [
         "patient_id",
```

### Comparing `opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations_combine.py` & `opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations_combine.py`

 * *Files identical despite different names*

### Comparing `opensafely-cohort-extractor-1.85.0/tests/dashboards/test_vaccinations_extract.py` & `opensafely-cohort-extractor-1.9.0/tests/dashboards/test_vaccinations_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 
-from cohortextractor import codelist
-from cohortextractor.dashboards.vaccinations_extract import (
-    patients_with_ages_and_practices_sql,
-    vaccination_events_sql,
-)
-from cohortextractor.mssql_utils import mssql_dbapi_connection_from_url
-from tests.test_tpp_backend import set_database_url, setup_function, setup_module
+from tests.test_tpp_backend import set_database_url, setup_module, setup_function
 from tests.tpp_backend_setup import (
-    CodedEvent,
-    MedicationDictionary,
-    MedicationIssue,
-    Organisation,
+    make_session,
     Patient,
     RegistrationHistory,
+    Organisation,
     Vaccination,
-    make_session,
+    MedicationIssue,
+    MedicationDictionary,
+    CodedEvent,
+)
+
+from cohortextractor import codelist
+from cohortextractor.mssql_utils import mssql_dbapi_connection_from_url
+from cohortextractor.dashboards.vaccinations_extract import (
+    patients_with_ages_and_practices_sql,
+    vaccination_events_sql,
 )
 
+
 # Reference these imported functions to keep pyflakes happy and to make it
 # clear these are functional pytest fixtures, not stray imports
 set_database_url
 setup_module
 setup_function
```

### Comparing `opensafely-cohort-extractor-1.85.0/tests/test_emis_backend.py` & `opensafely-cohort-extractor-1.9.0/tests/test_tpp_backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,389 +1,186 @@
 import csv
-import gzip
+import glob
+from unittest.mock import patch
 import os
-import tempfile
+import subprocess
 
-import pandas
 import pytest
 
-from cohortextractor import StudyDefinition, codelist, patients
-from cohortextractor.date_expressions import InvalidExpressionError
-from cohortextractor.emis_backend import quote, truncate_patient_id
-from cohortextractor.patients import (
-    max_recorded_value,
-    mean_recorded_value,
-    min_recorded_value,
-)
-from tests.emis_backend_setup import (
-    CPNS,
+from tests.tpp_backend_setup import make_database, make_session
+from tests.tpp_backend_setup import (
+    Appointment,
+    CodedEvent,
+    MedicationIssue,
+    MedicationDictionary,
+    Patient,
+    RegistrationHistory,
+    Organisation,
+    PatientAddress,
     ICNARC,
-    Immunisation,
-    Medication,
-    Observation,
     ONSDeaths,
-    Patient,
-    clear_database,
-    make_database,
-    make_session,
+    CPNS,
+    Vaccination,
+    VaccinationReference,
+    SGSS_Positive,
+    SGSS_Negative,
+    PotentialCareHomeAddress,
+    Household,
+    HouseholdMember,
+    EC,
+    EC_Diagnosis,
+    APCS,
+    APCS_Der,
+)
+
+from cohortextractor import (
+    StudyDefinition,
+    patients,
+    codelist,
 )
-from tests.helpers import assert_results
+from cohortextractor.mssql_utils import mssql_connection_params_from_url
+from cohortextractor.tpp_backend import quote, AppointmentStatus
 
 
 @pytest.fixture(autouse=True)
 def set_database_url(monkeypatch):
     # The StudyDefinition code expects a single DATABASE_URL to tell it where
     # to connect to, but the test environment needs to supply multiple
     # connections (one for each backend type) so we copy the value in here
-    if "EMIS_DATABASE_URL" in os.environ:
-        monkeypatch.setenv("DATABASE_URL", os.environ["EMIS_DATABASE_URL"])
+    if "TPP_DATABASE_URL" in os.environ:
+        monkeypatch.setenv("DATABASE_URL", os.environ["TPP_DATABASE_URL"])
 
 
 def setup_module(module):
     make_database()
 
 
-def teardown_module(module):
-    clear_database()
-
-
 def setup_function(function):
-    """
-    Ensure test database is empty
-    """
+    """Ensure test database is empty"""
     session = make_session()
-    session.query(Observation).delete()
+    session.query(CodedEvent).delete()
     session.query(ICNARC).delete()
     session.query(ONSDeaths).delete()
     session.query(CPNS).delete()
-    session.query(Immunisation).delete()
-    session.query(Medication).delete()
+    session.query(Vaccination).delete()
+    session.query(VaccinationReference).delete()
+    session.query(Appointment).delete()
+    session.query(SGSS_Positive).delete()
+    session.query(SGSS_Negative).delete()
+    session.query(MedicationIssue).delete()
+    session.query(MedicationDictionary).delete()
+    session.query(RegistrationHistory).delete()
+    session.query(Organisation).delete()
+    session.query(PotentialCareHomeAddress).delete()
+    session.query(PatientAddress).delete()
+    session.query(HouseholdMember).delete()
+    session.query(Household).delete()
+    session.query(EC_Diagnosis).delete()
+    session.query(EC).delete()
+    session.query(APCS_Der).delete()
+    session.query(APCS).delete()
     session.query(Patient).delete()
     session.commit()
 
-    delete_temporary_tables()
 
-
-def delete_temporary_tables():
-    """Delete all temporary tables."""
+def test_minimal_study_to_csv(tmp_path):
     session = make_session()
-    with session.bind.connect() as conn:
-        sql = r"SELECT NAME FROM sys.tables WHERE NAME LIKE '\_%' ESCAPE '\'"
-        tables = [row[0] for row in conn.execute(sql)]
-        for table in tables:
-            conn.execute(f"DROP TABLE {table}")
-
-
-@pytest.mark.parametrize("format", ["csv", "csv.gz", "feather", "dta", "dta.gz"])
-def test_minimal_study_to_file(tmp_path, format):
-    session = make_session()
-    patient_1 = Patient(date_of_birth="1980-01-01", gender=1, hashed_organisation="abc")
-    patient_2 = Patient(date_of_birth="1965-01-01", gender=2, hashed_organisation="abc")
+    patient_1 = Patient(DateOfBirth="1900-01-01", Sex="M")
+    patient_2 = Patient(DateOfBirth="1900-01-01", Sex="F")
     session.add_all([patient_1, patient_2])
     session.commit()
-    study = StudyDefinition(
-        population=patients.all(),
-        sex=patients.sex(),
-        age=patients.age_as_of("2020-01-01"),
-    )
-    filename = tmp_path / f"test.{format}"
-    study.to_file(filename)
-    cast = lambda x: x  # noqa
-    if format == "csv":
-        cast = str
-        with open(filename) as f:
-            results = list(csv.DictReader(f))
-    if format == "csv.gz":
-        cast = str
-        with gzip.open(filename, "rt") as f:
-            results = list(csv.DictReader(f))
-    elif format == "feather":
-        results = pandas.read_feather(filename).to_dict("records")
-    elif format in ("dta", "dta.gz"):
-        results = pandas.read_stata(filename).to_dict("records")
+    study = StudyDefinition(population=patients.all(), sex=patients.sex())
+    study.to_csv(tmp_path / "test.csv")
+    with open(tmp_path / "test.csv") as f:
+        results = list(csv.DictReader(f))
     assert results == [
-        {"patient_id": cast(patient_1.registration_id), "sex": "M", "age": cast(40)},
-        {"patient_id": cast(patient_2.registration_id), "sex": "F", "age": cast(55)},
+        {"patient_id": str(patient_1.Patient_ID), "sex": "M"},
+        {"patient_id": str(patient_2.Patient_ID), "sex": "F"},
     ]
 
 
-def test_minimal_study_with_reserved_keywords():
-    # Test that we can use reserved SQL keywords as study variables
-    session = make_session()
-    patient_1 = Patient(date_of_birth="1980-01-01", gender=1, hashed_organisation="abc")
-    patient_2 = Patient(date_of_birth="1965-01-01", gender=2, hashed_organisation="abc")
-    session.add_all([patient_1, patient_2])
-    session.commit()
-    study = StudyDefinition(
-        population=patients.all(),
-        all=patients.sex(),
-        asc=patients.age_as_of("2020-01-01"),
-    )
+def test_sql_error_propagates(tmp_path):
+    study = StudyDefinition(population=patients.all(), sex=patients.sex())
+    # A bit hacky: fiddle with the list of queries to insert a deliberate error
+    # at the end
+    study.backend.queries[-1] = "SELECT Foo FROM Bar"
+    with pytest.raises(Exception) as excinfo:
+        study.to_csv(tmp_path / "test.csv")
+    assert "Invalid object name 'Bar'" in str(excinfo.value)
 
-    assert_results(study.to_dicts(), all=["M", "F"], asc=["40", "55"])
+
+def test_correct_driver_used():
+    # We support multiple drivers but we want to make sure our tests are
+    # running against the same driver we use in production
+    study = StudyDefinition(population=patients.all())
+    module = study.backend.get_db_connection().__class__.__module__
+    assert module == "ctds"
 
 
 def test_meds():
     session = make_session()
 
+    asthma_medication = MedicationDictionary(
+        FullName="Asthma Drug", DMD_ID="0", MultilexDrug_ID="0"
+    )
     patient_with_med = Patient()
-    patient_with_med.medications = [Medication(snomed_concept_id=0)]
+    patient_with_med.MedicationIssues = [
+        MedicationIssue(MedicationDictionary=asthma_medication)
+    ]
     patient_without_med = Patient()
     session.add(patient_with_med)
     session.add(patient_without_med)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
-        asthma_meds=patients.with_these_medications(codelist([0], "snomed")),
+        asthma_meds=patients.with_these_medications(
+            codelist(asthma_medication.DMD_ID, "snomed")
+        ),
     )
     results = study.to_dicts()
     assert [x["asthma_meds"] for x in results] == ["1", "0"]
 
 
 def test_meds_with_count():
     session = make_session()
 
+    asthma_medication = MedicationDictionary(
+        FullName="Asthma Drug", DMD_ID="0", MultilexDrug_ID="0"
+    )
     patient_with_med = Patient()
-    patient_with_med.medications = [
-        Medication(snomed_concept_id=0, effective_date="2010-01-01"),
-        Medication(snomed_concept_id=0, effective_date="2015-01-01"),
-        Medication(snomed_concept_id=0, effective_date="2018-01-01"),
-        Medication(snomed_concept_id=0, effective_date="2020-01-01"),
+    patient_with_med.MedicationIssues = [
+        MedicationIssue(
+            MedicationDictionary=asthma_medication, ConsultationDate="2010-01-01"
+        ),
+        MedicationIssue(
+            MedicationDictionary=asthma_medication, ConsultationDate="2015-01-01"
+        ),
+        MedicationIssue(
+            MedicationDictionary=asthma_medication, ConsultationDate="2018-01-01"
+        ),
+        MedicationIssue(
+            MedicationDictionary=asthma_medication, ConsultationDate="2020-01-01"
+        ),
     ]
     patient_without_med = Patient()
     session.add(patient_with_med)
     session.add(patient_without_med)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         asthma_meds=patients.with_these_medications(
-            codelist([0], "snomed"),
-            on_or_after="2012-01-01",
-            return_number_of_matches_in_period=True,
-        ),
-        asthma_meds_with_duplicate_codes=patients.with_these_medications(
-            codelist([0, 0], "snomed"),
+            codelist(asthma_medication.DMD_ID, "snomed"),
             on_or_after="2012-01-01",
             return_number_of_matches_in_period=True,
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_meds"] for x in results] == ["3", "0"]
-    assert [x["asthma_meds_with_duplicate_codes"] for x in results] == ["3", "0"]
-
-
-def test_patients_with_vaccination_record():
-    covid_vacc = "840534001"
-    first_covid_vacc = "1324681000000101"
-    second_covid_vacc = "1324691000000104"
-    pf_vacc = "39115611000001103"
-    az_vacc = "39114911000001105"
-
-    covid_codelist = codelist(
-        [covid_vacc, first_covid_vacc, second_covid_vacc], "snomedct"
-    )
-    pf_codelist = codelist([pf_vacc], "dmd")
-    az_codelist = codelist([az_vacc], "dmd")
-    vacc_codelist = codelist([pf_vacc, az_vacc], "dmd")
-
-    pf_date_1 = "2020-12-01"
-    pf_date_2 = "2021-01-01"
-    az_date_1 = "2020-12-01"
-    az_date_2 = "2020-12-02"
-
-    session = make_session()
-    session.add_all(
-        [
-            # Has no immunisations
-            Patient(),
-            # Has two Pfizer vaccinations with consistent dates
-            Patient(
-                medications=[
-                    Medication(snomed_concept_id=pf_vacc, effective_date=pf_date_1),
-                    Medication(snomed_concept_id=pf_vacc, effective_date=pf_date_2),
-                ],
-                immunisations=[
-                    Immunisation(
-                        snomed_concept_id=first_covid_vacc, effective_date=pf_date_1
-                    ),
-                    Immunisation(
-                        snomed_concept_id=second_covid_vacc, effective_date=pf_date_2
-                    ),
-                ],
-            ),
-            # Has one AZ vaccination with inconsistent dates
-            Patient(
-                medications=[
-                    Medication(snomed_concept_id=az_vacc, effective_date=az_date_1),
-                ],
-                immunisations=[
-                    Immunisation(
-                        snomed_concept_id=first_covid_vacc, effective_date=az_date_2
-                    ),
-                ],
-            ),
-        ]
-    )
-    session.commit()
-
-    study = StudyDefinition(
-        population=patients.all(),
-        had_pf=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": pf_codelist,
-            },
-            tpp={},
-        ),
-        had_az=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": az_codelist,
-            },
-            tpp={},
-        ),
-        first_pf=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": pf_codelist,
-            },
-            tpp={},
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        second_pf=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": pf_codelist,
-            },
-            tpp={},
-            on_or_after="first_pf + 20 days",
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        last_pf=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": pf_codelist,
-            },
-            tpp={},
-            find_last_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        first_az=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": az_codelist,
-            },
-            tpp={},
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        second_az=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": az_codelist,
-            },
-            tpp={},
-            on_or_after="first_az + 20 days",
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        last_az=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-                "product_codes": az_codelist,
-            },
-            tpp={},
-            find_last_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        first_product=patients.with_vaccination_record(
-            emis={
-                "product_codes": vacc_codelist,
-            },
-            tpp={},
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        second_product=patients.with_vaccination_record(
-            emis={
-                "product_codes": vacc_codelist,
-            },
-            tpp={},
-            on_or_after="first_product + 20 days",
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        last_product=patients.with_vaccination_record(
-            emis={
-                "product_codes": vacc_codelist,
-            },
-            tpp={},
-            find_last_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        first_procedure=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-            },
-            tpp={},
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        second_procedure=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-            },
-            tpp={},
-            on_or_after="first_procedure + 20 days",
-            find_first_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        last_procedure=patients.with_vaccination_record(
-            emis={
-                "procedure_codes": covid_codelist,
-            },
-            tpp={},
-            find_last_match_in_period=True,
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-    )
-
-    assert_results(
-        study.to_dicts(),
-        had_pf=["0", "1", "0"],
-        had_az=["0", "0", "1"],
-        first_pf=["", pf_date_1, ""],
-        second_pf=["", pf_date_2, ""],
-        last_pf=["", pf_date_2, ""],
-        first_az=["", "", az_date_1],
-        second_az=["", "", ""],
-        last_az=["", "", az_date_2],
-        first_product=["", pf_date_1, az_date_1],
-        second_product=["", pf_date_2, ""],
-        last_product=["", pf_date_2, az_date_1],
-        first_procedure=["", pf_date_1, az_date_2],
-        second_procedure=["", pf_date_2, ""],
-        last_procedure=["", pf_date_2, az_date_2],
-    )
 
 
 def _make_clinical_events_selection(condition_code, patient_dates=None):
     # The default configuration of patients and dates which some tests assume
     if patient_dates is None:
         patient_dates = ["2001-06-01", "2002-06-01", None]
     session = make_session()
@@ -394,217 +191,215 @@
         elif isinstance(dates, str):
             dates = [dates]
         for date in dates:
             if isinstance(date, tuple):
                 date, value = date
             else:
                 value = 0.0
-            patient.observations.append(
-                Observation(
-                    snomed_concept_id=condition_code,
-                    effective_date=date,
-                    value_pq_1=value,
+            patient.CodedEvents.append(
+                CodedEvent(
+                    CTV3Code=condition_code, ConsultationDate=date, NumericValue=value
                 )
             )
         session.add(patient)
     session.commit()
 
 
 def test_clinical_event_without_filters():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     # No date criteria
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct")
+            codelist([condition_code], "ctv3")
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["1", "1", "0"]
 
 
 def test_clinical_event_with_max_date():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"), on_or_before="2001-12-01"
+            codelist([condition_code], "ctv3"), on_or_before="2001-12-01"
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["1", "0", "0"]
 
 
 def test_clinical_event_with_min_date():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"), on_or_after="2005-12-01"
+            codelist([condition_code], "ctv3"), on_or_after="2005-12-01"
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["0", "0", "0"]
 
 
 def test_clinical_event_with_min_and_max_date():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"), between=["2001-12-01", "2002-06-01"]
+            codelist([condition_code], "ctv3"), between=["2001-12-01", "2002-06-01"]
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["0", "1", "0"]
 
 
 def test_clinical_event_returning_first_date():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(
         condition_code,
         patient_dates=[
             None,
             # Include date before period starts, which should be ignored
             ["2001-01-01", "2002-06-01"],
             ["2001-06-01"],
         ],
     )
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             between=["2001-12-01", "2002-06-01"],
             returning="date",
             find_first_match_in_period=True,
             date_format="YYYY-MM-DD",
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["", "2002-06-01", ""]
 
 
 def test_clinical_event_returning_last_date():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(
         condition_code,
         patient_dates=[
             None,
             # Include date after period ends, which should be ignored
             ["2002-06-01", "2003-01-01"],
             ["2001-06-01"],
         ],
     )
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             between=["2001-12-01", "2002-06-01"],
             returning="date",
             find_last_match_in_period=True,
             date_format="YYYY-MM-DD",
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["", "2002-06-01", ""]
 
 
 def test_clinical_event_returning_year_only():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     # No date criteria
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             returning="date",
             find_first_match_in_period=True,
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["2001", "2002", ""]
 
 
 def test_clinical_event_returning_year_and_month_only():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(condition_code)
     # No date criteria
     study = StudyDefinition(
         population=patients.all(),
         asthma_condition=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             returning="date",
             find_first_match_in_period=True,
             date_format="YYYY-MM",
         ),
     )
     results = study.to_dicts()
     assert [x["asthma_condition"] for x in results] == ["2001-06", "2002-06", ""]
 
 
 def test_clinical_event_with_count():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(
         condition_code,
         patient_dates=[
             None,
             # Include date before period starts, which should be ignored
             ["2001-01-01", "2002-01-01", "2002-02-01", "2002-06-01"],
             ["2001-06-01"],
         ],
     )
     study = StudyDefinition(
         population=patients.all(),
         asthma_count=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             between=["2001-12-01", "2002-06-01"],
             returning="number_of_matches_in_period",
             find_first_match_in_period=True,
         ),
         asthma_count_date=patients.date_of("asthma_count", date_format="YYYY-MM"),
     )
     results = study.to_dicts()
     assert [x["asthma_count"] for x in results] == ["0", "3", "0"]
     assert [x["asthma_count_date"] for x in results] == ["", "2002-01", ""]
 
 
 def test_clinical_event_with_code():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(
         condition_code,
         patient_dates=[
             None,
             # Include date before period starts, which should be ignored
             ["2001-01-01", "2002-01-01", "2002-02-01", "2002-06-01"],
             ["2001-06-01"],
         ],
     )
     study = StudyDefinition(
         population=patients.all(),
         latest_asthma_code=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             between=["2001-12-01", "2002-06-01"],
             returning="code",
             find_last_match_in_period=True,
         ),
         latest_asthma_code_date=patients.date_of(
             "latest_asthma_code", date_format="YYYY-MM"
         ),
     )
     results = study.to_dicts()
-    assert [x["latest_asthma_code"] for x in results] == ["", str(condition_code), ""]
+    assert [x["latest_asthma_code"] for x in results] == ["", condition_code, ""]
     assert [x["latest_asthma_code_date"] for x in results] == ["", "2002-06", ""]
 
 
 def test_clinical_event_with_numeric_value():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     _make_clinical_events_selection(
         condition_code,
         patient_dates=[
             None,
             # Include date before period starts, which should be ignored
             [
                 ("2001-01-01", 1),
@@ -614,90 +409,44 @@
             ],
             [("2001-06-01", 7)],
         ],
     )
     study = StudyDefinition(
         population=patients.all(),
         asthma_value=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
+            codelist([condition_code], "ctv3"),
             between=["2001-12-01", "2002-06-01"],
             returning="numeric_value",
             find_first_match_in_period=True,
         ),
         asthma_value_date=patients.date_of("asthma_value", date_format="YYYY-MM"),
     )
     results = study.to_dicts()
     assert [x["asthma_value"] for x in results] == ["0.0", "2.0", "0.0"]
     assert [x["asthma_value_date"] for x in results] == ["", "2002-01", ""]
 
 
-def test_clinical_event_ignoring_missing_values():
-    condition_code = "195967001"
-    _make_clinical_events_selection(
-        condition_code,
-        patient_dates=[
-            [
-                ("2001-01-01", None),
-                ("2001-01-01", 0),
-                ("2001-01-02", 2),
-                ("2001-01-03", None),
-                ("2001-01-04", 4),
-                ("2001-01-05", None),
-                ("2001-01-05", 0),
-            ],
-        ],
-    )
-    study = StudyDefinition(
-        population=patients.all(),
-        first=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
-            returning="numeric_value",
-            ignore_missing_values=True,
-            find_first_match_in_period=True,
-        ),
-        last=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct"),
-            returning="numeric_value",
-            ignore_missing_values=True,
-            find_last_match_in_period=True,
-        ),
-    )
-    results = study.to_dicts()
-    assert [x["first"] for x in results] == ["2.0"]
-    assert [x["last"] for x in results] == ["4.0"]
-
-
 def test_clinical_event_with_category():
     session = make_session()
     session.add_all(
         [
             Patient(),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2018-01-01"
-                    ),
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2020-01-01"
-                    ),
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2018-01-01"),
+                    CodedEvent(CTV3Code="foo2", ConsultationDate="2020-01-01"),
                 ]
             ),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000003", effective_date="2019-01-01"
-                    )
-                ]
+                CodedEvents=[CodedEvent(CTV3Code="foo3", ConsultationDate="2019-01-01")]
             ),
         ]
     )
     session.commit()
-    codes = codelist(
-        [("10000001", "A"), ("10000002", "B"), ("10000003", "C")], "snomedct"
-    )
+    codes = codelist([("foo1", "A"), ("foo2", "B"), ("foo3", "C")], "ctv3")
     study = StudyDefinition(
         population=patients.all(),
         code_category=patients.with_these_clinical_events(
             codes, returning="category", find_last_match_in_period=True
         ),
         code_category_date=patients.date_of("code_category"),
     )
@@ -705,135 +454,98 @@
     assert [x["code_category"] for x in results] == ["", "B", "C"]
     assert [x["code_category_date"] for x in results] == ["", "2020", "2019"]
 
 
 def test_patient_registered_as_of():
     session = make_session()
 
-    patient_registered_in_2001 = Patient(
-        registered_date="2001-01-01", registration_end_date=None
-    )
-    patient_registered_in_2002 = Patient(
-        registered_date="2002-01-01", registration_end_date=None
-    )
-    patient_unregistered_in_2002 = Patient(
-        registered_date="2001-01-01", registration_end_date="2002-01-01"
-    )
+    patient_registered_in_2001 = Patient()
+    patient_registered_in_2002 = Patient()
+    patient_unregistered_in_2002 = Patient()
+    patient_registered_in_2001.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2001-01-01", EndDate="9999-01-01", Organisation=Organisation()
+        )
+    ]
+    patient_registered_in_2002.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2002-01-01", EndDate="9999-01-01", Organisation=Organisation()
+        )
+    ]
+    patient_unregistered_in_2002.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2001-01-01", EndDate="2002-01-01", Organisation=Organisation()
+        )
+    ]
 
     session.add(patient_registered_in_2001)
     session.add(patient_registered_in_2002)
     session.add(patient_unregistered_in_2002)
     session.commit()
 
     # No date criteria
     study = StudyDefinition(population=patients.registered_as_of("2002-03-02"))
     results = study.to_dicts()
-    assert len(results) == 2
-
-
-def test_patient_registered_as_of_with_date_variable():
-    session = make_session()
-
-    patient_unregistered_on_date_of_death = Patient(
-        registered_date="2001-01-01",
-        registration_end_date="2011-04-01",
-        date_of_death="2011-05-01",
-    )
-    patient_registered_on_date_of_death = Patient(
-        registered_date="2002-01-01",
-        registration_end_date=None,
-        date_of_death="2003-01-01",
-    )
-    patient_registered_on_ons_date_of_death = Patient(
-        registered_date="2001-01-01",
-        registration_end_date="2011-04-01",
-        date_of_death=None,
-        ONSDeath=[ONSDeaths(reg_stat_dod=20100101, upload_date="2021-02-02")],
-    )
-    patient_not_dead = Patient(
-        registered_date="2001-01-01",
-        registration_end_date="2002-01-01",
-        date_of_death=None,
-    )
-
-    session.add(patient_unregistered_on_date_of_death)
-    session.add(patient_registered_on_date_of_death)
-    session.add(patient_registered_on_ons_date_of_death)
-    session.add(patient_not_dead)
-    session.commit()
-
-    study = StudyDefinition(
-        date_of_death=patients.with_death_recorded_in_primary_care(
-            returning="date_of_death", date_format="YYYY-MM-DD"
-        ),
-        population=patients.registered_as_of("date_of_death"),
-    )
-    results = study.to_dicts()
-    assert len(results) == 1
-    assert results[0]["date_of_death"] == "2003-01-01"
-
-    study = StudyDefinition(
-        ons_death_date=patients.died_from_any_cause(
-            returning="date_of_death", date_format="YYYY-MM-DD"
-        ),
-        population=patients.registered_as_of("ons_death_date"),
-    )
-    results = study.to_dicts()
-    assert len(results) == 1
-    assert results[0]["ons_death_date"] == "2010-01-01"
+    assert [x["patient_id"] for x in results] == [
+        str(patient_registered_in_2001.Patient_ID),
+        str(patient_registered_in_2002.Patient_ID),
+    ]
 
 
 def test_patients_registered_with_one_practice_between():
     session = make_session()
 
-    patient_registered_in_2001 = Patient(
-        registered_date="2001-01-01", registration_end_date=None
-    )
-    patient_registered_in_2002 = Patient(
-        registered_date="2002-01-01", registration_end_date=None
-    )
-    patient_unregistered_in_2002 = Patient(
-        registered_date="2001-01-01", registration_end_date="2002-01-01"
-    )
+    patient_registered_in_2001 = Patient()
+    patient_registered_in_2002 = Patient()
+    patient_unregistered_in_2002 = Patient()
+    patient_registered_in_2001.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2001-01-01", EndDate="9999-01-01", Organisation=Organisation()
+        )
+    ]
+    patient_registered_in_2002.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2002-01-01", EndDate="9999-01-01", Organisation=Organisation()
+        )
+    ]
+    patient_unregistered_in_2002.RegistrationHistory = [
+        RegistrationHistory(
+            StartDate="2001-01-01", EndDate="2002-01-01", Organisation=Organisation()
+        )
+    ]
 
     session.add(patient_registered_in_2001)
     session.add(patient_registered_in_2002)
     session.add(patient_unregistered_in_2002)
     session.commit()
 
     study = StudyDefinition(
         population=patients.registered_with_one_practice_between(
             "2001-12-01", "2003-01-01"
         )
     )
     results = study.to_dicts()
-    assert len(results) == 1
+    assert [x["patient_id"] for x in results] == [
+        str(patient_registered_in_2001.Patient_ID)
+    ]
 
 
 @pytest.mark.parametrize("include_dates", ["none", "year", "month", "day"])
 def test_simple_bmi(include_dates):
     session = make_session()
 
-    weight_code = "27113001"
-    height_code = "271603002"
+    weight_code = "X76C7"
+    height_code = "XM01E"
 
-    patient = Patient(date_of_birth="1950-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=weight_code,
-            value_pq_1=50,
-            effective_date="2002-06-01",
-        )
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=weight_code, NumericValue=50, ConsultationDate="2002-06-01")
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=height_code,
-            value_pq_1=10,
-            effective_date="2001-06-01",
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=height_code, NumericValue=10, ConsultationDate="2001-06-01")
     )
     session.add(patient)
     session.commit()
 
     if include_dates == "none":
         bmi_date = None
         date_query = None
@@ -857,31 +569,25 @@
     assert [x["BMI"] for x in results] == ["0.5"]
     assert [x.get("BMI_date_measured") for x in results] == [bmi_date]
 
 
 def test_bmi_rounded():
     session = make_session()
 
-    weight_code = "27113001"
-    height_code = "271603002"
+    weight_code = "X76C7"
+    height_code = "XM01E"
 
-    patient = Patient(date_of_birth="1950-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=weight_code,
-            value_pq_1=10.12345,
-            effective_date="2001-06-01",
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(
+            CTV3Code=weight_code, NumericValue=10.12345, ConsultationDate="2001-06-01"
         )
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=height_code,
-            value_pq_1=10,
-            effective_date="2000-02-01",
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=height_code, NumericValue=10, ConsultationDate="2000-02-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -893,27 +599,23 @@
     assert [x["BMI"] for x in results] == ["0.1"]
     assert [x["BMI_date_measured"] for x in results] == ["2001-06-01"]
 
 
 def test_bmi_with_zero_values():
     session = make_session()
 
-    weight_code = "27113001"
-    height_code = "271603002"
+    weight_code = "X76C7"
+    height_code = "XM01E"
 
-    patient = Patient(date_of_birth="1950-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=weight_code, value_pq_1=0, effective_date="2001-06-01"
-        )
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=weight_code, NumericValue=0, ConsultationDate="2001-06-01")
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=height_code, value_pq_1=0, effective_date="2001-06-01"
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=height_code, NumericValue=0, ConsultationDate="2001-06-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -926,29 +628,23 @@
     assert [x["BMI"] for x in results] == ["0.0"]
     assert [x["BMI_date_measured"] for x in results] == ["2001-06-01"]
 
 
 def test_explicit_bmi_fallback():
     session = make_session()
 
-    weight_code = "27113001"
-    bmi_code = "301331008"
+    weight_code = "X76C7"
+    bmi_code = "22K.."
 
-    patient = Patient(date_of_birth="1950-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=weight_code,
-            value_pq_1=50,
-            effective_date="2001-06-01",
-        )
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=weight_code, NumericValue=50, ConsultationDate="2001-06-01")
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=bmi_code, value_pq_1=99, effective_date="2001-10-01"
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=bmi_code, NumericValue=99, ConsultationDate="2001-10-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -961,21 +657,19 @@
     assert [x["BMI"] for x in results] == ["99.0"]
     assert [x["BMI_date_measured"] for x in results] == ["2001-10-01"]
 
 
 def test_no_bmi_when_old_date():
     session = make_session()
 
-    bmi_code = "301331008"
+    bmi_code = "22K.."
 
-    patient = Patient(date_of_birth="1950-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=bmi_code, value_pq_1=99, effective_date="1994-12-31"
-        )
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=bmi_code, NumericValue=99, ConsultationDate="1994-12-31")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -988,21 +682,19 @@
     assert [x["BMI"] for x in results] == ["0.0"]
     assert [x["BMI_date_measured"] for x in results] == [""]
 
 
 def test_no_bmi_when_measurements_of_child():
     session = make_session()
 
-    bmi_code = "301331008"
+    bmi_code = "22K.."
 
-    patient = Patient(date_of_birth="2000-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=bmi_code, value_pq_1=99, effective_date="2001-01-01"
-        )
+    patient = Patient(DateOfBirth="2000-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=bmi_code, NumericValue=99, ConsultationDate="2001-01-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -1015,21 +707,19 @@
     assert [x["BMI"] for x in results] == ["0.0"]
     assert [x["BMI_date_measured"] for x in results] == [""]
 
 
 def test_no_bmi_when_measurement_after_reference_date():
     session = make_session()
 
-    bmi_code = "301331008"
+    bmi_code = "22K.."
 
-    patient = Patient(date_of_birth="1900-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=bmi_code, value_pq_1=99, effective_date="2001-01-01"
-        )
+    patient = Patient(DateOfBirth="1900-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=bmi_code, NumericValue=99, ConsultationDate="2001-01-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -1042,37 +732,27 @@
     assert [x["BMI"] for x in results] == ["0.0"]
     assert [x["BMI_date_measured"] for x in results] == [""]
 
 
 def test_bmi_when_only_some_measurements_of_child():
     session = make_session()
 
-    bmi_code = "301331008"
-    weight_code = "27113001"
-    height_code = "271603002"
-
-    patient = Patient(date_of_birth="1990-01-01")
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=bmi_code, value_pq_1=99, effective_date="1995-01-01"
-        )
+    bmi_code = "22K.."
+    weight_code = "X76C7"
+    height_code = "XM01E"
+
+    patient = Patient(DateOfBirth="1990-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=bmi_code, NumericValue=99, ConsultationDate="1995-01-01")
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=weight_code,
-            value_pq_1=50,
-            effective_date="2010-01-01",
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=weight_code, NumericValue=50, ConsultationDate="2010-01-01")
     )
-    patient.observations.append(
-        Observation(
-            snomed_concept_id=height_code,
-            value_pq_1=10,
-            effective_date="2010-01-01",
-        )
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code=height_code, NumericValue=10, ConsultationDate="2010-01-01")
     )
     session.add(patient)
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         BMI=patients.most_recent_bmi(
@@ -1082,246 +762,174 @@
         BMI_date_measured=patients.date_of("BMI", date_format="YYYY-MM-DD"),
     )
     results = study.to_dicts()
     assert [x["BMI"] for x in results] == ["0.5"]
     assert [x["BMI_date_measured"] for x in results] == ["2010-01-01"]
 
 
-@pytest.mark.parametrize(
-    "summary_function,expected",
-    [
-        (mean_recorded_value, [("96.0", "2020-02-10"), ("0.0", ""), ("0.0", "")]),
-        (min_recorded_value, [("90.0", "2020-02-10"), ("0.0", ""), ("0.0", "")]),
-        (max_recorded_value, [("100.0", "2020-02-10"), ("0.0", ""), ("0.0", "")]),
-    ],
-)
-def test_summary_recorded_values_on_most_recent_day(summary_function, expected):
-    code = "10000001"
+def test_mean_recorded_value():
+    code = "2469."
     session = make_session()
     patient = Patient()
     values = [
-        # These days are within the period but not the most recent, and should be ignored
-        ("2020-01-01", 110),
-        ("2020-01-02", 80),
-        # This is the most recent day; mean taken from these 3 measurements
         ("2020-02-10", 90),
         ("2020-02-10", 100),
         ("2020-02-10", 98),
         # This day is outside period and should be ignored
         ("2020-04-01", 110),
     ]
     for date, value in values:
-        patient.observations.append(
-            Observation(snomed_concept_id=code, value_pq_1=value, effective_date=date)
+        patient.CodedEvents.append(
+            CodedEvent(CTV3Code=code, NumericValue=value, ConsultationDate=date)
         )
     patient_with_old_reading = Patient()
-    patient_with_old_reading.observations.append(
-        Observation(snomed_concept_id=code, value_pq_1=100, effective_date="2010-01-01")
+    patient_with_old_reading.CodedEvents.append(
+        CodedEvent(CTV3Code=code, NumericValue=100, ConsultationDate="2010-01-01")
     )
     patient_with_no_reading = Patient()
     session.add_all([patient, patient_with_old_reading, patient_with_no_reading])
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
-        bp_systolic=summary_function(
-            codelist([code], system="snomedct"),
+        bp_systolic=patients.mean_recorded_value(
+            codelist([code], system="ctv3"),
             on_most_recent_day_of_measurement=True,
             between=["2018-01-01", "2020-03-01"],
         ),
         bp_systolic_date_measured=patients.date_of(
             "bp_systolic", date_format="YYYY-MM-DD"
         ),
     )
     results = study.to_dicts()
     results = [(i["bp_systolic"], i["bp_systolic_date_measured"]) for i in results]
-    assert results == expected
+    assert results == [("96.0", "2020-02-10"), ("0.0", ""), ("0.0", "")]
 
 
-@pytest.mark.parametrize(
-    "summary_function,expected",
-    [
-        (mean_recorded_value, ["95.6", "0.0", "0.0"]),
-        (min_recorded_value, ["80.0", "0.0", "0.0"]),
-        (max_recorded_value, ["110.0", "0.0", "0.0"]),
-    ],
-)
-def test_summary_recorded_values_across_date_range(summary_function, expected):
-    code = "113075003"
+def test_patient_random_sample():
     session = make_session()
-    patient = Patient()
-    values = [
-        # these 5 are within the period
-        ("2020-01-01", 110),
-        ("2020-01-02", 80),
-        ("2020-02-10", 90),
-        ("2020-02-10", 100),
-        ("2020-02-10", 98),
-        # This day is outside period and should be ignored
-        ("2020-04-01", 110),
-    ]
-    for date, value in values:
-        patient.observations.append(
-            Observation(snomed_concept_id=code, value_pq_1=value, effective_date=date)
-        )
-    patient_with_old_reading = Patient()
-    patient_with_old_reading.observations.append(
-        Observation(snomed_concept_id=code, value_pq_1=100, effective_date="2010-01-01")
-    )
-    patient_with_no_reading = Patient()
-    session.add_all([patient, patient_with_old_reading, patient_with_no_reading])
+    sample_size = 1000
+    for _ in range(sample_size):
+        patient = Patient()
+        session.add(patient)
     session.commit()
-    study = StudyDefinition(
-        population=patients.all(),
-        creatine=summary_function(
-            codelist([code], system="snomedct"),
-            on_most_recent_day_of_measurement=False,
-            between=["2018-01-01", "2020-03-01"],
-        ),
-    )
-    assert_results(study.to_dicts(), creatine=expected)
-
 
-def test_mean_recorded_value_across_date_range_include_measurement_date_error():
-    with pytest.raises(
-        AssertionError,
-        match="Can only include measurement date if on_most_recent_day_of_measurement is True",
-    ):
-        StudyDefinition(
-            population=patients.all(),
-            creatine=patients.mean_recorded_value(
-                codelist(["113075003"], system="snomedct"),
-                on_most_recent_day_of_measurement=False,
-                between=["2018-01-01", "2020-03-01"],
-                include_measurement_date=True,
-            ),
-        )
+    study = StudyDefinition(population=patients.random_sample(percent=20))
+    results = study.to_dicts()
+    # The method is approximate!
+    assert len(results) < (sample_size / 2)
 
 
 def test_patients_satisfying():
-    condition_code = "195967001"
+    condition_code = "ASTHMA"
     session = make_session()
-    patient_1 = Patient(date_of_birth="1940-01-01", gender=1)
-    patient_2 = Patient(date_of_birth="1940-01-01", gender=2)
-    patient_3 = Patient(date_of_birth="1990-01-01", gender=1)
-    patient_4 = Patient(date_of_birth="1940-01-01", gender=2)
-    patient_4.observations.append(
-        Observation(snomed_concept_id=condition_code, effective_date="2010-01-01")
+    patient_1 = Patient(DateOfBirth="1940-01-01", Sex="M")
+    patient_2 = Patient(DateOfBirth="1940-01-01", Sex="F")
+    patient_3 = Patient(DateOfBirth="1990-01-01", Sex="M")
+    patient_4 = Patient(DateOfBirth="1940-01-01", Sex="F")
+    patient_4.CodedEvents.append(
+        CodedEvent(CTV3Code=condition_code, ConsultationDate="2010-01-01")
     )
     session.add_all([patient_1, patient_2, patient_3, patient_4])
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         sex=patients.sex(),
         age=patients.age_as_of("2020-01-01"),
         has_asthma=patients.with_these_clinical_events(
-            codelist([condition_code], "snomedct")
+            codelist([condition_code], "ctv3")
         ),
-        at_risk=patients.satisfying("(age > 70 AND sex = 'M') OR has_asthma"),
+        at_risk=patients.satisfying("((age + 30) > 100 AND sex = 'M') OR has_asthma"),
     )
     results = study.to_dicts()
     assert [i["at_risk"] for i in results] == ["1", "0", "0", "1"]
 
 
 def test_patients_satisfying_with_hidden_columns():
-    condition_code = "195967001"
-    condition_code2 = "13645005"
+    condition_code = "ASTHMA"
+    condition_code2 = "COPD"
     session = make_session()
-    patient_1 = Patient(date_of_birth="1940-01-01", gender=1)
-    patient_2 = Patient(date_of_birth="1940-01-01", gender=2)
-    patient_3 = Patient(date_of_birth="1990-01-01", gender=1)
-    patient_4 = Patient(date_of_birth="1940-01-01", gender=2)
-    patient_4.observations.append(
-        Observation(snomed_concept_id=condition_code, effective_date="2010-01-01")
-    )
-    patient_5 = Patient(date_of_birth="1940-01-01", gender=2)
-    patient_5.observations.append(
-        Observation(snomed_concept_id=condition_code, effective_date="2010-01-01")
+    patient_1 = Patient(DateOfBirth="1940-01-01", Sex="M")
+    patient_2 = Patient(DateOfBirth="1940-01-01", Sex="F")
+    patient_3 = Patient(DateOfBirth="1990-01-01", Sex="M")
+    patient_4 = Patient(DateOfBirth="1940-01-01", Sex="F")
+    patient_4.CodedEvents.append(
+        CodedEvent(CTV3Code=condition_code, ConsultationDate="2010-01-01")
+    )
+    patient_5 = Patient(DateOfBirth="1940-01-01", Sex="F")
+    patient_5.CodedEvents.append(
+        CodedEvent(CTV3Code=condition_code, ConsultationDate="2010-01-01")
     )
-    patient_5.observations.append(
-        Observation(snomed_concept_id=condition_code2, effective_date="2010-01-01")
+    patient_5.CodedEvents.append(
+        CodedEvent(CTV3Code=condition_code2, ConsultationDate="2010-01-01")
     )
     session.add_all([patient_1, patient_2, patient_3, patient_4, patient_5])
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         sex=patients.sex(),
         age=patients.age_as_of("2020-01-01"),
         at_risk=patients.satisfying(
             """
             (age > 70 AND sex = "M")
             OR
             (has_asthma AND NOT copd)
             """,
             has_asthma=patients.with_these_clinical_events(
-                codelist([condition_code], "snomedct")
+                codelist([condition_code], "ctv3")
             ),
             copd=patients.with_these_clinical_events(
-                codelist([condition_code2], "snomedct")
+                codelist([condition_code2], "ctv3")
             ),
         ),
     )
     results = study.to_dicts()
     assert [i["at_risk"] for i in results] == ["1", "0", "0", "1", "0"]
     assert "has_asthma" not in results[0].keys()
 
 
 def test_patients_categorised_as():
     session = make_session()
     session.add_all(
         [
             Patient(
-                gender=1,
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2000-01-01"
-                    )
+                Sex="M",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2000-01-01")
                 ],
             ),
             Patient(
-                gender=2,
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2000-01-01"
-                    ),
-                    Observation(
-                        snomed_concept_id="20000001", effective_date="2000-01-01"
-                    ),
+                Sex="F",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo2", ConsultationDate="2000-01-01"),
+                    CodedEvent(CTV3Code="bar1", ConsultationDate="2000-01-01"),
                 ],
             ),
             Patient(
-                gender=1,
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2000-01-01"
-                    )
+                Sex="M",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo2", ConsultationDate="2000-01-01")
                 ],
             ),
             Patient(
-                gender=2,
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000003", effective_date="2000-01-01"
-                    )
+                Sex="F",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo3", ConsultationDate="2000-01-01")
                 ],
             ),
             Patient(
-                gender=2,
-                observations=[
-                    Observation(
-                        snomed_concept_id="20000001", effective_date="2000-01-01"
-                    ),
+                Sex="F",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="bar1", ConsultationDate="2000-01-01"),
                 ],
             ),
         ]
     )
     session.commit()
-    foo_codes = codelist(
-        [("10000001", "A"), ("10000002", "B"), ("10000003", "C")], "snomedct"
-    )
-    bar_codes = codelist(["20000001"], "snomedct")
+    foo_codes = codelist([("foo1", "A"), ("foo2", "B"), ("foo3", "C")], "ctv3")
+    bar_codes = codelist(["bar1"], "ctv3")
     study = StudyDefinition(
         population=patients.all(),
         category=patients.categorised_as(
             {
                 "W": "(foo_category = 'B' OR NOT foo_category) AND female_with_bar",
                 "X": "sex = 'F' AND (foo_category = 'B' OR foo_category = 'C')",
                 "Y": "sex = 'M' AND foo_category = 'A'",
@@ -1341,168 +949,321 @@
     assert [x["category"] for x in results] == ["Y", "W", "Z", "X", "W"]
     # Assert that internal columns do not appear
     assert "foo_category" not in results[0].keys()
     assert "female_with_bar" not in results[0].keys()
     assert "has_bar" not in results[0].keys()
 
 
-@pytest.mark.freeze_time("2020-02-15")
 def test_patients_registered_practice_as_of():
     session = make_session()
-    patient = Patient(
-        stp_code="789",
-        msoa="E0203",
-        english_region_name="London",
-        hashed_organisation="abc",
+    org_1 = Organisation(
+        STPCode="123", MSOACode="E0201", Region="East of England", Organisation_ID=1
     )
-
-    session.add_all([patient])
+    org_2 = Organisation(
+        STPCode="456", MSOACode="E0202", Region="Midlands", Organisation_ID=2
+    )
+    org_3 = Organisation(
+        STPCode="789", MSOACode="E0203", Region="London", Organisation_ID=3
+    )
+    org_4 = Organisation(
+        STPCode="910", MSOACode="E0204", Region="North West", Organisation_ID=4
+    )
+    patient = Patient()
+    patient.RegistrationHistory.append(
+        RegistrationHistory(
+            StartDate="1990-01-01", EndDate="2018-01-01", Organisation=org_1
+        )
+    )
+    # We deliberately create overlapping registration periods so we can check
+    # that we handle these correctly
+    patient.RegistrationHistory.append(
+        RegistrationHistory(
+            StartDate="2018-01-01", EndDate="2022-01-01", Organisation=org_2
+        )
+    )
+    patient.RegistrationHistory.append(
+        RegistrationHistory(
+            StartDate="2019-09-01", EndDate="2020-05-01", Organisation=org_3
+        )
+    )
+    patient.RegistrationHistory.append(
+        RegistrationHistory(
+            StartDate="2022-01-01", EndDate="9999-12-31", Organisation=org_4
+        )
+    )
+    patient_2 = Patient()
+    patient_2.RegistrationHistory.append(
+        RegistrationHistory(
+            StartDate="2010-01-01", EndDate="9999-12-31", Organisation=org_1
+        )
+    )
+    patient_3 = Patient()
+    patient_3.RegistrationHistory.append(
+        RegistrationHistory(StartDate="2010-01-01", EndDate="9999-12-31")
+    )
+    session.add_all([patient, patient_2, patient_3])
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
-        stp=patients.registered_practice_as_of("2020-02-01", returning="stp_code"),
-        msoa=patients.registered_practice_as_of("2020-02-01", returning="msoa"),
-        deprecated_msoa=patients.registered_practice_as_of(
-            "2020-01-01", returning="msoa_code"
-        ),
+        stp=patients.registered_practice_as_of("2020-01-01", returning="stp_code"),
+        msoa=patients.registered_practice_as_of("2020-01-01", returning="msoa_code"),
         region=patients.registered_practice_as_of(
-            "2020-02-01", returning="nuts1_region_name"
+            "2020-01-01", returning="nuts1_region_name"
         ),
         pseudo_id=patients.registered_practice_as_of(
-            "2020-02-01", returning="pseudo_id"
+            "2020-01-01", returning="pseudo_id"
         ),
     )
     results = study.to_dicts()
-    assert [i["stp"] for i in results] == ["789"]
-    assert [i["msoa"] for i in results] == ["E0203"]
-    assert [i["deprecated_msoa"] for i in results] == ["E0203"]
-    assert [i["region"] for i in results] == ["London"]
-    assert [i["pseudo_id"] for i in results] == ["abc"]
+    assert [i["stp"] for i in results] == ["789", "123", ""]
+    assert [i["msoa"] for i in results] == ["E0203", "E0201", ""]
+    assert [i["region"] for i in results] == ["London", "East of England", ""]
+    assert [i["pseudo_id"] for i in results] == ["3", "1", "0"]
 
 
-@pytest.mark.freeze_time("2020-02-15")
 def test_patients_address_as_of():
     session = make_session()
-    patient = Patient(imd_rank=300, rural_urban=2)
-    patient_no_address = Patient()
-    session.add_all([patient, patient_no_address])
+    session.add_all(
+        [
+            # We deliberately create overlapping address periods here to check
+            # that we handle these correctly
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="1990-01-01",
+                        EndDate="2018-01-01",
+                        ImdRankRounded=100,
+                        RuralUrbanClassificationCode=1,
+                    ),
+                    PatientAddress(
+                        StartDate="2018-01-01",
+                        EndDate="2020-02-01",
+                        ImdRankRounded=200,
+                        RuralUrbanClassificationCode=1,
+                    ),
+                    PatientAddress(
+                        StartDate="2019-01-01",
+                        EndDate="2022-01-01",
+                        ImdRankRounded=300,
+                        RuralUrbanClassificationCode=2,
+                    ),
+                    PatientAddress(
+                        StartDate="2022-01-01",
+                        EndDate="9999-12-31",
+                        ImdRankRounded=500,
+                        RuralUrbanClassificationCode=3,
+                    ),
+                ]
+            ),
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="1900-01-01",
+                        EndDate="9999-12-31",
+                        ImdRankRounded=-1,
+                        RuralUrbanClassificationCode=-1,
+                        MSOACode="NPC",
+                    ),
+                    PatientAddress(
+                        StartDate="1900-01-01",
+                        EndDate="9999-12-31",
+                        ImdRankRounded=600,
+                        RuralUrbanClassificationCode=4,
+                        MSOACode="E02002346",
+                    ),
+                ]
+            ),
+            # Patient with no address
+            Patient(),
+            # Patient with only old address
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="2010-01-01",
+                        EndDate="2015-01-01",
+                        ImdRankRounded=100,
+                        RuralUrbanClassificationCode=1,
+                    )
+                ]
+            ),
+        ]
+    )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         imd=patients.address_as_of(
-            "2020-02-01",
+            "2020-01-01",
             returning="index_of_multiple_deprivation",
             round_to_nearest=100,
         ),
         rural_urban=patients.address_as_of(
-            "2020-02-01", returning="rural_urban_classification"
+            "2020-01-01", returning="rural_urban_classification"
         ),
     )
-    results = study.to_dicts()
-    assert [i["imd"] for i in results] == ["300", "0"]
-    assert [i["rural_urban"] for i in results] == ["2", "0"]
+    assert_results(
+        study.to_dicts(), imd=["300", "600", "0", "0"], rural_urban=["2", "4", "0", "0"]
+    )
 
 
-def test_patients_with_death_recorded_in_primary_care():
+def test_patients_care_home_status_as_of():
     session = make_session()
     session.add_all(
         [
-            Patient(date_of_death=None),
-            Patient(date_of_death="2017-05-06"),
-            Patient(date_of_death="2019-06-07"),
-            Patient(date_of_death="2020-07-08"),
+            # Was in care home but no longer
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="2010-01-01",
+                        EndDate="2015-01-01",
+                        PotentialCareHomeAddress=[PotentialCareHomeAddress()],
+                    ),
+                    PatientAddress(StartDate="2015-01-01", EndDate="9999-01-01"),
+                ]
+            ),
+            # Currently in non-nursing care home
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="2015-01-01",
+                        EndDate="9999-01-01",
+                        PotentialCareHomeAddress=[
+                            PotentialCareHomeAddress(
+                                LocationRequiresNursing="N",
+                                LocationDoesNotRequireNursing="Y",
+                            )
+                        ],
+                    ),
+                ]
+            ),
+            # Currently in nursing home
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="2015-01-01",
+                        EndDate="9999-01-01",
+                        PotentialCareHomeAddress=[
+                            PotentialCareHomeAddress(
+                                LocationRequiresNursing="Y",
+                                LocationDoesNotRequireNursing="N",
+                            )
+                        ],
+                    ),
+                ]
+            ),
+            # Currently in a schrodin-home which both does and does not require nursing
+            Patient(
+                Addresses=[
+                    PatientAddress(
+                        StartDate="2015-01-01",
+                        EndDate="9999-01-01",
+                        PotentialCareHomeAddress=[
+                            PotentialCareHomeAddress(
+                                LocationRequiresNursing="Y",
+                                LocationDoesNotRequireNursing="Y",
+                            )
+                        ],
+                    ),
+                ]
+            ),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
-        has_died=patients.with_death_recorded_in_primary_care(),
-        date_of_death=patients.with_death_recorded_in_primary_care(
-            returning="date_of_death", date_format="YYYY-MM-DD"
-        ),
-        died_in_2019=patients.with_death_recorded_in_primary_care(
-            between=["2019-01-01", "2019-12-31"],
-            returning="date_of_death",
+        is_in_care_home=patients.care_home_status_as_of("2020-01-01"),
+        care_home_type=patients.care_home_status_as_of(
+            "2020-01-01",
+            categorised_as={
+                "PC": """
+                  IsPotentialCareHome
+                  AND LocationDoesNotRequireNursing='Y'
+                  AND LocationRequiresNursing='N'
+                """,
+                "PN": """
+                  IsPotentialCareHome
+                  AND LocationDoesNotRequireNursing='N'
+                  AND LocationRequiresNursing='Y'
+                """,
+                "PS": "IsPotentialCareHome",
+                "U": "DEFAULT",
+            },
         ),
     )
-    assert_results(
-        study.to_dicts(),
-        has_died=["0", "1", "1", "1"],
-        date_of_death=["", "2017-05-06", "2019-06-07", "2020-07-08"],
-        died_in_2019=["", "", "2019", ""],
-    )
+    results = study.to_dicts()
+    assert [i["is_in_care_home"] for i in results] == ["0", "1", "1", "1"]
+    assert [i["care_home_type"] for i in results] == ["U", "PC", "PN", "PS"]
 
 
 def test_patients_admitted_to_icu():
     session = make_session()
     session.add_all(
         [
             Patient(
                 ICNARC=[
                     ICNARC(
-                        icuadmissiondatetime="2020-03-01",
-                        originalicuadmissiondate="2020-03-01",
-                        basicdays_respiratorysupport=2,
-                        advanceddays_respiratorysupport=2,
+                        IcuAdmissionDateTime="2020-03-01",
+                        OriginalIcuAdmissionDate="2020-03-01",
+                        BasicDays_RespiratorySupport=2,
+                        AdvancedDays_RespiratorySupport=2,
                     )
                 ]
             ),
             Patient(
                 ICNARC=[
                     ICNARC(
-                        icuadmissiondatetime="2020-03-01",
-                        originalicuadmissiondate="2020-02-01",
-                        basicdays_respiratorysupport=1,
-                        advanceddays_respiratorysupport=0,
+                        IcuAdmissionDateTime="2020-03-01",
+                        OriginalIcuAdmissionDate="2020-02-01",
+                        BasicDays_RespiratorySupport=1,
+                        AdvancedDays_RespiratorySupport=0,
                     )
                 ]
             ),
             Patient(),
             Patient(
                 ICNARC=[
                     ICNARC(
-                        icuadmissiondatetime="2020-01-01",
-                        originalicuadmissiondate="2020-01-01",
-                        basicdays_respiratorysupport=1,
-                        advanceddays_respiratorysupport=0,
+                        IcuAdmissionDateTime="2020-01-01",
+                        OriginalIcuAdmissionDate="2020-01-01",
+                        BasicDays_RespiratorySupport=1,
+                        AdvancedDays_RespiratorySupport=0,
                     )
                 ]
             ),
             Patient(
                 ICNARC=[
                     ICNARC(
-                        icuadmissiondatetime="2020-03-01",
-                        originalicuadmissiondate=None,
-                        basicdays_respiratorysupport=0,
-                        advanceddays_respiratorysupport=1,
+                        IcuAdmissionDateTime="2020-03-01",
+                        OriginalIcuAdmissionDate=None,
+                        BasicDays_RespiratorySupport=0,
+                        AdvancedDays_RespiratorySupport=1,
                     ),
                     ICNARC(
-                        icuadmissiondatetime="2020-04-01",
-                        originalicuadmissiondate=None,
-                        basicdays_respiratorysupport=0,
-                        advanceddays_respiratorysupport=0,
+                        IcuAdmissionDateTime="2020-04-01",
+                        OriginalIcuAdmissionDate=None,
+                        BasicDays_RespiratorySupport=0,
+                        AdvancedDays_RespiratorySupport=0,
                     ),
                 ]
             ),
         ]
     )
     session.commit()
 
     study = StudyDefinition(
         population=patients.all(),
         icu_first=patients.admitted_to_icu(
             on_or_after="2020-02-01",
+            include_day=True,
             returning="date_admitted",
-            date_format="YYYY-MM-DD",
             find_first_match_in_period=True,
         ),
         icu_last=patients.admitted_to_icu(
             on_or_after="2020-02-01",
+            include_day=True,
             returning="date_admitted",
-            date_format="YYYY-MM-DD",
             find_last_match_in_period=True,
         ),
         icu_flag=patients.admitted_to_icu(
             on_or_after="2020-02-01", returning="binary_flag"
         ),
         resp_support=patients.admitted_to_icu(
             on_or_after="2020-02-01",
@@ -1512,20 +1273,14 @@
             on_or_after="2020-02-01",
             returning="had_basic_respiratory_support",
         ),
         advanced_support=patients.admitted_to_icu(
             on_or_after="2020-02-01",
             returning="had_advanced_respiratory_support",
         ),
-        icu_second=patients.admitted_to_icu(
-            on_or_after="icu_first + 1 day",
-            returning="date_admitted",
-            date_format="YYYY-MM-DD",
-            find_first_match_in_period=True,
-        ),
     )
 
     assert_results(
         study.to_dicts(),
         icu_first=[
             "2020-03-01",
             "2020-02-01",
@@ -1540,73 +1295,43 @@
             "",
             "2020-04-01",
         ],
         icu_flag=["1", "1", "0", "0", "1"],
         resp_support=["1", "1", "0", "0", "1"],
         basic_support=["1", "1", "0", "0", "0"],
         advanced_support=["1", "0", "0", "0", "1"],
-        icu_second=[
-            "",
-            "",
-            "",
-            "",
-            "2020-04-01",
-        ],
     )
 
 
 def test_patients_with_these_codes_on_death_certificate():
     code = "COVID"
     session = make_session()
+    patient_with_dupe = Patient()
     session.add_all(
         [
             # Not dead
-            Patient(nhs_no="aaa"),
+            Patient(),
             # Died after date cutoff
-            Patient(
-                nhs_no="bbb",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20210101, icd10u=code, upload_date="2020-04-01"
-                    )
-                ],
-            ),
+            ONSDeaths(Patient=Patient(), dod="2021-01-01", icd10u=code),
             # Died of something else
-            Patient(
-                nhs_no="ccc",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20200201, icd10u="MI", upload_date="2020-04-01"
-                    )
-                ],
-            ),
+            ONSDeaths(Patient=Patient(), dod="2020-02-01", icd10u="MI"),
             # Covid underlying cause
-            Patient(
-                nhs_no="ddd",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20200201,
-                        icd10u=code,
-                        icd10014="MI",
-                        upload_date="2020-04-01",
-                    )
-                ],
+            ONSDeaths(
+                Patient=patient_with_dupe, dod="2020-02-01", icd10u=code, ICD10014="MI"
             ),
-            # Covid not underlying cause
-            Patient(
-                nhs_no="eee",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20200301,
-                        icd10u="MI",
-                        icd10014=code,
-                        upload_date="2020-04-01",
-                    )
-                ],
+            # A duplicate (the raw data does contain exact dupes, unfortunately)
+            ONSDeaths(
+                Patient=patient_with_dupe, dod="2020-02-01", icd10u=code, ICD10014="MI"
+            ),
+            # A duplicate with a different date of death (which now we have to handle)
+            ONSDeaths(
+                Patient=patient_with_dupe, dod="2020-02-02", icd10u=code, ICD10014="MI"
             ),
+            # Covid not underlying cause
+            ONSDeaths(Patient=Patient(), dod="2020-03-01", icd10u="MI", ICD10014=code),
         ]
     )
     session.commit()
     covid_codelist = codelist([code], system="icd10")
     study = StudyDefinition(
         population=patients.all(),
         died_of_covid=patients.with_these_codes_on_death_certificate(
@@ -1637,32 +1362,19 @@
 
 
 def test_patients_died_from_any_cause():
     session = make_session()
     session.add_all(
         [
             # Not dead
-            Patient(nhs_no="aaa"),
+            Patient(),
             # Died after date cutoff
-            Patient(
-                nhs_no="bbb",
-                ONSDeath=[ONSDeaths(reg_stat_dod=20210101, upload_date="2021-02-02")],
-            ),
+            Patient(ONSDeath=[ONSDeaths(dod="2021-01-01")]),
             # Died
-            Patient(
-                nhs_no="ccc",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20200201, icd10u="A", upload_date="2020-02-02"
-                    ),
-                    ONSDeaths(
-                        reg_stat_dod=20200201, icd10u="A", upload_date="2021-02-02"
-                    ),
-                ],
-            ),
+            Patient(ONSDeath=[ONSDeaths(dod="2020-02-01", icd10u="A")]),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         died=patients.died_from_any_cause(on_or_before="2020-06-01"),
         date_died=patients.died_from_any_cause(
@@ -1684,21 +1396,21 @@
 def test_patients_with_death_recorded_in_cpns():
     session = make_session()
     session.add_all(
         [
             # Not dead
             Patient(),
             # Died after date cutoff
-            Patient(CPNS=[CPNS(dateofdeath="2021-01-01")]),
+            Patient(CPNS=[CPNS(DateOfDeath="2021-01-01")]),
             # Patient should be included
-            Patient(CPNS=[CPNS(dateofdeath="2020-02-01")]),
+            Patient(CPNS=[CPNS(DateOfDeath="2020-02-01")]),
             # Patient has multple entries but with the same date of death so
             # should be handled correctly
             Patient(
-                CPNS=[CPNS(dateofdeath="2020-03-01"), CPNS(dateofdeath="2020-03-01")]
+                CPNS=[CPNS(DateOfDeath="2020-03-01"), CPNS(DateOfDeath="2020-03-01")]
             ),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         cpns_death=patients.with_death_recorded_in_cpns(on_or_before="2020-06-01"),
@@ -1719,25 +1431,61 @@
 
 
 def test_patients_with_death_recorded_in_cpns_raises_error_on_bad_data():
     session = make_session()
     session.add_all(
         # Create a patient with duplicate CPNS entries recording an
         # inconsistent date of death
-        [Patient(CPNS=[CPNS(dateofdeath="2020-03-01"), CPNS(dateofdeath="2020-02-01")])]
+        [Patient(CPNS=[CPNS(DateOfDeath="2020-03-01"), CPNS(DateOfDeath="2020-02-01")])]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(), cpns_death=patients.with_death_recorded_in_cpns()
     )
     with pytest.raises(Exception):
         study.to_dicts()
 
 
-def test_duplicate_id_checking():
+def test_to_sql_passes():
+    session = make_session()
+    patient = Patient(DateOfBirth="1950-01-01")
+    patient.CodedEvents.append(
+        CodedEvent(CTV3Code="XYZ", NumericValue=50, ConsultationDate="2002-06-01")
+    )
+    session.add(patient)
+    session.commit()
+
+    study = StudyDefinition(
+        population=patients.with_these_clinical_events(codelist(["XYZ"], "ctv3"))
+    )
+    sql = "SET NOCOUNT ON; "  # don't output count after table output
+    sql += study.to_sql()
+    db_dict = mssql_connection_params_from_url(study.backend.database_url)
+    cmd = [
+        "sqlcmd",
+        "-S",
+        db_dict["host"] + "," + str(db_dict["port"]),
+        "-d",
+        db_dict["database"],
+        "-U",
+        db_dict["username"],
+        "-P",
+        db_dict["password"],
+        "-Q",
+        sql,
+        "-W",  # strip whitespace
+    ]
+    result = subprocess.run(
+        cmd, capture_output=True, check=True, encoding="utf8"
+    ).stdout
+    patient_id = result.splitlines()[-1]
+    assert patient_id == str(patient.Patient_ID)
+
+
+def test_duplicate_id_checking(tmp_path):
     study = StudyDefinition(population=patients.all())
     # A bit of a hack: overwrite the queries we're going to run with a query which
     # deliberately returns duplicate values
     study.backend.queries = [
         """
         SELECT * FROM (
           VALUES
@@ -1747,181 +1495,117 @@
             (1,4)
         ) t (patient_id, foo)
         """,
     ]
     with pytest.raises(RuntimeError):
         study.to_dicts()
     with pytest.raises(RuntimeError):
-        with tempfile.NamedTemporaryFile(mode="w+", suffix=".csv") as f:
-            study.to_file(f.name)
-
-
-def test_column_name_clashes_produce_errors():
-    with pytest.raises(ValueError):
-        StudyDefinition(
-            population=patients.all(),
-            age=patients.age_as_of("2020-01-01"),
-            status=patients.satisfying(
-                "age > 70 AND sex = 'M'",
-                sex=patients.sex(),
-                age=patients.age_as_of("2010-01-01"),
-            ),
-        )
-
-
-def test_recursive_definitions_produce_errors():
-    with pytest.raises(ValueError):
-        StudyDefinition(
-            population=patients.all(),
-            this=patients.satisfying("that = 1"),
-            that=patients.satisfying("this = 1"),
-        )
+        study.to_csv(tmp_path / "test.csv")
+    # Check that we don't produce a normal output file but we do leave a
+    # partial file
+    assert not os.path.exists(tmp_path / "test.csv")
+    partial_files = glob.glob(f"{tmp_path}/test.partial.*.csv")
+    assert len(partial_files) == 1
 
 
 def test_using_expression_in_population_definition():
     session = make_session()
     session.add_all(
         [
             Patient(
-                gender=1,
-                date_of_birth="1970-01-01",
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2000-01-01"
-                    )
+                Sex="M",
+                DateOfBirth="1970-01-01",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2000-01-01")
                 ],
             ),
-            Patient(gender=1, date_of_birth="1975-01-01"),
+            Patient(Sex="M", DateOfBirth="1975-01-01"),
             Patient(
-                gender=2,
-                date_of_birth="1980-01-01",
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2000-01-01"
-                    )
+                Sex="F",
+                DateOfBirth="1980-01-01",
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2000-01-01")
                 ],
             ),
-            Patient(gender=2, date_of_birth="1985-01-01"),
+            Patient(Sex="F", DateOfBirth="1985-01-01"),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.satisfying(
             "has_foo_code AND sex = 'M'",
             has_foo_code=patients.with_these_clinical_events(
-                codelist(["10000001"], "snomedct")
+                codelist(["foo1"], "ctv3")
             ),
             sex=patients.sex(),
         ),
         age=patients.age_as_of("2020-01-01"),
     )
     results = study.to_dicts()
     assert results[0].keys() == {"patient_id", "age"}
     assert [i["age"] for i in results] == ["50"]
 
 
 def test_quote():
     with pytest.raises(ValueError):
         quote("foo!")
-    assert quote("2012-02-01") == "DATE('2012-02-01')"
+    assert quote("2012-02-01") == "'20120201'"
     assert quote("2012") == "'2012'"
     assert quote(2012) == "2012"
     assert quote(0.1) == "0.1"
     assert quote("foo") == "'foo'"
 
 
 def test_number_of_episodes():
     session = make_session()
     session.add_all(
         [
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2010-01-01"
-                    ),
+                CodedEvents=[
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2010-01-01"),
                     # Throw in some irrelevant events
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2010-01-02"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000002", effective_date="2010-01-03"
-                    ),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2010-01-02"),
+                    CodedEvent(CTV3Code="mto2", ConsultationDate="2010-01-03"),
                     # These two should be merged in to the previous event
                     # because there's not more than 14 days between them
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2010-01-14"
-                    ),
-                    Observation(
-                        snomed_concept_id="10000003", effective_date="2010-01-20"
-                    ),
+                    CodedEvent(CTV3Code="foo2", ConsultationDate="2010-01-14"),
+                    CodedEvent(CTV3Code="foo3", ConsultationDate="2010-01-20"),
                     # This is just outside the limit so should count as another event
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2010-02-04"
-                    ),
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2010-02-04"),
                     # This shouldn't count because there's an "ignore" event on
                     # the same day (though at a different time)
-                    Observation(
-                        snomed_concept_id="10000001",
-                        effective_date="2012-01-01T10:45:00",
-                    ),
-                    Observation(
-                        snomed_concept_id="20000002",
-                        effective_date="2012-01-01T16:10:00",
-                    ),
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2012-01-01T10:45:00"),
+                    CodedEvent(CTV3Code="bar2", ConsultationDate="2012-01-01T16:10:00"),
                     # This should be another episode
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2015-03-05"
-                    ),
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2015-03-05"),
                     # This "ignore" event should have no effect because it occurs
                     # on a different day
-                    Observation(
-                        snomed_concept_id="20000001", effective_date="2015-03-06"
-                    ),
+                    CodedEvent(CTV3Code="bar1", ConsultationDate="2015-03-06"),
                     # This is after the time limit and so shouldn't count
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2020-02-05"
-                    ),
+                    CodedEvent(CTV3Code="foo1", ConsultationDate="2020-02-05"),
                 ]
             ),
             # This patient doesn't have any relevant events
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2010-01-01"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000002", effective_date="2010-01-14"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000003", effective_date="2010-01-20"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2010-02-04"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001",
-                        effective_date="2012-01-01T10:45:00",
-                    ),
-                    Observation(
-                        snomed_concept_id="40000004",
-                        effective_date="2012-01-01T16:10:00",
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2015-03-05"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2020-02-05"
-                    ),
+                CodedEvents=[
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2010-01-01"),
+                    CodedEvent(CTV3Code="mto2", ConsultationDate="2010-01-14"),
+                    CodedEvent(CTV3Code="mto3", ConsultationDate="2010-01-20"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2010-02-04"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2012-01-01T10:45:00"),
+                    CodedEvent(CTV3Code="mtr2", ConsultationDate="2012-01-01T16:10:00"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2015-03-05"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2020-02-05"),
                 ]
             ),
         ]
     )
     session.commit()
-    foo_codes = codelist(["10000001", "10000002", "10000003"], "snomedct")
-    bar_codes = codelist(["20000001", "20000002"], "snomedct")
+    foo_codes = codelist(["foo1", "foo2", "foo3"], "ctv3")
+    bar_codes = codelist(["bar1", "bar2"], "ctv3")
     study = StudyDefinition(
         population=patients.all(),
         episode_count=patients.with_these_clinical_events(
             foo_codes,
             on_or_before="2020-01-01",
             ignore_days_where_these_codes_occur=bar_codes,
             returning="number_of_episodes",
@@ -1936,102 +1620,93 @@
     )
     results = study.to_dicts()
     assert [i["episode_count"] for i in results] == ["3", "0"]
     assert [i["event_count"] for i in results] == ["5", "0"]
 
 
 def test_number_of_episodes_for_medications():
+    oral_steriod = MedicationDictionary(
+        FullName="Oral Steroid", DMD_ID="ab12", MultilexDrug_ID="1"
+    )
+    other_drug = MedicationDictionary(
+        FullName="Other Drug", DMD_ID="cd34", MultilexDrug_ID="2"
+    )
     session = make_session()
     session.add_all(
         [
             Patient(
-                medications=[
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2010-01-01"
+                MedicationIssues=[
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2010-01-01"
                     ),
                     # Throw in some irrelevant prescriptions
-                    Medication(
-                        snomed_concept_id="34343434", effective_date="2010-01-02"
+                    MedicationIssue(
+                        MedicationDictionary=other_drug, ConsultationDate="2010-01-02"
                     ),
-                    Medication(
-                        snomed_concept_id="34343434", effective_date="2010-01-03"
+                    MedicationIssue(
+                        MedicationDictionary=other_drug, ConsultationDate="2010-01-03"
                     ),
                     # These two should be merged in to the previous event
                     # because there's not more than 14 days between them
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2010-01-14"
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2010-01-14"
                     ),
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2010-01-20"
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2010-01-20"
                     ),
                     # This is just outside the limit so should count as another event
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2010-02-04"
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2010-02-04"
                     ),
                     # This shouldn't count because there's an "ignore" event on
                     # the same day (though at a different time)
-                    Medication(
-                        snomed_concept_id="12121212",
-                        effective_date="2012-01-01T10:45:00",
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod,
+                        ConsultationDate="2012-01-01T10:45:00",
                     ),
                     # This should be another episode
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2015-03-05"
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2015-03-05"
                     ),
                     # This is after the time limit and so shouldn't count
-                    Medication(
-                        snomed_concept_id="12121212", effective_date="2020-02-05"
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod, ConsultationDate="2020-02-05"
                     ),
                 ],
-                observations=[
+                CodedEvents=[
                     # This "ignore" event should cause us to skip one of the
                     # meds issues above
-                    Observation(
-                        snomed_concept_id="20000002",
-                        effective_date="2012-01-01T16:10:00",
-                    ),
+                    CodedEvent(CTV3Code="bar2", ConsultationDate="2012-01-01T16:10:00"),
                     # This "ignore" event should have no effect because it
                     # doesn't occur on the same day as any meds issue
-                    Observation(
-                        snomed_concept_id="20000001", effective_date="2015-03-06"
-                    ),
+                    CodedEvent(CTV3Code="bar1", ConsultationDate="2015-03-06"),
                 ],
             ),
             # This patient doesn't have any relevant events or prescriptions
             Patient(
-                medications=[
-                    Medication(
-                        snomed_concept_id="34343434", effective_date="2010-01-02"
+                MedicationIssues=[
+                    MedicationIssue(
+                        MedicationDictionary=other_drug, ConsultationDate="2010-01-02"
                     ),
-                    Medication(
-                        snomed_concept_id="34343434", effective_date="2010-01-03"
+                    MedicationIssue(
+                        MedicationDictionary=other_drug, ConsultationDate="2010-01-03"
                     ),
                 ],
-                observations=[
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2010-02-04"
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001",
-                        effective_date="2012-01-01T10:45:00",
-                    ),
-                    Observation(
-                        snomed_concept_id="40000004",
-                        effective_date="2012-01-01T16:10:00",
-                    ),
-                    Observation(
-                        snomed_concept_id="40000001", effective_date="2015-03-05"
-                    ),
+                CodedEvents=[
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2010-02-04"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2012-01-01T10:45:00"),
+                    CodedEvent(CTV3Code="mtr2", ConsultationDate="2012-01-01T16:10:00"),
+                    CodedEvent(CTV3Code="mto1", ConsultationDate="2015-03-05"),
                 ],
             ),
         ]
     )
     session.commit()
-    foo_codes = codelist(["12121212"], "snomed")
-    bar_codes = codelist(["20000001", "20000002"], "snomedct")
+    foo_codes = codelist(["ab12"], "snomed")
+    bar_codes = codelist(["bar1", "bar2"], "ctv3")
     study = StudyDefinition(
         population=patients.all(),
         episode_count=patients.with_these_medications(
             foo_codes,
             on_or_before="2020-01-01",
             ignore_days_where_these_clinical_codes_occur=bar_codes,
             returning="number_of_episodes",
@@ -2046,745 +1721,1138 @@
     )
     results = study.to_dicts()
     assert [i["episode_count"] for i in results] == ["3", "0"]
     assert [i["event_count"] for i in results] == ["5", "0"]
 
 
 def test_medications_returning_code_with_ignored_days():
+    oral_steriod = MedicationDictionary(
+        FullName="Oral Steroid", DMD_ID="ab12", MultilexDrug_ID="1"
+    )
+    other_drug = MedicationDictionary(
+        FullName="Other Drug", DMD_ID="cd34", MultilexDrug_ID="2"
+    )
     session = make_session()
     session.add_all(
         [
             Patient(
-                medications=[
-                    Medication(
-                        snomed_concept_id="34343434", effective_date="2010-01-03"
+                MedicationIssues=[
+                    MedicationIssue(
+                        MedicationDictionary=other_drug, ConsultationDate="2010-01-03"
                     ),
                     # This shouldn't count because there's an "ignore" event on
                     # the same day (though at a different time)
-                    Medication(
-                        snomed_concept_id="12121212",
-                        effective_date="2012-01-01T10:45:00",
+                    MedicationIssue(
+                        MedicationDictionary=oral_steriod,
+                        ConsultationDate="2012-01-01T10:45:00",
                     ),
                 ],
-                observations=[
+                CodedEvents=[
                     # This "ignore" event should cause us to skip one of the
                     # meds issues above
-                    Observation(
-                        snomed_concept_id="20000001",
-                        effective_date="2012-01-01T16:10:00",
-                    ),
+                    CodedEvent(CTV3Code="bar1", ConsultationDate="2012-01-01T16:10:00"),
                 ],
             ),
         ]
     )
     session.commit()
-    drug_codes = codelist(["12121212", "34343434"], "snomed")
-    annual_review_codes = codelist(["20000001"], "snomedct")
+    drug_codes = codelist(["ab12", "cd34"], "snomed")
+    annual_review_codes = codelist(["bar1"], "ctv3")
     study = StudyDefinition(
         population=patients.all(),
         most_recent_drug=patients.with_these_medications(
             drug_codes,
             ignore_days_where_these_clinical_codes_occur=annual_review_codes,
             returning="code",
         ),
         most_recent_drug_date=patients.date_of(
             "most_recent_drug", date_format="YYYY-MM-DD"
         ),
     )
     results = study.to_dicts()
-    assert [i["most_recent_drug"] for i in results] == ["34343434"]
+    assert [i["most_recent_drug"] for i in results] == ["cd34"]
     assert [i["most_recent_drug_date"] for i in results] == ["2010-01-03"]
 
 
+def test_patients_with_tpp_vaccination_record():
+    session = make_session()
+    vaccines = [
+        (1, "Hepatyrix", ["TYPHOID", "HEPATITIS A"]),
+        (2, "Madeva", ["INFLUENZA"]),
+        (3, "Optaflu", ["INFLUENZA"]),
+    ]
+    ids = {}
+    for name_id, name, contents in vaccines:
+        ids[name] = name_id
+        for content in contents:
+            session.add(
+                VaccinationReference(
+                    VaccinationName=name,
+                    VaccinationName_ID=name_id,
+                    VaccinationContent=content,
+                )
+            )
+    session.add_all(
+        [
+            Patient(
+                Vaccinations=[
+                    Vaccination(
+                        VaccinationName_ID=ids["Hepatyrix"],
+                        VaccinationDate="2010-01-01",
+                    ),
+                    Vaccination(
+                        VaccinationName_ID=ids["Optaflu"], VaccinationDate="2014-01-01"
+                    ),
+                ]
+            ),
+            Patient(
+                Vaccinations=[
+                    Vaccination(
+                        VaccinationName_ID=ids["Madeva"], VaccinationDate="2013-01-01"
+                    ),
+                    Vaccination(
+                        VaccinationName_ID=ids["Hepatyrix"],
+                        VaccinationDate="2015-01-01",
+                    ),
+                ]
+            ),
+        ]
+    )
+    session.commit()
+
+    study = StudyDefinition(
+        population=patients.all(),
+        value=patients.with_tpp_vaccination_record(
+            target_disease_matches="TYPHOID",
+            on_or_after="2012-01-01",
+        ),
+        date=patients.date_of("value"),
+    )
+    results = study.to_dicts()
+    assert [i["value"] for i in results] == ["0", "1"]
+    assert [i["date"] for i in results] == ["", "2015"]
+
+    study = StudyDefinition(
+        population=patients.all(),
+        value=patients.with_tpp_vaccination_record(
+            target_disease_matches="INFLUENZA",
+            on_or_after="2012-01-01",
+            find_last_match_in_period=True,
+            returning="date",
+        ),
+    )
+    assert [i["value"] for i in study.to_dicts()] == ["2014", "2013"]
+
+    study = StudyDefinition(
+        population=patients.all(),
+        value=patients.with_tpp_vaccination_record(
+            product_name_matches=["Madeva", "Hepatyrix"],
+            find_first_match_in_period=True,
+            returning="date",
+        ),
+    )
+    assert [i["value"] for i in study.to_dicts()] == ["2010", "2013"]
+
+
+def test_patients_with_gp_consultations():
+    session = make_session()
+    session.add_all(
+        [
+            Patient(
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="2014-01-01",
+                        EndDate="2020-05-01",
+                        Organisation=Organisation(GoLiveDate="2001-01-01"),
+                    )
+                ],
+                Appointments=[
+                    # Before period starts
+                    Appointment(
+                        SeenDate="2009-01-01", Status=AppointmentStatus.FINISHED
+                    ),
+                    # After period ends
+                    Appointment(
+                        SeenDate="2020-02-01", Status=AppointmentStatus.FINISHED
+                    ),
+                ],
+            ),
+            Patient(
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="2001-01-01",
+                        EndDate="2016-01-01",
+                        Organisation=Organisation(GoLiveDate="1999-10-01"),
+                    )
+                ],
+                Appointments=[
+                    Appointment(
+                        SeenDate="2011-01-01", Status=AppointmentStatus.FINISHED
+                    ),
+                    # Should not be counted
+                    Appointment(
+                        SeenDate="2012-01-01", Status=AppointmentStatus.DID_NOT_ATTEND
+                    ),
+                    Appointment(
+                        SeenDate="2013-01-01", Status=AppointmentStatus.FINISHED
+                    ),
+                ],
+            ),
+            # This patient was registered with one practice throughout the
+            # required period, but that practice wasn't using SystmOne so we
+            # don't have full consultation history
+            Patient(
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="2008-01-01",
+                        EndDate="2016-01-01",
+                        Organisation=Organisation(GoLiveDate="2012-01-01"),
+                    )
+                ],
+            ),
+        ]
+    )
+    session.commit()
+    study = StudyDefinition(
+        population=patients.all(),
+        consultation_count=patients.with_gp_consultations(
+            between=["2010-01-01", "2015-01-01"],
+            find_last_match_in_period=True,
+            returning="number_of_matches_in_period",
+        ),
+        latest_consultation_date=patients.date_of(
+            "consultation_count", date_format="YYYY-MM"
+        ),
+        has_history=patients.with_complete_gp_consultation_history_between(
+            "2010-01-01", "2015-01-01"
+        ),
+    )
+    results = study.to_dicts()
+    assert [x["latest_consultation_date"] for x in results] == ["", "2013-01", ""]
+    assert [x["consultation_count"] for x in results] == ["0", "2", "0"]
+    assert [x["has_history"] for x in results] == ["0", "1", "0"]
+
+
+def test_patients_with_test_result_in_sgss():
+    session = make_session()
+    session.add_all(
+        [
+            Patient(
+                SGSS_Positives=[
+                    SGSS_Positive(Earliest_Specimen_Date="2020-05-15"),
+                    SGSS_Positive(Earliest_Specimen_Date="2020-05-20"),
+                ],
+            ),
+            Patient(
+                SGSS_Negatives=[SGSS_Negative(Earliest_Specimen_Date="2020-04-01")],
+                SGSS_Positives=[SGSS_Positive(Earliest_Specimen_Date="2020-04-20")],
+            ),
+            Patient(
+                SGSS_Negatives=[SGSS_Negative(Earliest_Specimen_Date="2020-04-01")],
+            ),
+            Patient(),
+        ]
+    )
+    session.commit()
+    study = StudyDefinition(
+        population=patients.all(),
+        positive_covid_test_ever=patients.with_test_result_in_sgss(
+            pathogen="SARS-CoV-2",
+            test_result="positive",
+        ),
+        negative_covid_test_ever=patients.with_test_result_in_sgss(
+            pathogen="SARS-CoV-2",
+            test_result="negative",
+        ),
+        tested_before_may=patients.with_test_result_in_sgss(
+            pathogen="SARS-CoV-2", test_result="any", on_or_before="2020-05-01"
+        ),
+        first_positive_test_date=patients.with_test_result_in_sgss(
+            pathogen="SARS-CoV-2",
+            test_result="positive",
+            find_first_match_in_period=True,
+            returning="date",
+            date_format="YYYY-MM-DD",
+        ),
+    )
+    results = study.to_dicts()
+    assert [x["positive_covid_test_ever"] for x in results] == ["1", "1", "0", "0"]
+    assert [x["negative_covid_test_ever"] for x in results] == ["0", "1", "1", "0"]
+    assert [x["tested_before_may"] for x in results] == ["0", "1", "1", "0"]
+    assert [x["first_positive_test_date"] for x in results] == [
+        "2020-05-15",
+        "2020-04-20",
+        "",
+        "",
+    ]
+
+
+@pytest.mark.parametrize("positive", [True, False])
+def test_patients_with_test_result_in_sgss_raises_error_on_bad_data(positive):
+    kwargs = dict(
+        Earliest_Specimen_Date="2020-05-15", Organism_Species_Name="unexpected"
+    )
+    if positive:
+        patient = Patient(SGSS_Positives=[SGSS_Positive(**kwargs)])
+    else:
+        patient = Patient(SGSS_Negatives=[SGSS_Negative(**kwargs)])
+    session = make_session()
+    session.add(patient)
+    session.commit()
+    study = StudyDefinition(
+        population=patients.all(),
+        covid_test=patients.with_test_result_in_sgss(
+            pathogen="SARS-CoV-2",
+        ),
+    )
+    with pytest.raises(Exception):
+        study.to_dicts()
+
+
+def test_patients_date_of_birth():
+    session = make_session()
+    session.add_all(
+        [
+            Patient(DateOfBirth="1975-06-10"),
+            Patient(DateOfBirth="1999-10-15"),
+        ]
+    )
+    session.commit()
+    study = StudyDefinition(
+        population=patients.all(),
+        year_of_birth=patients.date_of_birth(),
+        month_of_birth=patients.date_of_birth(date_format="YYYY-MM"),
+    )
+    results = study.to_dicts()
+    assert [x["year_of_birth"] for x in results] == ["1975", "1999"]
+    assert [x["month_of_birth"] for x in results] == ["1975-06", "1999-10"]
+    # Requesting the exact day is not supported for IG reasons
+    with pytest.raises(Exception):
+        StudyDefinition(
+            population=patients.all(),
+            day_of_birth=patients.date_of_birth(date_format="YYYY-MM-DD"),
+        )
+
+
 def test_patients_aggregate_value_of():
     session = make_session()
     session.add_all(
         [
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id=111, value_pq_1=7, effective_date="2012-01-01"
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code="ABC", NumericValue=7, ConsultationDate="2012-01-01"
                     ),
-                    Observation(
-                        snomed_concept_id=222,
-                        value_pq_1=23,
-                        effective_date="2018-01-01",
+                    CodedEvent(
+                        CTV3Code="XYZ", NumericValue=23, ConsultationDate="2018-01-01"
                     ),
                 ]
             ),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id=111,
-                        value_pq_1=18,
-                        effective_date="2014-01-01",
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code="ABC", NumericValue=18, ConsultationDate="2014-01-01"
                     ),
-                    Observation(
-                        snomed_concept_id=222, value_pq_1=4, effective_date="2017-01-01"
+                    CodedEvent(
+                        CTV3Code="XYZ", NumericValue=4, ConsultationDate="2017-01-01"
                     ),
                 ]
             ),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id=111,
-                        value_pq_1=10,
-                        effective_date="2015-01-01",
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code="ABC", NumericValue=10, ConsultationDate="2015-01-01"
                     ),
                 ]
             ),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id=222, value_pq_1=8, effective_date="2019-01-01"
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code="XYZ", NumericValue=8, ConsultationDate="2019-01-01"
                     ),
                 ]
             ),
             Patient(),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
         # Values
         abc_value=patients.with_these_clinical_events(
-            codelist([111], system="snomedct"), returning="numeric_value"
+            codelist(["ABC"], system="ctv3"), returning="numeric_value"
         ),
         xyz_value=patients.with_these_clinical_events(
-            codelist([222], system="snomedct"), returning="numeric_value"
+            codelist(["XYZ"], system="ctv3"), returning="numeric_value"
         ),
         # Dates
-        abc_date=patients.date_of("abc_value", date_format="YYYY-MM-DD"),
-        xyz_date=patients.date_of("xyz_value", date_format="YYYY-MM-DD"),
+        abc_date=patients.date_of("abc_value"),
+        xyz_date=patients.date_of("xyz_value"),
         # Aggregates
         max_value=patients.maximum_of("abc_value", "xyz_value"),
         min_value=patients.minimum_of("abc_value", "xyz_value"),
         max_date=patients.maximum_of("abc_date", "xyz_date"),
         min_date=patients.minimum_of("abc_date", "xyz_date"),
-        # Aggregates with fixed dates
-        max_date_fixed=patients.maximum_of("abc_date", "2014-05-16"),
-        min_date_fixed=patients.minimum_of("xyz_date", "2017-11-10"),
     )
     results = study.to_dicts()
     assert [x["max_value"] for x in results] == ["23.0", "18.0", "10.0", "8.0", "0.0"]
     assert [x["min_value"] for x in results] == ["7.0", "4.0", "10.0", "8.0", "0.0"]
-    assert [x["max_date"] for x in results] == [
-        "2018-01-01",
-        "2017-01-01",
-        "2015-01-01",
-        "2019-01-01",
-        "",
-    ]
-    assert [x["min_date"] for x in results] == [
-        "2012-01-01",
-        "2014-01-01",
-        "2015-01-01",
-        "2019-01-01",
-        "",
-    ]
-    assert [x["max_date_fixed"] for x in results] == [
-        "2014-05-16",
-        "2014-05-16",
-        "2015-01-01",
-        "2014-05-16",
-        "2014-05-16",
-    ]
-    assert [x["min_date_fixed"] for x in results] == [
-        "2017-11-10",
-        "2017-01-01",
-        "2017-11-10",
-        "2017-11-10",
-        "2017-11-10",
-    ]
+    assert [x["max_date"] for x in results] == ["2018", "2017", "2015", "2019", ""]
+    assert [x["min_date"] for x in results] == ["2012", "2014", "2015", "2019", ""]
     # Test with hidden columns
     study_with_hidden_columns = StudyDefinition(
         population=patients.all(),
         max_value=patients.maximum_of(
             abc_value=patients.with_these_clinical_events(
-                codelist([111], system="snomedct"), returning="numeric_value"
+                codelist(["ABC"], system="ctv3"), returning="numeric_value"
             ),
             xyz_value=patients.with_these_clinical_events(
-                codelist([222], system="snomedct"), returning="numeric_value"
+                codelist(["XYZ"], system="ctv3"), returning="numeric_value"
             ),
         ),
     )
     results = study_with_hidden_columns.to_dicts()
     assert [x["max_value"] for x in results] == ["23.0", "18.0", "10.0", "8.0", "0.0"]
     assert "abc_value" not in results[0].keys()
 
 
-def test_patients_date_deregistered_from_all_supported_practices():
+def test_patients_household_as_of():
     session = make_session()
     session.add_all(
         [
-            # Never de-registered
-            Patient(registered_date="2001-01-01", registration_end_date=None),
-            # De-registered, but after cut-off date
-            Patient(registered_date="2001-01-01", registration_end_date="2020-01-01"),
-            # De-registered
-            Patient(registered_date="2001-01-01", registration_end_date="2010-01-01"),
+            Patient(),
+            Patient(
+                HouseholdMemberships=[
+                    HouseholdMember(
+                        Household=Household(
+                            Household_ID=123,
+                            HouseholdSize=2,
+                            Prison=True,
+                            MixedSoftwareHousehold=False,
+                            TppPercentage=100,
+                            MSOA="S02001286",
+                        )
+                    )
+                ]
+            ),
+            Patient(
+                HouseholdMemberships=[
+                    HouseholdMember(
+                        Household=Household(
+                            Household_ID=456,
+                            HouseholdSize=3,
+                            Prison=False,
+                            TppPercentage=66,
+                            MixedSoftwareHousehold=True,
+                            MSOA="S02001354",
+                        )
+                    )
+                ]
+            ),
+            # This shouldn't produce any output because the entry is flagged as
+            # No-Fixed-Abode/Unknown
+            Patient(
+                HouseholdMemberships=[
+                    HouseholdMember(
+                        Household=Household(
+                            Household_ID=789,
+                            HouseholdSize=4,
+                            NFA_Unknown=True,
+                            Prison=False,
+                            TppPercentage=100,
+                            MixedSoftwareHousehold=False,
+                            MSOA="S02001781",
+                        )
+                    )
+                ]
+            ),
         ]
     )
     session.commit()
     study = StudyDefinition(
         population=patients.all(),
-        dereg_date=patients.date_deregistered_from_all_supported_practices(
-            on_or_before="2015-01-01",
-            date_format="YYYY-MM",
+        household_id=patients.household_as_of("2020-02-01", returning="pseudo_id"),
+        household_size=patients.household_as_of(
+            "2020-02-01", returning="household_size"
+        ),
+        is_prison=patients.household_as_of("2020-02-01", returning="is_prison"),
+        mixed_ehr=patients.household_as_of(
+            "2020-02-01", returning="has_members_in_other_ehr_systems"
         ),
+        percent_tpp=patients.household_as_of(
+            "2020-02-01", returning="percentage_of_members_with_data_in_this_backend"
+        ),
+        msoa=patients.household_as_of("2020-02-01", returning="msoa"),
+    )
+    assert_results(
+        study.to_dicts(),
+        household_id=["0", "123", "456", "0"],
+        household_size=["0", "2", "3", "0"],
+        is_prison=["0", "1", "0", "0"],
+        mixed_ehr=["0", "0", "1", "0"],
+        percent_tpp=["0", "100", "66", "0"],
+        msoa=["", "S02001286", "S02001354", ""],
     )
-    assert_results(study.to_dicts(), dereg_date=["", "", "2010-01"])
+    # We currently only accept one specific date
+    with pytest.raises(ValueError):
+        StudyDefinition(
+            population=patients.all(),
+            size=patients.household_as_of("2020-05-01", returning="household_size"),
+        )
+
 
+def test_patients_attended_emergency_care():
+    discharge_to_ward = "306706006"
+    discharge_to_home = "306689006"
+    covid_19 = "1240751000000100"
+    not_covid_19 = "125605004"
 
-def test_dynamic_index_dates():
     session = make_session()
     session.add_all(
         [
+            # Patient with no episodes
+            Patient(Patient_ID=1),
+            # Patient with no episodes in period
+            Patient(
+                Patient_ID=2,
+                ECEpisodes=[
+                    EC(
+                        EC_Ident=1,
+                        Arrival_Date="2020-01-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_home,
+                        Diagnoses=[
+                            EC_Diagnosis(Patient_ID=3, EC_Diagnosis_01=covid_19)
+                        ],
+                    )
+                ],
+            ),
+            # Patient with some episodes in period
+            Patient(
+                Patient_ID=3,
+                ECEpisodes=[
+                    EC(
+                        EC_Ident=2,
+                        Arrival_Date="2020-01-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_home,
+                        Diagnoses=[
+                            EC_Diagnosis(Patient_ID=3, EC_Diagnosis_01=not_covid_19)
+                        ],
+                    ),
+                    EC(
+                        EC_Ident=3,
+                        Arrival_Date="2020-03-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_home,
+                        Diagnoses=[
+                            EC_Diagnosis(Patient_ID=3, EC_Diagnosis_01=not_covid_19)
+                        ],
+                    ),
+                ],
+            ),
+            # Patient with multiple episodes in period
             Patient(
-                observations=[
-                    Observation(effective_date="2020-01-15", snomed_concept_id=123),
-                    Observation(effective_date="2020-02-01", snomed_concept_id=123),
-                    Observation(effective_date="2020-03-01", snomed_concept_id=456),
-                    Observation(effective_date="2020-04-20", snomed_concept_id=123),
-                    Observation(effective_date="2020-05-01", snomed_concept_id=123),
-                    Observation(effective_date="2020-06-01", snomed_concept_id=456),
+                Patient_ID=4,
+                ECEpisodes=[
+                    EC(
+                        EC_Ident=4,
+                        Arrival_Date="2020-03-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_home,
+                        Diagnoses=[
+                            EC_Diagnosis(Patient_ID=3, EC_Diagnosis_01=not_covid_19)
+                        ],
+                    ),
+                    EC(
+                        EC_Ident=5,
+                        Arrival_Date="2020-05-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_ward,
+                        Diagnoses=[
+                            EC_Diagnosis(
+                                Patient_ID=3,
+                                EC_Diagnosis_01=covid_19,
+                                EC_Diagnosis_02=not_covid_19,
+                            )
+                        ],
+                    ),
+                    EC(
+                        EC_Ident=6,
+                        Arrival_Date="2020-07-01",
+                        Discharge_Destination_SNOMED_CT=discharge_to_ward,
+                        Diagnoses=[
+                            EC_Diagnosis(
+                                Patient_ID=3,
+                                EC_Diagnosis_01=not_covid_19,
+                                EC_Diagnosis_02=covid_19,
+                            )
+                        ],
+                    ),
                 ],
             ),
         ]
     )
     session.commit()
+
     study = StudyDefinition(
         population=patients.all(),
-        earliest_123=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
-            date_format="YYYY-MM-DD",
+        attended=patients.attended_emergency_care(
+            on_or_after="2020-02-01", returning="binary_flag"
+        ),
+        count=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+        ),
+        first_date=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
             find_first_match_in_period=True,
+            date_format="YYYY-MM-DD",
         ),
-        earliest_456=patients.with_these_clinical_events(
-            codelist(["456"], system="snomed"),
-            returning="date",
+        last_date=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
+            find_last_match_in_period=True,
             date_format="YYYY-MM-DD",
+        ),
+        first_destination=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="discharge_destination",
             find_first_match_in_period=True,
         ),
-        earliest_123_or_456=patients.minimum_of("earliest_123", "earliest_456"),
-        latest_123_before_456=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
-            date_format="YYYY-MM-DD",
+        last_destination=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="discharge_destination",
             find_last_match_in_period=True,
-            on_or_before="earliest_456",
         ),
-        latest_123_in_month_after_456=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
+        with_covid=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="binary_flag",
+            with_these_diagnoses=codelist([covid_19], "snomed"),
+        ),
+        first_date_with_covid=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
+            date_format="YYYY-MM-DD",
+            find_first_match_in_period=True,
+            with_these_diagnoses=codelist([covid_19], "snomed"),
+        ),
+        last_date_with_covid=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
             date_format="YYYY-MM-DD",
             find_last_match_in_period=True,
-            on_or_before="last_day_of_month(earliest_456) + 1 month",
+            with_these_diagnoses=codelist([covid_19], "snomed"),
         ),
-        next_123=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
+        first_date_discharged_to_ward=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
             date_format="YYYY-MM-DD",
             find_first_match_in_period=True,
-            on_or_after="earliest_123_or_456 + 1 day",
+            discharged_to=[discharge_to_ward],
+        ),
+        last_date_discharged_to_ward=patients.attended_emergency_care(
+            on_or_after="2020-02-01",
+            returning="date_arrived",
+            date_format="YYYY-MM-DD",
+            find_last_match_in_period=True,
+            discharged_to=[discharge_to_ward],
         ),
     )
+
     assert_results(
         study.to_dicts(),
-        earliest_123=["2020-01-15"],
-        earliest_456=["2020-03-01"],
-        earliest_123_or_456=["2020-01-15"],
-        latest_123_before_456=["2020-02-01"],
-        latest_123_in_month_after_456=["2020-04-20"],
-        next_123=["2020-02-01"],
+        attended=["0", "0", "1", "1"],
+        count=["0", "0", "1", "3"],
+        first_date=["", "", "2020-03-01", "2020-03-01"],
+        last_date=["", "", "2020-03-01", "2020-07-01"],
+        first_destination=["", "", discharge_to_home, discharge_to_home],
+        last_destination=["", "", discharge_to_home, discharge_to_ward],
+        with_covid=["0", "0", "0", "1"],
+        first_date_with_covid=["", "", "", "2020-05-01"],
+        last_date_with_covid=["", "", "", "2020-07-01"],
+        first_date_discharged_to_ward=["", "", "", "2020-05-01"],
+        last_date_discharged_to_ward=["", "", "", "2020-07-01"],
     )
 
 
-def test_dynamic_index_dates_with_invalid_expression():
-    with pytest.raises(InvalidExpressionError):
-        StudyDefinition(
-            population=patients.all(),
-            earliest_123=patients.with_these_clinical_events(
-                codelist([123], system="snomed"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-            latest_456_in_month_after_bar=patients.with_these_clinical_events(
-                codelist([456], system="snomed"),
-                on_or_before="last_day_of_month(earliest_bar) + 1 mnth",
-            ),
-        )
-
-
-@pytest.mark.parametrize(
-    "index_date,expected_event_dates",
-    [
-        (
-            "2020-02-15",  # nhs financial year 2019-04-01 to 2020-03-31
-            ["2019-05-01", "2020-02-15"],
-        ),
-        (
-            "2017-05-15",  # nhs financial year 2017-04-01 to 2018-03-31
-            ["2017-06-01", "2018-02-01"],
-        ),
-    ],
-)
-def test_nhs_financial_year_date_expressions(index_date, expected_event_dates):
+def test_patients_date_deregistered_from_all_supported_practices():
     session = make_session()
     session.add_all(
         [
-            # Event too early
-            Patient(
-                observations=[
-                    Observation(effective_date="2012-12-15", snomed_concept_id=123)
-                ],
-            ),
-            # Events in range 2019-04-01 to 2020-03-31
-            Patient(
-                observations=[
-                    Observation(effective_date="2019-05-01", snomed_concept_id=123)
-                ],
-            ),
-            Patient(
-                observations=[
-                    Observation(effective_date="2020-02-15", snomed_concept_id=123)
-                ],
-            ),
-            # Events in range 2017-04-01 to 2018-03-31
-            Patient(
-                observations=[
-                    Observation(effective_date="2018-02-01", snomed_concept_id=123)
-                ],
-            ),
-            Patient(
-                observations=[
-                    Observation(effective_date="2017-06-01", snomed_concept_id=123)
-                ],
-            ),
-            # Events out of range (at beginning/end of adjacent financial years)
-            Patient(
-                observations=[
-                    Observation(effective_date="2017-03-31", snomed_concept_id=123)
-                ],
-            ),
+            # Never de-registered
             Patient(
-                observations=[
-                    Observation(effective_date="2018-04-01", snomed_concept_id=123)
-                ],
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="2001-01-01",
+                        EndDate="9999-01-01",
+                        Organisation=Organisation(),
+                    )
+                ]
             ),
+            # De-registered, but after cut-off date
             Patient(
-                observations=[
-                    Observation(effective_date="2019-03-31", snomed_concept_id=123)
-                ],
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="2001-01-01",
+                        EndDate="2017-01-01",
+                        Organisation=Organisation(),
+                    ),
+                    RegistrationHistory(
+                        StartDate="2019-01-01",
+                        EndDate="2020-01-01",
+                        Organisation=Organisation(),
+                    ),
+                ]
             ),
+            # De-registered (but with a gap, and overlapping registrations)
             Patient(
-                observations=[
-                    Observation(effective_date="2020-04-01", snomed_concept_id=123)
-                ],
+                RegistrationHistory=[
+                    RegistrationHistory(
+                        StartDate="1990-01-01",
+                        EndDate="2005-01-01",
+                        Organisation=Organisation(),
+                    ),
+                    RegistrationHistory(
+                        StartDate="2010-01-01",
+                        EndDate="2015-05-19",
+                        Organisation=Organisation(),
+                    ),
+                    RegistrationHistory(
+                        StartDate="2015-04-10",
+                        EndDate="2017-10-04",
+                        Organisation=Organisation(),
+                    ),
+                ]
             ),
         ]
     )
     session.commit()
     study = StudyDefinition(
-        index_date=index_date,
-        population=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            between=[
-                "first_day_of_nhs_financial_year(index_date)",
-                "last_day_of_nhs_financial_year(index_date)",
-            ],
-        ),
-        event_date=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
-            date_format="YYYY-MM-DD",
-            between=[
-                "first_day_of_nhs_financial_year(index_date)",
-                "last_day_of_nhs_financial_year(index_date)",
-            ],
+        population=patients.all(),
+        dereg_date=patients.date_deregistered_from_all_supported_practices(
+            on_or_before="2018-02-01",
+            date_format="YYYY-MM",
         ),
     )
-    results = study.to_dicts()
-    event_dates = sorted([result["event_date"] for result in results])
-    assert event_dates == expected_event_dates
+    assert_results(study.to_dicts(), dereg_date=["", "", "2017-10"])
 
 
-@pytest.mark.parametrize(
-    "index_date,expected_event_dates",
-    [
-        (
-            "2020-08-15",  # school year 2019-09-01 to 2020-08-31
-            ["2019-10-01", "2020-02-15"],
-        ),
-        (
-            "2017-10-15",  # school year 2017-09-01 to 2018-08-31
-            ["2017-09-02", "2018-08-01"],
-        ),
-    ],
-)
-def test_school_year_date_expressions(index_date, expected_event_dates):
+def test_patients_admitted_to_hospital():
+    # Test period is on_or_after 2020-02-01
     session = make_session()
     session.add_all(
         [
-            # Event too early
-            Patient(
-                observations=[
-                    Observation(effective_date="2016-12-15", snomed_concept_id=123)
-                ],
-            ),
-            # Events in range 2019-09-01 to 2020-08-31
-            Patient(
-                observations=[
-                    Observation(effective_date="2019-10-01", snomed_concept_id=123)
-                ],
-            ),
+            # Patient with no episodes
+            Patient(Patient_ID=1),
+            # Patient with no episodes in period
             Patient(
-                observations=[
-                    Observation(effective_date="2020-02-15", snomed_concept_id=123)
-                ],
-            ),
-            # Events in range 2017-09-01 to 2018-08-31
-            Patient(
-                observations=[
-                    Observation(effective_date="2018-08-01", snomed_concept_id=123)
-                ],
-            ),
-            Patient(
-                observations=[
-                    Observation(effective_date="2017-09-02", snomed_concept_id=123)
-                ],
-            ),
-            # Events out of range (at beginning/end of adjacent school years)
-            Patient(
-                observations=[
-                    Observation(effective_date="2017-08-31", snomed_concept_id=123)
-                ],
-            ),
-            Patient(
-                observations=[
-                    Observation(effective_date="2018-09-01", snomed_concept_id=123)
+                Patient_ID=2,
+                APCSEpisodes=[
+                    APCS(
+                        APCS_Ident=1,
+                        Admission_Date="2020-01-01",
+                        Discharge_Date="2020-03-01",
+                        Der_Diagnosis_All="||AAAA ,XXXA, XXXB",
+                        Der_Procedure_All="||AAAA ,YYYA, YYYB",
+                        APCS_Der=APCS_Der(Patient_ID=2, Spell_Primary_Diagnosis="AAAA"),
+                    )
                 ],
             ),
+            # Patient with some episodes in period
             Patient(
-                observations=[
-                    Observation(effective_date="2019-08-31", snomed_concept_id=123)
+                Patient_ID=3,
+                APCSEpisodes=[
+                    APCS(
+                        APCS_Ident=2,
+                        Admission_Date="2020-01-01",
+                        Discharge_Date="2020-02-01",
+                        Der_Diagnosis_All="||BBBB ,XXXB, XXXC",
+                        Der_Procedure_All="||BBBB ,YYYB, YYYC",
+                        APCS_Der=APCS_Der(Patient_ID=3, Spell_Primary_Diagnosis="BBBB"),
+                    ),
+                    APCS(
+                        APCS_Ident=3,
+                        Admission_Date="2020-03-01",
+                        Discharge_Date="2020-04-01",
+                        Der_Diagnosis_All="||CCCC ,XXXC, XXXD",
+                        Der_Procedure_All="||CCCC ,YYYC, YYYD",
+                        APCS_Der=APCS_Der(Patient_ID=3, Spell_Primary_Diagnosis="CCCC"),
+                    ),
                 ],
             ),
+            # Patient with multiple episodes in period
             Patient(
-                observations=[
-                    Observation(effective_date="2020-09-01", snomed_concept_id=123)
+                Patient_ID=4,
+                APCSEpisodes=[
+                    APCS(
+                        APCS_Ident=4,
+                        Admission_Date="2020-03-01",
+                        Discharge_Date="2020-04-01",
+                        Der_Diagnosis_All="||DDDD ,XXXD, XXXE",
+                        Der_Procedure_All="||DDDD ,YYYD, YYYE",
+                        APCS_Der=APCS_Der(Patient_ID=4, Spell_Primary_Diagnosis="DDDD"),
+                    ),
+                    APCS(
+                        APCS_Ident=5,
+                        Admission_Date="2020-05-01",
+                        Discharge_Date="2020-06-01",
+                        Der_Diagnosis_All="||EEEE ,XXXE, XXXF",
+                        Der_Procedure_All="||EEEE ,YYYE, YYYF",
+                        APCS_Der=APCS_Der(Patient_ID=4, Spell_Primary_Diagnosis="EEEE"),
+                    ),
+                    APCS(
+                        APCS_Ident=6,
+                        Admission_Date="2020-07-01",
+                        Discharge_Date="2020-08-01",
+                        Der_Diagnosis_All="||FFFF ,XXXF, XXXG",
+                        Der_Procedure_All="||FFFF ,YYYF, YYYG",
+                        APCS_Der=APCS_Der(Patient_ID=4, Spell_Primary_Diagnosis="FFFF"),
+                    ),
                 ],
             ),
         ]
     )
     session.commit()
+
     study = StudyDefinition(
-        index_date=index_date,
-        population=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            between=[
-                "first_day_of_school_year(index_date)",
-                "last_day_of_school_year(index_date)",
-            ],
+        population=patients.all(),
+        admitted=patients.admitted_to_hospital(
+            on_or_after="2020-02-01", returning="binary_flag"
         ),
-        event_date=patients.with_these_clinical_events(
-            codelist(["123"], system="snomed"),
-            returning="date",
+        count=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+        ),
+        first_date_admitted=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="date_admitted",
+            find_first_match_in_period=True,
+            date_format="YYYY-MM-DD",
+        ),
+        last_date_admitted=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="date_admitted",
+            find_last_match_in_period=True,
+            date_format="YYYY-MM-DD",
+        ),
+        first_date_discharged=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="date_discharged",
+            find_first_match_in_period=True,
             date_format="YYYY-MM-DD",
-            between=[
-                "first_day_of_school_year(index_date)",
-                "last_day_of_school_year(index_date)",
-            ],
+        ),
+        last_date_discharged=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="date_discharged",
+            find_last_match_in_period=True,
+            date_format="YYYY-MM-DD",
+        ),
+        with_particular_primary_diagnosis=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="binary_flag",
+            with_these_primary_diagnoses=codelist([("EEEE", "cat1")], "icd10"),
+        ),
+        with_particular_diagnoses_1=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+            with_these_diagnoses=codelist([("XXXD", "cat2")], "icd10"),
+        ),
+        with_particular_diagnoses_2=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+            with_these_diagnoses=codelist(["XXXE"], "icd10"),
+        ),
+        with_particular_diagnoses_3=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+            with_these_diagnoses=codelist(["XXX"], "icd10"),
+        ),
+        with_particular_diagnoses_4=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+            with_these_diagnoses=codelist(["XXXC", "XXXD", "XXXE"], "icd10"),
+        ),
+        with_particular_procedures=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="number_of_matches_in_period",
+            with_these_procedures=codelist(["YYYC", "YYYD", "YYYE"], "icd10"),
+        ),
+        first_primary_diagnosis=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="primary_diagnosis",
+            find_first_match_in_period=True,
+        ),
+        last_primary_diagnosis=patients.admitted_to_hospital(
+            on_or_after="2020-02-01",
+            returning="primary_diagnosis",
+            find_last_match_in_period=True,
         ),
     )
-    results = study.to_dicts()
-    event_dates = sorted([result["event_date"] for result in results])
-    assert event_dates == expected_event_dates
 
+    assert_results(
+        study.to_dicts(),
+        admitted=["0", "0", "1", "1"],
+        count=["0", "0", "1", "3"],
+        first_date_admitted=["", "", "2020-03-01", "2020-03-01"],
+        last_date_admitted=["", "", "2020-03-01", "2020-07-01"],
+        first_date_discharged=["", "", "2020-04-01", "2020-04-01"],
+        last_date_discharged=["", "", "2020-04-01", "2020-08-01"],
+        with_particular_primary_diagnosis=["0", "0", "0", "1"],
+        with_particular_diagnoses_1=["0", "0", "1", "1"],
+        with_particular_diagnoses_2=["0", "0", "0", "2"],
+        with_particular_diagnoses_3=["0", "0", "1", "3"],
+        with_particular_diagnoses_4=["0", "0", "1", "2"],
+        with_particular_procedures=["0", "0", "1", "2"],
+        first_primary_diagnosis=["", "", "CCCC", "DDDD"],
+        last_primary_diagnosis=["", "", "CCCC", "FFFF"],
+    )
+
+
+def assert_results(results, **expected_values):
+    for col_name, expected_col_values in expected_values.items():
+        col_values = [row[col_name] for row in results]
+        assert col_values == expected_col_values, f"Unexpected results for {col_name}"
+
+
+def test_temporary_database_happy_path(tmp_path, monkeypatch):
+    temporary_database = os.environ["TPP_TEMP_DATABASE_NAME"]
+    monkeypatch.setenv("TEMP_DATABASE_NAME", temporary_database)
+    session = make_session()
+    session.add_all(
+        [
+            Patient(DateOfBirth="1960-01-01", Sex="M"),
+            Patient(DateOfBirth="1980-01-01", Sex="F"),
+        ]
+    )
+    session.commit()
+    study = StudyDefinition(
+        population=patients.all(),
+        sex=patients.sex(),
+        age=patients.age_as_of("1990-01-01"),
+    )
+    initial_temporary_tables = _list_table_in_db(session, temporary_database)
+    study.to_csv(tmp_path / "test.csv")
+    with open(tmp_path / "test.csv") as f:
+        results = list(csv.DictReader(f))
+    assert_results(results, sex=["M", "F"], age=["30", "10"])
+    # Check that the temporary table has been deleted
+    final_temporary_tables = _list_table_in_db(session, temporary_database)
+    assert final_temporary_tables == initial_temporary_tables
 
-def test_truncate_patient_id():
-    small_id = 123456789
-    # Remove the '0x' prefix
-    small_id_hex = hex(small_id)[2:]
-    assert truncate_patient_id(small_id_hex) == small_id // 2
 
-    large_id_hex = hex(987654321 + 2**100)[2:]
-    assert truncate_patient_id(large_id_hex) == 576460752303423488
+def test_temporary_database_with_failure(tmp_path, monkeypatch):
+    temporary_database = os.environ["TPP_TEMP_DATABASE_NAME"]
+    monkeypatch.setenv("TEMP_DATABASE_NAME", temporary_database)
+    session = make_session()
+    session.add_all(
+        [
+            Patient(DateOfBirth="1960-01-01", Sex="M"),
+            Patient(DateOfBirth="1980-01-01", Sex="F"),
+        ]
+    )
+    session.commit()
+    study_args = dict(
+        population=patients.all(),
+        sex=patients.sex(),
+        age=patients.age_as_of("2000-01-01"),
+    )
+    study = StudyDefinition(**study_args)
+    initial_temporary_tables = _list_table_in_db(session, temporary_database)
+    # Trigger error during data download process
+    with patch("cohortextractor.mssql_utils.csv") as csv_module:
+        csv_module.writer.side_effect = ValueError("deliberate error")
+        with pytest.raises(ValueError, match="deliberate error"):
+            study.to_csv(tmp_path / "fail.csv")
+    # Check that we've created one extra temporary table
+    temporary_tables = _list_table_in_db(session, temporary_database)
+    assert len(set(temporary_tables) - set(initial_temporary_tables)) == 1
+    # Delete all patient data so we can be sure the download below isn't just
+    # re-running the query
+    session.query(Patient).delete()
+    session.commit()
+    # Now try making a new study with the same definition, downloading again
+    # and check we have correct results
+    new_study = StudyDefinition(**study_args)
+    new_study.to_csv(tmp_path / "test.csv")
+    with open(tmp_path / "test.csv") as f:
+        results = list(csv.DictReader(f))
+    assert_results(results, sex=["M", "F"], age=["40", "20"])
+    # Check that the temporary table has been deleted
+    final_temporary_tables = _list_table_in_db(session, temporary_database)
+    assert final_temporary_tables == initial_temporary_tables
+
+
+def _list_table_in_db(session, database_name):
+    conn = session.connection()
+    results = conn.execute(
+        f"""
+        SELECT table_name FROM {database_name}.information_schema.tables
+        WHERE table_type = 'BASE TABLE'
+        """
+    )
+    return sorted(row[0] for row in results)
 
 
-def test_null_observation_dates_handled_correctly():
+def test_large_codelists_upload_correctly():
+    # 999 is the limit we can upload in a single batch so we want to be well
+    # above that
+    codes = [f"foo{i}" for i in range(3000)]
     session = make_session()
+    # Select codes from the beginning, middle and end of the codelist
     session.add_all(
         [
             Patient(
-                observations=[
-                    Observation(snomed_concept_id="10000001", effective_date=None),
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2020-02-05"
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code=codes[0],
+                        NumericValue=7,
                     ),
                 ]
             ),
             Patient(
-                observations=[
-                    Observation(
-                        snomed_concept_id="10000001", effective_date="2020-06-12"
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code=codes[1500],
+                        NumericValue=11,
                     ),
-                    Observation(
-                        snomed_concept_id="10000002", effective_date="2021-07-02"
+                ]
+            ),
+            Patient(
+                CodedEvents=[
+                    CodedEvent(
+                        CTV3Code=codes[-1],
+                        NumericValue=18,
                     ),
                 ]
             ),
         ]
     )
     session.commit()
-    codes = codelist(["10000001", "10000002"], "snomedct")
     study = StudyDefinition(
         population=patients.all(),
-        first_event_date=patients.with_these_clinical_events(
-            codes,
-            returning="date",
-            find_first_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        first_event_code=patients.with_these_clinical_events(
-            codes,
-            returning="code",
-            find_first_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        # This should be the same value as `event_date` but doing it this way
-        # makes it use a parition query so we can test that branch
-        date_of_first_code=patients.date_of(
-            "first_event_code", date_format="YYYY-MM-DD"
-        ),
-        last_event_date=patients.with_these_clinical_events(
-            codes,
-            returning="date",
-            find_last_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        last_event_code=patients.with_these_clinical_events(
-            codes,
-            returning="code",
-            find_last_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        date_of_last_code=patients.date_of("last_event_code", date_format="YYYY-MM-DD"),
-        pre2020_event_date=patients.with_these_clinical_events(
-            codes,
-            on_or_before="2020-01-01",
-            returning="date",
-            find_last_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        pre2020_event_code=patients.with_these_clinical_events(
-            codes,
-            on_or_before="2020-01-01",
-            returning="code",
-            find_last_match_in_period=True,
-            date_format="YYYY-MM-DD",
+        value=patients.with_these_clinical_events(
+            codelist(codes, system="ctv3"), returning="numeric_value"
         ),
-        date_of_pre2020_code=patients.date_of(
-            "pre2020_event_code", date_format="YYYY-MM-DD"
-        ),
-    )
-    assert_results(
-        study.to_dicts(),
-        first_event_date=["1900-01-01", "2020-06-12"],
-        date_of_first_code=["1900-01-01", "2020-06-12"],
-        last_event_date=["2020-02-05", "2021-07-02"],
-        date_of_last_code=["2020-02-05", "2021-07-02"],
-        pre2020_event_date=["1900-01-01", ""],
-        date_of_pre2020_code=["1900-01-01", ""],
     )
+    results = study.to_dicts()
+    assert_results(results, value=["7.0", "11.0", "18.0"])
 
 
-def test_patients_died_from_any_cause_dynamic_dates():
+def test_use_of_date_expressions():
     session = make_session()
     session.add_all(
         [
-            # Not dead
+            # Event too early
             Patient(
-                nhs_no="aaa",
-                medications=[
-                    Medication(snomed_concept_id="10", effective_date="2021-01-02"),
-                ],
-            ),
-            # Died more than 2 weeks after antipsychotic date
-            Patient(
-                nhs_no="bbb",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20210201,
-                        pseudonhsnumber="bbb",
-                        upload_date="2021-02-02",
-                    )
-                ],
-                medications=[
-                    Medication(snomed_concept_id="10", effective_date="2021-01-02")
-                ],
+                DateOfBirth="1980-01-01",
+                CodedEvents=[CodedEvent(ConsultationDate="2012-12-15", CTV3Code="foo")],
             ),
-            # Died, no antipsychotic
+            # Events in range
             Patient(
-                nhs_no="ccc",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20210115,
-                        icd10u="A",
-                        pseudonhsnumber="ccc",
-                        upload_date="2021-02-02",
-                    ),
-                ],
+                DateOfBirth="1980-05-01",
+                CodedEvents=[CodedEvent(ConsultationDate="2013-01-01", CTV3Code="foo")],
             ),
-            # Died within 2 weeks, antipsychotic before index date
             Patient(
-                nhs_no="ddd",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20200115,
-                        icd10u="A",
-                        pseudonhsnumber="ddd",
-                        upload_date="2021-02-02",
-                    ),
-                ],
-                medications=[
-                    Medication(snomed_concept_id="10", effective_date="2020-01-02"),
-                ],
+                DateOfBirth="1980-07-01",
+                CodedEvents=[CodedEvent(ConsultationDate="2015-12-31", CTV3Code="foo")],
             ),
-            # Died within 2 weeks of antipsychotic
+            # Event too late
             Patient(
-                nhs_no="eee",
-                ONSDeath=[
-                    ONSDeaths(
-                        reg_stat_dod=20210115,
-                        icd10u="A",
-                        pseudonhsnumber="eee",
-                        upload_date="2021-02-02",
-                    ),
-                ],
-                medications=[
-                    Medication(snomed_concept_id="10", effective_date="2021-01-02"),
-                ],
+                DateOfBirth="1980-01-01",
+                CodedEvents=[CodedEvent(ConsultationDate="2016-01-01", CTV3Code="foo")],
             ),
         ]
     )
     session.commit()
     study = StudyDefinition(
-        population=patients.all(),
-        index_date="2021-01-01",
-        antipsychotics_date=patients.with_these_medications(
-            codelist=codelist(["10"], "snomed"),
-            returning="date",
-            find_last_match_in_period=True,
-            between=["index_date", "last_day_of_month(index_date)"],
-            date_format="YYYY-MM-DD",
-            return_expectations={"incidence": 0.1},
-        ),
-        died_2weeks_post_antipsychotic=patients.died_from_any_cause(
-            between=["antipsychotics_date", "antipsychotics_date + 14 days"],
-            returning="binary_flag",
+        index_date="2015-06-01",
+        population=patients.with_these_clinical_events(
+            codelist(["foo"], system="ctv3"),
+            between=[
+                "first_day_of_year(index_date) - 2 years",
+                "last_day_of_year(index_date)",
+            ],
         ),
+        age=patients.age_as_of("index_date"),
     )
-    assert_results(
-        study.to_dicts(),
-        antipsychotics_date=["2021-01-02", "2021-01-02", "", "", "2021-01-02"],
-        died_2weeks_post_antipsychotic=["0", "0", "0", "0", "1"],
-    )
+    results = study.to_dicts()
+    assert_results(results, age=["35", "34"])
 
 
-def test_date_window_behaviour_literals():
+def test_patients_with_death_recorded_in_primary_care():
     session = make_session()
     session.add_all(
         [
-            Patient(
-                observations=[
-                    # This event is before the start date and is never captured
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-03T23:59:59"
-                    ),
-                    # These event is captured with and without the fix
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-04T00:00:00"
-                    ),
-                    # This event is after midnight on the end date, and is only captured with the fix
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-04T10:45:00"
-                    ),
-                    # This event is after the end date and is never captured
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-05T00:00:00"
-                    ),
-                ]
-            ),
+            Patient(DateOfDeath="9999-12-31"),
+            Patient(DateOfDeath="2017-05-06"),
+            Patient(DateOfDeath="2019-06-07"),
+            Patient(DateOfDeath="2020-07-08"),
         ]
     )
     session.commit()
-
     study = StudyDefinition(
         population=patients.all(),
-        event_count=patients.with_these_clinical_events(
-            codelist(["111"], "snomedct"),
-            between=["2021-01-04", "2021-01-04"],
-            returning="number_of_matches_in_period",
+        has_died=patients.with_death_recorded_in_primary_care(),
+        date_of_death=patients.with_death_recorded_in_primary_care(
+            returning="date_of_death", date_format="YYYY-MM-DD"
         ),
+        died_in_2019=patients.with_death_recorded_in_primary_care(
+            between=["2019-01-01", "2019-12-31"],
+            returning="date_of_death",
+        ),
+    )
+    assert_results(
+        study.to_dicts(),
+        has_died=["0", "1", "1", "1"],
+        date_of_death=["", "2017-05-06", "2019-06-07", "2020-07-08"],
+        died_in_2019=["", "", "2019", ""],
     )
 
-    results = study.to_dicts()
-    assert results[0]["event_count"] == "2"
+
+def test_date_expressions_are_handled_in_practice_address_and_care_home_methods():
+    study = StudyDefinition(
+        index_date="2020-01-01",
+        population=patients.all(),
+        practice=patients.registered_practice_as_of(
+            "index_date", returning="pseudo_id"
+        ),
+        address=patients.address_as_of(
+            "index_date", returning="rural_urban_classification"
+        ),
+        care_home=patients.care_home_status_as_of("index_date"),
+    )
+    # We don't care about the results, we just want to check that this doesn't
+    # blow up with an "invalid date" error
+    assert_results(study.to_dicts(), practice=[], address=[], care_home=[])
 
 
-def test_date_window_behaviour_variable():
+def test_extracting_at_different_index_dates():
+    codes = [f"foo{i}" for i in range(10)]
     session = make_session()
     session.add_all(
         [
             Patient(
-                observations=[
-                    # This is the last 222 event without the fix
-                    Observation(
-                        snomed_concept_id="2221", effective_date="2021-01-03T16:10:00"
-                    ),
-                    # This is the last 222 event with the fix
-                    Observation(
-                        snomed_concept_id="2222", effective_date="2021-01-04T16:10:00"
-                    ),
-                    # Thse two 111 event is on the date of 2221, but only one will be
-                    # captured without the fix.
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-03T00:00:00"
-                    ),
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-03T16:10:00"
-                    ),
-                    # These two 111 events are on the date of 2222, and both will be
-                    # captured with the fix.
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-04T16:10:00"
-                    ),
-                    Observation(
-                        snomed_concept_id="111", effective_date="2021-01-04T16:10:01"
-                    ),
+                CodedEvents=[
+                    CodedEvent(CTV3Code=codes[1], ConsultationDate="2020-01-14")
+                ]
+            ),
+            Patient(
+                CodedEvents=[
+                    CodedEvent(CTV3Code=codes[5], ConsultationDate="2020-02-10")
                 ]
             ),
         ]
     )
     session.commit()
-
     study = StudyDefinition(
+        index_date="2020-01-01",
         population=patients.all(),
-        last_222=patients.with_these_clinical_events(
-            codelist(["2221", "2222"], "snomedct"),
-            between=["2021-01-01", "2021-01-04"],
+        value=patients.with_these_clinical_events(
+            codelist(codes, system="ctv3"),
             returning="date",
             date_format="YYYY-MM-DD",
-            find_last_match_in_period=True,
-        ),
-        event_count=patients.with_these_clinical_events(
-            codelist(["111"], "snomedct"),
-            between=["last_222", "last_222"],
-            returning="number_of_matches_in_period",
+            between=["index_date", "index_date + 1 month"],
         ),
     )
-
+    study.set_index_date("2020-01-01")
+    results = study.to_dicts()
+    assert_results(results, value=["2020-01-14", ""])
+    study.set_index_date("2020-02-01")
     results = study.to_dicts()
-    assert results[0]["last_222"] == "2021-01-04"
-    assert results[0]["event_count"] == "2"
+    assert_results(results, value=["", "2020-02-10"])
```

### Comparing `opensafely-cohort-extractor-1.85.0/tests/test_expectation_generators.py` & `opensafely-cohort-extractor-1.9.0/tests/test_expectation_generators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from math import isclose, isnan
+import pytest
 
-import numpy as np
 import pandas as pd
-import pytest
+import numpy as np
+from math import isclose
 
-from cohortextractor import StudyDefinition, codelist, patients
+from cohortextractor import StudyDefinition
+from cohortextractor import patients
+from cohortextractor import codelist
 from cohortextractor.expectation_generators import generate
 
 
 @pytest.fixture(autouse=True)
 def set_randomstate():
     """Several tests include randomness in their output. Seed the PRNG to
     make tests deterministic.
@@ -285,44 +287,30 @@
     return_expectations = {
         "rate": "exponential_increase",
         "incidence": incidence,
         "date": {"earliest": "1900-01-01", "latest": "2020-01-01"},
         "float": {"distribution": "normal", "mean": 35, "stddev": 10},
     }
     result = generate(population_size, **return_expectations)
-    nonzero_results = result[result["float"] != 0.0]
-    assert abs(35 - int(nonzero_results["float"].mean())) < 5
+    assert abs(35 - int(result["float"].mean())) < 5
 
 
-def test_data_generator_int_normal():
+def test_data_generator_int():
     population_size = 10000
     incidence = 0.9
     return_expectations = {
         "rate": "exponential_increase",
         "incidence": incidence,
         "date": {"earliest": "1900-01-01", "latest": "2020-01-01"},
         "int": {"distribution": "normal", "mean": 10, "stddev": 1},
     }
     result = generate(population_size, **return_expectations)
     assert abs(10 - int(result["int"].mean())) < 3
 
 
-def test_data_generator_int_poisson():
-    population_size = 10000
-    incidence = 0.9
-    return_expectations = {
-        "rate": "exponential_increase",
-        "incidence": incidence,
-        "date": {"earliest": "1900-01-01", "latest": "2020-01-01"},
-        "int": {"distribution": "poisson", "mean": 5},
-    }
-    result = generate(population_size, **return_expectations)
-    assert abs(5 - int(result["int"].mean())) < 3
-
-
 def test_data_generator_bool():
     population_size = 10000
     incidence = 0.5
     return_expectations = {
         "rate": "exponential_increase",
         "incidence": incidence,
         "date": {"earliest": "1900-01-01", "latest": "2020-01-01"},
@@ -511,50 +499,14 @@
         ),
     )
     population_size = 10000
     result = study.make_df_from_expectations(population_size)
     assert result[~pd.isnull(result["asthma_condition"])].min()[0] < "1960-01-01"
 
 
-def test_column_refs_in_date_expressions_do_not_trigger_errors():
-    # Further down the road we want to actually interpret these expressions and
-    # generate appopriate dates, but for now we just need to not blow up when
-    # we encounter them
-    study = StudyDefinition(
-        population=patients.all(),
-        copd_exacerbation=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            between=["2001-12-01", "2002-06-01"],
-            returning="date",
-            return_expectations={
-                "rate": "exponential_increase",
-                "incidence": 0.2,
-                "date": {"earliest": "1990-01-01", "latest": "today"},
-            },
-            find_last_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-        drug_after_exacerbation=patients.with_these_medications(
-            codelist(["Y"], system="snomed"),
-            between=["copd_exacerbation", "copd_exacerbation + 3 months"],
-            returning="date",
-            return_expectations={
-                "rate": "exponential_increase",
-                "incidence": 0.2,
-                "date": {"earliest": "1990-01-01", "latest": "today"},
-            },
-            find_first_match_in_period=True,
-            date_format="YYYY-MM-DD",
-        ),
-    )
-    population_size = 10000
-    # Just ensure no exception is raised
-    study.make_df_from_expectations(population_size)
-
-
 def test_make_df_from_expectations_with_distribution_and_date():
     study = StudyDefinition(
         population=patients.all(),
         bmi=patients.most_recent_bmi(
             on_or_after="2010-02-01",
             minimum_age_at_measurement=16,
             return_expectations={
@@ -570,15 +522,18 @@
         ),
     )
     population_size = 10000
     result = study.make_df_from_expectations(population_size)
     assert list(sorted(result.columns)) == ["bmi", "bmi_date_measured"]
 
     # Check that the null-valued rows are aligned with each other
-    assert ((result["bmi"] == 0.0) == pd.isnull(result["bmi_date_measured"])).all()
+    assert (
+        result["bmi"][pd.isnull(result["bmi"])].fillna(0)
+        == result["bmi_date_measured"][pd.isnull(result["bmi_date_measured"])].fillna(0)
+    ).all()
 
 
 def test_make_df_from_expectations_with_mean_recorded_value():
     study = StudyDefinition(
         population=patients.all(),
         drug_x=patients.mean_recorded_value(
             codelist(["X"], system="ctv3"),
@@ -589,31 +544,30 @@
                 "incidence": 0.6,
                 "float": {"distribution": "normal", "mean": 35, "stddev": 10},
             },
         ),
     )
     population_size = 10000
     result = study.make_df_from_expectations(population_size)
-    nonzero_results = result[result["drug_x"] != 0.0]
-    assert abs(35 - int(nonzero_results["drug_x"].mean())) < 5
+    assert abs(35 - int(result["drug_x"].mean())) < 5
 
 
 def test_make_df_from_binary_default_outcome():
     study = StudyDefinition(
         population=patients.all(),
         died=patients.died_from_any_cause(
             return_expectations={
                 "date": {"earliest": "1900-01-01", "latest": "today"},
                 "incidence": 0.1,
             }
         ),
     )
     population_size = 10000
     result = study.make_df_from_expectations(population_size)
-    assert len(result[result.died == 1]) == 0.1 * population_size
+    assert len(result[~pd.isnull(result.died)]) == 0.1 * population_size
 
 
 def test_make_df_from_expectations_with_number_of_episodes():
     study = StudyDefinition(
         population=patients.all(),
         episode_count=patients.with_these_clinical_events(
             codelist(["A", "B", "C"], system="ctv3"),
@@ -676,14 +630,15 @@
     population_size = 10000
     # Just ensuring no exception is raised
     result = study.make_df_from_expectations(population_size)
     assert len(result[pd.isnull(result.sex_default)]) == 0
 
 
 def test_make_df_from_expectations_doesnt_alter_date_defaults():
+
     study = StudyDefinition(
         default_expectations={
             "rate": "exponential_increase",
             "incidence": 1.0,
             "date": {"earliest": "1900-01-01", "latest": "today"},
             "category": {"ratios": {"M": 0.5, "F": 0.5}},
         },
@@ -824,336 +779,7 @@
         ),
     )
     population_size = 1000
     result = study.make_df_from_expectations(population_size)
     dates = result.dereg_date.dropna()
     assert dates.max() <= "2018-02"
     assert dates.min() >= "1980-01"
-
-
-def test_make_df_from_expectations_with_aggregate_of():
-    # aggregate of variables defined in their own right
-    study = StudyDefinition(
-        default_expectations={
-            "date": {"earliest": "1900-01-01", "latest": "today"},
-            "rate": "exponential_increase",
-            "incidence": 0.2,
-        },
-        population=patients.all(),
-        fixed_date=patients.fixed_value("1980-10-20"),
-        date_1=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        date_2=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        date_min=patients.minimum_of(
-            "date_1",
-            "date_2",
-        ),
-        date_max=patients.maximum_of(
-            "date_1",
-            "date_2",
-        ),
-        date_min_fixed=patients.minimum_of(
-            "date_1",
-            "fixed_date",
-        ),
-        date_min_fixed_inline=patients.minimum_of(
-            "date_1",
-            "1990-05-20",
-        ),
-        int_1=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="number_of_matches_in_period",
-            return_expectations={
-                "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                "incidence": 0.5,
-            },
-        ),
-        int_2=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="number_of_matches_in_period",
-            return_expectations={
-                "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                "incidence": 0.5,
-            },
-        ),
-        int_min=patients.minimum_of("int_1", "int_2"),
-        int_max=patients.maximum_of("int_1", "int_2"),
-    )
-    population_size = 10000
-    result = study.make_df_from_expectations(population_size)
-    assert len(result) == population_size
-    for _, row in result.iterrows():
-        dates = [d for d in [row["date_1"], row["date_2"]] if isinstance(d, str)]
-        if dates:
-            date_min = min(dates)
-            date_max = max(dates)
-        else:
-            date_min = float("nan")
-            date_max = float("nan")
-        assert_nan_equal(row["date_min"], date_min)
-        assert_nan_equal(row["date_max"], date_max)
-        ints = [i for i in [row["int_1"], row["int_2"]] if isinstance(i, int)]
-        if ints:
-            int_min = min(ints)
-            int_max = max(ints)
-        else:
-            int_min = float("nan")
-            int_max = float("nan")
-        assert_nan_equal(row["int_min"], int_min)
-        assert_nan_equal(row["int_max"], int_max)
-        assert row["date_min_fixed"] <= "1980-10-20"
-        assert row["date_min_fixed_inline"] <= "1990-05-20"
-        assert row["fixed_date"] == "1980-10-20"
-
-    # aggregate of variables defined only within aggregate function
-    study = StudyDefinition(
-        default_expectations={
-            "date": {"earliest": "1900-01-01", "latest": "today"},
-            "rate": "exponential_increase",
-            "incidence": 1,
-        },
-        # We use an expression here (never mind that it's a trivial and
-        # pointless one) as that triggers a bug which we want to ensure we've
-        # fixed
-        population=patients.satisfying(
-            "foo OR bar", foo=patients.all(), bar=patients.all()
-        ),
-        date_min=patients.maximum_of(
-            date_1=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-            date_2=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-        ),
-        date_max=patients.maximum_of(
-            date_3=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-            date_4=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-        ),
-        int_min=patients.minimum_of(
-            int_1=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-            int_2=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-        ),
-        int_max=patients.maximum_of(
-            int_3=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-            int_4=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-        ),
-    )
-    population_size = 10000
-    result = study.make_df_from_expectations(population_size)
-    for _, row in result.iterrows():
-        print(row)
-        assert pd.notna(row["date_min"])
-        assert pd.notna(row["date_max"])
-        assert pd.notna(row["int_min"])
-        assert pd.notna(row["int_max"])
-
-    # aggregate of variables defined both inside and outside aggregation
-    study = StudyDefinition(
-        default_expectations={
-            "date": {"earliest": "1900-01-01", "latest": "today"},
-            "rate": "exponential_increase",
-            "incidence": 0.2,
-        },
-        population=patients.all(),
-        date_1=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        date_2=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="date",
-            date_format="YYYY-MM-DD",
-        ),
-        date_min=patients.minimum_of(
-            "date_1",
-            "date_2",
-            date_3=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-        ),
-        date_max=patients.maximum_of(
-            "date_1",
-            "date_2",
-            date_4=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="date",
-                date_format="YYYY-MM-DD",
-            ),
-        ),
-        int_1=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="number_of_matches_in_period",
-            return_expectations={
-                "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                "incidence": 0.5,
-            },
-        ),
-        int_2=patients.with_these_clinical_events(
-            codelist(["X"], system="ctv3"),
-            returning="number_of_matches_in_period",
-            return_expectations={
-                "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                "incidence": 0.5,
-            },
-        ),
-        int_min=patients.minimum_of(
-            "int_1",
-            "int_2",
-            int_3=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-        ),
-        int_max=patients.maximum_of(
-            "int_1",
-            "int_2",
-            int_4=patients.with_these_clinical_events(
-                codelist(["X"], system="ctv3"),
-                returning="number_of_matches_in_period",
-                return_expectations={
-                    "int": {"distribution": "normal", "mean": 25, "stddev": 5},
-                    "incidence": 0.5,
-                },
-            ),
-        ),
-    )
-    population_size = 10000
-    result = study.make_df_from_expectations(population_size)
-    for _, row in result.iterrows():
-        print(row)
-        dates = [d for d in [row["date_1"], row["date_2"]] if isinstance(d, str)]
-        if dates:
-            assert row["date_min"] <= min(dates)
-            assert row["date_max"] >= max(dates)
-        ints = [i for i in [row["int_1"], row["int_2"]] if isinstance(i, int)]
-        if ints:
-            assert row["int_min"] <= min(ints)
-            assert row["int_max"] >= max(ints)
-
-
-def assert_nan_equal(v1, v2):
-    assert (
-        not isinstance(v1, str) and not isinstance(v2, str) and isnan(v1) and isnan(v2)
-    ) or v1 == v2
-
-
-def test_make_df_from_expectations_with_using_dates_as_categories():
-    study = StudyDefinition(
-        default_expectations={
-            "date": {"earliest": "1900-01-01", "latest": "today"},
-            "rate": "exponential_increase",
-            "incidence": 0.2,
-        },
-        population=patients.all(),
-        eligible_date=patients.categorised_as(
-            {
-                "2020-04-14": "age >= 80",
-                "2020-06-16": "age >= 70 AND age < 80",
-                "2020-08-18": "DEFAULT",
-            },
-            age=patients.age_as_of("2020-01-01"),
-            return_expectations={
-                "category": {
-                    "ratios": {
-                        "2020-04-14": 0.25,
-                        "2020-06-16": 0.25,
-                        "2020-08-18": 0.5,
-                    }
-                },
-                "incidence": 1,
-            },
-        ),
-    )
-    population_size = 100
-    result = study.make_df_from_expectations(population_size)
-    assert set(result.eligible_date) == set(["2020-08-18", "2020-06-16", "2020-04-14"])
-
-
-def test_make_df_from_expectations_with_covid_therapeutics():
-    study = StudyDefinition(
-        population=patients.all(),
-        therapeutic_approved=patients.with_covid_therapeutics(
-            with_these_statuses=["Approved", "Treatment Complete"],
-            returning="therapeutic",
-            return_expectations={
-                "rate": "universal",
-                "date": {"earliest": "1900-01-01", "latest": "today"},
-                "category": {
-                    "ratios": {
-                        "Approved": 0.25,
-                        "Treatment Complete": 0.25,
-                        "Treatment Not Started": 0.25,
-                        "Treatment Stopped": 0.25,
-                    }
-                },
-            },
-        ),
-        start_date=patients.with_covid_therapeutics(
-            with_these_statuses=["Approved", "Treatment Complete"],
-            returning="date",
-            return_expectations={
-                "rate": "exponential_increase",
-                "incidence": 0.2,
-                "date": {"earliest": "1900-01-01", "latest": "today"},
-            },
-        ),
-    )
-    population_size = 1000
-    # Just ensuring no exception is raised
-    result = study.make_df_from_expectations(population_size)
-    assert len(result[pd.isnull(result.therapeutic_approved)]) == 0
-    assert len(result[pd.isnull(result.start_date)]) == 800
```

