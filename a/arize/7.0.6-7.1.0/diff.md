# Comparing `tmp/arize-7.0.6.tar.gz` & `tmp/arize-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.6.tar", last modified: Fri Jun 23 23:18:18 2023, max compression
+gzip compressed data, was "arize-7.1.0.tar", last modified: Mon Jun 26 21:01:01 2023, max compression
```

## Comparing `arize-7.0.6.tar` & `arize-7.1.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.165696 arize-7.0.6/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.0.6/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.0.6/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-23 23:18:18.166301 arize-7.0.6/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.0.6/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.046826 arize-7.0.6/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-23 23:13:32.000000 arize-7.0.6/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    28894 2023-06-23 23:03:21.000000 arize-7.0.6/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.0.6/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.065660 arize-7.0.6/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.069277 arize-7.0.6/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.074547 arize-7.0.6/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/session.py
--rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/publicexporter_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.079696 arize-7.0.6/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.081758 arize-7.0.6/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.108897 arize-7.0.6/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.116670 arize-7.0.6/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.133017 arize-7.0.6/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.135695 arize-7.0.6/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.142782 arize-7.0.6/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-23 23:03:21.000000 arize-7.0.6/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.155145 arize-7.0.6/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.0.6/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.054498 arize-7.0.6/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      429 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.0.6/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-06-23 23:18:18.168879 arize-7.0.6/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.162170 arize-7.0.6/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49474 2023-06-23 23:03:21.000000 arize-7.0.6/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.0.6/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.283121 arize-7.1.0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.1.0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.1.0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-26 21:01:01.283336 arize-7.1.0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.1.0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.231870 arize-7.1.0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-26 20:59:58.000000 arize-7.1.0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    31982 2023-06-26 20:59:58.000000 arize-7.1.0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.1.0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.245214 arize-7.1.0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.247189 arize-7.1.0/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.251312 arize-7.1.0/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/session.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.256106 arize-7.1.0/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.257608 arize-7.1.0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.266926 arize-7.1.0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.267733 arize-7.1.0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.270194 arize-7.1.0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.271744 arize-7.1.0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.274302 arize-7.1.0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50975 2023-06-26 20:59:58.000000 arize-7.1.0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.280500 arize-7.1.0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.1.0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.237134 arize-7.1.0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      429 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.1.0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-06-26 21:01:01.284280 arize-7.1.0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.282373 arize-7.1.0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    59500 2023-06-26 20:59:58.000000 arize-7.1.0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.1.0/tests/test_utils.py
```

### Comparing `arize-7.0.6/LICENSE.md` & `arize-7.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/PKG-INFO` & `arize-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.6
+Version: 7.1.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.6/README.md` & `arize-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/api.py` & `arize-7.1.0/arize/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
     MIN_PREDICTION_ID_LEN,
 )
 from arize.utils.logging import logger
 from google.protobuf.json_format import MessageToDict
-from google.protobuf.wrappers_pb2 import DoubleValue
+from google.protobuf.wrappers_pb2 import BoolValue, DoubleValue
 from requests_futures.sessions import FuturesSession
 
 from . import public_pb2 as pb2
 from .__init__ import __version__
 from .bounded_executor import BoundedExecutor
 from .utils.types import (
     CATEGORICAL_MODEL_TYPES,
@@ -124,14 +124,16 @@
         prediction_label: Optional[PredictionLabelTypes] = None,
         actual_label: Optional[ActualLabelTypes] = None,
         features: Optional[Dict[str, Union[str, bool, float, int]]] = None,
         embedding_features: Optional[Dict[str, Embedding]] = None,
         shap_values: Optional[Dict[str, float]] = None,
         tags: Optional[Dict[str, Union[str, bool, float, int]]] = None,
         batch_id: Optional[str] = None,
+        prompt: Optional[Embedding] = None,
+        response: Optional[Embedding] = None,
     ) -> cf.Future:
         """
         Logs a record to Arize via a POST request.
 
         Arguments:
         ----------
             model_id (str): A unique name to identify your model in the Arize platform.
@@ -153,22 +155,28 @@
             actual_label (bool, int, float, str, Tuple[str, float], ObjectDetectionLabel or
                 RankingActualLabel; optional): The ground truth value for a given model input. This will be
                 be matched to the prediction with the same prediction_id as the one in this call. Defaults
                 to None.
             features (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing
                 human readable and debuggable model features. Defaults to None.
             embedding_features (Dict[str, Embedding], optional): Dictionary containing model
-                embedding features. Keys must be strings. Values must be of Embedding type. Defaults to
+                embedding features. Keys must be strings. Values must be of type Embedding. Defaults to
                 None.
             shap_values (Dict[str, float], optional): Dictionary containing human readable and
                 debuggable model features keys, along with SHAP feature importance values. Defaults to None.
             tags (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing human
                 readable and debuggable model tags. Defaults to None.
             batch_id (str, optional): Used to distinguish different batch of data under the same
                 model_id and model_version. Required for VALIDATION environments. Defaults to None.
+            prompt (Embedding, optional): Embedding object containing the embedding vector (required) and raw
+                text (optional, but recommended) for the input text on which your GENERATIVE_LLM model acts
+                on. Required for GENERATIVE_LLM models. Defaults to None.
+            response (Embedding, optional): Embedding object containing the embedding vector (required) and
+                raw text (optional, but recommended) for the text GENERATIVE_LLM model generates.
+                Required for GENERATIVE_LLM models. Defaults to None.
 
         Returns:
         --------
             `concurrent.futures.Future` object
         """
         # Validate model_id
         if not isinstance(model_id, str):
@@ -209,19 +217,27 @@
 
         # Validate embedding_features type
         if embedding_features:
             if model_type == ModelTypes.OBJECT_DETECTION:
                 # Check that there is only 1 embedding feature for OD model types
                 if len(embedding_features.keys()) > 1:
                     raise ValueError("Object Detection models only support one embedding feature")
+            if model_type == ModelTypes.GENERATIVE_LLM:
+                # Check reserved keys are not used
+                reserved_emb_feat_names = {"prompt", "response"}
+                if reserved_emb_feat_names & embedding_features.keys():
+                    raise KeyError(
+                        "embedding features cannot use the reserved feature names ('prompt', 'response') "
+                        "for GENERATIVE_LLM models"
+                    )
             for emb_name, emb_obj in embedding_features.items():
                 _validate_mapping_key(emb_name)
                 # Must verify embedding type
                 if not isinstance(emb_obj, Embedding):
-                    raise TypeError(f'Embedding feature "{emb_name}" must be of embedding type')
+                    raise TypeError(f'Embedding feature "{emb_name}" must be of type Embedding')
                 emb_obj.validate(emb_name)
 
         # Validate tag types
         if tags:
             for tag_name, tag_value in tags.items():
                 _validate_mapping_key(tag_name)
                 val = convert_element(tag_value)
@@ -258,16 +274,37 @@
                 )
             if not is_timestamp_in_range(now, prediction_timestamp):
                 raise ValueError(
                     f"prediction_timestamp: {prediction_timestamp} is out of range."
                     f"Prediction timestamps must be within {MAX_FUTURE_YEARS_FROM_CURRENT_TIME} year in the "
                     f"future and {MAX_PAST_YEARS_FROM_CURRENT_TIME} years in the past from the current time."
                 )
+
+        # Validate GENERATIVE_LLM models requirements
+        if model_type == ModelTypes.GENERATIVE_LLM:
+            if prompt is None or response is None:
+                raise ValueError(
+                    "The following fields cannot be None for GENERATIVE_LLM models: prompt, response"
+                )
+            for emb_name, emb_obj in {"prompt": prompt, "response": response}.items():
+                # Must verify embedding type
+                if not isinstance(emb_obj, Embedding):
+                    raise TypeError("Both prompt and response objects must be of type Embedding")
+                emb_obj.validate(emb_name)
+        else:
+            if prompt is not None or response is not None:
+                raise ValueError(
+                    "The fields 'prompt' and 'response' must be None for model types other "
+                    "than GENERATIVE_LLM"
+                )
+
         # Construct the prediction
         p = None
+        if model_type == ModelTypes.GENERATIVE_LLM and prediction_label is None:
+            prediction_label = 1
         if prediction_label is not None:
             if model_version is not None and not isinstance(model_version, str):
                 raise TypeError(
                     f"model_version {model_version} is type {type(model_version)}, but must be a "
                     f"str"
                 )
             _validate_label(
@@ -285,16 +322,21 @@
                 model_version=model_version,
             )
             if features is not None:
                 converted_feats = convert_dictionary(features)
                 feats = pb2.Prediction(features=converted_feats)
                 p.MergeFrom(feats)
 
-            if embedding_features is not None:
-                converted_embedding_feats = convert_dictionary(embedding_features)
+            if embedding_features or prompt or response:
+                # NOTE: Deep copy is necessary to avoid side effects on the original input dictionary
+                combined_embedding_features = {k: v for k, v in embedding_features.items()}
+                # Map prompt/response as embedding features for generative models
+                if model_type == ModelTypes.GENERATIVE_LLM:
+                    combined_embedding_features.update({"prompt": prompt, "response": response})
+                converted_embedding_feats = convert_dictionary(combined_embedding_features)
                 embedding_feats = pb2.Prediction(features=converted_embedding_feats)
                 p.MergeFrom(embedding_feats)
 
             if tags is not None:
                 converted_tags = convert_dictionary(tags)
                 tgs = pb2.Prediction(tags=converted_tags)
                 p.MergeFrom(tgs)
@@ -363,14 +405,15 @@
             space_key=self._space_key,
             model_id=model_id,
             prediction_id=prediction_id,
             prediction=p,
             actual=a,
             feature_importances=fi,
             environment_params=env_params,
+            is_generative_llm_record=BoolValue(value=model_type == ModelTypes.GENERATIVE_LLM),
         )
         return self._post(record=rec, uri=self._uri, indexes=None)
 
     def _post(self, record, uri, indexes):
         resp = self._session.post(
             uri,
             headers=self._headers,
@@ -399,34 +442,34 @@
     embedding_features: Dict[str, Embedding],
 ):
     if model_type in NUMERIC_MODEL_TYPES:
         _validate_numeric_label(model_type, label)
     elif model_type in CATEGORICAL_MODEL_TYPES:
         _validate_categorical_label(model_type, label)
     elif model_type == ModelTypes.OBJECT_DETECTION:
-        _validate_object_detection_label(
-            prediction_or_actual, model_type, label, embedding_features
-        )
+        _validate_object_detection_label(prediction_or_actual, label, embedding_features)
     elif model_type == ModelTypes.RANKING:
-        _validate_ranking_label(prediction_or_actual, model_type, label)
+        _validate_ranking_label(label)
+    elif model_type == ModelTypes.GENERATIVE_LLM:
+        _validate_generative_llm_label(label)
     else:
         raise TypeError(
             f"model_type {model_type} is type {type(model_type)}, but must be of "
             f"arize.utils.ModelTypes"
         )
 
 
 def _validate_numeric_label(
     model_type: ModelTypes,
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
 ):
     if not isinstance(label, (float, int)):
         raise TypeError(
             f"label {label} has type {type(label)}, but must be either float or int for "
-            f"ModelTypes.{model_type}"
+            f"{model_type}"
         )
 
 
 def _validate_categorical_label(
     model_type: ModelTypes,
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
 ):
@@ -440,49 +483,62 @@
             and isinstance(label[0], (str, bool))
             and isinstance(label[1], float)
         )
     )
     if not is_valid:
         raise TypeError(
             f"label {label} has type {type(label)}, but must be str, bool, int, float or Tuple[str, "
-            f"float] for ModelTypes.{model_type}"
+            f"float] for {model_type}"
         )
 
 
 def _validate_object_detection_label(
     prediction_or_actual: str,
-    model_type: ModelTypes,
     label: ObjectDetectionLabel,
     embedding_features: Dict[str, Embedding],
 ):
     if not isinstance(label, ObjectDetectionLabel):
         raise TypeError(
-            f"label {label} has type {type(label)}, but must be ObjectDetectionLabel for ModelTypes"
-            f".{model_type}"
+            f"label {label} has type {type(label)}, but must be ObjectDetectionLabel for"
+            f"{ModelTypes.OBJECT_DETECTION}"
         )
     if embedding_features is None:
         raise ValueError("Cannot use Object Detection Labels without an embedding feature")
     if len(embedding_features.keys()) != 1:
         raise ValueError("Object Detection Labels must be sent with exactly one embedding feature")
     label.validate(prediction_or_actual=prediction_or_actual)
 
 
 def _validate_ranking_label(
-    prediction_or_actual: str,
-    model_type: ModelTypes,
     label: Union[RankingPredictionLabel, RankingActualLabel],
 ):
     if not isinstance(label, (RankingPredictionLabel, RankingActualLabel)):
         raise TypeError(
             f"label {label} has type {type(label)}, but must be RankingPredictionLabel"
-            f"or RankingActualLabel for ModelTypes.{model_type}"
+            f"or RankingActualLabel for {ModelTypes.RANKING}"
         )
     label.validate()
 
 
+def _validate_generative_llm_label(
+    label: Union[str, bool, int, float],
+):
+    is_valid = (
+        isinstance(label, str)
+        or isinstance(label, bool)
+        or isinstance(label, int)
+        or isinstance(label, float)
+    )
+    if not is_valid:
+        raise TypeError(
+            f"label {label} has type {type(label)}, but must be str, bool, int, float "
+            f"for {ModelTypes.GENERATIVE_LLM}"
+        )
+
+
 def _get_label(
     prediction_or_actual: str,
     value: Union[
         str,
         bool,
         int,
         float,
@@ -492,15 +548,15 @@
         RankingActualLabel,
     ],
     model_type: ModelTypes,
 ) -> Union[pb2.PredictionLabel, pb2.ActualLabel]:
     value = convert_element(value)
     if model_type in NUMERIC_MODEL_TYPES:
         return _get_numeric_label(prediction_or_actual, value)
-    elif model_type in CATEGORICAL_MODEL_TYPES:
+    elif model_type in CATEGORICAL_MODEL_TYPES or model_type == ModelTypes.GENERATIVE_LLM:
         return _get_score_categorical_label(prediction_or_actual, value)
     elif model_type == ModelTypes.OBJECT_DETECTION:
         return _get_object_detection_label(prediction_or_actual, value)
     elif model_type == ModelTypes.RANKING:
         return _get_ranking_label(value)
     raise ValueError(
         f"model_type must be one of: {[mt.prediction_or_actual for mt in ModelTypes]} "
```

### Comparing `arize-7.0.6/arize/bounded_executor.py` & `arize-7.1.0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/bulk_client.py` & `arize-7.1.0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/bulk_client_shap.py` & `arize-7.1.0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/client_shap_values.py` & `arize-7.1.0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/log_client.py` & `arize-7.1.0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/log_pandas_dataframe.py` & `arize-7.1.0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/preproduction_client.py` & `arize-7.1.0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/client.py` & `arize-7.1.0/arize/exporter/core/client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/query.py` & `arize-7.1.0/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/session.py` & `arize-7.1.0/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/publicexporter_pb2.py` & `arize-7.1.0/arize/exporter/publicexporter_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/constants.py` & `arize-7.1.0/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/errors.py` & `arize-7.1.0/arize/exporter/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/schema_parser.py` & `arize-7.1.0/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/validation.py` & `arize-7.1.0/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/auto_generator.py` & `arize-7.1.0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/base_generators.py` & `arize-7.1.0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/cv_generators.py` & `arize-7.1.0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/errors.py` & `arize-7.1.0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/models.py` & `arize-7.1.0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/nlp_generators.py` & `arize-7.1.0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/tabular_generators.py` & `arize-7.1.0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.1.0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/logger.py` & `arize-7.1.0/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.1.0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/validation/errors.py` & `arize-7.1.0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/validation/validator.py` & `arize-7.1.0/arize/pandas/validation/validator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/public_pb2.py` & `arize-7.1.0/arize/public_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\x99\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\x86\x03\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x12:\n\x0bscore_value\x18\x05 \x01(\x0b\x32#.public.ScoreCategorical.ScoreValueH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1a\x1b\n\nScoreValue\x12\r\n\x05value\x18\x01 \x01(\x01\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xef\x01\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\xe7\x01\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\x83\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\x95\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x42\x06\n\x04\x64\x61ta\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x8b\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"H\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\xd7\'\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\xff\x08\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\x8c\x15\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\"T\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\x9a\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x12\x12\n\x0eGENERATIVE_LLM\x10\x07\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\xd7\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x12<\n\x18is_generative_llm_record\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\x86\x03\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x12:\n\x0bscore_value\x18\x05 \x01(\x0b\x32#.public.ScoreCategorical.ScoreValueH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1a\x1b\n\nScoreValue\x12\r\n\x05value\x18\x01 \x01(\x01\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xef\x01\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\xe7\x01\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\x83\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\x95\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x42\x06\n\x04\x64\x61ta\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x8b\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"H\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\xd7\'\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\xff\x08\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\x8c\x15\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\"T\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\x9a\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x12\x12\n\x0eGENERATIVE_LLM\x10\x07\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3')
 
 
 
 _BULKRECORD = DESCRIPTOR.message_types_by_name['BulkRecord']
 _RECORD = DESCRIPTOR.message_types_by_name['Record']
 _RECORD_ENVIRONMENTPARAMS = _RECORD.nested_types_by_name['EnvironmentParams']
 _RECORD_ENVIRONMENTPARAMS_TRAINING = _RECORD_ENVIRONMENTPARAMS.nested_types_by_name['Training']
@@ -567,127 +567,127 @@
   _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._options = None
   _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_options = b'8\001'
   _SCHEMA_GENERICSCHEMA.fields_by_name['actual_numeric_sequence']._options = None
   _SCHEMA_GENERICSCHEMA.fields_by_name['actual_numeric_sequence']._serialized_options = b'\030\001'
   _BULKRECORD._serialized_start=90
   _BULKRECORD._serialized_end=242
   _RECORD._serialized_start=245
-  _RECORD._serialized_end=910
-  _RECORD_ENVIRONMENTPARAMS._serialized_start=597
-  _RECORD_ENVIRONMENTPARAMS._serialized_end=886
-  _RECORD_ENVIRONMENTPARAMS_TRAINING._serialized_start=815
-  _RECORD_ENVIRONMENTPARAMS_TRAINING._serialized_end=825
-  _RECORD_ENVIRONMENTPARAMS_VALIDATION._serialized_start=827
-  _RECORD_ENVIRONMENTPARAMS_VALIDATION._serialized_end=857
-  _RECORD_ENVIRONMENTPARAMS_PRODUCTION._serialized_start=859
-  _RECORD_ENVIRONMENTPARAMS_PRODUCTION._serialized_end=871
-  _PREPRODUCTIONRECORD._serialized_start=913
-  _PREPRODUCTIONRECORD._serialized_end=1215
-  _PREPRODUCTIONRECORD_VALIDATIONRECORD._serialized_start=1082
-  _PREPRODUCTIONRECORD_VALIDATIONRECORD._serialized_end=1150
-  _PREPRODUCTIONRECORD_TRAININGRECORD._serialized_start=1152
-  _PREPRODUCTIONRECORD_TRAININGRECORD._serialized_end=1200
-  _SCORECATEGORICAL._serialized_start=1218
-  _SCORECATEGORICAL._serialized_end=1608
-  _SCORECATEGORICAL_CATEGORY._serialized_start=1463
-  _SCORECATEGORICAL_CATEGORY._serialized_end=1491
-  _SCORECATEGORICAL_SCOREVALUE._serialized_start=1493
-  _SCORECATEGORICAL_SCOREVALUE._serialized_end=1520
-  _SCORECATEGORICAL_SCORECATEGORY._serialized_start=1522
-  _SCORECATEGORICAL_SCORECATEGORY._serialized_end=1600
-  _OBJECTDETECTION._serialized_start=1611
-  _OBJECTDETECTION._serialized_end=1788
-  _OBJECTDETECTION_BOUNDINGBOX._serialized_start=1691
-  _OBJECTDETECTION_BOUNDINGBOX._serialized_end=1788
-  _RANKINGPREDICTION._serialized_start=1791
-  _RANKINGPREDICTION._serialized_end=1924
-  _RANKINGACTUAL._serialized_start=1926
-  _RANKINGACTUAL._serialized_end=2034
-  _LABEL._serialized_start=2037
-  _LABEL._serialized_end=2167
-  _PREDICTIONLABEL._serialized_start=2170
-  _PREDICTIONLABEL._serialized_end=2409
-  _ACTUALLABEL._serialized_start=2412
-  _ACTUALLABEL._serialized_end=2643
-  _PREDICTION._serialized_start=2646
-  _PREDICTION._serialized_end=3033
-  _PREDICTION_FEATURESENTRY._serialized_start=2911
-  _PREDICTION_FEATURESENTRY._serialized_end=2973
-  _PREDICTION_TAGSENTRY._serialized_start=2975
-  _PREDICTION_TAGSENTRY._serialized_end=3033
-  _VALUE._serialized_start=3036
-  _VALUE._serialized_end=3185
-  _MULTIVALUE._serialized_start=3187
-  _MULTIVALUE._serialized_end=3215
-  _EMBEDDING._serialized_start=3218
-  _EMBEDDING._serialized_end=3455
-  _EMBEDDING_RAWDATA._serialized_start=3344
-  _EMBEDDING_RAWDATA._serialized_end=3419
-  _EMBEDDING_TOKENARRAY._serialized_start=3421
-  _EMBEDDING_TOKENARRAY._serialized_end=3449
-  _ACTUAL._serialized_start=3458
-  _ACTUAL._serialized_end=3690
-  _ACTUAL_TAGSENTRY._serialized_start=2975
-  _ACTUAL_TAGSENTRY._serialized_end=3033
-  _FEATUREIMPORTANCES._serialized_start=3693
-  _FEATUREIMPORTANCES._serialized_end=3923
-  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_start=3866
-  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_end=3923
-  _PREDICTIONANDACTUAL._serialized_start=3925
-  _PREDICTIONANDACTUAL._serialized_end=4018
-  _FILEHEADER._serialized_start=4021
-  _FILEHEADER._serialized_end=4160
-  _FILEHEADER_ENVIRONMENT._serialized_start=4088
-  _FILEHEADER_ENVIRONMENT._serialized_end=4160
-  _SCHEMA._serialized_start=4163
-  _SCHEMA._serialized_end=9242
-  _SCHEMA_CONSTANTS._serialized_start=4609
-  _SCHEMA_CONSTANTS._serialized_end=4774
-  _SCHEMA_ARIZECONCLUSIONS._serialized_start=4776
-  _SCHEMA_ARIZECONCLUSIONS._serialized_end=4794
-  _SCHEMA_ARIZEEXPLANATIONS._serialized_start=4796
-  _SCHEMA_ARIZEEXPLANATIONS._serialized_end=4815
-  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_start=4817
-  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_end=4842
-  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_start=4844
-  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_end=4870
-  _SCHEMA_ARROWSCHEMA._serialized_start=4873
-  _SCHEMA_ARROWSCHEMA._serialized_end=6024
-  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_start=5856
-  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_end=5916
-  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_start=5918
-  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_end=6024
-  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_start=6027
-  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_end=6174
-  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_start=6176
-  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_end=6286
-  _SCHEMA_GENERICSCHEMA._serialized_start=6289
-  _SCHEMA_GENERICSCHEMA._serialized_end=8989
-  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_start=7916
-  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_end=7953
-  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_start=7955
-  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_end=8020
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_start=8023
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_end=8465
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_start=8143
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_end=8338
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=8286
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=8338
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=8340
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=8465
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_start=8468
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_end=8989
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_start=8610
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_end=8839
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=8286
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=8338
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=8842
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=8989
-  _SCHEMA_ENVIRONMENT._serialized_start=8991
-  _SCHEMA_ENVIRONMENT._serialized_end=9075
-  _SCHEMA_MODELTYPE._serialized_start=9078
-  _SCHEMA_MODELTYPE._serialized_end=9232
-  _ARROWFILEUPLOADRESPONSE._serialized_start=9244
-  _ARROWFILEUPLOADRESPONSE._serialized_end=9317
-  _USERFILEUPLOADRESPONSE._serialized_start=9319
-  _USERFILEUPLOADRESPONSE._serialized_end=9377
+  _RECORD._serialized_end=972
+  _RECORD_ENVIRONMENTPARAMS._serialized_start=659
+  _RECORD_ENVIRONMENTPARAMS._serialized_end=948
+  _RECORD_ENVIRONMENTPARAMS_TRAINING._serialized_start=877
+  _RECORD_ENVIRONMENTPARAMS_TRAINING._serialized_end=887
+  _RECORD_ENVIRONMENTPARAMS_VALIDATION._serialized_start=889
+  _RECORD_ENVIRONMENTPARAMS_VALIDATION._serialized_end=919
+  _RECORD_ENVIRONMENTPARAMS_PRODUCTION._serialized_start=921
+  _RECORD_ENVIRONMENTPARAMS_PRODUCTION._serialized_end=933
+  _PREPRODUCTIONRECORD._serialized_start=975
+  _PREPRODUCTIONRECORD._serialized_end=1277
+  _PREPRODUCTIONRECORD_VALIDATIONRECORD._serialized_start=1144
+  _PREPRODUCTIONRECORD_VALIDATIONRECORD._serialized_end=1212
+  _PREPRODUCTIONRECORD_TRAININGRECORD._serialized_start=1214
+  _PREPRODUCTIONRECORD_TRAININGRECORD._serialized_end=1262
+  _SCORECATEGORICAL._serialized_start=1280
+  _SCORECATEGORICAL._serialized_end=1670
+  _SCORECATEGORICAL_CATEGORY._serialized_start=1525
+  _SCORECATEGORICAL_CATEGORY._serialized_end=1553
+  _SCORECATEGORICAL_SCOREVALUE._serialized_start=1555
+  _SCORECATEGORICAL_SCOREVALUE._serialized_end=1582
+  _SCORECATEGORICAL_SCORECATEGORY._serialized_start=1584
+  _SCORECATEGORICAL_SCORECATEGORY._serialized_end=1662
+  _OBJECTDETECTION._serialized_start=1673
+  _OBJECTDETECTION._serialized_end=1850
+  _OBJECTDETECTION_BOUNDINGBOX._serialized_start=1753
+  _OBJECTDETECTION_BOUNDINGBOX._serialized_end=1850
+  _RANKINGPREDICTION._serialized_start=1853
+  _RANKINGPREDICTION._serialized_end=1986
+  _RANKINGACTUAL._serialized_start=1988
+  _RANKINGACTUAL._serialized_end=2096
+  _LABEL._serialized_start=2099
+  _LABEL._serialized_end=2229
+  _PREDICTIONLABEL._serialized_start=2232
+  _PREDICTIONLABEL._serialized_end=2471
+  _ACTUALLABEL._serialized_start=2474
+  _ACTUALLABEL._serialized_end=2705
+  _PREDICTION._serialized_start=2708
+  _PREDICTION._serialized_end=3095
+  _PREDICTION_FEATURESENTRY._serialized_start=2973
+  _PREDICTION_FEATURESENTRY._serialized_end=3035
+  _PREDICTION_TAGSENTRY._serialized_start=3037
+  _PREDICTION_TAGSENTRY._serialized_end=3095
+  _VALUE._serialized_start=3098
+  _VALUE._serialized_end=3247
+  _MULTIVALUE._serialized_start=3249
+  _MULTIVALUE._serialized_end=3277
+  _EMBEDDING._serialized_start=3280
+  _EMBEDDING._serialized_end=3517
+  _EMBEDDING_RAWDATA._serialized_start=3406
+  _EMBEDDING_RAWDATA._serialized_end=3481
+  _EMBEDDING_TOKENARRAY._serialized_start=3483
+  _EMBEDDING_TOKENARRAY._serialized_end=3511
+  _ACTUAL._serialized_start=3520
+  _ACTUAL._serialized_end=3752
+  _ACTUAL_TAGSENTRY._serialized_start=3037
+  _ACTUAL_TAGSENTRY._serialized_end=3095
+  _FEATUREIMPORTANCES._serialized_start=3755
+  _FEATUREIMPORTANCES._serialized_end=3985
+  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_start=3928
+  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_end=3985
+  _PREDICTIONANDACTUAL._serialized_start=3987
+  _PREDICTIONANDACTUAL._serialized_end=4080
+  _FILEHEADER._serialized_start=4083
+  _FILEHEADER._serialized_end=4222
+  _FILEHEADER_ENVIRONMENT._serialized_start=4150
+  _FILEHEADER_ENVIRONMENT._serialized_end=4222
+  _SCHEMA._serialized_start=4225
+  _SCHEMA._serialized_end=9304
+  _SCHEMA_CONSTANTS._serialized_start=4671
+  _SCHEMA_CONSTANTS._serialized_end=4836
+  _SCHEMA_ARIZECONCLUSIONS._serialized_start=4838
+  _SCHEMA_ARIZECONCLUSIONS._serialized_end=4856
+  _SCHEMA_ARIZEEXPLANATIONS._serialized_start=4858
+  _SCHEMA_ARIZEEXPLANATIONS._serialized_end=4877
+  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_start=4879
+  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_end=4904
+  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_start=4906
+  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_end=4932
+  _SCHEMA_ARROWSCHEMA._serialized_start=4935
+  _SCHEMA_ARROWSCHEMA._serialized_end=6086
+  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_start=5918
+  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_end=5978
+  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_start=5980
+  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_end=6086
+  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_start=6089
+  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_end=6236
+  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_start=6238
+  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_end=6348
+  _SCHEMA_GENERICSCHEMA._serialized_start=6351
+  _SCHEMA_GENERICSCHEMA._serialized_end=9051
+  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_start=7978
+  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_end=8015
+  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_start=8017
+  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_end=8082
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_start=8085
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_end=8527
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_start=8205
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_end=8400
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=8348
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=8400
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=8402
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=8527
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_start=8530
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_end=9051
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_start=8672
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_end=8901
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=8348
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=8400
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=8904
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=9051
+  _SCHEMA_ENVIRONMENT._serialized_start=9053
+  _SCHEMA_ENVIRONMENT._serialized_end=9137
+  _SCHEMA_MODELTYPE._serialized_start=9140
+  _SCHEMA_MODELTYPE._serialized_end=9294
+  _ARROWFILEUPLOADRESPONSE._serialized_start=9306
+  _ARROWFILEUPLOADRESPONSE._serialized_end=9379
+  _USERFILEUPLOADRESPONSE._serialized_start=9381
+  _USERFILEUPLOADRESPONSE._serialized_end=9439
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arize-7.0.6/arize/utils/constants.py` & `arize-7.1.0/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/logging.py` & `arize-7.1.0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/model_mapping.json` & `arize-7.1.0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/types.py` & `arize-7.1.0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/utils.py` & `arize-7.1.0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize.egg-info/PKG-INFO` & `arize-7.1.0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.6
+Version: 7.1.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.6/arize.egg-info/SOURCES.txt` & `arize-7.1.0/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/setup.cfg` & `arize-7.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/tests/test_api.py` & `arize-7.1.0/tests/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,32 +19,26 @@
     Environments,
     ModelTypes,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
 )
 from arize.utils.utils import get_python_version
-from google.protobuf.wrappers_pb2 import DoubleValue, StringValue
+from google.protobuf.wrappers_pb2 import BoolValue, DoubleValue, StringValue
 
 BOOL_VAL = True
 STR_VAL = "arize"
 INT_VAL = 5
 FLOAT_VAL = 20.20
 NP_FLOAT = float(1.2)
 file_to_open = Path(__file__).parent / "fixtures/mpg.csv"
 
 inputs = {
     "model_id": "model_v0",
     "model_version": "v1.2.3.4",
-    "model_type_numeric": ModelTypes.NUMERIC,
-    "model_type_score_categorical": ModelTypes.SCORE_CATEGORICAL,
-    "model_type_regression": ModelTypes.REGRESSION,
-    "model_type_binary_classification": ModelTypes.BINARY_CLASSIFICATION,
-    "model_type_object_detection": ModelTypes.OBJECT_DETECTION,
-    "model_type_ranking": ModelTypes.RANKING,
     "batch_id": "batch_id",
     "batch": "batch1234",
     "api_key": "API_KEY",
     "prediction_id": "prediction_0",
     "label_bool": BOOL_VAL,
     "label_str": STR_VAL,
     "label_int": INT_VAL,
@@ -97,31 +91,41 @@
     "feature_importances": {
         "feature_str": FLOAT_VAL,
         "feature_double": FLOAT_VAL,
         "feature_int": INT_VAL,
         "feature_bool": BOOL_VAL,
         "feature_numpy_float": NP_FLOAT,
     },
+    "prompt": Embedding(
+        vector=pd.Series([4.0, 5.0, 6.0, 7.0]),
+        data="This is a test prompt",
+    ),
+    "response": Embedding(
+        vector=pd.Series([4.0, 5.0, 6.0, 7.0]),
+        data="This is a test response",
+    ),
 }
 
 
 def _build_expected_record(
     ep: pb2.Record.EnvironmentParams = None,
     p: pb2.PredictionLabel = None,
     a: pb2.ActualLabel = None,
     fi: pb2.FeatureImportances = None,
+    is_generative_llm_record: BoolValue = BoolValue(value=False),
 ) -> pb2.Record:
     return pb2.Record(
         space_key=inputs["space_key"],
         model_id=inputs["model_id"],
         prediction_id=str(inputs["prediction_id"]),
         prediction=p,
         actual=a,
         feature_importances=fi,
         environment_params=ep,
+        is_generative_llm_record=is_generative_llm_record,
     )
 
 
 def _get_proto_environment_params(
     env: Environments,
 ) -> pb2.Record.EnvironmentParams:
     env_params = None
@@ -145,28 +149,42 @@
             model_version=inputs["model_version"],
         )
     elif type == "numeric_float":
         return pb2.Prediction(
             prediction_label=pb2.PredictionLabel(numeric=inputs["label_float"]),
             model_version=inputs["model_version"],
         )
-    elif type == "score_categorical_bool":
+    elif type == "score_categorical_bool" or type == "generative_bool":
         sc = pb2.ScoreCategorical()
         sc.category.category = str(inputs["label_bool"])
         return pb2.Prediction(
             prediction_label=pb2.PredictionLabel(score_categorical=sc),
             model_version=inputs["model_version"],
         )
-    elif type == "score_categorical_str":
+    elif type == "score_categorical_str" or type == "generative_str":
         sc = pb2.ScoreCategorical()
         sc.category.category = inputs["label_str"]
         return pb2.Prediction(
             prediction_label=pb2.PredictionLabel(score_categorical=sc),
             model_version=inputs["model_version"],
         )
+    elif type == "score_categorical_int" or type == "generative_int":
+        sc = pb2.ScoreCategorical()
+        sc.score_value.value = inputs["label_int"]
+        return pb2.Prediction(
+            prediction_label=pb2.PredictionLabel(score_categorical=sc),
+            model_version=inputs["model_version"],
+        )
+    elif type == "score_categorical_float" or type == "generative_float":
+        sc = pb2.ScoreCategorical()
+        sc.score_value.value = inputs["label_float"]
+        return pb2.Prediction(
+            prediction_label=pb2.PredictionLabel(score_categorical=sc),
+            model_version=inputs["model_version"],
+        )
     elif type == "score_categorical_tuple":
         sc = pb2.ScoreCategorical()
         sc.score_category.category = inputs["label_str"]
         sc.score_category.score = inputs["label_float"]
         return pb2.Prediction(
             prediction_label=pb2.PredictionLabel(score_categorical=sc),
             model_version=inputs["model_version"],
@@ -207,26 +225,38 @@
         return pb2.Actual(
             actual_label=pb2.ActualLabel(numeric=inputs["label_int"]),
         )
     elif type == "numeric_float":
         return pb2.Actual(
             actual_label=pb2.ActualLabel(numeric=inputs["label_float"]),
         )
-    elif type == "score_categorical_bool":
+    elif type == "score_categorical_bool" or type == "generative_bool":
         sc = pb2.ScoreCategorical()
         sc.category.category = str(inputs["label_bool"])
         return pb2.Actual(
             actual_label=pb2.ActualLabel(score_categorical=sc),
         )
-    elif type == "score_categorical_str":
+    elif type == "score_categorical_str" or type == "generative_str":
         sc = pb2.ScoreCategorical()
         sc.category.category = inputs["label_str"]
         return pb2.Actual(
             actual_label=pb2.ActualLabel(score_categorical=sc),
         )
+    elif type == "score_categorical_int" or type == "generative_int":
+        sc = pb2.ScoreCategorical()
+        sc.score_value.value = inputs["label_int"]
+        return pb2.Actual(
+            actual_label=pb2.ActualLabel(score_categorical=sc),
+        )
+    elif type == "score_categorical_float" or type == "generative_float":
+        sc = pb2.ScoreCategorical()
+        sc.score_value.value = inputs["label_float"]
+        return pb2.Actual(
+            actual_label=pb2.ActualLabel(score_categorical=sc),
+        )
     elif type == "score_categorical_tuple":
         sc = pb2.ScoreCategorical()
         sc.score_category.category = inputs["label_str"]
         sc.score_category.score = inputs["label_float"]
         return pb2.Actual(
             actual_label=pb2.ActualLabel(score_categorical=sc),
         )
@@ -314,14 +344,44 @@
                 ),
             )
         ),
     }
     return pb2.Prediction(features=embedding_features)
 
 
+def _attach_prompt_and_response_to_prediction() -> pb2.Prediction:
+    input_prompt = inputs["prompt"]
+    input_response = inputs["response"]
+    embedding_features = {
+        "prompt": pb2.Value(
+            embedding=pb2.Embedding(
+                vector=input_prompt.vector,
+                raw_data=pb2.Embedding.RawData(
+                    tokenArray=pb2.Embedding.TokenArray(
+                        tokens=[input_prompt.data],  # List of a single string
+                    )
+                ),
+                link_to_data=StringValue(value=input_prompt.link_to_data),
+            )
+        ),
+        "response": pb2.Value(
+            embedding=pb2.Embedding(
+                vector=input_response.vector,
+                raw_data=pb2.Embedding.RawData(
+                    tokenArray=pb2.Embedding.TokenArray(
+                        tokens=[input_response.data],  # List of a single string
+                    )
+                ),
+                link_to_data=StringValue(value=input_response.link_to_data),
+            )
+        ),
+    }
+    return pb2.Prediction(features=embedding_features)
+
+
 def _attach_tags_to_prediction() -> pb2.Prediction:
     tags = {
         "tag_str": pb2.Value(string=STR_VAL),
         "tag_double": pb2.Value(double=FLOAT_VAL),
         "tag_int": pb2.Value(int=INT_VAL),
         "tag_bool": pb2.Value(string=str(BOOL_VAL)),
     }
@@ -360,15 +420,15 @@
 
 def test_build_pred_and_actual_label_bool():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_score_categorical"],
+        model_type=ModelTypes.SCORE_CATEGORICAL,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_bool"],
         actual_label=inputs["label_bool"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
@@ -392,15 +452,15 @@
 
 def test_build_pred_and_actual_label_str():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_score_categorical"],
+        model_type=ModelTypes.SCORE_CATEGORICAL,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_str"],
         actual_label=inputs["label_str"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
@@ -424,28 +484,28 @@
 
 def test_build_pred_and_actual_label_int():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_int"],
         actual_label=inputs["label_int"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_regression"],
+        model_type=ModelTypes.REGRESSION,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_int"],
         actual_label=inputs["label_int"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
@@ -469,28 +529,28 @@
 
 def test_build_pred_and_actual_label_float():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         actual_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_regression"],
+        model_type=ModelTypes.REGRESSION,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         actual_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
@@ -514,28 +574,28 @@
 
 def test_build_pred_and_actual_label_tuple():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_score_categorical"],
+        model_type=ModelTypes.SCORE_CATEGORICAL,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_tuple"],
         actual_label=inputs["label_tuple"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_binary_classification"],
+        model_type=ModelTypes.BINARY_CLASSIFICATION,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_tuple"],
         actual_label=inputs["label_tuple"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
@@ -569,15 +629,15 @@
         relevance_score=inputs["ranking_relevance_score"],
     )
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_ranking"],
+        model_type=ModelTypes.RANKING,
         prediction_id=inputs["prediction_id"],
         prediction_label=pred_label,
         actual_label=act_label,
         features=inputs["features"],
         tags=inputs["tags"],
     )
 
@@ -606,29 +666,29 @@
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
             prediction_timestamp=wrong_min_time,
-            model_type=inputs["model_type_numeric"],
+            model_type=ModelTypes.NUMERIC,
             prediction_id=inputs["prediction_id"],
             prediction_label=inputs["label_float"],
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert f"prediction_timestamp: {wrong_min_time} is out of range." in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
             prediction_timestamp=wrong_max_time,
-            model_type=inputs["model_type_numeric"],
+            model_type=ModelTypes.NUMERIC,
             prediction_id=inputs["prediction_id"],
             prediction_label=inputs["label_float"],
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert f"prediction_timestamp: {wrong_max_time} is out of range." in str(excinfo.value)
 
@@ -665,15 +725,15 @@
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_ranking"],
+            model_type=ModelTypes.RANKING,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Rank must be between 1 and 100, inclusive. Found 101" in str(excinfo.value)
@@ -693,15 +753,15 @@
     )
 
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_ranking"],
+            model_type=ModelTypes.RANKING,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Prediction Group ID must be a string" in str(excinfo.value)
@@ -714,15 +774,15 @@
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_ranking"],
+            model_type=ModelTypes.RANKING,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Prediction Group ID must have length between 1 and 36. Found 42" in str(excinfo.value)
@@ -741,15 +801,15 @@
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_ranking"],
+            model_type=ModelTypes.RANKING,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Relevance Labels must be not contain empty strings" in str(excinfo.value)
@@ -768,15 +828,15 @@
     )
 
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_ranking"],
+            model_type=ModelTypes.RANKING,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Relevance score must be a float or an int" in str(excinfo.value)
@@ -793,15 +853,15 @@
         categories=inputs["object_detection_categories"],
     )
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_object_detection"],
+        model_type=ModelTypes.OBJECT_DETECTION,
         prediction_id=inputs["prediction_id"],
         prediction_label=pred_label,
         actual_label=act_label,
         features=inputs["features"],
         embedding_features=inputs["object_detection_embedding_feature"],
         tags=inputs["tags"],
     )
@@ -825,15 +885,15 @@
 
 def test_build_prediction_no_embedding_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         features=inputs["features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
@@ -852,15 +912,15 @@
 # Structured features refer to any feature that is not an embedding
 def test_build_prediction_no_structured_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
@@ -878,15 +938,15 @@
 
 def test_build_prediction_no_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
     ep = _get_proto_environment_params(Environments.PRODUCTION)
@@ -902,15 +962,15 @@
 
 def test_build_prediction_no_tags():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
     )
 
     #   Get environment in proto format
@@ -928,15 +988,15 @@
 
 def test_build_prediction_no_tags_no_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
     )
 
     #   Get environment in proto format
     ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
@@ -965,15 +1025,15 @@
 
 
 def test_model_version_optional():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         environment=Environments.PRODUCTION,
-        model_type=inputs["model_type_numeric"],
+        model_type=ModelTypes.NUMERIC,
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
     )
 
     #   Get environment in proto format
     ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
@@ -987,15 +1047,15 @@
 
 def test_missing_environment():
     c = get_stubbed_client()
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            model_type=inputs["model_type_numeric"],
+            model_type=ModelTypes.NUMERIC,
             prediction_id=inputs["prediction_id"],
             prediction_label=inputs["label_str"],
             actual_label=inputs["label_str"],
             features=inputs["features"],
             embedding_features=inputs["embedding_features"],
             tags=inputs["tags"],
         )
@@ -1012,15 +1072,15 @@
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert (
@@ -1038,15 +1098,15 @@
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Each bounding box's coordinates must be a collection of 4 floats." in str(excinfo.value)
@@ -1057,15 +1117,15 @@
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Bounding box's coordinates cannot be negative. Found [-0.1, 0.2, 0.3, 0.4]" in str(
@@ -1076,15 +1136,15 @@
 def test_valid_prediction_id_embeddings():
     c = get_stubbed_client()
 
     # test case - too long prediction_id
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
-            model_type=inputs["model_type_binary_classification"],
+            model_type=ModelTypes.BINARY_CLASSIFICATION,
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
             prediction_id="A" * 129,
             prediction_label=inputs["label_str"],
             actual_label=inputs["label_str"],
             features=inputs["features"],
             embedding_features=inputs["embedding_features"],
@@ -1110,15 +1170,15 @@
             "prediction_label": inputs["label_str"],
         },
     ]
     for case in correct_cases:
         try:
             _ = c.log(
                 model_id=inputs["model_id"],
-                model_type=inputs["model_type_binary_classification"],
+                model_type=ModelTypes.BINARY_CLASSIFICATION,
                 model_version=inputs["model_version"],
                 environment=case["environment"],
                 prediction_id=case["prediction_id"],
                 prediction_label=case["prediction_label"],
                 actual_label=inputs["label_str"],
                 features=inputs["features"],
                 embedding_features=inputs["embedding_features"],
@@ -1164,15 +1224,15 @@
             "err_msg": f"The string length of prediction_id {long_prediction_id} must be between",
         },
     ]
     for case in incorrect_cases:
         with pytest.raises(ValueError) as exc_info:
             _ = c.log(
                 model_id=inputs["model_id"],
-                model_type=inputs["model_type_binary_classification"],
+                model_type=ModelTypes.BINARY_CLASSIFICATION,
                 model_version=inputs["model_version"],
                 environment=case["environment"],
                 prediction_id=case["prediction_id"],
                 prediction_label=case["prediction_label"],
                 actual_label=inputs["label_str"],
                 features=inputs["features"],
                 embedding_features=inputs["embedding_features"],
@@ -1190,15 +1250,15 @@
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Object Detection Label categories must be a list of strings" in str(excinfo.value)
@@ -1213,15 +1273,15 @@
         scores=[-0.4],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Bounding box confidence scores must be between 0 and 1, inclusive" in str(excinfo.value)
@@ -1232,35 +1292,228 @@
         scores=[1.2],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
-            model_type=inputs["model_type_object_detection"],
+            model_type=ModelTypes.OBJECT_DETECTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Bounding box confidence scores must be between 0 and 1, inclusive" in str(excinfo.value)
 
 
+def test_valid_label_type_generative_model():
+    c = get_stubbed_client()
+    # Test allowed label types
+    for label_type in ["str", "bool", "int", "float"]:
+        prediction_label = inputs[f"label_{label_type}"]
+        actual_label = prediction_label
+        record = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.GENERATIVE_LLM,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=prediction_label,
+            actual_label=actual_label,
+            features=inputs["features"],
+            embedding_features=inputs["embedding_features"],
+            tags=inputs["tags"],
+            prompt=inputs["prompt"],
+            response=inputs["response"],
+        )
+        #   Get environment in proto format
+        ep = _get_proto_environment_params(Environments.PRODUCTION)
+        #   Start constructing expected result by building the prediction
+        p = _build_basic_prediction(f"generative_{label_type}")
+        a = _build_basic_actual(f"generative_{label_type}")
+        #   Add props to prediction according to this test
+        p.MergeFrom(_attach_features_to_prediction())
+        p.MergeFrom(_attach_embedding_features_to_prediction())
+        p.MergeFrom(_attach_prompt_and_response_to_prediction())
+        p.MergeFrom(_attach_tags_to_prediction())
+        #   Add props to actual according to this test
+        a.MergeFrom(_attach_tags_to_actual())
+        #   Build expected record using built prediction
+        expected_record = _build_expected_record(
+            p=p, a=a, ep=ep, is_generative_llm_record=BoolValue(value=True)
+        )
+        #   Check result is as expected
+        assert record == expected_record
+
+
+def test_default_prediction_label_generative_model():
+    c = get_stubbed_client()
+    # Test allowed label types
+    record = c.log(
+        model_id=inputs["model_id"],
+        model_version=inputs["model_version"],
+        environment=Environments.PRODUCTION,
+        model_type=ModelTypes.GENERATIVE_LLM,
+        prediction_id=inputs["prediction_id"],
+        actual_label=inputs["label_int"],
+        features=inputs["features"],
+        embedding_features=inputs["embedding_features"],
+        tags=inputs["tags"],
+        prompt=inputs["prompt"],
+        response=inputs["response"],
+    )
+    #   Get environment in proto format
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
+    #   Start constructing expected result by building the prediction
+    # This prediction was not passed to the log call, but should be
+    # created by default for GENERATIVE models
+    sc = pb2.ScoreCategorical()
+    sc.score_value.value = 1
+    p = pb2.Prediction(
+        prediction_label=pb2.PredictionLabel(score_categorical=sc),
+        model_version=inputs["model_version"],
+    )
+    a = _build_basic_actual("generative_int")
+    #   Add props to prediction according to this test
+    p.MergeFrom(_attach_features_to_prediction())
+    p.MergeFrom(_attach_embedding_features_to_prediction())
+    p.MergeFrom(_attach_prompt_and_response_to_prediction())
+    p.MergeFrom(_attach_tags_to_prediction())
+    #   Add props to actual according to this test
+    a.MergeFrom(_attach_tags_to_actual())
+    #   Build expected record using built prediction
+    expected_record = _build_expected_record(
+        p=p, a=a, ep=ep, is_generative_llm_record=BoolValue(value=True)
+    )
+    #   Check result is as expected
+    assert record == expected_record
+
+
+def test_invalid_generative_model():
+    c = get_stubbed_client()
+
+    # Test that GENERATIVE_LLM models must contain prompt and response. Missing prompt
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.GENERATIVE_LLM,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            prompt=inputs["prompt"],
+        )
+    assert "The following fields cannot be None for GENERATIVE_LLM models: prompt, response" in str(
+        excinfo.value
+    )
+    # Test that GENERATIVE_LLM models must contain prompt and response. Missing response
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.GENERATIVE_LLM,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            response=inputs["response"],
+        )
+    assert "The following fields cannot be None for GENERATIVE_LLM models: prompt, response" in str(
+        excinfo.value
+    )
+    # Test that GENERATIVE_LLM models cannot contain embedding named prompt or response
+    with pytest.raises(KeyError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.GENERATIVE_LLM,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            embedding_features={"prompt": inputs["prompt"]},
+            prompt=inputs["prompt"],
+            response=inputs["response"],
+        )
+    assert (
+        "embedding features cannot use the reserved feature names ('prompt', 'response') "
+        "for GENERATIVE_LLM models" in str(excinfo.value)
+    )
+    # Test that prompt and repsonse must be Embedding type for GENERATIVE_LLM models
+    with pytest.raises(TypeError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.GENERATIVE_LLM,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            prompt=2,
+            response=inputs["response"],
+        )
+    assert "Both prompt and response objects must be of type Embedding" in str(excinfo.value)
+
+
+def test_invalid_prompt_response_for_model_type():
+    c = get_stubbed_client()
+
+    # Test that 'prompt' must be None for models other than GENERATIVE_LLM
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.SCORE_CATEGORICAL,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            prompt=inputs["prompt"],
+        )
+    assert (
+        "The fields 'prompt' and 'response' must be None for model types other than GENERATIVE_LLM"
+        in str(excinfo.value)
+    )
+    # Test that 'response' must be None for models other than GENERATIVE_LLM
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            model_type=ModelTypes.SCORE_CATEGORICAL,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=1,
+            features=inputs["features"],
+            tags=inputs["tags"],
+            response=inputs["response"],
+        )
+    assert (
+        "The fields 'prompt' and 'response' must be None for model types other than GENERATIVE_LLM"
+        in str(excinfo.value)
+    )
+
+
 def test_invalid_tags():
     c = get_stubbed_client()
     wrong_tags = {
         "tag_str_incorrect": "a" * (MAX_TAG_LENGTH + 1),
     }
 
     # test case - too long tag value
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
-            model_type=inputs["model_type_binary_classification"],
+            model_type=ModelTypes.BINARY_CLASSIFICATION,
             model_version=inputs["model_version"],
             environment=Environments.PRODUCTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=inputs["label_str"],
             actual_label=inputs["label_str"],
             features=inputs["features"],
             tags=wrong_tags,
```

### Comparing `arize-7.0.6/tests/test_utils.py` & `arize-7.1.0/tests/test_utils.py`

 * *Files identical despite different names*

