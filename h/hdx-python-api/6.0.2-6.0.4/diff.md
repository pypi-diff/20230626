# Comparing `tmp/hdx-python-api-6.0.2.tar.gz` & `tmp/hdx_python_api-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-api-6.0.2.tar", last modified: Tue Jun 20 01:39:57 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdx-python-api-6.0.2.tar` & `hdx_python_api-6.0.4.tar`

### file list

```diff
@@ -1,149 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.930198 hdx-python-api-6.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.934198 hdx-python-api-6.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.934198 hdx-python-api-6.0.2/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    42389 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.930198 hdx-python-api-6.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.930198 hdx-python-api-6.0.2/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.934198 hdx-python-api-6.0.2/src/hdx/api/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx/api/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24827 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/api/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/api/hdx_base_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/api/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.938198 hdx-python-api-6.0.2/src/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   111856 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9457 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/date_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    28494 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/hdxobject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/indicator_resource_view_template.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    11097 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24274 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4532 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7678 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15004 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9685 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22494 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/data/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.938198 hdx-python-api-6.0.2/src/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3863 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/src/hdx/facades/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.938198 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 01:39:57.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:39:56.000000 hdx-python-api-6.0.2/src/hdx_python_api.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.934198 hdx-python-api-6.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.938198 hdx-python-api-6.0.2/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)   169336 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/Tag_Mapping_ChainRuleError.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.942198 hdx-python-api-6.0.2/tests/fixtures/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/empty.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_base_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_dataset_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_email_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_organization_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      147 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_resource_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_resource_view_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_showcase_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_user_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/hdx_vocabulary_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/config/user_agent_config_wrong.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    25870 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/dataset_search_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.942198 hdx-python-api-6.0.2/tests/fixtures/datastore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23724 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/empty.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.942198 hdx-python-api-6.0.2/tests/fixtures/gen_resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/gen_resource/test_data_no_years.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    13842 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/organization_show_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.942198 hdx-python-api-6.0.2/tests/fixtures/qc_from_rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/resource_formats.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/showcase_all_search_results.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/test_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/test_data.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.946198 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/
--rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   319924 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    92805 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   290790 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   230593 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   216041 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   842238 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48523 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.946198 hdx-python-api-6.0.2/tests/fixtures/update_logic/
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_logic/update_logic_resources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/fixtures/update_logic/update_logic_resources_new.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.946198 hdx-python-api-6.0.2/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.946198 hdx-python-api-6.0.2/tests/hdx/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)    34755 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3009 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/api/test_locations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44943 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/tests/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9940 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49148 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    75535 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19570 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45958 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19114 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23053 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21174 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   116054 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/data/test_vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/tests/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5957 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5651 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/tests/hdx/facades/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:39:57.950198 hdx-python-api-6.0.2/workingexample/
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/workingexample/my_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/workingexample/my_resource.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/workingexample/my_resource.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-06-20 01:39:40.000000 hdx-python-api-6.0.2/workingexample/run.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    42394 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/main.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/locations.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   111985 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     5798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3545 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28599 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    24275 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    44945 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49155 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    45959 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/run.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/LICENSE
+-rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/README.md
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/PKG-INFO
```

### Comparing `hdx-python-api-6.0.2/.github/workflows/publish.yml` & `hdx_python_api-6.0.4/.github/workflows/publish.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-    - name: Get history and tags for SCM versioning to work
+    - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Publish with tox and twine
+        pip install --upgrade hatch
+    - name: Build with hatch
+      run: |
+        hatch build
+    - name: Publish with hatch
       env:
-        TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
+        HATCH_INDEX_USER: ${{secrets.HATCH_INDEX_USER}}
+        HATCH_INDEX_AUTH: ${{secrets.HATCH_INDEX_AUTH}}
       run: |
-        tox -e publish
+        hatch publish
```

### Comparing `hdx-python-api-6.0.2/.github/workflows/run-python-tests.yml` & `hdx_python_api-6.0.4/.github/workflows/run-python-tests.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Test with tox/pytest
+        pip install --upgrade hatch
+    - name: Test with hatch/pytest
       run: |
-        tox
+        hatch run test:test
+    - name: Check styling
+      if: always()
+      run: |
+        hatch run lint:style
     - name: Publish Unit Test Results
       uses: EnricoMi/publish-unit-test-result-action@v2
       if: always()
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
-        junit_files: .tox/*.xml
-    - name: Upload Coverage Results
-      uses: codecov/codecov-action@v3
-      if: success()
+        junit_files: test-results.xml
+    - name: Publish in Coveralls
+      uses: coverallsapp/github-action@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        flag-name: tests
+        format: lcov
```

### Comparing `hdx-python-api-6.0.2/.gitignore` & `hdx_python_api-6.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/LICENSE` & `hdx_python_api-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/PKG-INFO` & `hdx_python_api-6.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.2
+Version: 6.0.4
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
-Home-page: https://github.com/OCHA-DAP/hdx-python-api
-Author: Michael Rans
-Author-email: rans@email.com
+Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
+Author-email: Michael Rans <rans@email.com>
 License: MIT
-Keywords: HDX,API,library,CKAN
-Platform: any
+License-File: LICENSE
+Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
+Requires-Dist: ckanapi>=4.7
+Requires-Dist: defopt>=6.4.0
+Requires-Dist: email-validator
+Requires-Dist: hdx-python-country>=3.5.1
+Requires-Dist: makefun
+Requires-Dist: ndg-httpsclient
+Requires-Dist: pyasn1
+Requires-Dist: pyopenssl
+Requires-Dist: quantulum3
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-api/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-api)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-api.svg)](https://pypistats.org/packages/hdx-python-api)
 
 The HDX Python API Library is designed to enable you to easily develop code that 
 interacts with the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) 
 platform. The major goal of the library is to make pushing and pulling data from HDX as 
 simple as possible for the end user.
```

### Comparing `hdx-python-api-6.0.2/README.md` & `hdx_python_api-6.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-api/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-api)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-api.svg)](https://pypistats.org/packages/hdx-python-api)
 
 The HDX Python API Library is designed to enable you to easily develop code that 
 interacts with the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) 
 platform. The major goal of the library is to make pushing and pulling data from HDX as 
 simple as possible for the end user.
```

### Comparing `hdx-python-api-6.0.2/doc/main.md` & `hdx_python_api-6.0.4/documentation/main.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 4. Scroll down to the bottom of the profile page
 5. Copy the API key which will be of the form: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
 6. You can either:
 
     a.  Pass this key as a parameter or within a dictionary
     
     b.  Create a JSON or YAML file. The default path is
-            **.hdx\_configuration.yml** in the current user's home
+            **.hdx\_configuration.yaml** in the current user's home
             directory. Then put in the YAML file:
 
             hdx_key: "HDX API KEY"
 
 ## Installing the Library
 
 To include the HDX Python library in your project, you must **pip install** or add to 
@@ -152,15 +152,15 @@
 
 1. If you just want to read data from HDX, then an API key is not necessary. However, 
 if you want to write data to HDX, then you need to register on the website to obtain an 
 API key. Please see above about where to find it on the website. Once you have it, then 
 put it into a file in your home directory:
 
         cd ~
-        echo "hdx_key: \"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx\"" > .hdx_configuration.yml
+        echo "hdx_key: \"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx\"" > .hdx_configuration.yaml
 
 2. If you are using the Docker image, you can jump to step 6, otherwise install 
 virtualenv if not installed:
 
         pip install virtualenv
 
     On some Linux distributions, you can do the following instead to install from the 
@@ -266,15 +266,15 @@
 
 The easiest way to get started is to use the facades and configuration defaults. The 
 facades set up both logging and HDX configuration.
 
 The default configuration loads an internal HDX configuration located within the 
 library, and assumes that there is an API key file called **.hdxkey** in the current 
 user's home directory **\~** and a YAML project configuration located relative to your 
-working directory at **config/project\_configuration.yml** which you must create. The 
+working directory at **config/project\_configuration.yaml** which you must create. The 
 project configuration is used for any configuration specific to your project.
 
 The default logging configuration reads a configuration file internal to the library 
 that sets up an coloured console handler outputting at INFO level and a file handler 
 writing to errors.log at ERROR level.
 
 ## Facades
@@ -460,15 +460,15 @@
 Larger amounts of static metadata are best added from files. YAML is very human readable 
 and recommended, while JSON is also accepted eg.
 
     dataset.update_from_yaml([path])
 
     dataset.update_from_json([path])
 
-The default path if unspecified is **config/hdx\_TYPE\_static.yml** for YAML and
+The default path if unspecified is **config/hdx\_TYPE\_static.yaml** for YAML and
 **config/hdx\_TYPE\_static.json** for JSON where TYPE is an HDX object's type like 
 dataset or resource eg. **config/hdx\_showcase\_static.json**. The YAML file takes the 
 following form:
 
     owner_org: "acled"
     maintainer: "acled"
     ...
@@ -1057,15 +1057,15 @@
 A complete example can be found here: <https://github.com/OCHA-DAP/hdx-scraper-idmc>
 
 In particular, take a look at the files **run.py**, **idmc.py** and the **config** 
 folder. If you run it unchanged, it will overwrite the existing datasets in the IDMC 
 organisation! Therefore, you should run it against a test server. If you use it as a 
 basis for your code, you will need to modify the dataset **name**  in **idmc.py** and 
 change the organisation information to your organisation. Also update metadata in 
-**config/hdx\_dataset\_static.yml** appropriately.
+**config/hdx\_dataset\_static.yaml** appropriately.
 
 The IDMC scraper creates a dataset per country in HDX, populating all the required 
 metadata. It then creates resources with files held on the HDX filestore.
 
 # Brief History
 
 The first iteration of a scraper for ACLED was written without the HDX Python library
```

### Comparing `hdx-python-api-6.0.2/src/hdx/api/configuration.py` & `hdx_python_api-6.0.4/src/hdx/api/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,59 +4,59 @@
 from base64 import b64decode
 from collections import UserDict
 from os.path import expanduser, isfile, join
 from typing import Any, Dict, Optional, Tuple
 
 import ckanapi
 import requests
+
+from . import __version__
 from hdx.utilities.dictandlist import merge_two_dictionaries
 from hdx.utilities.email import Email
 from hdx.utilities.loader import load_json, load_yaml
 from hdx.utilities.path import script_dir_plus_file
 from hdx.utilities.session import get_session
 from hdx.utilities.useragent import UserAgent, UserAgentError
 
-from . import __version__
-
 logger = logging.getLogger(__name__)
 
 
 class ConfigurationError(Exception):
     pass
 
 
 class Configuration(UserDict):
     """Configuration for HDX
 
     Args:
         **kwargs: See below
         user_agent (str): User agent string. HDXPythonLibrary/X.X.X- is prefixed. Must be supplied if remoteckan is not.
-        user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+        user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
         user_agent_lookup (str): Lookup key for YAML. Ignored if user_agent supplied.
         hdx_url (str): HDX url to use. Overrides hdx_site.
         hdx_site (str): HDX site to use eg. prod, test.
         hdx_read_only (bool): Whether to access HDX in read only mode. Defaults to False.
         hdx_key (str): Your HDX key. Ignored if hdx_read_only = True.
         hdx_config_dict (dict): HDX configuration dictionary to use instead of above 3 parameters OR
         hdx_config_json (str): Path to JSON HDX configuration OR
         hdx_config_yaml (str): Path to YAML HDX configuration
         project_config_dict (dict): Project configuration dictionary OR
         project_config_json (str): Path to JSON Project configuration OR
         project_config_yaml (str): Path to YAML Project configuration
         hdx_base_config_dict (dict): HDX base configuration dictionary OR
         hdx_base_config_json (str): Path to JSON HDX base configuration OR
-        hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yml.
+        hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yaml.
     """
 
     _configuration = None
     home_folder = expanduser("~")
     default_hdx_base_config_yaml = script_dir_plus_file(
-        "hdx_base_configuration.yml", ConfigurationError
+        "hdx_base_configuration.yaml", ConfigurationError
     )
-    default_hdx_config_yaml = join(home_folder, ".hdx_configuration.yml")
+    default_hdx_config_yaml = join(home_folder, ".hdx_configuration.yaml")
 
     prefix = f"HDXPythonLibrary/{__version__}"
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__()
 
         self._session = None
@@ -121,21 +121,23 @@
             if hdx_config_yaml:
                 raise ConfigurationError(
                     "More than one HDX configuration given!"
                 )
         else:
             if not hdx_config_yaml:
                 hdx_config_yaml = Configuration.default_hdx_config_yaml
+                if not isfile(hdx_config_yaml):
+                    hdx_config_yaml = hdx_config_yaml.replace(".yaml", ".yml")
                 if isfile(hdx_config_yaml):
                     logger.info(
                         f"No HDX configuration parameter. Using default configuration file: {hdx_config_yaml}."
                     )
                 else:
                     logger.info(
-                        f"No HDX configuration parameter and no configuration file at default path: {hdx_config_yaml}."
+                        f"No HDX configuration parameter and no configuration file at default path: {Configuration.default_hdx_config_yaml}."
                     )
                     hdx_config_yaml = None
                     hdx_config_dict = dict()
             if hdx_config_yaml:
                 logger.info(
                     f"Loading HDX configuration from: {hdx_config_yaml}"
                 )
@@ -411,15 +413,15 @@
     ) -> Tuple[requests.Session, str]:
         """
         Create session and user agent from configuration
 
         Args:
             session (requests.Session): requests Session object to use. Defaults to calling hdx.utilities.session.get_session()
             user_agent (Optional[str]): User agent string. HDXPythonLibrary/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
             use_env (bool): Whether to read environment variables. Defaults to False.
 
         Returns:
             Tuple[requests.Session, str]: Tuple of (session, user agent)
 
         """
@@ -505,15 +507,15 @@
         | username: "user"
         | password: "pass"
 
         Args:
             **kwargs: See below
             email_config_dict (dict): HDX configuration dictionary OR
             email_config_json (str): Path to JSON HDX configuration OR
-            email_config_yaml (str): Path to YAML HDX configuration. Defaults to ~/hdx_email_configuration.yml.
+            email_config_yaml (str): Path to YAML HDX configuration. Defaults to ~/hdx_email_configuration.yaml.
 
         Returns:
             None
         """
         self._emailer = Email(**kwargs)
 
     @classmethod
@@ -538,29 +540,29 @@
         """
         Construct the HDX configuration
 
         Args:
             configuration (Optional[Configuration]): Configuration instance. Defaults to setting one up from passed arguments.
             **kwargs: See below
             user_agent (str): User agent string. HDXPythonLibrary/X.X.X- is prefixed. Must be supplied if remoteckan is not.
-            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (str): Lookup key for YAML. Ignored if user_agent supplied.
             hdx_url (str): HDX url to use. Overrides hdx_site.
             hdx_site (str): HDX site to use eg. prod, test.
             hdx_read_only (bool): Whether to access HDX in read only mode. Defaults to False.
             hdx_key (str): Your HDX key. Ignored if hdx_read_only = True.
             hdx_config_dict (dict): HDX configuration dictionary to use instead of above 3 parameters OR
             hdx_config_json (str): Path to JSON HDX configuration OR
             hdx_config_yaml (str): Path to YAML HDX configuration
             project_config_dict (dict): Project configuration dictionary OR
             project_config_json (str): Path to JSON Project configuration OR
             project_config_yaml (str): Path to YAML Project configuration
             hdx_base_config_dict (dict): HDX base configuration dictionary OR
             hdx_base_config_json (str): Path to JSON HDX base configuration OR
-            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yml.
+            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yaml.
 
         Returns:
             None
 
         """
         if configuration is None:
             cls._configuration = Configuration(**kwargs)
@@ -578,29 +580,29 @@
         Create HDX configuration
 
         Args:
             configuration (Optional[Configuration]): Configuration instance. Defaults to setting one up from passed arguments.
             remoteckan (Optional[ckanapi.RemoteCKAN]): CKAN instance. Defaults to setting one up from configuration.
             **kwargs: See below
             user_agent (str): User agent string. HDXPythonLibrary/X.X.X- is prefixed. Must be supplied if remoteckan is not.
-            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (str): Lookup key for YAML. Ignored if user_agent supplied.
             hdx_url (str): HDX url to use. Overrides hdx_site.
             hdx_site (str): HDX site to use eg. prod, test.
             hdx_read_only (bool): Whether to access HDX in read only mode. Defaults to False.
             hdx_key (str): Your HDX key. Ignored if hdx_read_only = True.
             hdx_config_dict (dict): HDX configuration dictionary to use instead of above 3 parameters OR
             hdx_config_json (str): Path to JSON HDX configuration OR
             hdx_config_yaml (str): Path to YAML HDX configuration
             project_config_dict (dict): Project configuration dictionary OR
             project_config_json (str): Path to JSON Project configuration OR
             project_config_yaml (str): Path to YAML Project configuration
             hdx_base_config_dict (dict): HDX base configuration dictionary OR
             hdx_base_config_json (str): Path to JSON HDX base configuration OR
-            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yml.
+            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yaml.
 
         Returns:
             str: HDX site url
 
         """
         kwargs = cls._environment_variables(**kwargs)
         cls.setup(configuration, **kwargs)
@@ -618,29 +620,29 @@
         Create HDX configuration. Can only be called once (will raise an error if called more than once).
 
         Args:
             configuration (Optional[Configuration]): Configuration instance. Defaults to setting one up from passed arguments.
             remoteckan (Optional[ckanapi.RemoteCKAN]): CKAN instance. Defaults to setting one up from configuration.
             **kwargs: See below
             user_agent (str): User agent string. HDXPythonLibrary/X.X.X- is prefixed. Must be supplied if remoteckan is not.
-            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (str): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (str): Lookup key for YAML. Ignored if user_agent supplied.
             hdx_url (str): HDX url to use. Overrides hdx_site.
             hdx_site (str): HDX site to use eg. prod, test.
             hdx_read_only (bool): Whether to access HDX in read only mode. Defaults to False.
             hdx_key (str): Your HDX key. Ignored if hdx_read_only = True.
             hdx_config_dict (dict): HDX configuration dictionary to use instead of above 3 parameters OR
             hdx_config_json (str): Path to JSON HDX configuration OR
             hdx_config_yaml (str): Path to YAML HDX configuration
             project_config_dict (dict): Project configuration dictionary OR
             project_config_json (str): Path to JSON Project configuration OR
             project_config_yaml (str): Path to YAML Project configuration
             hdx_base_config_dict (dict): HDX base configuration dictionary OR
             hdx_base_config_json (str): Path to JSON HDX base configuration OR
-            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yml.
+            hdx_base_config_yaml (str): Path to YAML HDX base configuration. Defaults to library's internal hdx_base_configuration.yaml.
 
         Returns:
             str: HDX site url
 
         """
         if cls._configuration is not None:
             raise ConfigurationError("Configuration already created!")
```

### Comparing `hdx-python-api-6.0.2/src/hdx/api/hdx_base_configuration.yml` & `hdx_python_api-6.0.4/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/src/hdx/api/locations.py` & `hdx_python_api-6.0.4/src/hdx/api/locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Locations in HDX"""
 from typing import Dict, List, Optional, Tuple
 
-from hdx.utilities.typehint import ListTuple
-
 from hdx.api.configuration import Configuration
+from hdx.utilities.typehint import ListTuple
 
 
 class Locations:
     """Methods to help with countries and continents"""
 
     _validlocations = None
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/dataset.py` & `hdx_python_api-6.0.4/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 """Dataset class containing all logic for creating, checking, and updating datasets and associated resources.
 """
 import json
 import logging
 import sys
 from copy import deepcopy
 from datetime import datetime
-from os.path import join
+from os.path import isfile, join
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
     Tuple,
     Union,
 )
 
-from hdx.location.country import Country
-from hdx.utilities.base_downloader import BaseDownload
-from hdx.utilities.dateparse import (
-    default_date,
-    default_enddate,
-    now_utc,
-    parse_date,
-    parse_date_range,
-)
-from hdx.utilities.dictandlist import merge_two_dictionaries, write_list_to_csv
-from hdx.utilities.downloader import Download
-from hdx.utilities.path import script_dir_plus_file
-from hdx.utilities.saver import save_json
-from hdx.utilities.typehint import ListTuple, ListTupleDict
-from hdx.utilities.uuid import is_valid_uuid
 from hxl.input import InputOptions, munge_url
 
 import hdx.data.filestore_helper as filestore_helper
 import hdx.data.organization as org_module
 import hdx.data.resource as res_module
 import hdx.data.resource_view as resource_view
 import hdx.data.showcase as sc_module
@@ -45,14 +30,29 @@
 import hdx.data.vocabulary as vocabulary
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
 from hdx.data.dataset_title_helper import DatasetTitleHelper
 from hdx.data.date_helper import DateHelper
 from hdx.data.hdxobject import HDXError, HDXObject
 from hdx.data.resource_matcher import ResourceMatcher
+from hdx.location.country import Country
+from hdx.utilities.base_downloader import BaseDownload
+from hdx.utilities.dateparse import (
+    default_date,
+    default_enddate,
+    now_utc,
+    parse_date,
+    parse_date_range,
+)
+from hdx.utilities.dictandlist import merge_two_dictionaries, write_list_to_csv
+from hdx.utilities.downloader import Download
+from hdx.utilities.path import script_dir_plus_file
+from hdx.utilities.saver import save_json
+from hdx.utilities.typehint import ListTuple, ListTupleDict
+from hdx.utilities.uuid import is_valid_uuid
 
 if TYPE_CHECKING:
     from hdx.data.organization import Organization
     from hdx.data.resource import Resource
     from hdx.data.showcase import Showcase
     from hdx.data.user import User
 
@@ -414,20 +414,20 @@
             )
             reordered_resources.append(resource)
         self.resources = reordered_resources
         if hxl_update:
             self.hxl_update()
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_dataset_static.yml")
+        self, path: str = join("config", "hdx_dataset_static.yaml")
     ) -> None:
         """Update dataset metadata with static metadata from YAML file
 
         Args:
-            path (str): Path to YAML dataset metadata. Defaults to config/hdx_dataset_static.yml.
+            path (str): Path to YAML dataset metadata. Defaults to config/hdx_dataset_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
         self.separate_resources()
 
@@ -2085,15 +2085,15 @@
         "date_format": "%Y", "aggregate_col": "null"}.
 
         Creation of the resource view will be delayed until after the next
         dataset create or update if a resource id is not yet available.
 
         Args:
             resource (Union[Resource,Dict,str,int]): Either resource id or name, resource metadata from a Resource object or a dictionary or position. Defaults to 0.
-            path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yml or internal template).
+            path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yaml or internal template).
             bites_disabled (Optional[ListTuple[bool]]): Which QC bites should be disabled. Defaults to None (all bites enabled).
             indicators (Optional[ListTuple[Dict]]): Indicator codes, QC titles and units for resource view template. Defaults to None (don't use template).
             findreplace (Optional[Dict]): Replacements for anything else in resource view. Defaults to None.
 
         Returns:
             resource_view.ResourceView: The resource view if QuickCharts created, None is not
         """
@@ -2107,18 +2107,21 @@
         if "id" in res:
             resourceview_data = {"resource_id": res["id"]}
         else:
             resourceview_data = {"resource_name": res["name"]}
         resourceview = resource_view.ResourceView(resourceview_data)
         if path is None:
             if indicators is None:
-                path = join("config", "hdx_resource_view_static.yml")
+                path = join("config", "hdx_resource_view_static.yaml")
+                if not isfile(path):
+                    path = path.replace(".yaml", ".yml")
             else:
                 path = script_dir_plus_file(
-                    "indicator_resource_view_template.yml", NotRequestableError
+                    "indicator_resource_view_template.yaml",
+                    NotRequestableError,
                 )
         resourceview.update_from_yaml(path=path)
 
         def replace_string(instr, what, withwhat):
             return instr.replace(what, str(withwhat))
 
         defaults = {
@@ -2311,15 +2314,15 @@
 
         Creation of the resource view will be delayed until after the next
         dataset create or update if a resource id is not yet available and will
         be disabled if there are no valid charts to display.
 
         Args:
             resource (Union[Resource,Dict,str,int]): Either resource id or name, resource metadata from a Resource object or a dictionary or position. Defaults to 0.
-            path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yml or internal template).
+            path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yaml or internal template).
             bites_disabled (Optional[ListTuple[bool]]): Which QC bites should be disabled. Defaults to None (all bites enabled).
             indicators (Optional[ListTuple[Dict]]): Indicator codes, QC titles and units for resource view template. Defaults to None (don't use template).
             findreplace (Optional[Dict]): Replacements for anything else in resource view. Defaults to None.
 
         Returns:
             resource_view.ResourceView: The resource view if QuickCharts created, None is not
         """
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.0.4/src/hdx/data/dataset_title_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import logging
 import re
 from datetime import datetime, timedelta
 from string import punctuation, whitespace
 from typing import List, Match, Optional, Tuple
 
 from dateutil.parser import ParserError
+from quantulum3 import parser
+
 from hdx.utilities.dateparse import parse_date, parse_date_range
 from hdx.utilities.text import (
     PUNCTUATION_MINUS_BRACKETS,
     remove_end_characters,
     remove_from_end,
     remove_string,
 )
-from quantulum3 import parser
 
 logger = logging.getLogger(__name__)
 
 
 class DatasetTitleHelper:
     YEAR_PATTERN = re.compile(r"([12]\d\d\d)")
     VERSION_PATTERN = re.compile(r"(\d)?(\d)?\d")
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/date_helper.py` & `hdx_python_api-6.0.4/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.0.4/src/hdx/data/filestore_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/src/hdx/data/hdxobject.py` & `hdx_python_api-6.0.4/src/hdx/data/hdxobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """HDXObject abstract class containing helper functions for creating, checking, and updating HDX objects.
 New HDX objects should extend this in similar fashion to Resource for example.
 """
 import copy
 import logging
 from abc import ABC, abstractmethod
 from collections import UserDict
+from os.path import isfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from ckanapi.errors import NotFound
+
+from hdx.api.configuration import Configuration
 from hdx.utilities.dictandlist import merge_two_dictionaries
 from hdx.utilities.loader import (
     load_json_into_existing_dict,
     load_yaml_into_existing_dict,
 )
 from hdx.utilities.typehint import ListTuple
 
-from hdx.api.configuration import Configuration
-
 logger = logging.getLogger(__name__)
 
 
 class HDXError(Exception):
     pass
 
 
@@ -65,14 +66,16 @@
 
         Args:
             path (str): Path to YAML dataset metadata
 
         Returns:
             None
         """
+        if not isfile(path):
+            path = path.replace(".yaml", ".yml")
         self.data = load_yaml_into_existing_dict(self.data, path)
 
     def update_from_json(self, path: str) -> None:
         """Update metadata with static metadata from JSON file
 
         Args:
             path (str): Path to JSON dataset metadata
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/indicator_resource_view_template.yml` & `hdx_python_api-6.0.4/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/src/hdx/data/organization.py` & `hdx_python_api-6.0.4/src/hdx/data/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Organization class containing all logic for creating, checking, and updating organizations."""
 import logging
 from os.path import join
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from hdx.utilities.typehint import ListTuple
-
 import hdx.data.dataset
 import hdx.data.user as user_module
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError, HDXObject
+from hdx.utilities.typehint import ListTuple
 
 if TYPE_CHECKING:
     from hdx.data.user import User
 
 logger = logging.getLogger(__name__)
 
 
@@ -46,20 +45,20 @@
             "create": "organization_create",
             "delete": "organization_delete",
             "list": "organization_list",
             "autocomplete": "organization_autocomplete",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_organization_static.yml")
+        self, path: str = join("config", "hdx_organization_static.yaml")
     ) -> None:
         """Update organization metadata with static metadata from YAML file
 
         Args:
-            path (str): Path to YAML dataset metadata. Defaults to config/hdx_organization_static.yml.
+            path (str): Path to YAML dataset metadata. Defaults to config/hdx_organization_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/resource.py` & `hdx_python_api-6.0.4/src/hdx/data/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Resource class containing all logic for creating, checking, and updating resources."""
 import logging
 from datetime import datetime
 from os.path import join
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from hdx.utilities.dateparse import now_utc
-from hdx.utilities.downloader import Download
-from hdx.utilities.typehint import ListTuple
-from hdx.utilities.uuid import is_valid_uuid
-
 import hdx.data.dataset
 import hdx.data.filestore_helper as filestore_helper
 from hdx.api.configuration import Configuration
 from hdx.data.date_helper import DateHelper
 from hdx.data.hdxobject import HDXError, HDXObject
 from hdx.data.resource_view import ResourceView
+from hdx.utilities.dateparse import now_utc
+from hdx.utilities.downloader import Download
+from hdx.utilities.typehint import ListTuple
+from hdx.utilities.uuid import is_valid_uuid
 
 logger = logging.getLogger(__name__)
 
 
 class Resource(HDXObject):
     """Resource class containing all logic for creating, checking, and updating
     resources.
@@ -57,20 +56,20 @@
             "search": "resource_search",
             "broken": "hdx_mark_broken_link_in_resource",
             "datastore_delete": "datastore_delete",
             "datastore_search": "datastore_search",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_resource_static.yml")
+        self, path: str = join("config", "hdx_resource_static.yaml")
     ) -> None:
         """Update resource metadata with static metadata from YAML file
 
         Args:
-            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_resource_static.yml.
+            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_resource_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.0.4/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/src/hdx/data/resource_view.py` & `hdx_python_api-6.0.4/src/hdx/data/resource_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Resource view class containing all logic for creating, checking, and updating resource views."""
 import logging
 from os.path import join
 from typing import Any, Dict, List, Optional, Union
 
-from hdx.utilities.typehint import ListTuple
-from hdx.utilities.uuid import is_valid_uuid
-
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError, HDXObject
+from hdx.utilities.typehint import ListTuple
+from hdx.utilities.uuid import is_valid_uuid
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceView(HDXObject):
     """ResourceView class containing all logic for creating, checking, and updating resource views.
 
@@ -42,20 +41,20 @@
             "create": "resource_view_create",
             "delete": "resource_view_delete",
             "list": "resource_view_list",
             "reorder": "resource_view_reorder",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_resource_view_static.yml")
+        self, path: str = join("config", "hdx_resource_view_static.yaml")
     ) -> None:
         """Update resource view metadata with static metadata from YAML file
 
         Args:
-            path (Optional[str]): Path to YAML resource view metadata. Defaults to config/hdx_resource_view_static.yml.
+            path (Optional[str]): Path to YAML resource view metadata. Defaults to config/hdx_resource_view_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/showcase.py` & `hdx_python_api-6.0.4/src/hdx/data/showcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Showcase class containing all logic for creating, checking, and updating showcases."""
 import logging
 import sys
 from os.path import join
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.typehint import ListTuple
-from hdx.utilities.uuid import is_valid_uuid
-
 import hdx.data.dataset
 import hdx.data.vocabulary
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXObject
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.typehint import ListTuple
+from hdx.utilities.uuid import is_valid_uuid
 
 logger = logging.getLogger(__name__)
 
 
 class Showcase(HDXObject):
     """Showcase class containing all logic for creating, checking, and updating showcases.
 
@@ -52,20 +51,20 @@
             "associate": "ckanext_showcase_package_association_create",
             "disassociate": "ckanext_showcase_package_association_delete",
             "list_datasets": "ckanext_showcase_package_list",
             "list_showcases": "ckanext_package_showcase_list",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_showcase_static.yml")
+        self, path: str = join("config", "hdx_showcase_static.yaml")
     ) -> None:
         """Update showcase metadata with static metadata from YAML file
 
         Args:
-            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_showcase_static.yml.
+            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_showcase_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/user.py` & `hdx_python_api-6.0.4/src/hdx/data/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """User class containing all logic for creating, checking, and updating users."""
 import logging
 from os.path import join
 from typing import Any, Dict, List, Optional
 
-from hdx.utilities.typehint import ListTuple
-
 import hdx.data.organization
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXObject
+from hdx.utilities.typehint import ListTuple
 
 logger = logging.getLogger(__name__)
 
 
 class User(HDXObject):
     """User class containing all logic for creating, checking, and updating users.
 
@@ -43,20 +42,20 @@
             "delete": "user_delete",
             "list": "user_list",
             "listorgs": "organization_list_for_user",
             "autocomplete": "user_autocomplete",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_user_static.yml")
+        self, path: str = join("config", "hdx_user_static.yaml")
     ) -> None:
         """Update user metadata with static metadata from YAML file
 
         Args:
-            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_user_static.yml.
+            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_user_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/data/vocabulary.py` & `hdx_python_api-6.0.4/src/hdx/data/vocabulary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Vocabulary class containing all logic for creating, checking, and updating vocabularies."""
 import logging
 from collections import OrderedDict
 from os.path import join
 from typing import Any, Dict, List, Optional, Tuple
 
-from hdx.utilities.downloader import Download
-from hdx.utilities.typehint import ListTuple
-
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXObject
+from hdx.utilities.downloader import Download
+from hdx.utilities.typehint import ListTuple
 
 logger = logging.getLogger(__name__)
 
 
 class ChainRuleError(Exception):
     pass
 
@@ -58,20 +57,20 @@
             "create": "vocabulary_create",
             "delete": "vocabulary_delete",
             "list": "vocabulary_list",
             "autocomplete": "tag_autocomplete",
         }
 
     def update_from_yaml(
-        self, path: str = join("config", "hdx_vocabulary_static.yml")
+        self, path: str = join("config", "hdx_vocabulary_static.yaml")
     ) -> None:
         """Update vocabulary metadata with static metadata from YAML file
 
         Args:
-            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_vocabulary_static.yml.
+            path (Optional[str]): Path to YAML dataset metadata. Defaults to config/hdx_vocabulary_static.yaml.
 
         Returns:
             None
         """
         super().update_from_yaml(path)
 
     def update_from_json(
```

### Comparing `hdx-python-api-6.0.2/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.0.4/src/hdx/facades/infer_arguments.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Facade to simplify project setup that calls project main function with kwargs"""
 import logging
 import sys
 from inspect import getdoc
 from typing import Any, Callable, Optional  # noqa: F401
 
 import defopt
-from hdx.utilities.easy_logging import setup_logging
-from hdx.utilities.useragent import UserAgent
 from makefun import with_signature
 
 from hdx.api import __version__
 from hdx.api.configuration import Configuration
+from hdx.utilities.easy_logging import setup_logging
+from hdx.utilities.useragent import UserAgent
 
 logger = logging.getLogger(__name__)
 setup_logging(log_file="errors.log")
 
 
 def facade(projectmainfn: Callable[[Any], None], **kwargs: Any):
     """Facade to simplify project setup that calls project main function. It infers
```

### Comparing `hdx-python-api-6.0.2/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.0.4/src/hdx/facades/keyword_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Facade to simplify project setup that calls project main function with kwargs"""
 import logging
 from typing import Any, Callable
 
-from hdx.utilities.easy_logging import setup_logging
-from hdx.utilities.useragent import UserAgent
-
 from hdx.api import __version__
 from hdx.api.configuration import Configuration
+from hdx.utilities.easy_logging import setup_logging
+from hdx.utilities.useragent import UserAgent
 
 logger = logging.getLogger(__name__)
 setup_logging(log_file="errors.log")
 
 
 def facade(projectmainfn: Callable[[Any], None], **kwargs: Any):
     """Facade to simplify project setup that calls project main function
```

### Comparing `hdx-python-api-6.0.2/src/hdx/facades/simple.py` & `hdx_python_api-6.0.4/src/hdx/facades/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Facade to simplify project setup that calls project main function"""
 import logging
 from typing import Any, Callable
 
-from hdx.utilities.easy_logging import setup_logging
-from hdx.utilities.useragent import UserAgent
-
 from hdx.api import __version__
 from hdx.api.configuration import Configuration
+from hdx.utilities.easy_logging import setup_logging
+from hdx.utilities.useragent import UserAgent
 
 logger = logging.getLogger(__name__)
 setup_logging(log_file="errors.log")
 
 
 def facade(projectmainfn: Callable[[None], None], **kwargs: Any):
     """Facade to simplify project setup that calls project main function
```

### Comparing `hdx-python-api-6.0.2/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.0.4/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/config/hdx_dataset_static.yml` & `hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/config/hdx_resource_view_static.yml` & `hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/dataset_search_results.yml` & `hdx_python_api-6.0.4/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.0.4/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.0.4/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.4/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/organization_show_results.yml` & `hdx_python_api-6.0.4/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/resource_formats.json` & `hdx_python_api-6.0.4/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/showcase_all_search_results.yml` & `hdx_python_api-6.0.4/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/test_data.csv` & `hdx_python_api-6.0.4/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/test_data.zip` & `hdx_python_api-6.0.4/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_logic/update_logic_resources.yml` & `hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/fixtures/update_logic/update_logic_resources_new.yml` & `hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.0.4/tests/hdx/api/test_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Configuration Tests"""
 from os.path import join
 
 import ckanapi
 import pytest
-from hdx.utilities.loader import LoadError
-from hdx.utilities.useragent import UserAgentError
 
 from hdx.api import __version__
 from hdx.api.configuration import Configuration, ConfigurationError
+from hdx.utilities.loader import LoadError
+from hdx.utilities.useragent import UserAgentError
 
 
 class TestConfiguration:
     @pytest.fixture(scope="class")
     def hdx_base_config_yaml(self, configfolder):
-        return join(configfolder, "hdx_base_config.yml")
+        return join(configfolder, "hdx_base_config.yaml")
 
     @pytest.fixture(scope="class")
     def hdx_base_config_json(self, configfolder):
         return join(configfolder, "hdx_base_config.json")
 
     @pytest.fixture(scope="class")
     def hdx_missing_site_config_json(self, configfolder):
@@ -25,31 +25,31 @@
 
     @pytest.fixture(scope="class")
     def project_config_json(self, configfolder):
         return join(configfolder, "project_configuration.json")
 
     @pytest.fixture(scope="class")
     def user_agent_config_yaml(self, configfolder):
-        return join(configfolder, "user_agent_config.yml")
+        return join(configfolder, "user_agent_config.yaml")
 
     @pytest.fixture(scope="class")
     def user_agent_config2_yaml(self, configfolder):
-        return join(configfolder, "user_agent_config2.yml")
+        return join(configfolder, "user_agent_config2.yaml")
 
     @pytest.fixture(scope="class")
     def user_agent_config3_yaml(self, configfolder):
-        return join(configfolder, "user_agent_config3.yml")
+        return join(configfolder, "user_agent_config3.yaml")
 
     @pytest.fixture(scope="class")
     def empty_yaml(self, configfolder):
-        return join(configfolder, "empty.yml")
+        return join(configfolder, "empty.yaml")
 
     @pytest.fixture(scope="class")
     def user_agent_config_wrong_yaml(self, configfolder):
-        return join(configfolder, "user_agent_config_wrong.yml")
+        return join(configfolder, "user_agent_config_wrong.yaml")
 
     def test_init(
         self,
         hdx_config_json,
         hdx_config_yaml,
         hdx_base_config_yaml,
         hdx_base_config_json,
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/api/test_locations.py` & `hdx_python_api-6.0.4/tests/hdx/api/test_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """HDX Location Tests"""
-from hdx.location.country import Country
-
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
+from hdx.location.country import Country
 
 
 class MyConfiguration:
     def call_remoteckan(self, a, b):
         return [{"name": "zaf", "title": "South Africa"}]
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/conftest.py` & `hdx_python_api-6.0.4/tests/hdx/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 @pytest.fixture(scope="session")
 def configfolder(fixturesfolder):
     return join(fixturesfolder, "config")
 
 
 @pytest.fixture(scope="session")
 def hdx_config_yaml(configfolder):
-    return join(configfolder, "hdx_config.yml")
+    return join(configfolder, "hdx_config.yaml")
 
 
 @pytest.fixture(scope="session")
 def hdx_config_json(configfolder):
     return join(configfolder, "hdx_config.json")
 
 
 @pytest.fixture(scope="session")
 def project_config_yaml():
-    return join("tests", "fixtures", "config", "project_configuration.yml")
+    return join("tests", "fixtures", "config", "project_configuration.yaml")
 
 
 @pytest.fixture(scope="session")
 def locations():
     Locations.set_validlocations(
         [
             {
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/__init__.py` & `hdx_python_api-6.0.4/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 import json
 import re
 import tempfile
 from os import remove
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.loader import load_yaml
-
-from hdx.api import __version__
-from hdx.api.configuration import Configuration
-from hdx.data.dataset import Dataset, NotRequestableError
-from hdx.data.hdxobject import HDXError
-from hdx.data.resource import Resource
-from hdx.data.resource_view import ResourceView
 
 from . import (
     MockResponse,
     dataset_data,
     dataset_mockshow,
     dataset_resultdict,
     resources_data,
@@ -27,16 +18,26 @@
 from .test_resource_view import (
     resource_view_list,
     resource_view_mockcreate,
     resource_view_mocklist,
     resource_view_mockshow,
 )
 from .test_vocabulary import vocabulary_mockshow
+from hdx.api import __version__
+from hdx.api.configuration import Configuration
+from hdx.data.dataset import Dataset, NotRequestableError
+from hdx.data.hdxobject import HDXError
+from hdx.data.resource import Resource
+from hdx.data.resource_view import ResourceView
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.loader import load_yaml
 
-searchdict = load_yaml(join("tests", "fixtures", "dataset_search_results.yml"))
+searchdict = load_yaml(
+    join("tests", "fixtures", "dataset_search_results.yaml")
+)
 dataset_list = [
     "acled-conflict-data-for-libya",
     "acled-conflict-data-for-liberia",
     "acled-conflict-data-for-lesotho",
     "acled-conflict-data-for-kenya",
     "acled-conflict-data-for-guinea",
     "acled-conflict-data-for-ghana",
@@ -188,15 +189,15 @@
 class TestDatasetCore:
     @pytest.fixture(scope="class")
     def test_file(self):
         return join("tests", "fixtures", "test_data.csv")
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
-        return join("tests", "fixtures", "config", "hdx_dataset_static.yml")
+        return join("tests", "fixtures", "config", "hdx_dataset_static.yaml")
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join("tests", "fixtures", "config", "hdx_dataset_static.json")
 
     @pytest.fixture(scope="function")
     def read(self):
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_noncore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,14 @@
 """Dataset Tests (noncore methods)"""
 import copy
 import json
 from datetime import datetime, timezone
 from os.path import join
 
 import pytest
-from hdx.location.country import Country
-from hdx.utilities.compare import assert_files_same
-from hdx.utilities.dateparse import parse_date_range
-from hdx.utilities.downloader import Download
-from hdx.utilities.path import temp_dir
-from hdx.utilities.saver import save_text
-
-from hdx.api.configuration import Configuration
-from hdx.data.dataset import Dataset
-from hdx.data.hdxobject import HDXError
-from hdx.data.organization import Organization
-from hdx.data.user import User
-from hdx.data.vocabulary import Vocabulary
 
 from . import (
     MockResponse,
     dataset_data,
     dataset_mockshow,
     organization_data,
     resources_data,
@@ -35,14 +22,26 @@
     resource_view_mockcreate,
     resource_view_mocklist,
     resource_view_mockshow,
 )
 from .test_showcase import showcase_resultdict
 from .test_user import user_mockshow
 from .test_vocabulary import vocabulary_mockshow
+from hdx.api.configuration import Configuration
+from hdx.data.dataset import Dataset
+from hdx.data.hdxobject import HDXError
+from hdx.data.organization import Organization
+from hdx.data.user import User
+from hdx.data.vocabulary import Vocabulary
+from hdx.location.country import Country
+from hdx.utilities.compare import assert_files_same
+from hdx.utilities.dateparse import parse_date_range
+from hdx.utilities.downloader import Download
+from hdx.utilities.path import temp_dir
+from hdx.utilities.saver import save_text
 
 
 class TestDatasetNoncore:
     association = None
     url = "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-api/main/tests/fixtures/test_data.csv"
     hxltags = {
         "EVENT_ID_CNTY": "#event+code",
@@ -66,15 +65,15 @@
         "FATALITIES": "#affected+killed",
         "ISO3": "#country+code",
     }
 
     @pytest.fixture(scope="class")
     def static_resource_view_yaml(self):
         return join(
-            "tests", "fixtures", "config", "hdx_resource_view_static.yml"
+            "tests", "fixtures", "config", "hdx_resource_view_static.yaml"
         )
 
     @pytest.fixture(scope="function")
     def vocabulary_read(self):
         class MockSession:
             @staticmethod
             def post(url, data, headers, files, allow_redirects, auth=None):
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_organization.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """Organization Tests"""
 import copy
 import json
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.loader import load_yaml
 
+from . import MockResponse, organization_data, user_data
+from .test_user import user_mockshow
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.organization import Organization
 from hdx.data.user import User
-
-from . import MockResponse, organization_data, user_data
-from .test_user import user_mockshow
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.loader import load_yaml
 
 resultdict = load_yaml(
-    join("tests", "fixtures", "organization_show_results.yml")
+    join("tests", "fixtures", "organization_show_results.yaml")
 )
 
 organization_list = [
     "acaps",
     "accion-contra-el-hambre-acf-spain",
     "acf-west-africa",
     "acled",
     "acted",
     "action-contre-la-faim",
     "adeso",
     "afd",
     "afdb",
     "afghanistan-protection-cluster",
 ]
-searchdict = load_yaml(join("tests", "fixtures", "dataset_search_results.yml"))
+searchdict = load_yaml(
+    join("tests", "fixtures", "dataset_search_results.yaml")
+)
 
 organization_autocomplete = [
     {
         "title": "INNAGO",
         "id": "5a63012e-6c41-420c-8c33-e84b277fdc90",
         "name": "innago",
     }
@@ -101,15 +102,15 @@
         )
 
 
 class TestOrganization:
     @pytest.fixture(scope="class")
     def static_yaml(self):
         return join(
-            "tests", "fixtures", "config", "hdx_organization_static.yml"
+            "tests", "fixtures", "config", "hdx_organization_static.yaml"
         )
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join(
             "tests", "fixtures", "config", "hdx_organization_static.json"
         )
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_resource.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 import json
 import os
 from datetime import datetime, timezone
 from os import remove
 from os.path import basename, join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.downloader import DownloadError
 
+from . import MockResponse, dataset_resultdict
+from .test_resource_view import resource_view_list, resource_view_mocklist
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.resource import Resource
-
-from . import MockResponse, dataset_resultdict
-from .test_resource_view import resource_view_list, resource_view_mocklist
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.downloader import DownloadError
 
 resultdict = {
     "cache_last_updated": None,
     "package_id": "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d",
     "webstore_last_updated": None,
     "datastore_active": None,
     "id": "de6549d8-268b-4dfe-adaf-a4ae5c8510d5",
@@ -327,24 +326,24 @@
         "resource_type": "api",
     }
 
     datastore = None
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
-        return join("tests", "fixtures", "config", "hdx_resource_static.yml")
+        return join("tests", "fixtures", "config", "hdx_resource_static.yaml")
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join("tests", "fixtures", "config", "hdx_resource_static.json")
 
     @pytest.fixture(scope="class")
     def topline_yaml(self):
         return join(
-            "tests", "fixtures", "config", "hdx_datasource_topline.yml"
+            "tests", "fixtures", "config", "hdx_datasource_topline.yaml"
         )
 
     @pytest.fixture(scope="class")
     def topline_json(self):
         return join(
             "tests", "fixtures", "config", "hdx_datasource_topline.json"
         )
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

```diff
@@ -1,20 +1,19 @@
 """Resource view Tests"""
 import copy
 import json
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
 
+from . import MockResponse
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.resource_view import ResourceView
-
-from . import MockResponse
+from hdx.utilities.dictandlist import merge_two_dictionaries
 
 hxl_preview_config = '{"configVersion":2,"bites":[{"init":true,"type":"key figure","filteredValues":[],"errorMsg":null,"ingredient":{"aggregateColumn":null,"valueColumn":"#affected+killed","aggregateFunction":"sum"},"dataTitle":"#affected+killed","displayCategory":"Key Figures","unit":null,"hashCode":-1955043658,"title":"Sum of fatalities","value":null},{"init":true,"type":"chart","filteredValues":[],"errorMsg":null,"swapAxis":true,"showGrid":true,"pieChart":false,"ingredient":{"aggregateColumn":"#adm1+name","valueColumn":"#affected+killed","aggregateFunction":"sum"},"dataTitle":"#affected+killed","displayCategory":"Charts","hashCode":738289179,"title":"Sum of fatalities grouped by admin1","values":null,"categories":null},{"init":true,"type":"chart","filteredValues":[],"errorMsg":null,"swapAxis":true,"showGrid":true,"pieChart":false,"ingredient":{"aggregateColumn":"#adm2+name","valueColumn":"#affected+killed","aggregateFunction":"sum"},"dataTitle":"#affected+killed","displayCategory":"Charts","hashCode":766918330,"title":"Sum of fatalities grouped by admin2","values":null,"categories":null}]}'
 
 resource_view_list = [
     {
         "description": "",
         "resource_id": "25982d1c-f45a-45e1-b14e-87d367413045",
@@ -131,15 +130,15 @@
         "title": "Data Explorer",
         "view_type": "recline_view",
     }
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
         return join(
-            "tests", "fixtures", "config", "hdx_resource_view_static.yml"
+            "tests", "fixtures", "config", "hdx_resource_view_static.yaml"
         )
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join(
             "tests", "fixtures", "config", "hdx_resource_view_static.json"
         )
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_showcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Showcase Tests"""
 import copy
 import json
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.loader import load_yaml
 
+from . import MockResponse
+from .test_vocabulary import vocabulary_mockshow
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.showcase import Showcase
-
-from . import MockResponse
-from .test_vocabulary import vocabulary_mockshow
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.loader import load_yaml
 
 showcase_resultdict = {
     "relationships_as_object": [],
     "num_tags": 2,
     "id": "05e392bf-04e0-4ca6-848c-4e87bba10746",
     "metadata_created": "2017-07-03T07:50:49.474517",
     "metadata_modified": "2017-07-03T08:12:43.726624",
@@ -53,18 +52,18 @@
     "url": "http://visualisation/url/",
     "title": "MyShowcase1",
     "image_display_url": "http://myvisual/visual.png",
     "name": "showcase-1",
 }
 
 datasetsdict = load_yaml(
-    join("tests", "fixtures", "dataset_search_results.yml")
+    join("tests", "fixtures", "dataset_search_results.yaml")
 )
 allsearchdict = load_yaml(
-    join("tests", "fixtures", "showcase_all_search_results.yml")
+    join("tests", "fixtures", "showcase_all_search_results.yaml")
 )
 
 
 def mockshow(url, datadict):
     if "package_list" in url:
         result = json.dumps(datasetsdict["results"])
         return MockResponse(
@@ -179,15 +178,15 @@
         "tags": [{"name": "economy"}, {"name": "health"}],
         "dataset_ids": ["a89c6260-6392-416e-bcbc-eb2c5f1d7add"],
     }
     association = None
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
-        return join("tests", "fixtures", "config", "hdx_showcase_static.yml")
+        return join("tests", "fixtures", "config", "hdx_showcase_static.yaml")
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join("tests", "fixtures", "config", "hdx_showcase_static.json")
 
     @pytest.fixture(scope="function")
     def read(self):
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_update_dataset_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from os.path import join
 
 import pytest
-from hdx.location.country import Country
 
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
 from hdx.data.vocabulary import Vocabulary
+from hdx.location.country import Country
 
 
 class TestUpdateDatasetResourcesLogic:
     file_mapping = {
         "SDG 4 Global and Thematic data": "sdg_data_zwe.csv",
         "SDG 4 Global and Thematic indicator list": "sdg_indicatorlist_zwe.csv",
         "SDG 4 Global and Thematic metadata": "sdg_metadata_zwe.csv",
@@ -26,15 +26,15 @@
 
     @pytest.fixture(scope="function")
     def configuration(self):
         Configuration._create(
             hdx_read_only=True,
             user_agent="test",
             project_config_yaml=join(
-                "tests", "fixtures", "config", "project_configuration.yml"
+                "tests", "fixtures", "config", "project_configuration.yaml"
             ),
         )
         Locations.set_validlocations([{"name": "zmb", "title": "Zambia"}])
         Country.countriesdata(use_live=False)
         Vocabulary._tags_dict = dict()
         Vocabulary._approved_vocabulary = {
             "tags": [
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_update_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from os.path import join
 
 import pytest
-from hdx.location.country import Country
-from hdx.utilities.loader import load_yaml
-from hdx.utilities.text import multiple_replace
 from slugify import slugify
 
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
 from hdx.data.vocabulary import Vocabulary
+from hdx.location.country import Country
+from hdx.utilities.loader import load_yaml
+from hdx.utilities.text import multiple_replace
 
 
 class TestUpdateLogic:
     @pytest.fixture(scope="function")
     def configuration(self):
         Configuration._create(
             hdx_read_only=True,
             user_agent="test",
             project_config_yaml=join(
-                "tests", "fixtures", "config", "project_configuration.yml"
+                "tests", "fixtures", "config", "project_configuration.yaml"
             ),
         )
         Locations.set_validlocations([{"name": "zmb", "title": "Zambia"}])
         Country.countriesdata(use_live=False)
         Vocabulary._tags_dict = dict()
         Vocabulary._approved_vocabulary = {
             "tags": [
@@ -40,19 +40,19 @@
 
     @pytest.fixture(scope="class")
     def fixture_path(self):
         return join("tests", "fixtures", "update_logic")
 
     @pytest.fixture(scope="class")
     def new_resources_yaml(self, fixture_path):
-        return join(fixture_path, "update_logic_resources_new.yml")
+        return join(fixture_path, "update_logic_resources_new.yaml")
 
     @pytest.fixture(scope="class")
     def resources_yaml(self, fixture_path):
-        return join(fixture_path, "update_logic_resources.yml")
+        return join(fixture_path, "update_logic_resources.yaml")
 
     @pytest.fixture(scope="class")
     def dataset_data(self):
         return {
             "name": "who-data-for-zambia",
             "title": "Zambia - Health Indicators",
             "private": False,
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_user.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """User Tests"""
 import copy
 import json
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
-from hdx.utilities.loader import load_yaml
 
+from . import MockResponse, user_data
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.user import User
-
-from . import MockResponse, user_data
+from hdx.utilities.dictandlist import merge_two_dictionaries
+from hdx.utilities.loader import load_yaml
 
 resultdict = {
     "openid": None,
     "about": "Data Scientist",
     "apikey": "31e86726-2993-4d82-be93-3d2133c81d94",
     "display_name": "xxx",
     "name": "MyUser1",
@@ -26,15 +25,17 @@
     "activity_streams_email_notifications": False,
     "state": "active",
     "number_of_edits": 0,
     "fullname": "xxx xxx",
     "id": "9f3e9973-7dbe-4c65-8820-f48578e3ffea",
     "number_created_packages": 0,
 }
-orgdict = load_yaml(join("tests", "fixtures", "organization_show_results.yml"))
+orgdict = load_yaml(
+    join("tests", "fixtures", "organization_show_results.yaml")
+)
 orgdict2 = copy.deepcopy(orgdict)
 del orgdict2["users"]
 del orgdict2["packages"]
 del orgdict2["extras"]
 orglist = [orgdict2]
 
 result2dict = copy.deepcopy(resultdict)
@@ -124,15 +125,15 @@
     sender = "me@gmail.com"
     mail_options = ["a", "b"]
     rcpt_options = [1, 2]
     email_config_dict.update(smtp_initargs)
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
-        return join("tests", "fixtures", "config", "hdx_user_static.yml")
+        return join("tests", "fixtures", "config", "hdx_user_static.yaml")
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join("tests", "fixtures", "config", "hdx_user_static.json")
 
     @pytest.fixture(scope="function")
     def read(self):
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.0.4/tests/hdx/data/test_vocabulary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Vocabulary Tests"""
 import copy
 import json
 from os.path import join
 
 import pytest
-from hdx.utilities.dictandlist import merge_two_dictionaries
 from requests.exceptions import RetryError
 
+from . import MockResponse
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.vocabulary import ChainRuleError, Vocabulary
-
-from . import MockResponse
+from hdx.utilities.dictandlist import merge_two_dictionaries
 
 vocabulary_list = [
     {
         "tags": [],
         "id": "57f71f5f-adb0-48fd-ab2c-6b93b9d30332",
         "name": "Topics",
     },
@@ -2297,15 +2296,17 @@
     vocabulary_data = {
         "tags": [{"name": "economy"}, {"name": "health"}],
         "name": "Things",
     }
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
-        return join("tests", "fixtures", "config", "hdx_vocabulary_static.yml")
+        return join(
+            "tests", "fixtures", "config", "hdx_vocabulary_static.yaml"
+        )
 
     @pytest.fixture(scope="class")
     def static_json(self):
         return join(
             "tests", "fixtures", "config", "hdx_vocabulary_static.json"
         )
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/facades/__init__.py` & `hdx_python_api-6.0.4/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.2/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.0.4/tests/hdx/facades/test_infer_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Simple Facade Tests"""
 import sys
 
 import pytest
-from hdx.utilities.useragent import UserAgent
 
+from . import my_testfnia, testresult
 from hdx.api.configuration import ConfigurationError
 from hdx.facades.infer_arguments import facade
-
-from . import my_testfnia, testresult
+from hdx.utilities.useragent import UserAgent
 
 
 class TestInferArguments:
     def test_facade(
         self,
         monkeypatch,
         hdx_config_yaml,
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.0.4/tests/hdx/facades/test_keyword_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Simple Facade Tests"""
 import pytest
-from hdx.utilities.useragent import UserAgent, UserAgentError
 
+from . import my_testfnkw, testresult
 from hdx.api import __version__
 from hdx.facades.keyword_arguments import facade
-
-from . import my_testfnkw, testresult
+from hdx.utilities.useragent import UserAgent, UserAgentError
 
 
 class TestKeywordArguments:
     def test_facade(self, monkeypatch, hdx_config_yaml, project_config_yaml):
         UserAgent.clear_global()
         my_user_agent = "test"
         testresult.actual_result = None
```

### Comparing `hdx-python-api-6.0.2/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.0.4/tests/hdx/facades/test_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Simple Facade Tests"""
 import pytest
-from hdx.utilities.useragent import UserAgent, UserAgentError
 
+from . import my_excfn, my_testfn, my_testkeyfn, my_testuafn, testresult
 from hdx.api import __version__
 from hdx.facades.simple import facade
-
-from . import my_excfn, my_testfn, my_testkeyfn, my_testuafn, testresult
+from hdx.utilities.useragent import UserAgent, UserAgentError
 
 
 class TestSimple:
     def test_facade(self, monkeypatch, hdx_config_yaml, project_config_yaml):
         UserAgent.clear_global()
         my_user_agent = "test"
         testresult.actual_result = None
```

### Comparing `hdx-python-api-6.0.2/workingexample/my_resource.xlsx` & `hdx_python_api-6.0.4/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

