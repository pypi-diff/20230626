# Comparing `tmp/hdx_python_utilities-3.6.0.tar.gz` & `tmp/hdx_python_utilities-3.6.1.tar.gz`

## Comparing `hdx_python_utilities-3.6.0.tar` & `hdx_python_utilities-3.6.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0    35300 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/main.md
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/_version.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/compare.py
--rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0        0        0    61800 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/downloader.py
--rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0        0        0     8054 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/email.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/encoding.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0        0        0     2967 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/html.py
--rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/loader.py
--rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/path.py
--rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/retriever.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/saver.py
--rwxr-xr-x   0        0        0     7647 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/session.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/state.py
--rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/text.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/typehint.py
--rwxr-xr-x   0        0        0     6838 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/useragent.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/uuid.py
--rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/compare/test_csv_processing2.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/empty.yml
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_email_configuration.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/json_csv.yml
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.yml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/smtp_config.yml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config_wrong.yml
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/basicauth.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params.yml
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params_tree.yml
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xlsx_processing.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/html/response.html
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/loader/empty.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/loader/empty.yml
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test_hxl.csv
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out2.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out2.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out5.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out6.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out7.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out8.csv
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out8.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0        0        0    47752 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0        0        0     5363 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0        0        0    10273 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/utils.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/LICENSE
--rwxr-xr-x   0        0        0     1727 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/README.md
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    35309 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/main.md
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/_version.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/compare.py
+-rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0        0        0    61802 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0        0        0     8056 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/email.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/encoding.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0        0        0     2968 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/html.py
+-rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/loader.py
+-rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/path.py
+-rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/retriever.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/saver.py
+-rwxr-xr-x   0        0        0     7648 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/session.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/state.py
+-rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/text.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0        0        0     7151 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/useragent.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/src/hdx/utilities/uuid.py
+-rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/compare/test_csv_processing2.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/hdx_email_configuration.yaml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/json_csv.yaml
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/smtp_config.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/basicauth.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params.yaml
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/extra_params_tree.yaml
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xlsx_processing.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/html/response.html
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/loader/empty.yaml
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/test_hxl.csv
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/retriever/fallbacks/test.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out2.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out2.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out5.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out6.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out7.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out8.csv
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/out8.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0        0        0    47756 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0        0        0     5657 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0        0        0    10274 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0        0        0     3541 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/tests/hdx/utilities/utils.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/LICENSE
+-rwxr-xr-x   0        0        0     1727 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/README.md
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.1/PKG-INFO
```

### Comparing `hdx_python_utilities-3.6.0/CONTRIBUTING.md` & `hdx_python_utilities-3.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/requirements.txt` & `hdx_python_utilities-3.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/.config/pre-commit-config.yaml` & `hdx_python_utilities-3.6.1/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/.github/workflows/publish.yaml` & `hdx_python_utilities-3.6.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/.github/workflows/run-python-tests.yaml` & `hdx_python_utilities-3.6.1/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/documentation/main.md` & `hdx_python_utilities-3.6.1/documentation/main.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,25 +78,25 @@
 - `download_json` returns the JSON in a Python dictionary
 - `download_yaml` returns the YAML in a Python dictionary
 - `get_tabular_rows` returns headers and an iterator (through rows)
 
 Note that a single `Download` object cannot be used in parallel: each download operation 
 must be completed before starting the next. 
 
-For example, given YAML file extraparams.yml:
+For example, given YAML file extraparams.yaml:
 
     mykey:
         basic_auth: "XXXXXXXX"
         locale: "en"
 
 We can create a downloader as shown below that will use the authentication defined in 
 `basic\_auth` and add the parameter `locale=en` to each request (eg. for get request 
 <http://myurl/lala?param1=p1&locale=en>):
 
-    with Download(user_agent="test", extra_params_yaml="extraparams.yml", extra_params_lookup="mykey") as downloader:
+    with Download(user_agent="test", extra_params_yaml="extraparams.yaml", extra_params_lookup="mykey") as downloader:
         response = downloader.download(url)  # get requests library response
         json = response.json()
 
         # Download file to folder/filename
         f = downloader.download_file("http://myurl", post=False,
                                      parameters=OrderedDict([("b", "4"), ("d", "3")]),
                                      folder=tmpdir, filename=filename)
@@ -336,34 +336,34 @@
     assert date == expected_date
 
 ## Loading and saving JSON and YAML
 
 Examples:
 
     # Load YAML
-    mydict = load_yaml("my_yaml.yml")
+    mydict = load_yaml("my_yaml.yaml")
 
     # Load 2 YAMLs and merge into dictionary
-    mydict = load_and_merge_yaml("my_yaml1.yml", "my_yaml2.yml")
+    mydict = load_and_merge_yaml("my_yaml1.yaml", "my_yaml2.yaml")
 
     # Load YAML into existing dictionary
-    mydict = load_yaml_into_existing_dict(existing_dict, "my_yaml.yml")
+    mydict = load_yaml_into_existing_dict(existing_dict, "my_yaml.yaml")
 
     # Load JSON
-    mydict = load_json("my_json.yml")
+    mydict = load_json("my_json.yaml")
 
     # Load 2 JSONs and merge into dictionary
     mydict = load_and_merge_json("my_json1.json", "my_json2.json")
 
     # Load JSON into existing dictionary
     mydict = load_json_into_existing_dict(existing_dict, "my_json.json")
 
     # Save dictionary to YAML file in pretty format
     # preserving order if it is an OrderedDict
-    save_yaml(mydict, "mypath.yml", pretty=True, sortkeys=False)
+    save_yaml(mydict, "mypath.yaml", pretty=True, sortkeys=False)
 
     # Save dictionary to JSON file in compact form
     # sorting the keys
     save_json(mydict, "mypath.json", pretty=False, sortkeys=False)
 
 ## Loading and saving HXLated csv and/or JSON
 
@@ -815,9 +815,9 @@
 Examples:
 
     assert is_valid_uuid("jpsmith") is False
     assert is_valid_uuid("c9bf9e57-1685-4c89-bafb-ff5af830be8a") is True
 
 ## Easy building and packaging
 
-The pyproject.toml, setup.cfg, .readthedocs.yml and GitHub Actions workflows 
+The pyproject.toml, setup.cfg, .readthedocs.yaml and GitHub Actions workflows 
 provide a template that can be used by other projects or libraries.
```

### Comparing `hdx_python_utilities-3.6.0/documentation/pydoc-markdown.yaml` & `hdx_python_utilities-3.6.1/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/base_downloader.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/compare.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/dateparse.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/dictandlist.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/downloader.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class Download(BaseDownload):
     """Download class with various download operations. Requires either global
     user agent to be set or appropriate user agent parameter(s) to be
     completed.
 
     Args:
         user_agent (Optional[str]): User agent string. HDXPythonUtilities/X.X.X- is prefixed.
-        user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+        user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
         user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
         use_env (bool): Whether to read environment variables. Defaults to True.
         fail_on_missing_file (bool): Raise an exception if any specified configuration files are missing. Defaults to True.
         verify (bool): Whether to verify SSL certificates. Defaults to True.
         rate_limit (Optional[Dict]): Rate limiting per host eg. {"calls": 1, "period": 0.1}. Defaults to None.
         **kwargs: See below
         auth (Tuple[str, str]): Authorisation information in tuple form (user, pass) OR
@@ -1251,15 +1251,15 @@
         params or headers. It can have keys that correspond to the input
         arguments of Download's constructor __init__ (or the other arguments of
         this method).
 
         Args:
             custom_configs (Dict[str, Dict]): Optional dictionary of custom configurations.
             user_agent (Optional[str]): User agent string. HDXPythonUtilities/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
             use_env (bool): Whether to read environment variables. Defaults to True.
             fail_on_missing_file (bool): Raise an exception if any specified configuration files are missing. Defaults to True.
             rate_limit (Optional[Dict]): Rate limiting per host eg. {"calls": 1, "period": 0.1}. Defaults to None.
             **kwargs: See below
             auth (Tuple[str, str]): Authorisation information in tuple form (user, pass) OR
             basic_auth (str): Authorisation information in basic auth string form (Basic xxxxxxxxxxxxxxxx) OR
```

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/easy_logging.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/email.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
      | password: "pass"
      | sender: "a@b.com"    (if not supplied username is used as sender)
 
     Args:
         **kwargs: See below
         email_config_dict (dict): HDX configuration dictionary OR
         email_config_json (str): Path to JSON HDX configuration OR
-        email_config_yaml (str): Path to YAML HDX configuration. Defaults to ~/hdx_email_configuration.yml.
+        email_config_yaml (str): Path to YAML HDX configuration. Defaults to ~/hdx_email_configuration.yaml.
     """
 
     default_email_config_yaml = join(
-        expanduser("~"), "hdx_email_configuration.yml"
+        expanduser("~"), "hdx_email_configuration.yaml"
     )
 
     def __init__(self, **kwargs: Any) -> None:
         email_config_found = False
         email_config_dict = kwargs.get("email_config_dict", None)
         if email_config_dict:
             email_config_found = True
```

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/encoding.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/errors_onexit.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/frictionless_wrapper.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/frictionless_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/html.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         """Get BeautifulSoup object for a url. Requires either global user
         agent to be set or appropriate user agent parameter(s) to be completed.
 
         Args:
             url (str): url to read
             downloader (Download): Download object. Defaults to creating a Download object with given user agent values.
             user_agent (Optional[str]): User agent string. HDXPythonUtilities/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
 
         Returns:
             BeautifulSoup: The BeautifulSoup object for a url
         """
         if not downloader:
             downloader = Download(
```

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/loader.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/path.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/retriever.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/saver.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/session.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """Set up and return Session object that is set up with retrying. Requires
     either global user agent to be set or appropriate user agent parameter(s)
     to be completed. If the EXTRA_PARAMS or BASIC_AUTH environment variable is
     supplied, the extra_params* parameters will be ignored.
 
     Args:
         user_agent (Optional[str]): User agent string. HDXPythonUtilities/X.X.X- is prefixed.
-        user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+        user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
         user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
         use_env (bool): Whether to read environment variables. Defaults to True.
         fail_on_missing_file (bool): Raise an exception if any specified configuration files are missing. Defaults to True.
         verify (bool): Whether to verify SSL certificates. Defaults to True.
         **kwargs: See below
         auth (Tuple[str, str]): Authorisation information in tuple form (user, pass) OR
         basic_auth (str): Authorisation information in basic auth string form (Basic xxxxxxxxxxxxxxxx) OR
```

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/state.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/text.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/useragent.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/useragent.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class UserAgentError(Exception):
     pass
 
 
 class UserAgent:
-    default_user_agent_config_yaml = join(expanduser("~"), ".useragent.yml")
+    default_user_agent_config_yaml = join(expanduser("~"), ".useragent.yaml")
     user_agent = None
 
     @staticmethod
     def _environment_variables(**kwargs: Any) -> Any:
         """Overwrite keyword arguments with environment variables.
 
         Args:
@@ -78,21 +78,26 @@
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
 
         Returns:
             str: user agent
         """
         if not user_agent_config_yaml:
             user_agent_config_yaml = cls.default_user_agent_config_yaml
-            logger.info(
-                f"No user agent or user agent config file given. Using default user agent config file: {user_agent_config_yaml}."
-            )
-        if not isfile(user_agent_config_yaml):
-            raise UserAgentError(
-                "User_agent should be supplied in a YAML config file. It can be your project's name for example."
-            )
+            if not isfile(user_agent_config_yaml):
+                user_agent_config_yaml = user_agent_config_yaml.replace(
+                    ".yaml", ".yml"
+                )
+            if isfile(user_agent_config_yaml):
+                logger.info(
+                    f"No user agent or user agent config file given. Using default user agent config file: {user_agent_config_yaml}."
+                )
+            else:
+                raise UserAgentError(
+                    f"User_agent should be supplied in a YAML config file and no configuration file at default path: {cls.default_user_agent_config_yaml}. User agent can be your project's name for example."
+                )
         logger.info(
             f"Loading user agent config from: {user_agent_config_yaml}"
         )
         user_agent_config_dict = load_yaml(user_agent_config_yaml)
         if user_agent_lookup:
             user_agent_config_dict = user_agent_config_dict.get(
                 user_agent_lookup
@@ -112,15 +117,15 @@
         user_agent_lookup: Optional[str] = None,
         **kwargs: Any,
     ) -> str:
         """Get full user agent string.
 
         Args:
             user_agent (Optional[str]): User agent string. HDXPythonLibrary/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
 
         Returns:
             str: Full user agent string
         """
         kwargs = UserAgent._environment_variables(**kwargs)
         user_agent = kwargs.pop("user_agent", user_agent)
@@ -150,15 +155,15 @@
         user_agent_lookup: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Set global user agent string.
 
         Args:
             user_agent (Optional[str]): User agent string. HDXPythonLibrary/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
 
         Returns:
             None
         """
         cls.user_agent = cls._create(
             user_agent, user_agent_config_yaml, user_agent_lookup, **kwargs
@@ -173,15 +178,15 @@
         **kwargs: Any,
     ) -> str:
         """Get full user agent string from parameters if supplied falling back
         on global user agent if set.
 
         Args:
             user_agent (Optional[str]): User agent string. HDXPythonLibrary/X.X.X- is prefixed.
-            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yml.
+            user_agent_config_yaml (Optional[str]): Path to YAML user agent configuration. Ignored if user_agent supplied. Defaults to ~/.useragent.yaml.
             user_agent_lookup (Optional[str]): Lookup key for YAML. Ignored if user_agent supplied.
 
         Returns:
             str: Full user agent string
         """
         if (
             user_agent
```

### Comparing `hdx_python_utilities-3.6.0/src/hdx/utilities/uuid.py` & `hdx_python_utilities-3.6.1/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/test_data.csv` & `hdx_python_utilities-3.6.1/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/config/json_csv.yml` & `hdx_python_utilities-3.6.1/tests/fixtures/config/json_csv.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.json` & `hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.yml` & `hdx_python_utilities-3.6.1/tests/fixtures/config/logging_config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.xlsx` & `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xls_processing.xls` & `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx_python_utilities-3.6.1/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/fixtures/html/response.html` & `hdx_python_utilities-3.6.1/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/conftest.py` & `hdx_python_utilities-3.6.1/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_compare.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dateparse.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dictandlist.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_downloader.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     @pytest.fixture(scope="class")
     def downloaderfolder(self, fixturesfolder):
         return join(fixturesfolder, self.downloaderfoldername)
 
     @pytest.fixture(scope="class")
     def fixturefile(self, downloaderfolder):
-        return join(downloaderfolder, "extra_params_tree.yml")
+        return join(downloaderfolder, "extra_params_tree.yaml")
 
     @pytest.fixture(scope="class")
     def fixtureurl(self):
         return "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-utilities/main/tests/fixtures/test_data.csv"
 
     @pytest.fixture(scope="class")
     def fixtureurlexcel(self):
@@ -117,15 +117,15 @@
         with Download(auth=("u", "p")) as downloader:
             assert downloader.session.auth == ("u", "p")
         basicauth = "Basic dXNlcjpwYXNz"
         with Download(basic_auth=basicauth) as downloader:
             assert downloader.session.auth == ("user", "pass")
         with Download(basic_auth_file=basicauthfile) as downloader:
             assert downloader.session.auth == ("testuser", "testpass")
-        extraparamsyamltree = join(downloaderfolder, "extra_params_tree.yml")
+        extraparamsyamltree = join(downloaderfolder, "extra_params_tree.yaml")
         with Download(
             extra_params_yaml=extraparamsyamltree, extra_params_lookup="mykey"
         ) as downloader:
             assert downloader.session.auth == ("testuser", "testpass")
         monkeypatch.setenv("BASIC_AUTH", basicauth)
         with Download() as downloader:
             assert downloader.session.auth == ("user", "pass")
@@ -168,15 +168,15 @@
         with pytest.raises(SessionError):
             Download(
                 extra_params_yaml=extraparamsyamltree,
                 extra_params_lookup="missingkey",
             )
         with pytest.raises(IOError):
             Download(basic_auth_file="NOTEXIST")
-        extraparamsyaml = join(downloaderfolder, "extra_params.yml")
+        extraparamsyaml = join(downloaderfolder, "extra_params.yaml")
         test_url = "http://www.lalala.com/lala"
         with Download(
             basic_auth_file=basicauthfile, extra_params_dict={"key1": "val1"}
         ) as downloader:
             assert downloader.session.auth == ("testuser", "testpass")
             assert downloader.get_full_url(test_url) == f"{test_url}?key1=val1"
         key = "Authorization"
@@ -363,15 +363,15 @@
             downloader.download_file(
                 fixturefile, filename=filename, path=join(tmpdir, filename)
             )
         with Download() as downloader:
             f = downloader.download_file(fixturefile, folder=tmpdir)
             fpath = abspath(f)
             remove(f)
-            assert fpath == abspath(join(tmpdir, "extra_params_tree.yml"))
+            assert fpath == abspath(join(tmpdir, "extra_params_tree.yaml"))
             f = downloader.download_file(fixtureurl, folder=tmpdir)
             fpath = abspath(f)
             remove(f)
             assert fpath == abspath(join(tmpdir, "test_data.csv"))
             f = downloader.download_file(
                 fixtureurl, folder=tmpdir, filename=filename
             )
```

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_easy_logging.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_email.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestEmail:
     @pytest.fixture(scope="class")
     def email_json(self, configfolder):
         return join(configfolder, "hdx_email_configuration.json")
 
     @pytest.fixture(scope="class")
     def email_yaml(self, configfolder):
-        return join(configfolder, "hdx_email_configuration.yml")
+        return join(configfolder, "hdx_email_configuration.yaml")
 
     def test_mail(self, mocksmtp):
         smtp_initargs = {
             "host": "localhost",
             "port": 123,
             "local_hostname": "mycomputer.fqdn.com",
             "timeout": 3,
```

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_encoding.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_errors_onexit.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_html.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_loader.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,42 +113,42 @@
 a
 test"""
     expected_text_newlines_to_spaces = """  hello this is a test    """
 
     def test_load_empty(self, fixturesfolder):
         loaderfolder = join(fixturesfolder, "loader")
         with pytest.raises(LoadError):
-            load_text(join(loaderfolder, "empty.yml"))
+            load_text(join(loaderfolder, "empty.yaml"))
         with pytest.raises(LoadError):
-            load_yaml(join(loaderfolder, "empty.yml"))
+            load_yaml(join(loaderfolder, "empty.yaml"))
         with pytest.raises(LoadError):
             load_json(join(loaderfolder, "empty.json"))
 
     def test_load_and_merge_yaml(self, configfolder):
         result = load_and_merge_yaml(
             [
-                join(configfolder, "hdx_config.yml"),
-                join(configfolder, "project_configuration.yml"),
+                join(configfolder, "hdx_config.yaml"),
+                join(configfolder, "project_configuration.yaml"),
             ]
         )
         assert list(result.items()) == list(TestLoader.expected_yaml.items())
 
     def test_load_and_merge_json(self, configfolder):
         result = load_and_merge_json(
             [
                 join(configfolder, "hdx_config.json"),
                 join(configfolder, "project_configuration.json"),
             ]
         )
         assert list(result.items()) == list(TestLoader.expected_json.items())
 
     def test_load_yaml_into_existing_dict(self, configfolder):
-        existing_dict = load_yaml(join(configfolder, "hdx_config.yml"))
+        existing_dict = load_yaml(join(configfolder, "hdx_config.yaml"))
         result = load_yaml_into_existing_dict(
-            existing_dict, join(configfolder, "project_configuration.yml")
+            existing_dict, join(configfolder, "project_configuration.yaml")
         )
         assert list(result.items()) == list(TestLoader.expected_yaml.items())
 
     def test_load_json_into_existing_dict(self, configfolder):
         existing_dict = load_json(join(configfolder, "hdx_config.json"))
         result = load_json_into_existing_dict(
             existing_dict, join(configfolder, "project_configuration.json")
```

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_path.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_retriever.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_saver.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     @pytest.fixture(scope="class")
     def saverfolder(self, fixturesfolder):
         return join(fixturesfolder, "saver")
 
     @pytest.fixture(scope="class")
     def json_csv_configuration(self, fixturesfolder):
-        return load_yaml(join(fixturesfolder, "config", "json_csv.yml"))
+        return load_yaml(join(fixturesfolder, "config", "json_csv.yaml"))
 
     @pytest.mark.parametrize(
         "filename,pretty,sortkeys",
         [
             ("pretty-false_sortkeys-false.yaml", False, False),
             ("pretty-false_sortkeys-true.yaml", False, True),
             ("pretty-true_sortkeys-false.yaml", True, False),
```

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_state.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_text.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_useragent.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/test_useragent.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from hdx.utilities.loader import LoadError
 from hdx.utilities.useragent import UserAgent, UserAgentError
 
 
 class TestUserAgent:
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
 
     def test_user_agent(
         self,
         monkeypatch,
         user_agent_config_yaml,
         user_agent_config2_yaml,
         user_agent_config3_yaml,
```

### Comparing `hdx_python_utilities-3.6.0/tests/hdx/utilities/utils.py` & `hdx_python_utilities-3.6.1/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/.gitignore` & `hdx_python_utilities-3.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/LICENSE` & `hdx_python_utilities-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/README.md` & `hdx_python_utilities-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/pyproject.toml` & `hdx_python_utilities-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.6.0/PKG-INFO` & `hdx_python_utilities-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-utilities
-Version: 3.6.0
+Version: 3.6.1
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-utilities
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,date,datetime,dict,json,library,list,streaming,tabular data,time,timezone,utilities,yaml
 Classifier: Development Status :: 5 - Production/Stable
```

