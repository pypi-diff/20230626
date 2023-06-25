# Comparing `tmp/hdx_python_utilities-3.5.9.tar.gz` & `tmp/hdx_python_utilities-3.6.0.tar.gz`

## Comparing `hdx_python_utilities-3.5.9.tar` & `hdx_python_utilities-3.6.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.github/workflows/run-python-tests.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0    35300 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/main.md
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/pydoc-markdown.yml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/_version.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/compare.py
--rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0        0        0    61800 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/downloader.py
--rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0        0        0     8054 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/email.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/encoding.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0        0        0     2967 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/html.py
--rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/loader.py
--rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/path.py
--rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/retriever.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/saver.py
--rwxr-xr-x   0        0        0     7647 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/session.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/state.py
--rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/text.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/typehint.py
--rwxr-xr-x   0        0        0     6838 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/useragent.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/uuid.py
--rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/compare/test_csv_processing2.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/empty.yml
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_email_configuration.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/json_csv.yml
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.yml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/smtp_config.yml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config_wrong.yml
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/basicauth.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params.yml
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params_tree.yml
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xlsx_processing.xlsx
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/html/response.html
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/loader/empty.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/loader/empty.yml
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test_hxl.csv
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out2.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out2.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out5.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out6.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out7.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out8.csv
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out8.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0        0        0    47752 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0        0        0     5363 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0        0        0    10273 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/utils.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/LICENSE
--rwxr-xr-x   0        0        0     1725 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/README.md
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/pyproject.toml
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    35300 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/main.md
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/_version.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/compare.py
+-rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0        0        0    61800 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0        0        0     8054 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/email.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/encoding.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0        0        0     2967 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/html.py
+-rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/loader.py
+-rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/path.py
+-rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/retriever.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/saver.py
+-rwxr-xr-x   0        0        0     7647 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/session.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/state.py
+-rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/text.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0        0        0     6838 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/useragent.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/src/hdx/utilities/uuid.py
+-rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/compare/test_csv_processing2.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/empty.yml
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_config.yml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/hdx_email_configuration.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/json_csv.yml
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.yml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/project_configuration.yml
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/smtp_config.yml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config.yml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config2.yml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config3.yml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/config/user_agent_config_wrong.yml
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/basicauth.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params.yml
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/extra_params_tree.yml
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xlsx_processing.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/html/response.html
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/loader/empty.yml
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/test_hxl.csv
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/retriever/fallbacks/test.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out2.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out2.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out5.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out6.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out7.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out8.csv
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/out8.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0        0        0    47752 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0        0        0     5363 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0        0        0    10273 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/tests/hdx/utilities/utils.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/LICENSE
+-rwxr-xr-x   0        0        0     1727 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/README.md
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 hdx_python_utilities-3.6.0/PKG-INFO
```

### Comparing `hdx_python_utilities-3.5.9/CONTRIBUTING.md` & `hdx_python_utilities-3.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/requirements.txt` & `hdx_python_utilities-3.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/.config/pre-commit-config.yaml` & `hdx_python_utilities-3.6.0/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/.github/workflows/publish.yml` & `hdx_python_utilities-3.6.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/.github/workflows/run-python-tests.yml` & `hdx_python_utilities-3.6.0/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/documentation/main.md` & `hdx_python_utilities-3.6.0/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/documentation/pydoc-markdown.yml` & `hdx_python_utilities-3.6.0/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/base_downloader.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/compare.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/dateparse.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/dictandlist.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/downloader.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/easy_logging.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/email.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/email.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/encoding.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/errors_onexit.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/frictionless_wrapper.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/frictionless_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/html.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/loader.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/path.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/retriever.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/saver.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/session.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/session.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/state.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/text.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/useragent.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/src/hdx/utilities/uuid.py` & `hdx_python_utilities-3.6.0/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/test_data.csv` & `hdx_python_utilities-3.6.0/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/config/json_csv.yml` & `hdx_python_utilities-3.6.0/tests/fixtures/config/json_csv.yml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.json` & `hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.yml` & `hdx_python_utilities-3.6.0/tests/fixtures/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.xlsx` & `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xls_processing.xls` & `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx_python_utilities-3.6.0/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/fixtures/html/response.html` & `hdx_python_utilities-3.6.0/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/conftest.py` & `hdx_python_utilities-3.6.0/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_compare.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dateparse.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dictandlist.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_downloader.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_easy_logging.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_email.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_email.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_encoding.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_errors_onexit.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_html.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_loader.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_loader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_path.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_retriever.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_saver.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_saver.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_state.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_state.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_text.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_useragent.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/test_useragent.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/tests/hdx/utilities/utils.py` & `hdx_python_utilities-3.6.0/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/.gitignore` & `hdx_python_utilities-3.6.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -90,9 +90,9 @@
 
 # Rope project settings
 .ropeproject
 
 # IntelliJ
 .idea/
 
-# setuptools_scm
+# hatch-vcs
 _version.py
```

### Comparing `hdx_python_utilities-3.5.9/LICENSE` & `hdx_python_utilities-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/README.md` & `hdx_python_utilities-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-utilities/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-utilities?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-utilities.svg)](https://pypistats.org/packages/hdx-python-utilities)
 
 The HDX Python Utilities Library provides a range of helpful utilities for Python developers.
 Note that these are not specific to HDX.
```

### Comparing `hdx_python_utilities-3.5.9/pyproject.toml` & `hdx_python_utilities-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_utilities-3.5.9/PKG-INFO` & `hdx_python_utilities-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-utilities
-Version: 3.5.9
+Version: 3.6.0
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-utilities
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,date,datetime,dict,json,library,list,streaming,tabular data,time,timezone,utilities,yaml
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,15 +46,15 @@
 Requires-Dist: html5lib; extra == 'html'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-loguru; extra == 'test'
 Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-utilities/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-utilities?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-utilities.svg)](https://pypistats.org/packages/hdx-python-utilities)
 
 The HDX Python Utilities Library provides a range of helpful utilities for Python developers.
 Note that these are not specific to HDX.
```

