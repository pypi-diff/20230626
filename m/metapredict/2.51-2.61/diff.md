# Comparing `tmp/metapredict-2.51.tar.gz` & `tmp/metapredict-2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapredict-2.51.tar", last modified: Thu Mar 16 14:33:31 2023, max compression
+gzip compressed data, was "metapredict-2.61.tar", last modified: Mon Jun 26 19:17:13 2023, max compression
```

## Comparing `metapredict-2.51.tar` & `metapredict-2.61.tar`

### file list

```diff
@@ -1,109 +1,124 @@
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.723037 metapredict-2.51/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2020-09-11 15:11:02.000000 metapredict-2.51/.codecov.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1438 2021-09-07 15:37:07.000000 metapredict-2.51/.gitignore
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2020-09-11 15:11:02.000000 metapredict-2.51/.lgtm.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1110 2020-09-11 15:11:02.000000 metapredict-2.51/.travis.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2020-09-11 15:11:02.000000 metapredict-2.51/CODE_OF_CONDUCT.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1095 2020-09-11 15:11:02.000000 metapredict-2.51/LICENSE
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      118 2020-09-11 15:11:02.000000 metapredict-2.51/MANIFEST.in
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    69815 2023-03-16 14:33:31.723125 metapredict-2.51/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    69489 2023-03-16 13:10:36.000000 metapredict-2.51/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.706439 metapredict-2.51/devtools/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3218 2020-09-11 15:11:02.000000 metapredict-2.51/devtools/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.706664 metapredict-2.51/devtools/conda-envs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      161 2020-09-11 15:11:02.000000 metapredict-2.51/devtools/conda-envs/test_env.yaml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.706866 metapredict-2.51/devtools/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2020-09-11 15:11:02.000000 metapredict-2.51/devtools/scripts/create_conda_env.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.706993 metapredict-2.51/devtools/travis-ci/
--rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1299 2020-09-11 15:11:02.000000 metapredict-2.51/devtools/travis-ci/before_install.sh
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.709149 metapredict-2.51/docs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2021-05-20 21:14:54.000000 metapredict-2.51/docs/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2020-09-11 15:11:02.000000 metapredict-2.51/docs/Makefile
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      588 2020-09-17 15:02:00.000000 metapredict-2.51/docs/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.709358 metapredict-2.51/docs/_static/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2020-09-11 15:11:02.000000 metapredict-2.51/docs/_static/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.709550 metapredict-2.51/docs/_templates/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2020-09-11 15:11:02.000000 metapredict-2.51/docs/_templates/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     7106 2022-08-02 16:56:29.000000 metapredict-2.51/docs/changes.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5532 2020-09-17 16:31:38.000000 metapredict-2.51/docs/conf.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    13996 2022-08-02 16:56:29.000000 metapredict-2.51/docs/getting_started.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      340 2021-09-02 15:10:58.000000 metapredict-2.51/docs/how_to_cite.rst
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.710685 metapredict-2.51/docs/images/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)   101434 2022-02-16 16:25:40.000000 metapredict-2.51/docs/images/confidence_scores_disorder.png
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    52195 2022-02-16 16:24:28.000000 metapredict-2.51/docs/images/meta_predict_disorder.png
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    51024 2022-02-16 16:26:33.000000 metapredict-2.51/docs/images/python_meta_predict_MadeUpProtein.png
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      533 2022-08-02 16:56:29.000000 metapredict-2.51/docs/index.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2020-09-11 15:11:02.000000 metapredict-2.51/docs/make.bat
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      290 2021-09-07 15:29:22.000000 metapredict-2.51/docs/requirements.txt
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.712075 metapredict-2.51/docs/usage/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      937 2022-08-02 16:56:29.000000 metapredict-2.51/docs/usage/acknowledgements.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      514 2022-08-02 16:56:29.000000 metapredict-2.51/docs/usage/api.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    16392 2022-08-02 16:56:29.000000 metapredict-2.51/docs/usage/command-line.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1418 2021-05-20 21:27:02.000000 metapredict-2.51/docs/usage/troubleshooting.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    33015 2022-08-02 16:56:29.000000 metapredict-2.51/docs/usage/using-in-python.rst
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.723514 metapredict-2.51/metapredict/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    10244 2023-01-06 19:07:53.000000 metapredict-2.51/metapredict/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3546 2023-03-16 13:10:36.000000 metapredict-2.51/metapredict/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      497 2023-03-16 14:33:31.723544 metapredict-2.51/metapredict/_version.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.716519 metapredict-2.51/metapredict/backend/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2022-10-20 14:03:01.000000 metapredict-2.51/metapredict/backend/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4493 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/backend/brnn_architecture.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4353 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/backend/data_structures.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    15127 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/backend/domain_definition.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2285 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/backend/encode_sequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    11156 2022-02-24 01:43:42.000000 metapredict-2.51/metapredict/backend/meta_graph.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    11313 2022-02-15 15:47:31.000000 metapredict-2.51/metapredict/backend/meta_predict_disorder.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    10590 2023-03-16 14:24:59.000000 metapredict-2.51/metapredict/backend/meta_tools.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3160 2022-03-09 16:47:29.000000 metapredict-2.51/metapredict/backend/metameta_hybrid_predict.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.717647 metapredict-2.51/metapredict/backend/networks/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2022-03-09 16:49:28.000000 metapredict-2.51/metapredict/backend/networks/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5898 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/backend/networks/metaDisorder.pt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5898 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/backend/networks/meta_predict_disorder_100e_v1.pt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    23626 2022-02-14 15:38:39.000000 metapredict-2.51/metapredict/backend/networks/metameta_2_7_22_nl2_hs20_b32_V3.pt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    29258 2021-09-03 13:48:42.000000 metapredict-2.51/metapredict/backend/networks/metapredict_network_v2_200epochs_nl1_hs20.pt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    69475 2022-02-12 19:24:15.000000 metapredict-2.51/metapredict/backend/networks/metapredict_network_v3_200epochs_nl2_hs20.pt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5164 2022-03-09 16:47:35.000000 metapredict-2.51/metapredict/backend/py_predictor_v2.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5038 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/backend/uniprot_predictions.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.718221 metapredict-2.51/metapredict/data/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      234 2020-09-16 21:57:23.000000 metapredict-2.51/metapredict/data/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3201 2020-09-14 21:25:30.000000 metapredict-2.51/metapredict/data/test_data.fasta
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    62895 2023-03-15 20:20:23.000000 metapredict-2.51/metapredict/meta.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       88 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/metapredict_exceptions.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      153 2022-02-12 19:24:44.000000 metapredict-2.51/metapredict/parameters.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.719941 metapredict-2.51/metapredict/tests/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2021-08-31 18:15:04.000000 metapredict-2.51/metapredict/tests/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      205 2021-08-31 17:51:57.000000 metapredict-2.51/metapredict/tests/__init__.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.720673 metapredict-2.51/metapredict/tests/input_data/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     8687 2021-07-28 21:37:15.000000 metapredict-2.51/metapredict/tests/input_data/DisorderPredictionssp_P04637_P53_HUMANC.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      414 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/tests/input_data/testing.fasta
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1569 2021-05-19 20:12:53.000000 metapredict-2.51/metapredict/tests/input_data/three_seqs.fasta
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    15680 2022-06-07 13:17:14.000000 metapredict-2.51/metapredict/tests/local_data.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.720879 metapredict-2.51/metapredict/tests/output/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    10186 2022-03-03 22:13:25.000000 metapredict-2.51/metapredict/tests/output/test.csv
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2835 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/tests/test_domain_functions.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3085 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/tests/test_graph_disorder.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2021-05-20 19:35:11.000000 metapredict-2.51/metapredict/tests/test_graph_fasta.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     8226 2022-08-02 16:56:29.000000 metapredict-2.51/metapredict/tests/test_metapredict.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3605 2022-02-12 19:24:44.000000 metapredict-2.51/metapredict/tests/test_uniprot_functionality.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      848 2022-02-12 19:24:44.000000 metapredict-2.51/metapredict/tests/test_write_fasta.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.714310 metapredict-2.51/metapredict.egg-info/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    69815 2023-03-16 14:33:31.000000 metapredict-2.51/metapredict.egg-info/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2795 2023-03-16 14:33:31.000000 metapredict-2.51/metapredict.egg-info/SOURCES.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-03-16 14:33:31.000000 metapredict-2.51/metapredict.egg-info/dependency_links.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       82 2023-03-16 14:33:31.000000 metapredict-2.51/metapredict.egg-info/requires.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-03-16 14:33:31.000000 metapredict-2.51/metapredict.egg-info/top_level.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      563 2020-09-17 15:29:03.000000 metapredict-2.51/readthedocs.yml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-03-16 14:33:31.722867 metapredict-2.51/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3225 2022-02-12 19:24:44.000000 metapredict-2.51/scripts/metapredict-graph-disorder
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2410 2021-08-05 17:39:35.000000 metapredict-2.51/scripts/metapredict-graph-pLDDT
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4503 2023-03-16 13:53:40.000000 metapredict-2.51/scripts/metapredict-multipredict
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2877 2022-07-08 17:07:49.000000 metapredict-2.51/scripts/metapredict-name
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1538 2022-02-12 19:24:44.000000 metapredict-2.51/scripts/metapredict-predict-disorder
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4490 2023-03-15 20:54:01.000000 metapredict-2.51/scripts/metapredict-predict-idrs
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1270 2022-08-02 16:56:29.000000 metapredict-2.51/scripts/metapredict-predict-pLDDT
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1429 2022-02-12 19:24:44.000000 metapredict-2.51/scripts/metapredict-quick-graph
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      851 2022-02-12 19:24:44.000000 metapredict-2.51/scripts/metapredict-quick-predict
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2475 2022-08-02 16:56:29.000000 metapredict-2.51/scripts/metapredict-uniprot
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-03-16 14:33:31.723387 metapredict-2.51/setup.cfg
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3059 2023-03-15 20:30:55.000000 metapredict-2.51/setup.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2020-09-11 15:11:02.000000 metapredict-2.51/versioneer.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.607265 metapredict-2.61/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2020-09-11 15:11:02.000000 metapredict-2.61/.codecov.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1597 2023-06-16 17:45:57.000000 metapredict-2.61/.gitignore
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2020-09-11 15:11:02.000000 metapredict-2.61/.lgtm.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1110 2020-09-11 15:11:02.000000 metapredict-2.61/.travis.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2020-09-11 15:11:02.000000 metapredict-2.61/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1095 2020-09-11 15:11:02.000000 metapredict-2.61/LICENSE
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      118 2020-09-11 15:11:02.000000 metapredict-2.61/MANIFEST.in
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5025 2023-06-26 19:17:13.607352 metapredict-2.61/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4736 2023-06-16 17:45:57.000000 metapredict-2.61/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.587343 metapredict-2.61/devtools/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3218 2020-09-11 15:11:02.000000 metapredict-2.61/devtools/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.587699 metapredict-2.61/devtools/conda-envs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      161 2020-09-11 15:11:02.000000 metapredict-2.61/devtools/conda-envs/test_env.yaml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.588449 metapredict-2.61/devtools/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2020-09-11 15:11:02.000000 metapredict-2.61/devtools/scripts/create_conda_env.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.588642 metapredict-2.61/devtools/travis-ci/
+-rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1299 2020-09-11 15:11:02.000000 metapredict-2.61/devtools/travis-ci/before_install.sh
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.590472 metapredict-2.61/docs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2021-05-20 21:14:54.000000 metapredict-2.61/docs/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2020-09-11 15:11:02.000000 metapredict-2.61/docs/Makefile
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      588 2020-09-17 15:02:00.000000 metapredict-2.61/docs/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.590620 metapredict-2.61/docs/_static/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2020-09-11 15:11:02.000000 metapredict-2.61/docs/_static/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.590750 metapredict-2.61/docs/_templates/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2020-09-11 15:11:02.000000 metapredict-2.61/docs/_templates/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      304 2023-06-16 17:45:57.000000 metapredict-2.61/docs/changes.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5497 2023-06-16 17:45:57.000000 metapredict-2.61/docs/conf.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    14055 2023-06-16 17:45:57.000000 metapredict-2.61/docs/getting_started.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      746 2023-06-16 17:45:57.000000 metapredict-2.61/docs/how_to_cite.rst
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.591930 metapredict-2.61/docs/images/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)   101434 2022-02-16 16:25:40.000000 metapredict-2.61/docs/images/confidence_scores_disorder.png
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    52195 2022-02-16 16:24:28.000000 metapredict-2.61/docs/images/meta_predict_disorder.png
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    51024 2022-02-16 16:26:33.000000 metapredict-2.61/docs/images/python_meta_predict_MadeUpProtein.png
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      533 2022-08-02 16:56:29.000000 metapredict-2.61/docs/index.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2020-09-11 15:11:02.000000 metapredict-2.61/docs/make.bat
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      295 2023-06-16 17:45:57.000000 metapredict-2.61/docs/requirements.txt
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.595439 metapredict-2.61/docs/usage/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      937 2022-08-02 16:56:29.000000 metapredict-2.61/docs/usage/acknowledgements.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      514 2022-08-02 16:56:29.000000 metapredict-2.61/docs/usage/api.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    16894 2023-06-16 17:45:57.000000 metapredict-2.61/docs/usage/command-line.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1843 2023-06-16 17:45:57.000000 metapredict-2.61/docs/usage/troubleshooting.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    38721 2023-06-16 17:45:57.000000 metapredict-2.61/docs/usage/using-in-python.rst
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.607831 metapredict-2.61/metapredict/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    10244 2023-05-25 18:01:16.000000 metapredict-2.61/metapredict/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4269 2023-06-22 18:31:09.000000 metapredict-2.61/metapredict/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      497 2023-06-26 19:17:13.607866 metapredict-2.61/metapredict/_version.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.599511 metapredict-2.61/metapredict/backend/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     8196 2023-05-25 18:01:42.000000 metapredict-2.61/metapredict/backend/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    23276 2023-06-26 19:10:11.000000 metapredict-2.61/metapredict/backend/batch_predict.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4493 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/backend/brnn_architecture.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.601341 metapredict-2.61/metapredict/backend/cython/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)  1016478 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict/backend/cython/domain_definition.c
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     8438 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/backend/cython/domain_definition.pyx
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4353 2022-08-02 16:56:29.000000 metapredict-2.61/metapredict/backend/data_structures.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    17238 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/backend/domain_definition.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2285 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/backend/encode_sequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    11156 2022-02-24 01:43:42.000000 metapredict-2.61/metapredict/backend/meta_graph.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    11313 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/backend/meta_predict_disorder.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    11040 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/backend/meta_tools.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3161 2023-05-10 21:49:57.000000 metapredict-2.61/metapredict/backend/metameta_hybrid_predict.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.602388 metapredict-2.61/metapredict/backend/networks/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2022-03-09 16:49:28.000000 metapredict-2.61/metapredict/backend/networks/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5898 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/backend/networks/metaDisorder.pt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5898 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/backend/networks/meta_predict_disorder_100e_v1.pt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    23626 2022-02-14 15:38:39.000000 metapredict-2.61/metapredict/backend/networks/metameta_2_7_22_nl2_hs20_b32_V3.pt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    29258 2021-09-03 13:48:42.000000 metapredict-2.61/metapredict/backend/networks/metapredict_network_v2_200epochs_nl1_hs20.pt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    69475 2022-02-12 19:24:15.000000 metapredict-2.61/metapredict/backend/networks/metapredict_network_v3_200epochs_nl2_hs20.pt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5939 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/backend/py_predictor_v2.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5476 2023-05-10 21:49:57.000000 metapredict-2.61/metapredict/backend/uniprot_predictions.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.603028 metapredict-2.61/metapredict/data/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      234 2020-09-16 21:57:23.000000 metapredict-2.61/metapredict/data/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3201 2020-09-14 21:25:30.000000 metapredict-2.61/metapredict/data/test_data.fasta
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    70790 2023-06-26 19:10:11.000000 metapredict-2.61/metapredict/meta.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       88 2022-08-02 16:56:29.000000 metapredict-2.61/metapredict/metapredict_exceptions.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      153 2022-02-12 19:24:44.000000 metapredict-2.61/metapredict/parameters.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.604537 metapredict-2.61/metapredict/tests/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2021-08-31 18:15:04.000000 metapredict-2.61/metapredict/tests/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      913 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/__init__.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.604891 metapredict-2.61/metapredict/tests/cli_tests/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1137 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/cli_tests/__init__.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.605022 metapredict-2.61/metapredict/tests/cli_tests/input/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1569 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/cli_tests/input/three_seqs.fasta
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     7764 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/cli_tests/test_metapredict-predict-disorder.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     8175 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/cli_tests/test_metapredict-predict-idrs.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.605974 metapredict-2.61/metapredict/tests/input_data/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     8687 2021-07-28 21:37:15.000000 metapredict-2.61/metapredict/tests/input_data/DisorderPredictionssp_P04637_P53_HUMANC.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1257 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/input_data/build_data.ipynb
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)   353405 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/input_data/test_scores_100.npy
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    58261 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/input_data/test_seqs_100.fasta
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      414 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/tests/input_data/testing.fasta
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1569 2021-05-19 20:12:53.000000 metapredict-2.61/metapredict/tests/input_data/three_seqs.fasta
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    15680 2022-06-07 13:17:14.000000 metapredict-2.61/metapredict/tests/local_data.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.606090 metapredict-2.61/metapredict/tests/output/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    10186 2022-03-03 22:13:25.000000 metapredict-2.61/metapredict/tests/output/test.csv
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       34 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/pytest.ini
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5986 2023-06-26 19:10:11.000000 metapredict-2.61/metapredict/tests/test_batch_vs_single.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1398 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/test_cython_v_python.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2835 2022-08-02 16:56:29.000000 metapredict-2.61/metapredict/tests/test_domain_functions.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3085 2022-08-02 16:56:29.000000 metapredict-2.61/metapredict/tests/test_graph_disorder.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2021-05-20 19:35:11.000000 metapredict-2.61/metapredict/tests/test_graph_fasta.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    10008 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/test_metapredict.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3666 2023-06-16 17:45:57.000000 metapredict-2.61/metapredict/tests/test_uniprot_functionality.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      848 2022-02-12 19:24:44.000000 metapredict-2.61/metapredict/tests/test_write_fasta.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.597698 metapredict-2.61/metapredict.egg-info/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5025 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict.egg-info/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3369 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      100 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict.egg-info/requires.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-06-26 19:17:13.000000 metapredict-2.61/metapredict.egg-info/top_level.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      563 2020-09-17 15:29:03.000000 metapredict-2.61/readthedocs.yml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-26 19:17:13.607145 metapredict-2.61/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3225 2022-02-12 19:24:44.000000 metapredict-2.61/scripts/metapredict-graph-disorder
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2410 2021-08-05 17:39:35.000000 metapredict-2.61/scripts/metapredict-graph-pLDDT
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2877 2022-07-08 17:07:49.000000 metapredict-2.61/scripts/metapredict-name
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1538 2022-02-12 19:24:44.000000 metapredict-2.61/scripts/metapredict-predict-disorder
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5708 2023-06-16 17:45:57.000000 metapredict-2.61/scripts/metapredict-predict-idrs
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1270 2022-08-02 16:56:29.000000 metapredict-2.61/scripts/metapredict-predict-pLDDT
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1429 2022-02-12 19:24:44.000000 metapredict-2.61/scripts/metapredict-quick-graph
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      851 2022-02-12 19:24:44.000000 metapredict-2.61/scripts/metapredict-quick-predict
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2475 2022-08-02 16:56:29.000000 metapredict-2.61/scripts/metapredict-uniprot
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-06-26 19:17:13.607684 metapredict-2.61/setup.cfg
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3965 2023-06-26 19:10:11.000000 metapredict-2.61/setup.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2020-09-11 15:11:02.000000 metapredict-2.61/versioneer.py
```

### Comparing `metapredict-2.51/.gitignore` & `metapredict-2.61/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 *$py.class
 
 # C extensions
 *.so
 .DS_Store
 *~
 
+metapredict/tests/test_cli/output/*
+
+# cython-specific stuff
+metapredict/backend/cython/domain_definition.c
+metapredict/backend/cython/domain_definition.html
+
 # other .DS_Store
 metapredict/.DS_Store
 
 # ignore test output
 metapredict/tests/output/*
 
 # ignore built docs
```

### Comparing `metapredict-2.51/.travis.yml` & `metapredict-2.61/.travis.yml`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/CODE_OF_CONDUCT.md` & `metapredict-2.61/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/LICENSE` & `metapredict-2.61/LICENSE`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/devtools/README.md` & `metapredict-2.61/devtools/README.md`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/devtools/scripts/create_conda_env.py` & `metapredict-2.61/devtools/scripts/create_conda_env.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/devtools/travis-ci/before_install.sh` & `metapredict-2.61/devtools/travis-ci/before_install.sh`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/.DS_Store` & `metapredict-2.61/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/Makefile` & `metapredict-2.61/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/README.md` & `metapredict-2.61/docs/README.md`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/conf.py` & `metapredict-2.61/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 
 import metapredict
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'metapredict'
-copyright = ("2020, Ryan Emenecker - Holehouse Lab - WUSM. Project structure based on the "
-             "Computational Molecular Science Python Cookiecutter version 1.3")
-author = 'Ryan Emenecker - Holehouse Lab - WUSM'
+copyright = ("2020-2023, Ryan Emenecker - Holehouse Lab - Washington University School of Medicine.")
+author = 'Ryan Emenecker - Holehouse Lab, Washington University School of Medicine'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
 release = ''
```

### Comparing `metapredict-2.51/docs/getting_started.rst` & `metapredict-2.61/docs/getting_started.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,110 +4,147 @@
 
 What is metapredict?
 ====================
 **metapredict** is a software tool to predict intrinsically disordered regions in protein sequences. It is provided as a downloadable Python tool that includes a Python application programming interface (API) and a set of command-line tools for working with FASTA files. 
 
 Our goal in building **metapredict** was to develop a robust, accurate, and high-performance predictor of intrinsic disorder that is also easy to install and use. As such, **metapredict** is implemented in Python and can be installed directly via `pip` (see below).
 
-**Important update** - as of February 15, 2022 we have updated metapredict to V2. This comes with important changes that improve the accuracy of metapredict. Please see the section on the update *Major update to metapredict predictions to increase overall accuracy* below. In addition, this update changes the functionality of the *predict_disorder_domains()* function, so please read the documentation on that function if you were using it previously. 
+metapredict is ALSO available via a `webserver for single sequence prediction <http://https://metapredict.net>`__ and `a Google Colab notebook for batch prediction <https://colab.research.google.com/github/idptools/metapredict/blob/master/colab/metapredict_colab.ipynb>`__. However, this documentation here focuses on the Python package which provides both a set of Python library functions and a set of command-line tools.
 
-We recently released a `preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ documenting all these changes and more!
 
-As well as providing a set of high-performance software tools, **metapredict** is provided as a stand-alone web server which can predict disorder profiles, scores, and contiguous IDRs for single sequences.
+metapredict updates and news
+===============================
+May 2023: Update to default version (metapredict V2-FF)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-To access the web server go to `metapredict.net <http://metapredict.net/>`_. 
+As of May 2023, we have pushed our improved version metapredict V2-FF. metapredict V2-FF does not change any of the predictions, but does implement substantial performance improvements. Notably these are realized by using the :code:`predict_disorder_batch()` function. 
 
-How does metapredict work?
-===========================
-**metapredict** is a bit different than your typical protein disorder predictor. Instead of predicting the percent chance that a residue within a sequence might be disordered, **metapredict** tries to predict the *consensus disorder* score for the residue. Consensus disorder reports on the fraction of independent disorder predictors that would predict a given residue as disordered.
+February 2022: Update to default version (metapredict V2)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-This already seems complicated...
-----------------------------------
+As of February 15, 2022 we have updated metapredict to V2. This comes with important changes that improve the accuracy of metapredict. Please see the section on the update *Major update to metapredict predictions to increase overall accuracy* below. In addition, this update changes the functionality of the *predict_disorder_domains()* function, so please read the documentation on that function if you were using it previously. 
 
-**metapredict** is a deep-learning-based predictor trained on consensus disorder data from 8 different predictors, as pre-computed and provided by `MobiDB <https://mobidb.bio.unipd.it/>`_. Functionally, this means each residue is assigned a score between 0 and 1 which reflects the confidence we have that the residue is disordered (or not). If the score was 0.5, this means half of the predictors predict that residue to be disordered. In this way, **metapredict** can help you quickly determine the likelihood that residues are disordered by giving you an approximation of what other predictors would predict (things got pretty 'meta' there, hence the name **metapredict**).
+These changes are detailed in a `permanent preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ that lives on bioRxiv. We ask you still cite the original metapredict article rather than this preprint.
 
+July 2021: Initial version (metapredict v1)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+The initial version of metapredict was released in July 2021 with the corresponding paper published shortly thereafter in Biophysical Journal:
 
-Major update to metapredict predictions to increase overall accuracy
-------------------------------------------------------------------------
-We are always working to make metapredict better, and we have recently managed just that. More details will be below, but the short story is that we have made significant improvements in the accuracy of disorder predictions using metapredict. By analyzing our new network using the Disprot-PDB dataset predictions, we found that the MCC (which is a measurement accounting for false positives, false negatives, true positives, and true negatives) for metapredict increased from 0.588 for the old (original) network to 0.7 for our new network. To put this in perspective, our original network was ranked 12th most accurate when analyzing the Disprot-PDB dataset, and by our own estimates V2 is now ranked as the 2nd most accurate available predictor. 
+Emenecker, R. J., Griffith, D. & Holehouse, A. S. Metapredict: a fast, accurate, and easy-to-use predictor of consensus disorder and structure. Biophys. J. 120, 4312–4319 (2021).
 
-For more information on the changes made please see our recent preprint:
 
-Emenecker, R. J., Griffith, D., & Holehouse, A. S. (2022). Metapredict V2: 
-`An update to metapredict, a fast, accurate, and easy-to-use predictor of consensus disorder and structure.  <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ In bioRxiv (p. 2022.06.06.494887). https://doi.org/10.1101/2022.06.06.494887
 
-Any questions, please don't hesitate to reach out!
+Installation
+==============
+The current stable version of **metapredict** is available through GitHub or the Python Package Index (PyPI). 
 
+To install through PyPI, run:
 
-But wait! I need the old metapredict predictions!!!
-====================================================
-No worries! We left users access to the old network. The *default network is now our new, more accurate network*. However, by calling ``-l`` or ``--legacy`` from the command line or by specifying ``legacy=True`` from Python, you will be able to use the original metapredict network. We wanted to keep making metapredict better, but we also wanted to minimize disruptions to anyone currently relying on the original metapredict predictions for whatever reason.
+.. code-block:: bash
 
+	$ pip install metapredict
 
-So... how exactly was this more accurate metapredict network made?
-=========================================================================
-We didn't think it was possible, but metapredict has somehow become *even more meta*. Get ready, because things are about to get a little weird. When we implemented the AlphaFold2 pLDDT prediction feature (see section below), we noticed that there were occasional discrepancies between metapredict and the predicted pLDDT (ppLDDT) scores. When the ppLDDT scores get high enough, it is unlikely that a given region is actually disordered. So, we developed a version of metapredict that we originally called 'metapredict-hybrid' that essentially combined aspects of the ppLDDT scores and the original metapredict scores. We found that this 'hybrid predictor' was **much better** than the original metapredict disorder predictor at predicting disordered regions. **But we didn't stop there.** 
 
-We think one of metapredicts best features is *it is really really fast*. This 'hybrid-predictor' was a little on the slow side, coming in at about 1/3 the speed of the original metapredict predictor. This is still VERY fast, but we thought we could do better. So, we took a little over 300,000 protein sequences and generated metapredict-hybrid scores for those sequences. We then fed those sequences and the corresponding metapredict-hybrid scores and generated a new bidirectional recurrent neural network (BRNN) using PARROT. We then tested this new network against the original metapredict-hybrid predictions and the original metapredict network. The new network that was trained on metapredict-hybrid scores *actually outperformed the metapredict-hybrid predictions when benchmarking against Disprot-PDB*. Importantly, this new (super accurate) network was only 30% slower than the original metapredict network, which is substantially better than the 70% hit that metapredict-hybrid took. 
- 
-**TL;DR** We made the original metapredict predictor using a network trained on consensus scores from MobiDB. We then trained a network on AlphaFold2 pLDDT scores. Next, we made a predictor that combined prediction values from the original metapredict predictor and the AlphaFold2 pLDDT predictor to make very accurate disorder predictions. Finally, we took hundreds of thousands of proteins, generated disorder prediction scores using the aforementioned combination of the original metapredict predictions and the AlphaFold2 predictions, and then trained our final network on those scores. **That's pretty dang meta.**
+You can also install the current development version from
 
+.. code-block:: bash
 
-Generating AlphaFold2 pLDDT scores in metapredict
-======================================================
-In addition, metapredict offers predicted confidence scores from AlphaFold2. These predicted scores use a bidirectional recurrent neural network (BRNN) trained on the per residue pLDDT (predicted IDDT-Ca) confidence scores generated by AlphaFold2 (AF2). The confidence scores (pLDDT) from the proteomes of *Danio rerio*, *Candida albicans*, *Mus musculus*, *Escherichia coli*, *Drosophila melanogaster*, *Methanocaldococcus jannaschii*, *Plasmodium falciparum*, *Mycobacterium tuberculosis*, *Caenorhabditis elegans*, *Dictyostelium discoideum*, *Trypanosoma cruzi*, *Saccharomyces cerevisiae*, *Schizosaccharomyces pombe*, *Rattus norvegicus*, *Homo sapiens*, *Arabidopsis thaliana*, *Zea mays*, *Leishmania infantum*, *Staphylococcus aureus*, *Glycine max*, and *Oryza sativa* were used to generate the BRNN. These confidence scores measure the local confidence that AlphaFold2 has in its predicted structure. The scores go from 0-100 where 0 represents low confidence and 100 represents high confidence. For more information, please see: *Highly accurate protein structure prediction with AlphaFold* https://doi.org/10.1038/s41586-021-03819-2. In describing these scores, the team states that regions with pLDDT scores of less than 50 should not be interpreted except as *possible* disordered regions.
+	$ pip install git+https://git@github.com/idptools/parrot
 
 
-What might the predicted confidence scores from AlphaFold2 be used for?
-========================================================================
-These scores can be used for many applications such as generating a quick preview of which regions of your protein of interest AF2 might be able to predict with high confidence, or which regions of your protein *might* be disordered. AF2 is not (strictly speaking) a disorder predictor, and the confidence scores are not directly representative of protein disorder. Therefore, any conclusions drawn with regards to disorder from predicted AF2 confidence scores should be interpreted with care, but they may be able to provide an additional metric to assess the likelihood that any given protein region may be disordered.
+To clone the GitHub repository and gain the ability to modify a local copy of the code, run
 
+.. code-block:: bash
 
-Why is metapredict useful?
-===========================
-Consensus disorder scores are really useful as they distribute the biases and uncertainty associated with any specific predictor. However, a drawback of consensus disorder databases (like MobiDB) is that they can only give you values of *previously predicted protein sequences*. **metapredict** provides a way around this, allowing arbitrary sequences to be analyzed! 
+	$ git clone https://github.com/idptools/metapredict.git
+	$ cd metapredict
+	$ pip install -e .
+	
+Note you will need the -e flag to ensure the `cython` code compiles correctly, but this also means the installed version is linked to the local version of the code.	
 
-The major advantages that **metapredict** offers over existing predictors is performance, ease of use, and ease of installation. Given **metapredict** uses a pre-trained bidirectional recurrent neural network, on hardware we've tested **metapredict** gives ~10,000 residues per second prediction power. This means that predicting disorder across entire proteomes is accessible in minutes - for example it takes ~20 minutes to predict disorder for every human protein in the reviewed human proteome (~23000 sequences). We provide **metapredict** as a simple-to-use Python library to integrate into existing Python workflows, and as a set of command-line tools for the stand-alone prediction of data from direct input or from FASTA files.
+This will install **metapredict** locally. If you modify the source code in the local repository, be sure to re-install with `pip`.
 
 
-How to cite metapredict
-===========================
+About
+======
+It's important to understand how tools were built and developed. Below we provide a quick overview of how metapredict works and was trained.
+
+How does metapredict work?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+**metapredict V2** (the current default version) works by combining consensus disorder predictions (which is how V1 was developed) with structural predictions to assign a residue as being disordered or folded. 
+
+The original metapredict (V1) was purely a consensus disorder predictor.  Instead of predicting the percent chance that a residue within a sequence might be disordered, **metapredict** tries to predict the *consensus disorder* score for the residue. Consensus disorder reports on the fraction of independent disorder predictors that would predict a given residue as disordered.
+
+As of metapredict V2 (including V2-FF) the overall disorder prediction combines the V1 consensus disorder score with inverted AlphaFold2 predictions in a single deep learning network that provides robust, accurate, and fast assignment of individual residues as being either disordered or folded.
+
+How was metapredict V1 trained?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**metapredict V1** is a deep-learning-based predictor trained on consensus disorder data from 8 different predictors, as pre-computed and provided by `MobiDB <https://mobidb.bio.unipd.it/>`_. Functionally, this means each residue is assigned a score between 0 and 1 which reflects the confidence we have that the residue is disordered (or not). If the score was 0.5, this means half of the predictors predict that residue to be disordered. In this way, **metapredict V1** can determine the likelihood that residues are disordered by giving you an approximation of what other predictors would predict (things got pretty 'meta' there, hence the name **metapredict**).
+
+Note that metapredict V1 predictions are available via the :code:`legacy=True` flag.
 
-If you use metapredict for your work, please cite the metapredict paper - 
+
+How was metapredict V2 trained?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+V2 was trained by generating an initial hybrid score that combined AlphaFold2 predicted pLDDT scores with consensus disorder along with some signal process algorithms to make a new structure/disorder consensus prediction. Finally, we trained a new deep learning network to predict our hybrid network (meta meta), substantially improving accuracy with very little loss in performance.
+
+These changes and new assessment of performance are available in our preprint: `An update to metapredict, a fast, accurate, and easy-to-use predictor of consensus disorder and structure.  <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ In bioRxiv (p. 2022.06.06.494887). https://doi.org/10.1101/2022.06.06.494887
  
-Emenecker RJ, Griffith D, Holehouse AS, metapredict: a fast, accurate, and easy-to-use predictor of consensus disorder and structure, Biophysical Journal (2021), doi: https:// doi.org/10.1016/j.bpj.2021.08.039.
 
-Additionally, if you are using V2 (which is now the default) please make this clear in methods section. You should not feel obliged to cite the `V2 preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_, and this pre-print exists soley so we could fully document the changes and test some edge cases in an accessible and clear way.
+As per the 2023 Critical Assessment of Intrinsic Disorder (CAID) competition, metapredict V2 is ranked the 9th most accurate disorder predictor available. However, importantly, it is among the fastest regardless of accuracy, and is accessible across multiple platforms, via a web server, and with very few software dependencies. Among the top 10, the difference in accuracy is 0.95 to 0.93 AUC, suggesting to us that all top 10 predictors are highly accurate. In short, we believe metapredict V2 hits a sweet spot of accuracy and performance.
 
+How does metapredict V2 differ from V2-FF
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Installation
-==============
-**metapredict** is available through GitHub or the Python Package Index (PyPI). To install through PyPI, run
+metapredict V2 and V2-FF are identical in terms of predictions and features, with the major difference being that metapredict V2-FF offers batched predictions. Batched predictions are automatically parallelized on either the CPU or GPU. In addition, we rewrote the metapredict domain decomposition algorithm in C to provide a 10-20x improvement in performance for this step.
 
-.. code-block:: bash
+We note that V2-FF was released after CAID, so the performance reported there is the V2 network performance. Because metapredict V2-FF is implemented in a `Google Colab notebook for batch prediction <https://colab.research.google.com/github/idptools/metapredict/blob/master/colab/metapredict_colab.ipynb>`__ you don't have to take our word for it that it's fast; just upload a proteome and see for yourself! 
 
-	$ pip install metapredict
 
-To clone the GitHub repository and gain the ability to modify a local copy of the code, run
+Generating predicted pLDDT (AlphaFold2 confidence) scores in metapredict
+-----------------------------------------------------------------------------
+In addition to predicting disorder scores, metapredict offers predicted confidence scores from AlphaFold2. These predicted scores use a bidirectional recurrent neural network (BRNN) trained on the per residue pLDDT (predicted IDDT-Ca) confidence scores generated by AlphaFold2 (AF2). The confidence scores (pLDDT) from the proteomes of *Danio rerio*, *Candida albicans*, *Mus musculus*, *Escherichia coli*, *Drosophila melanogaster*, *Methanocaldococcus jannaschii*, *Plasmodium falciparum*, *Mycobacterium tuberculosis*, *Caenorhabditis elegans*, *Dictyostelium discoideum*, *Trypanosoma cruzi*, *Saccharomyces cerevisiae*, *Schizosaccharomyces pombe*, *Rattus norvegicus*, *Homo sapiens*, *Arabidopsis thaliana*, *Zea mays*, *Leishmania infantum*, *Staphylococcus aureus*, *Glycine max*, and *Oryza sativa* were used to generate the BRNN. These confidence scores measure the local confidence that AlphaFold2 has in its predicted structure. The scores go from 0-100 where 0 represents low confidence and 100 represents high confidence. For more information, please see: *Highly accurate protein structure prediction with AlphaFold* https://doi.org/10.1038/s41586-021-03819-2. In describing these scores, the team states that regions with pLDDT scores of less than 50 should not be interpreted except as *possible* disordered regions.
 
-.. code-block:: bash
 
-	$ git clone https://github.com/idptools/metapredict.git
-	$ cd metapredict
-	$ pip install .
+What might the predicted confidence scores from AlphaFold2 be used for?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+These scores can be used for many applications such as generating a quick preview of which regions of your protein of interest AF2 might be able to predict with high confidence, or which regions of your protein *might* be disordered. 
+
+AF2 is not (strictly speaking) a disorder predictor, and the confidence scores are not directly representative of protein disorder. Therefore, any conclusions drawn with regards to disorder from predicted AF2 confidence scores should be interpreted with care, but they may be able to provide an additional metric to assess the likelihood that any given protein region may be disordered.
+
+
+Why is metapredict useful?
+===========================
+We think **metapredict** is useful for three main reasons.
+
+1. It's highly accurate, provide strong boundaries between disordered and folded regions.
+2. It's incredibly fast; on CPUs one can predict every IDR in the human proteome in ~5 minutes. On modest GPUs one can predict every IDR in the human proteome in 40 seconds. This stands in stark contrast to other predictors which place length caps on sequences and can take hours per sequence.
+3. It is easy to use and distributed via a wide range of channels. In addition to this Python package, metapredict is distributed as a stand-alone webserver, colab notebooks for large-scale predictions, and as an `API for SHEPHARD <https://shephard.readthedocs.io/en/latest/apis.html#metapredict>`__, our general-purpose toolkit for working with an annotating large protein datasets. This Python package further implements metapredict as both Python modules and as a set of command-line tools. 
+
+In summary, we believe metapredict provides the three key ingredients of a useful disorder predictor: it's extremely accurate, it's incredibly fast, and it's very easy to use.
+
+How to cite
+===========================
+
+If you use metapredict for your work, please cite the metapredict paper 
+
+Emenecker, R. J., Griffith, D. & Holehouse, A. S. Metapredict: a fast, accurate, and easy-to-use predictor of consensus disorder and structure. Biophys. J. 120, 4312–4319 (2021).
+	
+Additionally, if you are using V2 (which is now the default) please make this clear in methods section. You should not feel obliged to cite the `V2 preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_, and this pre-print exists solely so we could fully document the changes and test some edge cases in an accessible and clear way.
+
 
-This will install **metapredict** locally. If you modify the source code in the local repository, be sure to re-install with `pip`.
 
-Known installation/execution issues
+Known installation issues
 ====================================
 
 Below we include documentation on known issues. 
 
 macOS libiomp clash 
-=======================
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 PyTorch currently ships with its own version of the OpenMP library (``libiomp.dylib``). Unfortunately when numpy is installed from ``conda`` (although not from ``pip``) this leads to a collision because the ``conda``-derived numpy library also includes a local copy of the ``libiomp5.dylib`` library. This leads to the following error message (included here for google-ability).
 
 .. code-block:: none 
 
    OMP: Error #15: Initializing libiomp5.dylib, but found libomp.dylib already initialized.
    OMP: Hint This means that multiple copies of the OpenMP runtime have been linked into the program.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metapredict-2.51/docs/images/confidence_scores_disorder.png` & `metapredict-2.61/docs/images/confidence_scores_disorder.png`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/images/meta_predict_disorder.png` & `metapredict-2.61/docs/images/meta_predict_disorder.png`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/images/python_meta_predict_MadeUpProtein.png` & `metapredict-2.61/docs/images/python_meta_predict_MadeUpProtein.png`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/index.rst` & `metapredict-2.61/docs/index.rst`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/make.bat` & `metapredict-2.61/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/usage/acknowledgements.rst` & `metapredict-2.61/docs/usage/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/usage/api.rst` & `metapredict-2.61/docs/usage/api.rst`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/docs/usage/command-line.rst` & `metapredict-2.61/docs/usage/command-line.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 Using the original metapredict network
 ---------------------------------------
 
 We have recently updated the network that makes predictions for metapredict to massively improve accuracy. However, if you need to use the original metapredict predictor as opposed to our new, updated predictor, use the ``-l`` or ``--legacy`` flag!
 
 
-Predicting Disorder from Fasta Files
----------------------------------------
+Predicting disorder scores from fasta files
+--------------------------------------------
 
 The ``metapredict-predict-disorder`` command from the command line takes a .fasta file as input and returns disorder scores for the sequences in the FASTA file.
 
 Once metapredict is installed, the user can run ``metapredict-predict-disorder`` from the command line:
 
 .. code-block:: bash
 	
 	$ metapredict-predict-disorder <Path to .fasta file> 
 
 **Example:** 
 
 .. code-block:: bash
 	
 	$ metapredict-predict-disorder /Users/thisUser/Desktop/interestingProteins.fasta 
-
+	
+	
+Note that as of metapredict V2-FF this will automatically parallelize on a GPU or CPU if available. A progress bar will also be generated in the terminal.	
 
 **Additional Usage:**
 
 **Specifying where to save the output -** 
 If you would like to specify where to save the output, simply use the ``-o`` or ``--output-file`` flag and then specify the file path and file name. By default this command will save the output file as disorder_scores.csv to your current working directory. However, you can specify the file name in the output path.
 
 **Example:** 
@@ -43,16 +45,64 @@
 
 **Example:** 
 
 .. code-block:: bash
     
     $ metapredict-predict-disorder /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_disorder_predictions.csv -l
 
-Predicting Disorder from a Sequence
-------------------------------------
+
+Predicting IDRs from a fasta file
+----------------------------------------
+
+The ``metapredict-predict-idrs`` command from the command line takes a .fasta file as input and returns a .fasta file containing the IDRs for every sequence from the input .fasta file. 
+
+.. code-block:: bash
+
+	$ metapredict-predict-idrs <Path to .fasta file> 
+
+**Example**
+
+.. code-block:: bash
+	
+	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta 
+
+Note that as of metapredict V2-FF this will automatically parallelize on a GPU or CPU if available. A progress bar will also be generated in the terminal.
+
+**Additional Usage**
+
+**specifying where to save the output -** 
+If you would like to specify where to save the output, simply use the ``-o`` or ``--output-file`` flag and then specify the file path and file name.
+
+**Example**
+
+.. code-block:: bash
+	
+	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta
+
+**Using the original metapredict predictor**
+To use the original metapredict predictor as opposed to our new, updated predictor, use the ``-l`` or ``--legacy`` flag! Note that if legacy mode is requested no parallelization is possible.
+
+**Example**
+
+.. code-block:: bash
+	
+	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta -l
+
+**Changing output threshold for disorder-**
+To change the cutoff value for something to be considered disordered, simply use the ``--threshold`` flag and then specify your value. For legacy, the default is 0.42. For the new version of metapredict, the value is 0.5. 
+
+**Example**
+
+.. code-block:: bash
+	
+	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta --threshold 0.3
+
+
+Predicting disorder scores from sequence
+------------------------------------------
 
 ``metapredict-quick-predict`` is a command that will let you input a sequence and get disorder values immediately printed to the terminal. The only argument that can be input is the sequence.
 
 **Example:**
 
 .. code-block:: bash
 	
@@ -65,15 +115,15 @@
 **Example:** 
 
 .. code-block:: bash
     
     $ metapredict-quick-predict ISQQMQAQPAMVKSQQQQQQQQQQHQHQQQQLQQQQQLQMSQQQVQQQGIYNNGTIAVA -l
 
 
-Predicting AlphaFold2 Confidence Scores from a Fasta File
+Predicting AlphaFold2 confidence scores from a fasta file
 ------------------------------------------------------------
 
 The ``metapredict-predict-pLDDT`` command from the command line takes a .fasta file as input and returns predicted AlphaFold2 pLDDT confidence scores for the sequences in the FASTA file.
 
 .. code-block:: bash
 	
 	$ metapredict-predict-pLDDT <Path to .fasta file>
@@ -93,16 +143,16 @@
 
 .. code-block:: bash
 	
 	$ metapredict-predict-pLDDT /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_pLDDT_predictions.csv
 
 
 
-Graphing Disorder from a Fasta file
-------------------------------------
+Plotting disorder profiles from a fasta file
+-----------------------------------------------
 
 The ``metapredict-graph-disorder`` command from the command line takes a .fasta file as input and returns a graph for every sequence within the .fasta file. **Warning** This will return a graph for every sequence in the FASTA file.  
 
 .. code-block:: bash
 
     $ metapredict-graph-disorder <Path to .fasta file> 
 
@@ -182,16 +232,16 @@
 
 .. code-block:: bash
     
     $ metapredict-graph-disorder /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/DisorderGraphsFolder/ --disorder-threshold 0.5 -l
 
 
 
-Quick Graphing
----------------
+Quick graphing of disorder scores
+-------------------------------------
 
 ``metapredict-quick-graph`` is a command that will let you input a sequence and get a plot of the disorder back immediately. You cannot input fasta files for this command. The command only takes three arguments, 1. the sequence 2. *optional* DPI ``-D``  or ``--dpi`` of the output graph which defaults to 150 DPI, and 3. *optional* to include predicted AlphaFold2 confidence scores, use the ``p`` or ``--pLDDT`` flag.
 
 **Example:**
 
 .. code-block:: bash
 	
@@ -215,18 +265,18 @@
 **Example:** 
 
 .. code-block:: bash
     
     $ metapredict-quick-graph ISQQMQAQPAMVKSQQQQQQQQQQHQHQQQQLQQQQQLQMSQQQVQQQGIYNNGTIAVAN -l
 
 
-Graphing using Uniprot ID
---------------------------
+Graphing disorder scores using UniProt ID
+---------------------------------------------
 
-``metapredict-uniprot`` is a command that will let you input any Uniprot ID and get a plot of the disorder for the corresponding protein. The default behavior is to have a plot automatically appear. Apart from the Uniprot ID which is required for this command, the command has four possible additional *optional* arguments, 1. To include predicted AlphaFold2 pLDDT confidence scores, use the ``-p``  or ``--pLDDT`` flag. DPI can be changed with the ``-D``  or ``--dpi`` flags, default is 150 DPI, 3. Using ``-o``  or ``--output-file`` will save the plot to a specified directory (default is current directory) - filenames and file extensions (pdf, jpg, png, etc) can be specified here. If there is no file name specified, it will save as the Uniprot ID and as a .png, 4. ``-t``  or ``--title`` will let you specify the title of the plot. By default the title will be *Disorder for* followed by the Uniprot ID.
+``metapredict-uniprot`` is a command that will let you input any UniProt ID and get a plot of the disorder for the corresponding protein. The default behavior is to have a plot automatically appear. Apart from the UniProt ID which is required for this command, the command has four possible additional *optional* arguments, 1. To include predicted AlphaFold2 pLDDT confidence scores, use the ``-p``  or ``--pLDDT`` flag. DPI can be changed with the ``-D``  or ``--dpi`` flags, default is 150 DPI, 3. Using ``-o``  or ``--output-file`` will save the plot to a specified directory (default is current directory) - filenames and file extensions (pdf, jpg, png, etc) can be specified here. If there is no file name specified, it will save as the UniProt ID and as a .png, 4. ``-t``  or ``--title`` will let you specify the title of the plot. By default the title will be *Disorder for* followed by the UniProt ID.
 
 **Example:**
 
 .. code-block:: bash
 	
 	$ metapredict-uniprot Q8RYC8
 
@@ -270,23 +320,23 @@
     
     $ metapredict-uniprot Q8RYC8 -l
 
 
 Graphing disorder using the common name of a protein
 -----------------------------------------------------
 
-Sometimes you just don't know the Uniprot ID for your favorite protein, and looking it up can be a pain. With the ``metapredict-name`` command, you can input the common name of your favorite protein and get a graph in return. Metapredict will also print the name of the organisms and the uniprot ID it found so you know you're looking at the correct protein. This is because this functionality queries your input protein name on Uniprot and takes the top hit. Sometimes this is the protein you're looking for, but not always. To increase the likelihood of success, use your protein name and the organism name for this command.
+Sometimes you just don't know the UniProt ID for your favorite protein, and looking it up can be a pain. With the ``metapredict-name`` command, you can input the common name of your favorite protein and get a graph in return. Metapredict will also print the name of the organisms and the UniProt ID it found so you know you're looking at the correct protein. This is because this functionality queries your input protein name on UniProt and takes the top hit. Sometimes this is the protein you're looking for, but not always. To increase the likelihood of success, use your protein name and the organism name for this command.
 
 *Example*
 
 .. code-block:: bash
     
     $ metapredict-name p53 
 
-will graph the metapredict disorder scores for the Homo sapiens p53 protein. This is because Homo sapiens p53 is the top hit on Uniprot when you search p53. However...
+will graph the metapredict disorder scores for the Homo sapiens p53 protein. This is because Homo sapiens p53 is the top hit on UniProt when you search p53. However...
 
 .. code-block:: bash
     
     $ metapredict-name p53 chicken
 
 will graph the p53 from Gallus gallus!
 
@@ -332,38 +382,38 @@
 **Example**
 
 .. code-block:: bash
     
     $ metapredict-name p53 -l
 
 
-**Printing the full Uniprot ID to your terminal**
+**Printing the full UniProt ID to your terminal**
 
-To have your terminal print the entire Uniprot ID as well as the full protein sequence from your specified protein upon graphing, use the ``-v`` or ``--verbose`` flag.
+To have your terminal print the entire UniProt ID as well as the full protein sequence from your specified protein upon graphing, use the ``-v`` or ``--verbose`` flag.
 
 **Example**
 
 .. code-block:: bash
     
     $ metapredict-name p53 -v
 
 
 **Turning off all printing to the terminal**
 
-By default, the *metapredict-name* command prints the uniprot ID as well as other information related to your protein to the terminal. The purpose of this is to make it explicitly clear which protein was graphed because grabbing the top hit from Uniprot *does not guarantee* that it is the protein you want or expected. However, this behavior can be turned off by using the ``-s`` or ``--silent`` flag.
+By default, the *metapredict-name* command prints the UniProt ID as well as other information related to your protein to the terminal. The purpose of this is to make it explicitly clear which protein was graphed because grabbing the top hit from UniProt *does not guarantee* that it is the protein you want or expected. However, this behavior can be turned off by using the ``-s`` or ``--silent`` flag.
 
 **Example**
 
 .. code-block:: bash
     
     $ metapredict-name p53 -s
 
 
 
-Graphing Predicted AlphaFold2 pLDDT Scores from a fasta file
+Graphing predicted AlphaFold2 pLDDT scores from a fasta file
 -------------------------------------------------------------------
 
 The ``metapredict-graph-pLDDT`` command from the command line takes a .fasta file as input and returns a graph of the predicted AlphaFold2 pLDDT confidence score for every sequence within the .fasta file. **Warning** This will return a graph for every sequence in the FASTA file. 
 
 .. code-block:: bash
 	
 	$ metapredict-graph-pLDDT <Path to .fasta file> 
@@ -413,49 +463,8 @@
 **Example**
 
 .. code-block:: bash
 	
 	$ metapredict-graph-pLDDT /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/pLDDTGraphsFolder/ --indexed-filenames
 
 
-Predicting IDRs from a fasta file
--------------------------------------------------------------------
-
-The ``metapredict-predict-idrs`` command from the command line takes a .fasta file as input and returns a .fasta file containing the IDRs for every sequence from the input .fasta file. 
-
-	$ metapredict-predict-idrs <Path to .fasta file> 
-
-**Example**
-
-.. code-block:: bash
-	
-	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta 
-
-**Additional Usage**
-
-**specifying where to save the output -** 
-If you would like to specify where to save the output, simply use the ``-o`` or ``--output-file`` flag and then specify the file path and file name.
-
-**Example**
-
-.. code-block:: bash
-	
-	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta
-
-**Using the original metapredict predictor**
-To use the original metapredict predictor as opposed to our new, updated predictor, use the ``-l`` or ``--legacy`` flag!
-
-**Example**
-
-.. code-block:: bash
-	
-	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta -l
-
-**Changing output threshold for disorder-**
-To change the cutoff value for something to be considered disordered, simply use the ``--threshold`` flag and then specify your value. For legacy, the default is 0.42. For the new version of metapredict, the value is 0.5. 
-
-**Example**
-
-.. code-block:: bash
-	
-	$ metapredict-predict-idrs /Users/thisUser/Desktop/interestingProteins.fasta -o /Users/thisUser/Desktop/disorder_predictions/my_idrs.fasta --threshold 0.3
```

### Comparing `metapredict-2.51/docs/usage/using-in-python.rst` & `metapredict-2.61/docs/usage/using-in-python.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,47 @@
-
 metapredict in Python
-=====================
+=======================
 
 In addition to using metapredict from the command line, you can also use it directly in Python. This enables metapredict to be incorporated into your bioinformatic workflows with ease
 
 First import metapredict:
 
 .. code-block:: python
 
 	import metapredict as meta
 
 Once metapredict is imported, you can work with individual sequences or .fasta files. :doc:`For a list of all metapredict's public-facing functions and their documentation click here  <api>`
 
-Important update to predict_disorder_domains() function for V2.0 and above
-------------------------------------------------------------------------------
+Important updates
+---------------------
+
+Update to metapredict V2-FF (May 2023)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+In May 2023 the default version of metapredict updated to be V2-FF. V2-FF introduces one primary difference from the user's perspective; disorder scores and disordered domains can now be predicted in parallel batches using:
+
+.. code-block:: python
+	
+	import metapredict as meta
+	
+	# batch disorder in batch
+	meta.predict_disorder_batch(...) 
+		
+If GPU are available, batch prediction will automatically use GPUs. If not, batch prediction will distribute predictions across the CPUs. While all the original functionality is preserved, :code:`predict_disorder_batch()`, offers a 5-10x speedup on CPUs and 30-40x speedup on GPUs.  
+
+:code:`predict_disorder_batch()` can take in a list of sequences or a dictionary of sequences, and returns a list or dictionary that maps input index back to a two-position list of sequence and disorder scores or, if :code:`return_disorder_domains` is set to True, a list of :code:`DisorderDomain` objects.
+
+This functionality is described in detail in the function documentation under the Python Module Documentation entry for :code:`predict_disorder_batch()`.
 
-As of February 15, 2022 we have updated metapredict to V2. V2 provides a major improvement in accuracy and interpretability, and works by incorporating in predictions made from AlphaFold2  to provide a new underlying prediction network. The original metapredict network is still available using the ``legacy=True`` flag. For more information, please see the section on the update *Major update to metapredict predictions to increase overall accuracy* below. In addition, this update changes the functionality of the ``predict_disorder_domains()`` function, so please read the documentation on that function if you were using it previously! 
 
-We recently released a `preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ documenting all these changes and more!
+Update to metapredict V2 (Feb 2022)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+As of February 15, 2022 we have updated metapredict to V2. V2 provides a major improvement in accuracy and interpretability and works by incorporating in predictions made from AlphaFold2  to provide a new underlying prediction network. The original metapredict network is still available using the ``legacy=True`` flag. For more information, please see the section on the update *Major update to metapredict predictions to increase overall accuracy* below. In addition, this update changes the functionality of the ``predict_disorder_domains()`` function, so please read the documentation on that function if you were using it previously! 
+
+We released a `preprint <https://www.biorxiv.org/content/10.1101/2022.06.06.494887v2>`_ documenting all these changes and more!
 
 
 Predicting Disorder
 --------------------
 
 The ``predict_disorder()`` function will return a list of predicted disorder consensus values for the residues of the input sequence. The input sequence should be a string made of valid amino acids. Running -
 
@@ -210,15 +230,15 @@
 **Example**
 
 .. code-block:: python
 
 	meta.predict_disorder_domains("MKAPSNGFLPSSNEGEKKPINSQLWHACAGPLV", minimum_IDR_size = 10)
 
 **Altering the minimum folded domain size -**
-The minimum folded domain size defines where we expect the limit of small folded domains to be. *NOTE* this is not a hard limit and functions more to modulate the removal of large gaps. In other words, gaps less than this size are treated less strictly. *Note* that, in addition, gaps < 35 are evaluated with a threshold of 0.35 x ``disorder_threshold`` and gaps < 20 are evaluated with a threshold of 0.25 x disorder_threshold. These two lengthscales were decided based on the fact that coiled-coiled regions (which are IDRs in isolation) often show up with reduced apparent disorder within IDRs but can be as short as 20-30 residues. The folded_domain_threshold is used based on the idea that it allows a 'shortest reasonable' folded domain to be identified. Default=50.
+The minimum folded domain size defines where we expect the limit of small folded domains to be. *NOTE* this is not a hard limit and functions more to modulate the removal of large gaps. In other words, gaps less than this size are treated less strictly. *Note* that, in addition, gaps < 35 are evaluated with a threshold of 0.35 x ``disorder_threshold`` and gaps < 20 are evaluated with a threshold of 0.25 x disorder_threshold. These two length-scales were decided based on the fact that coiled-coiled regions (which are IDRs in isolation) often show up with reduced apparent disorder within IDRs but can be as short as 20-30 residues. The folded_domain_threshold is used based on the idea that it allows a 'shortest reasonable' folded domain to be identified. Default=50.
 
 **Example**
 
 .. code-block:: python
 
 	meta.predict_disorder_domains("MKAPSNGFLPSSNEGEKKPINSQLWHACAGPLV", minimum_folded_domain = 60)
 
@@ -259,15 +279,15 @@
 
 	58.537
 
 ``Percent_disorder()`` has two modes defined by the ``mode`` keyword: ``threshold`` and ``disorder_domains``. 
 
 The default usage is with the ``threshold`` mode. In this case, each residue is evaluated against a threshold value, where disorder scores above that threshold count towards disordered residues. This mode uses a threshold value of 0.5 (for V2) or 0.3 (for legacy), although the threshold can be changed (see below).
 
-The alternative mode, ``disorder_domains``, makes use of metapredictis ``predict_disorder_domains()`` functionality. Now, the sequence is divided up into IDRs and folded domains, and then the percentage disordered is based on what fraction of residues fall into IDRs. The underlying disorder domain prediction uses the default disorder thresholds as per the  ``predict_disorder_domains()` function, but this can be over-ridden if a ``disorder_threshold`` keyword is passed. For example:
+The alternative mode, ``disorder_domains``, makes use of metapredict's ``predict_disorder_domains()`` functionality. Now, the sequence is divided up into IDRs and folded domains, and then the percentage disordered is based on what fraction of residues fall into IDRs. The underlying disorder domain prediction uses the default disorder thresholds as per the  ``predict_disorder_domains()` function, but this can be over-ridden if a ``disorder_threshold`` keyword is passed. For example:
 
 .. code-block:: python
 
 	meta.percent_disorder("DSSPEAPAEPPKDVPHDWLPYSYVFGLGTPHGHPPADFGLR", mode='disorder_domains')
 
 would output - 
 
@@ -494,15 +514,15 @@
 
 	meta.predict_pLDDT_fasta("/Users/thisUser/Desktop/coolSequences.fasta")
 
 
 Predict Disorder Using Uniprot ID
 -----------------------------------
 
-By using the ``predict_disorder_uniprot()`` function, you can return predicted consensus disorder values for the amino acid sequence of a protein by specifying the Uniprot ID. 
+By using the ``predict_disorder_uniprot()`` function, you can return predicted consensus disorder values for the amino acid sequence of a protein by specifying the UniProt ID. 
 
 **Example**
 
 .. code-block:: python
 
     meta.predict_disorder_uniprot("Q8N6T3")
 
@@ -516,15 +536,15 @@
     
      meta.predict_disorder_uniprot("Q8N6T3", legacy=True)
 
 
 Predicting AlphaFold2 Confidence Scores Using Uniprot ID
 -----------------------------------------------------------
 
-By using the ``predict_pLDDT_uniprot`` function, you can generate predicted AlphaFold2 pLDDT confidence scores by inputting a Uniprot ID.
+By using the ``predict_pLDDT_uniprot`` function, you can generate predicted AlphaFold2 pLDDT confidence scores by inputting a UniProt ID.
 
 **Example**
 
 .. code-block:: python
 
     meta.predict_pLDDT_uniprot('P16892')
 
@@ -610,18 +630,18 @@
 By using the ``graph_pLDDT_fasta`` function, you can graph predicted AlphaFold2 pLDDT confidence scores for the amino acid sequences in a .fasta file. This works the same as ``graph_disorder_fasta`` but instead returns graphs with just the predicted AlphaFold2 pLDDT scores.
 
 .. code-block:: python
 
     meta.graph_pLDDT_fasta("/Users/thisUser/Desktop/coolSequences.fasta", output_dir="/Users/thisUser/Desktop/folderForGraphs")
 
 
-Generating Graphs Using Uniprot ID
+Generating Graphs Using UniProt ID
 ------------------------------------
 
-By using the ``graph_disorder_uniprot()`` function, you can graph predicted consensus disorder values for the amino acid sequence of a protein by specifying the Uniprot ID. 
+By using the ``graph_disorder_uniprot()`` function, you can graph predicted consensus disorder values for the amino acid sequence of a protein by specifying the UniProt ID. 
 
 **Example**
 
 .. code-block:: python
 
     meta.graph_disorder_uniprot("Q8N6T3")
 
@@ -649,15 +669,15 @@
 
 **Example:** 
 
 .. code-block:: python
     
     meta.graph_disorder_uniprot("Q8N6T3", legacy=True)
 
-Generating AlphaFold2 Confidnce Score Graphs Using Uniprot ID
+Generating AlphaFold2 Confidence Score Graphs Using UniProt ID
 --------------------------------------------------------------
 
 Just like with disorder predictions, you can also get AlphaFold2 pLDDT confidence score graphs using the Uniprot ID. This will **only display the pLDDT confidence scores** and not the predicted disorder scores. 
 
 **Example**
 
 .. code-block:: python
@@ -708,14 +728,96 @@
 **Example:** 
 
 .. code-block:: python
     
     meta.predict_disorder_domains_uniprot('Q8N6T3' legacy=True)
 
 
+
+Batch prediction of disorder scores or disordered domains
+---------------------------------------------------------
+
+As of metapredict V2-FF (V2.6), metapredict enables GPU or CPU enabled batch prediction.
+
+
+Predicting disorder scores in batch mode
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The simplest usage is to pass a list of sequences to :code:`predict_disorder_batch()` e.g.:
+
+.. code-block:: python
+
+	seqs = ['APSPASPPASPSA','PQPQPQPWQPWPQPW','ASDASFPAPSDPASDPA']
+
+	return_data = meta.predict_disorder_batch(seqs)
+	
+In this scenario, :code:`return_data` is a list of three elements, where each element is itself a list that has two elements; the sequence and the per-residue disorder scores as an :code:`np.ndarray`:
+
+.. code-block:: python
+
+	[['APSPASPPASPSA',
+	  array([0.8983, 0.9628, 0.9682, 0.9767, 0.9798, 0.9904, 0.9774, 0.9711,
+	         0.9656, 0.969 , 0.9361, 0.8879, 0.7606], dtype=float32)],
+	 ['PQPQPQPWQPWPQPW',
+	  array([0.9251, 0.9448, 0.949 , 0.9393, 0.9276, 0.9132, 0.8923, 0.8575,
+	         0.8385, 0.8138, 0.7777, 0.7366, 0.7164, 0.6184, 0.4999],
+	        dtype=float32)],
+	 ['ASDASFPAPSDPASDPA',
+	  array([0.8881, 0.9427, 0.95  , 0.9415, 0.9431, 0.9336, 0.9295, 0.9304,
+	         0.9299, 0.9377, 0.9351, 0.9235, 0.9137, 0.9203, 0.8864, 0.83  ,
+	         0.7037], dtype=float32)]]
+
+Note also that by default this function will print a progress bar to report on how quickly predictions are running. If this is not desired, the progress bar can be turned off using :code:`show_progress_bar=False` option in the function signature.
+
+In addition to passing in a list of sequences, you can also pass in a dictionary of sequences with protein_id:sequence mapping. In this case, the function will return a dictionary that has the same key-value pairing as the input dictionary, but instead of key-value (protein_id:[sequence, disorder prediction]). In this way, predicting disorder scores for large sets of sequences becomes straight forward. 
+
+Predicting disordered domains in batch mode
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+For disordered domains, the same function can be used with  :code:`return_domains=True` set. If this is the case, the same input/output behavior (lists or dictionaries as inputs) can be used, but rather than returning a two-position list of sequence and disorder score, the return type is a single DisorderDomain object. 
+
+DisorderDomain objects are data structures that present a set of information about a protein. Each object has six so-called "dot variables" (object variables) that provide distinct information:
+
+* `sequence` - reports on the sequence of the full protein
+* `disorder` - reports on the per-residue disorder score for the whole protein (i.e. the same information that would be reported if :code:`return_domains=False` 
+* `disordered_domain_boundaries` - is a list with 0 or more sublists, where those sublists define the start and end positions of the IDRs within the protein sequence. These domain boundaries follow Python notation, i.e. if a disordered region ran between residue 1 and 10 in a protein, the boundaries would be [0,9].
+* `folded_domain_boundaries` - same conceptual idea as described for the `disordered_domain_boundaries`, except here the reciprocal folded domain boundaries are reported.
+* `disordered_domains` - the actual amino acid sequence of the IDRs - i.e. the length of `disordered_domains` is the same as the length of `disordered_domain_boundaries`.
+* `folded_domains` - the actual amino acid sequence of the folded domains - i.e. the length of `folded_domains` is the same as the length of `folded_domain_boundaries`.
+
+As an example:
+
+.. code-block:: python
+
+	seqs = ['APSPASPPASPSA','PQPQPQPWQPWPQPW','ASDASFPAPSDPASDPA']
+
+	return_data = meta.predict_disorder_batch(seqs, return_domains=True)
+
+	# if we then examined one of the return objects
+	tmp = return_data[0]
+	
+	print(tmp)
+	
+		DisorderObject for sequence with 13 residues, 1 IDRs, and 0 folded domains
+		Available dot variables are:
+		  .sequence
+		  .disorder
+		  .disordered_domain_boundaries
+		  .folded_domain_boundaries
+		  .disordered_domains
+		  .folded_domains
+		  
+	print(tmp.disordered_domains)
+		['APSPASPPASPSA']
+		
+	print(disorder)
+		[0.8983 0.9628 0.9682 0.9767 0.9798 0.9904 0.9774 0.9711 0.9656 		0.969 0.9361 0.8879 0.7606]
+		
+The various options for changing the definition of a disordered domain are also available to be passed to :code:`meta.predict_disorder_batch()`. For a complete list of possible input variables we recommend checking out the corresponding Python module documentation.
+
+
 Predicting Disorder Domains from external scores:
 --------------------------------------------------
 
 The ``predict_disorder_domains_from_external_scores()`` function takes in an disorder scores, an amino acid sequence (optinally), and returns a DisorderObject. This function lets you use other disorder predictor scores and still use the predict_disorder_domains() functionality. The DisorderObject has 6 dot variables that can be called to get information about your input sequence. They are as follows: 
 
 .sequence : str    
     Amino acid sequence
```

### Comparing `metapredict-2.51/metapredict/.DS_Store` & `metapredict-2.61/metapredict/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -252,161 +252,161 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 0007  ................
 00001010: 0062 0061 0063 006b 0065 006e 0064 6277  .b.a.c.k.e.n.dbw
-00001020: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
+00001020: 7370 626c 6f62 0000 00b6 6270 6c69 7374  spblob....bplist
 00001030: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00001040: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00001050: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00001060: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00001070: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 00001080: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00001090: 6465 6261 7208 0908 095f 1017 7b7b 3937  debar...._..{{97
-000010a0: 2c20 3435 357d 2c20 7b38 3130 2c20 3435  , 455}, {810, 45
-000010b0: 357d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  5}}...#/;R_klmno
-000010c0: 8900 0000 0000 0001 0100 0000 0000 0000  ................
-000010d0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000010e0: 8a00 0000 0700 6200 6100 6300 6b00 6500  ......b.a.c.k.e.
-000010f0: 6e00 6464 7363 6c62 6f6f 6c00 0000 0007  n.ddsclbool.....
-00001100: 0062 0061 0063 006b 0065 006e 0064 6c67  .b.a.c.k.e.n.dlg
-00001110: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
-00001120: 0007 0062 0061 0063 006b 0065 006e 0064  ...b.a.c.k.e.n.d
-00001130: 6c73 7643 626c 6f62 0000 02f7 6270 6c69  lsvCblob....bpli
-00001140: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00001150: 1853 540a 5658 6963 6f6e 5369 7a65 5f10  .ST.VXiconSize_.
-00001160: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001170: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001180: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00001190: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-000011a0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-000011b0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-000011c0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000011d0: 0009 ae0c 151a 1f23 282d 3237 3c41 4549  .......#(-27<AEI
-000011e0: 4dd4 0d0e 0f10 0a12 0a14 5776 6973 6962  M.........Wvisib
-000011f0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00001200: 6e67 5a69 6465 6e74 6966 6965 7209 10ac  ngZidentifier...
-00001210: 0954 6e61 6d65 d410 0e0f 0d16 1718 1858  .Tname.........X
-00001220: 7562 6971 7569 7479 1023 0808 d40d 0e0f  ubiquity.#......
-00001230: 100a 1c18 1e09 10b5 085c 6461 7465 4d6f  .........\dateMo
-00001240: 6469 6669 6564 d40d 0e0f 1018 1c18 2208  dified........".
-00001250: 085b 6461 7465 4372 6561 7465 64d4 0d0e  .[dateCreated...
-00001260: 0f10 0a25 1827 0910 6108 5473 697a 65d4  ...%.'..a.Tsize.
-00001270: 0d0e 0f10 0a2a 0a2c 0910 7309 546b 696e  .....*.,..s.Tkin
-00001280: 64d4 0d0e 0f10 182f 0a31 0810 6409 556c  d....../.1..d.Ul
-00001290: 6162 656c d40d 0e0f 1018 340a 3608 104b  abel......4.6..K
-000012a0: 0957 7665 7273 696f 6ed4 0d0e 0f10 1839  .Wversion......9
-000012b0: 0a3b 0811 012c 0958 636f 6d6d 656e 7473  .;...,.Xcomments
-000012c0: d40d 0e0f 1018 3e18 4008 10c8 085e 6461  ......>.@....^da
-000012d0: 7465 4c61 7374 4f70 656e 6564 d40d 0e0f  teLastOpened....
-000012e0: 1018 3e18 4408 085a 7368 6172 654f 776e  ..>.D..ZshareOwn
-000012f0: 6572 d40d 0e0f 1018 3e18 4808 085f 100f  er......>.H.._..
-00001300: 7368 6172 654c 6173 7445 6469 746f 72d4  shareLastEditor.
-00001310: 100e 0f0d 4a1c 1818 5964 6174 6541 6464  ....J...YdateAdd
-00001320: 6564 0808 d40d 0e0f 1018 4f18 5108 10d2  ed........O.Q...
-00001330: 085f 1010 696e 7669 7461 7469 6f6e 5374  ._..invitationSt
-00001340: 6174 7573 0823 402a 0000 0000 0000 546e  atus.#@*......Tn
-00001350: 616d 6509 1400 0000 0000 0000 0000 0000  ame.............
-00001360: 0000 0000 0100 0800 1900 2200 3400 3c00  ..........".4.<.
-00001370: 5000 5900 6400 7700 8c00 9500 9600 a500  P.Y.d.w.........
-00001380: ae00 b600 bc00 c600 d100 d200 d400 d500  ................
-00001390: da00 e300 ec00 ee00 ef00 f000 f900 fa00  ................
-000013a0: fc00 fd01 0a01 1301 1401 1501 2101 2a01  ............!.*.
-000013b0: 2b01 2d01 2e01 3301 3c01 3d01 3f01 4001  +.-...3.<.=.?.@.
-000013c0: 4501 4e01 4f01 5101 5201 5801 6101 6201  E.N.O.Q.R.X.a.b.
-000013d0: 6401 6501 6d01 7601 7701 7a01 7b01 8401  d.e.m.v.w.z.{...
-000013e0: 8d01 8e01 9001 9101 a001 a901 aa01 ab01  ................
-000013f0: b601 bf01 c001 c101 d301 dc01 e601 e701  ................
-00001400: e801 f101 f201 f401 f502 0802 0902 1202  ................
-00001410: 1702 1800 0000 0000 0002 0100 0000 0000  ................
-00001420: 0000 5700 0000 0000 0000 0000 0000 0000  ..W.............
-00001430: 0002 2900 0000 0700 6200 6100 6300 6b00  ..).....b.a.c.k.
-00001440: 6500 6e00 646c 7376 7062 6c6f 6200 0002  e.n.dlsvpblob...
-00001450: 7062 706c 6973 7430 30d8 0102 0304 0506  pbplist00.......
-00001460: 0708 090a 0b1d 4647 0a49 5869 636f 6e53  ......FG.IXiconS
-00001470: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-00001480: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00001490: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-000014a0: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-000014b0: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-000014c0: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-000014d0: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-000014e0: 0000 0000 0000 09d9 0c0d 0e0f 1011 1213  ................
-000014f0: 1415 1e23 282d 3236 3b40 5863 6f6d 6d65  ...#(-26;@Xcomme
-00001500: 6e74 7355 6c61 6265 6c57 7665 7273 696f  ntsUlabelWversio
-00001510: 6e5b 6461 7465 4372 6561 7465 6454 7369  n[dateCreatedTsi
-00001520: 7a65 5c64 6174 654d 6f64 6966 6965 6454  ze\dateModifiedT
-00001530: 6b69 6e64 546e 616d 655e 6461 7465 4c61  kindTname^dateLa
-00001540: 7374 4f70 656e 6564 d416 1718 191a 1b0a  stOpened........
-00001550: 1d55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
-00001560: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
-00001570: 0711 012c 0908 d416 1718 191f 200a 1d10  ...,........ ...
-00001580: 0510 6409 08d4 1617 1819 2425 0a1d 1006  ..d.......$%....
-00001590: 104b 0908 d416 1718 1929 2a1d 1d10 0210  .K.......)*.....
-000015a0: b508 08d4 1617 1819 2e2f 1d0a 1003 1061  ........./.....a
-000015b0: 0809 d416 1718 1933 2a1d 0a10 0108 09d4  .......3*.......
-000015c0: 1617 1819 3738 0a0a 1004 1073 0909 d416  ....78.....s....
-000015d0: 1718 193c 3d0a 0a10 0010 ac09 09d4 1617  ...<=...........
-000015e0: 1819 4142 1d1d 1008 10c8 0808 0823 402a  ..AB.........#@*
-000015f0: 0000 0000 0000 546e 616d 6509 1400 0000  ......Tname.....
-00001600: 0000 0000 0000 0000 0000 0000 0100 0800  ................
-00001610: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00001620: 8c00 9500 9600 a900 b200 b800 c000 cc00  ................
-00001630: d100 de00 e300 e800 f701 0001 0601 0c01  ................
-00001640: 1601 1e01 2001 2301 2401 2501 2e01 3001  .... .#.$.%...0.
-00001650: 3201 3301 3401 3d01 3f01 4101 4201 4301  2.3.4.=.?.A.B.C.
-00001660: 4c01 4e01 5001 5101 5201 5b01 5d01 5f01  L.N.P.Q.R.[.]._.
-00001670: 6001 6101 6a01 6c01 6d01 6e01 7701 7901  `.a.j.l.m.n.w.y.
-00001680: 7b01 7c01 7d01 8601 8801 8a01 8b01 8c01  {.|.}...........
-00001690: 9501 9701 9901 9a01 9b01 9c01 a501 aa01  ................
-000016a0: ab00 0000 0000 0002 0100 0000 0000 0000  ................
-000016b0: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-000016c0: bc00 0000 0700 6200 6100 6300 6b00 6500  ......b.a.c.k.e.
-000016d0: 6e00 646d 6f44 4462 6c6f 6200 0000 080f  n.dmoDDblob.....
-000016e0: 1eea ddae 86c2 4100 0000 0700 6200 6100  ......A.....b.a.
-000016f0: 6300 6b00 6500 6e00 646d 6f64 4462 6c6f  c.k.e.n.dmodDblo
-00001700: 6200 0000 080f 1eea ddae 86c2 4100 0000  b...........A...
-00001710: 0700 6200 6100 6300 6b00 6500 6e00 6470  ..b.a.c.k.e.n.dp
-00001720: 6831 5363 6f6d 7000 0000 0000 0000 0000  h1Scomp.........
-00001730: 0000 0700 6200 6100 6300 6b00 6500 6e00  ....b.a.c.k.e.n.
-00001740: 6476 5372 6e6c 6f6e 6700 0000 0100 0000  dvSrnlong.......
-00001750: 0400 6400 6100 7400 6162 7773 7062 6c6f  ..d.a.t.abwspblo
-00001760: 6200 0000 b862 706c 6973 7430 30d6 0102  b....bplist00...
-00001770: 0304 0506 0708 0708 0b08 5d53 686f 7753  ..........]ShowS
-00001780: 7461 7475 7342 6172 5b53 686f 7754 6f6f  tatusBar[ShowToo
-00001790: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-000017a0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-000017b0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-000017c0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-000017d0: 0809 0809 5f10 187b 7b36 312c 2034 3536  ...._..{{61, 456
-000017e0: 7d2c 207b 3131 3138 2c20 3438 387d 7d09  }, {1118, 488}}.
-000017f0: 0815 232f 3b52 5f6b 6c6d 6e6f 8a00 0000  ..#/;R_klmno....
-00001800: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
-00001810: 0000 0000 0000 0000 0000 0000 8b00 0000  ................
-00001820: 0400 6400 6100 7400 6164 7363 6c62 6f6f  ..d.a.t.adsclboo
-00001830: 6c00 0000 0004 0064 0061 0074 0061 7653  l......d.a.t.avS
-00001840: 726e 6c6f 6e67 0000 0001 0000 0005 0074  rnlong.........t
-00001850: 0065 0073 0074 0073 6277 7370 626c 6f62  .e.s.t.sbwspblob
-00001860: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00001870: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00001880: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00001890: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-000018a0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-000018b0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-000018c0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-000018d0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-000018e0: 0809 5f10 187b 7b31 3433 2c20 3533 387d  .._..{{143, 538}
-000018f0: 2c20 7b39 3632 2c20 3432 387d 7d09 0817  , {962, 428}}...
-00001900: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-00001910: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00001920: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-00001930: 0500 7400 6500 7300 7400 7376 5372 6e6c  ..t.e.s.t.svSrnl
-00001940: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
+00001090: 6465 6261 7208 0908 095f 1016 7b7b 3233  debar...._..{{23
+000010a0: 322c 2030 7d2c 207b 3831 302c 2037 3338  2, 0}, {810, 738
+000010b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f88  }}...#/;R_klmno.
+000010c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000010d0: 0000 0000 0000 0000 0000 0000 0000 0089  ................
+000010e0: 0000 0007 0062 0061 0063 006b 0065 006e  .....b.a.c.k.e.n
+000010f0: 0064 6473 636c 626f 6f6c 0000 0000 0700  .ddsclbool......
+00001100: 6200 6100 6300 6b00 6500 6e00 646c 6731  b.a.c.k.e.n.dlg1
+00001110: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
+00001120: 0700 6200 6100 6300 6b00 6500 6e00 646c  ..b.a.c.k.e.n.dl
+00001130: 7376 4362 6c6f 6200 0002 f762 706c 6973  svCblob....bplis
+00001140: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+00001150: 5354 0a56 5869 636f 6e53 697a 655f 100f  ST.VXiconSize_..
+00001160: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00001170: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00001180: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+00001190: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+000011a0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+000011b0: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+000011c0: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+000011d0: 09ae 0c15 1a1f 2328 2d32 373c 4145 494d  ......#(-27<AEIM
+000011e0: d40d 0e0f 100a 120a 1457 7669 7369 626c  .........Wvisibl
+000011f0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+00001200: 675a 6964 656e 7469 6669 6572 0910 ac09  gZidentifier....
+00001210: 546e 616d 65d4 100e 0f0d 1617 1818 5875  Tname.........Xu
+00001220: 6269 7175 6974 7910 2308 08d4 0d0e 0f10  biquity.#.......
+00001230: 0a1c 181e 0910 b508 5c64 6174 654d 6f64  ........\dateMod
+00001240: 6966 6965 64d4 0d0e 0f10 181c 1822 0808  ified........"..
+00001250: 5b64 6174 6543 7265 6174 6564 d40d 0e0f  [dateCreated....
+00001260: 100a 2518 2709 1061 0854 7369 7a65 d40d  ..%.'..a.Tsize..
+00001270: 0e0f 100a 2a0a 2c09 1073 0954 6b69 6e64  ....*.,..s.Tkind
+00001280: d40d 0e0f 1018 2f0a 3108 1064 0955 6c61  ....../.1..d.Ula
+00001290: 6265 6cd4 0d0e 0f10 1834 0a36 0810 4b09  bel......4.6..K.
+000012a0: 5776 6572 7369 6f6e d40d 0e0f 1018 390a  Wversion......9.
+000012b0: 3b08 1101 2c09 5863 6f6d 6d65 6e74 73d4  ;...,.Xcomments.
+000012c0: 0d0e 0f10 183e 1840 0810 c808 5e64 6174  .....>.@....^dat
+000012d0: 654c 6173 744f 7065 6e65 64d4 0d0e 0f10  eLastOpened.....
+000012e0: 183e 1844 0808 5a73 6861 7265 4f77 6e65  .>.D..ZshareOwne
+000012f0: 72d4 0d0e 0f10 183e 1848 0808 5f10 0f73  r......>.H.._..s
+00001300: 6861 7265 4c61 7374 4564 6974 6f72 d410  hareLastEditor..
+00001310: 0e0f 0d4a 1c18 1859 6461 7465 4164 6465  ...J...YdateAdde
+00001320: 6408 08d4 0d0e 0f10 184f 1851 0810 d208  d........O.Q....
+00001330: 5f10 1069 6e76 6974 6174 696f 6e53 7461  _..invitationSta
+00001340: 7475 7308 2340 2a00 0000 0000 0054 6e61  tus.#@*......Tna
+00001350: 6d65 0914 0000 0000 0000 0000 0000 0000  me..............
+00001360: 0000 0001 0008 0019 0022 0034 003c 0050  .........".4.<.P
+00001370: 0059 0064 0077 008c 0095 0096 00a5 00ae  .Y.d.w..........
+00001380: 00b6 00bc 00c6 00d1 00d2 00d4 00d5 00da  ................
+00001390: 00e3 00ec 00ee 00ef 00f0 00f9 00fa 00fc  ................
+000013a0: 00fd 010a 0113 0114 0115 0121 012a 012b  ...........!.*.+
+000013b0: 012d 012e 0133 013c 013d 013f 0140 0145  .-...3.<.=.?.@.E
+000013c0: 014e 014f 0151 0152 0158 0161 0162 0164  .N.O.Q.R.X.a.b.d
+000013d0: 0165 016d 0176 0177 017a 017b 0184 018d  .e.m.v.w.z.{....
+000013e0: 018e 0190 0191 01a0 01a9 01aa 01ab 01b6  ................
+000013f0: 01bf 01c0 01c1 01d3 01dc 01e6 01e7 01e8  ................
+00001400: 01f1 01f2 01f4 01f5 0208 0209 0212 0217  ................
+00001410: 0218 0000 0000 0000 0201 0000 0000 0000  ................
+00001420: 0057 0000 0000 0000 0000 0000 0000 0000  .W..............
+00001430: 0229 0000 0007 0062 0061 0063 006b 0065  .).....b.a.c.k.e
+00001440: 006e 0064 6c73 7670 626c 6f62 0000 0270  .n.dlsvpblob...p
+00001450: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00001460: 0809 0a0b 1d46 470a 4958 6963 6f6e 5369  .....FG.IXiconSi
+00001470: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00001480: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001490: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000014a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000014b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000014c0: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+000014d0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+000014e0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
+000014f0: 151e 2328 2d32 363b 4058 636f 6d6d 656e  ..#(-26;@Xcommen
+00001500: 7473 556c 6162 656c 5776 6572 7369 6f6e  tsUlabelWversion
+00001510: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+00001520: 655c 6461 7465 4d6f 6469 6669 6564 546b  e\dateModifiedTk
+00001530: 696e 6454 6e61 6d65 5e64 6174 654c 6173  indTname^dateLas
+00001540: 744f 7065 6e65 64d4 1617 1819 1a1b 0a1d  tOpened.........
+00001550: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+00001560: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+00001570: 1101 2c09 08d4 1617 1819 1f20 0a1d 1005  ..,........ ....
+00001580: 1064 0908 d416 1718 1924 250a 1d10 0610  .d.......$%.....
+00001590: 4b09 08d4 1617 1819 292a 1d1d 1002 10b5  K.......)*......
+000015a0: 0808 d416 1718 192e 2f1d 0a10 0310 6108  ......../.....a.
+000015b0: 09d4 1617 1819 332a 1d0a 1001 0809 d416  ......3*........
+000015c0: 1718 1937 380a 0a10 0410 7309 09d4 1617  ...78.....s.....
+000015d0: 1819 3c3d 0a0a 1000 10ac 0909 d416 1718  ..<=............
+000015e0: 1941 421d 1d10 0810 c808 0808 2340 2a00  .AB.........#@*.
+000015f0: 0000 0000 0054 6e61 6d65 0914 0000 0000  .....Tname......
+00001600: 0000 0000 0000 0000 0000 0001 0008 0019  ................
+00001610: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00001620: 0095 0096 00a9 00b2 00b8 00c0 00cc 00d1  ................
+00001630: 00de 00e3 00e8 00f7 0100 0106 010c 0116  ................
+00001640: 011e 0120 0123 0124 0125 012e 0130 0132  ... .#.$.%...0.2
+00001650: 0133 0134 013d 013f 0141 0142 0143 014c  .3.4.=.?.A.B.C.L
+00001660: 014e 0150 0151 0152 015b 015d 015f 0160  .N.P.Q.R.[.]._.`
+00001670: 0161 016a 016c 016d 016e 0177 0179 017b  .a.j.l.m.n.w.y.{
+00001680: 017c 017d 0186 0188 018a 018b 018c 0195  .|.}............
+00001690: 0197 0199 019a 019b 019c 01a5 01aa 01ab  ................
+000016a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+000016b0: 0000 0000 0000 0000 0000 0000 0000 01bc  ................
+000016c0: 0000 0007 0062 0061 0063 006b 0065 006e  .....b.a.c.k.e.n
+000016d0: 0064 6d6f 4444 626c 6f62 0000 0008 0f1e  .dmoDDblob......
+000016e0: eadd ae86 c241 0000 0007 0062 0061 0063  .....A.....b.a.c
+000016f0: 006b 0065 006e 0064 6d6f 6444 626c 6f62  .k.e.n.dmodDblob
+00001700: 0000 0008 0f1e eadd ae86 c241 0000 0007  ...........A....
+00001710: 0062 0061 0063 006b 0065 006e 0064 7068  .b.a.c.k.e.n.dph
+00001720: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
+00001730: 0007 0062 0061 0063 006b 0065 006e 0064  ...b.a.c.k.e.n.d
+00001740: 7653 726e 6c6f 6e67 0000 0001 0000 0004  vSrnlong........
+00001750: 0064 0061 0074 0061 6277 7370 626c 6f62  .d.a.t.abwspblob
+00001760: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+00001770: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+00001780: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+00001790: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+000017a0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+000017b0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+000017c0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+000017d0: 0908 095f 1018 7b7b 3631 2c20 3435 367d  ..._..{{61, 456}
+000017e0: 2c20 7b31 3131 382c 2034 3838 7d7d 0908  , {1118, 488}}..
+000017f0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
+00001800: 0000 0101 0000 0000 0000 000d 0000 0000  ................
+00001810: 0000 0000 0000 0000 0000 008b 0000 0004  ................
+00001820: 0064 0061 0074 0061 6473 636c 626f 6f6c  .d.a.t.adsclbool
+00001830: 0000 0000 0400 6400 6100 7400 6176 5372  ......d.a.t.avSr
+00001840: 6e6c 6f6e 6700 0000 0100 0000 0500 7400  nlong.........t.
+00001850: 6500 7300 7400 7362 7773 7062 6c6f 6200  e.s.t.sbwspblob.
+00001860: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00001870: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00001880: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00001890: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+000018a0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+000018b0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+000018c0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+000018d0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+000018e0: 095f 1018 7b7b 3134 332c 2035 3338 7d2c  ._..{{143, 538},
+000018f0: 207b 3936 322c 2034 3238 7d7d 0908 1725   {962, 428}}...%
+00001900: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
+00001910: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00001920: 0000 0000 0000 0000 0000 009a 0000 0005  ................
+00001930: 0074 0065 0073 0074 0073 7653 726e 6c6f  .t.e.s.t.svSrnlo
+00001940: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0074 7355 6c61 6265 6c57 7665 7273 696f  .tsUlabelWversio
-00002510: 6e5b 6461 7465 4372 6561 7465 6454 7369  n[dateCreatedTsi
-00002520: 7a65 5c64 6174 654d 6f64 6966 6965 6454  ze\dateModifiedT
-00002530: 6b69 6e64 546e 616d 655e 6461 7465 4c61  kindTname^dateLa
-00002540: 7374 4f70 656e 6564 d416 1718 191a 1b0a  stOpened........
-00002550: 1d55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
-00002560: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
-00002570: 0711 012c 0908 d416 1718 191f 200a 1d10  ...,........ ...
-00002580: 0510 6409 08d4 1617 1819 2425 0a1d 1006  ..d.......$%....
-00002590: 104b 0908 d416 1718 1929 2a1d 1d10 0210  .K.......)*.....
-000025a0: b508 08d4 1617 1819 2e2f 1d0a 1003 1061  ........./.....a
-000025b0: 0809 d416 1718 1933 2a1d 0a10 0108 09d4  .......3*.......
-000025c0: 1617 1819 3738 0a0a 1004 1073 0909 d416  ....78.....s....
-000025d0: 1718 193c 3d0a 0a10 0010 ac09 09d4 1617  ...<=...........
-000025e0: 1819 4142 1d1d 1008 10c8 0808 0823 402a  ..AB.........#@*
-000025f0: 0000 0000 0000 546e 616d 6509 1400 0000  ......Tname.....
-00002600: 0000 0000 0000 0000 0000 0000 0100 0800  ................
-00002610: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00002620: 8c00 9500 9600 a900 b200 b800 c000 cc00  ................
-00002630: d100 de00 e300 e800 f701 0001 0601 0c01  ................
-00002640: 1601 1e01 2001 2301 2401 2501 2e01 3001  .... .#.$.%...0.
-00002650: 3201 3301 3401 3d01 3f01 4101 4201 4301  2.3.4.=.?.A.B.C.
-00002660: 4c01 4e01 5001 5101 5201 5b01 5d01 5f01  L.N.P.Q.R.[.]._.
-00002670: 6001 6101 6a01 6c01 6d01 6e01 7701 7901  `.a.j.l.m.n.w.y.
-00002680: 7b01 7c01 7d01 8601 8801 8a01 8b01 8c01  {.|.}...........
-00002690: 9501 9701 9901 9a01 9b01 9c01 a501 aa01  ................
-000026a0: ab00 0000 0000 0002 0100 0000 0000 0000  ................
-000026b0: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-000026c0: bc00 0000 0700 6200 6100 6300 6b00 6500  ......b.a.c.k.e.
-000026d0: 6e00 646d 6f44 4462 6c6f 6200 0000 080f  n.dmoDDblob.....
-000026e0: 1eea ddae 86c2 4100 0000 0700 6200 6100  ......A.....b.a.
-000026f0: 6300 6b00 6500 6e00 646d 6f64 4462 6c6f  c.k.e.n.dmodDblo
-00002700: 6200 0000 080f 1eea ddae 86c2 4100 0000  b...........A...
-00002710: 0700 6200 6100 6300 6b00 6500 6e00 6470  ..b.a.c.k.e.n.dp
-00002720: 6831 5363 6f6d 7000 0000 0000 0000 0000  h1Scomp.........
-00002730: 0000 0700 6200 6100 6300 6b00 6500 6e00  ....b.a.c.k.e.n.
-00002740: 6476 5372 6e6c 6f6e 6700 0000 0100 0000  dvSrnlong.......
-00002750: 0400 6400 6100 7400 6162 7773 7062 6c6f  ..d.a.t.abwspblo
-00002760: 6200 0000 b862 706c 6973 7430 30d6 0102  b....bplist00...
-00002770: 0304 0506 0708 0708 0b08 5d53 686f 7753  ..........]ShowS
-00002780: 7461 7475 7342 6172 5b53 686f 7754 6f6f  tatusBar[ShowToo
-00002790: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-000027a0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-000027b0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-000027c0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-000027d0: 0809 0809 5f10 187b 7b36 312c 2034 3536  ...._..{{61, 456
-000027e0: 7d2c 207b 3131 3138 2c20 3438 387d 7d09  }, {1118, 488}}.
-000027f0: 0815 232f 3b52 5f6b 6c6d 6e6f 8a00 0000  ..#/;R_klmno....
-00002800: 0000 0001                                ....
+00002500: 0073 556c 6162 656c 5776 6572 7369 6f6e  .sUlabelWversion
+00002510: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+00002520: 655c 6461 7465 4d6f 6469 6669 6564 546b  e\dateModifiedTk
+00002530: 696e 6454 6e61 6d65 5e64 6174 654c 6173  indTname^dateLas
+00002540: 744f 7065 6e65 64d4 1617 1819 1a1b 0a1d  tOpened.........
+00002550: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+00002560: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+00002570: 1101 2c09 08d4 1617 1819 1f20 0a1d 1005  ..,........ ....
+00002580: 1064 0908 d416 1718 1924 250a 1d10 0610  .d.......$%.....
+00002590: 4b09 08d4 1617 1819 292a 1d1d 1002 10b5  K.......)*......
+000025a0: 0808 d416 1718 192e 2f1d 0a10 0310 6108  ......../.....a.
+000025b0: 09d4 1617 1819 332a 1d0a 1001 0809 d416  ......3*........
+000025c0: 1718 1937 380a 0a10 0410 7309 09d4 1617  ...78.....s.....
+000025d0: 1819 3c3d 0a0a 1000 10ac 0909 d416 1718  ..<=............
+000025e0: 1941 421d 1d10 0810 c808 0808 2340 2a00  .AB.........#@*.
+000025f0: 0000 0000 0054 6e61 6d65 0914 0000 0000  .....Tname......
+00002600: 0000 0000 0000 0000 0000 0001 0008 0019  ................
+00002610: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00002620: 0095 0096 00a9 00b2 00b8 00c0 00cc 00d1  ................
+00002630: 00de 00e3 00e8 00f7 0100 0106 010c 0116  ................
+00002640: 011e 0120 0123 0124 0125 012e 0130 0132  ... .#.$.%...0.2
+00002650: 0133 0134 013d 013f 0141 0142 0143 014c  .3.4.=.?.A.B.C.L
+00002660: 014e 0150 0151 0152 015b 015d 015f 0160  .N.P.Q.R.[.]._.`
+00002670: 0161 016a 016c 016d 016e 0177 0179 017b  .a.j.l.m.n.w.y.{
+00002680: 017c 017d 0186 0188 018a 018b 018c 0195  .|.}............
+00002690: 0197 0199 019a 019b 019c 01a5 01aa 01ab  ................
+000026a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+000026b0: 0000 0000 0000 0000 0000 0000 0000 01bc  ................
+000026c0: 0000 0007 0062 0061 0063 006b 0065 006e  .....b.a.c.k.e.n
+000026d0: 0064 6d6f 4444 626c 6f62 0000 0008 0f1e  .dmoDDblob......
+000026e0: eadd ae86 c241 0000 0007 0062 0061 0063  .....A.....b.a.c
+000026f0: 006b 0065 006e 0064 6d6f 6444 626c 6f62  .k.e.n.dmodDblob
+00002700: 0000 0008 0f1e eadd ae86 c241 0000 0007  ...........A....
+00002710: 0062 0061 0063 006b 0065 006e 0064 7068  .b.a.c.k.e.n.dph
+00002720: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
+00002730: 0007 0062 0061 0063 006b 0065 006e 0064  ...b.a.c.k.e.n.d
+00002740: 7653 726e 6c6f 6e67 0000 0001 0000 0004  vSrnlong........
+00002750: 0064 0061 0074 0061 6277 7370 626c 6f62  .d.a.t.abwspblob
+00002760: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+00002770: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+00002780: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+00002790: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+000027a0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+000027b0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+000027c0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+000027d0: 0908 095f 1018 7b7b 3631 2c20 3435 367d  ..._..{{61, 456}
+000027e0: 2c20 7b31 3131 382c 2034 3838 7d7d 0908  , {1118, 488}}..
+000027f0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
+00002800: 0000 0101                                ....
```

### Comparing `metapredict-2.51/metapredict/__init__.py` & `metapredict-2.61/metapredict/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # Handle omplib error 
 if IGNORE_LIBOMP_ERROR:
     if sys.platform == 'darwin':
         os.environ['KMP_DUPLICATE_LIB_OK']='True'
 
 
 # Standardized function to check performance
-def print_performance(seq_len=500, num_seqs=100, verbose=True, legacy=False):
+def print_performance(seq_len=500, num_seqs=100, verbose=True, batch=True, legacy=False, batch_mode=None, variable_length=False):
     """
     Function that lets you test metapredicts performance on your local hardware.
 
     Parameters
     --------------
     seqlen : int 
         Length of each random sequence to be tested. Default = 500.
@@ -48,18 +48,28 @@
     num_seqs : int
         Number of sequences to compute over. Default = 100.
 
     verbose : bool
         Flag which, if true, means the function prints a summary when finished. If 
         false simply returns an integer
 
+    batch : bool
+        Flag which, if set to true, means we use batch mode, else we use serial mode.
+
     legacy : bool
         Flag which determines if legacy (v1) or updated (v2) metapredict networks
         are used.
 
+    batch_mode : int
+        Flag which defines which batch_mode algorithm to use for batched predictions.
+        Default = None which means the mode is dynamically picked. Can also be 1 or 2.
+
+    variable_length : bool
+        Flag which, if provided, means sequences vary between 20 and seq_len length.
+
     Returns
     ---------------
     int
         Returns the nearest number of sequences-per-second metapredict is currently
         predicting. For ref, on a spring 2020 MBP this value was ~10,000 sequences per
         second.
 
@@ -69,27 +79,39 @@
     import random
     import time
     VALID_AMINO_ACIDS = ['A','C','D','E','F','G','H','I','K','L','M','N','P','Q','R','S','T','V','W','Y']
 
     def genseq(n):
         """
         Function that generates a random 
-        """    
-        return "".join([random.choice(VALID_AMINO_ACIDS) for i in range(n)])
+        """
+        if variable_length:
+            local_n = random.randint(20,seq_len)
+        else:
+            local_n = n
+        return "".join([random.choice(VALID_AMINO_ACIDS) for i in range(local_n)])
 
     seqs = []
+    n_res = 0
     for i in range(num_seqs):
-        seqs.append(genseq(seq_len))
+        s = genseq(seq_len)
+        seqs.append(s)
+        n_res = n_res + len(s)
 
     start = time.time()
-    for i in seqs:
-        predict_disorder(i, legacy=legacy)
+
+    if batch:
+        predict_disorder_batch(seqs, batch_mode=batch_mode)
+
+    else:
+        for i in seqs:
+            predict_disorder(i, legacy=legacy)
 
     end = time.time()
-    r_per_second = (seq_len*num_seqs)/(end - start)
+    r_per_second = (n_res)/(end - start)
 
     if verbose:
         print(f'Predicting {r_per_second:f} residues per second!')
 
     return r_per_second
     
 def print_metapredict_legacy_network_version():
```

### Comparing `metapredict-2.51/metapredict/backend/brnn_architecture.py` & `metapredict-2.61/metapredict/backend/brnn_architecture.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/data_structures.py` & `metapredict-2.61/metapredict/backend/data_structures.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/domain_definition.py` & `metapredict-2.61/metapredict/backend/domain_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 import numpy as np
 import scipy
 from scipy.signal import savgol_filter
 from metapredict.metapredict_exceptions import DomainError
+
+
+## Note - this code block means that metapredict can be installed and imported without throwing an exception, which
+# in turn means it can be easily built on readthedocs without needing to compile Cython in line there.
+# This fix was added in May 2023
+try:
+    from .cython.domain_definition import build_domains_from_values as CYTHON_build_domains_from_values    
+except ModuleNotFoundError as e:
+    print('ERROR: Cython module was not found. This will happen if your installation did not correctly compile the cython modules')
+
+
+    # build a mock function
+    def CYTHON_build_domains_from_values(a,b,c,d,e,f):
+        raise ModuleNotFoundError('Could not import build_domains_from_values() in metapredict.backend.cython.domain_definition. Cython code has not compiled')
+
+    
 """
 Functions for extracting out discrete disordered domains based on the linear disorder score
 calculated by metapredict.
 
 """
 
 
@@ -278,15 +294,16 @@
 
 def get_domains(sequence,
                 disorder,
                 disorder_threshold=0.42,
                 minimum_IDR_size=12,
                 minimum_folded_domain=50,
                 gap_closure=10,
-                override_folded_domain_minsize=False):
+                override_folded_domain_minsize=False,
+                use_python = False):
     """
 
     Parameters
     -------------
     sequence : str
         Amino acid sequence
 
@@ -320,14 +337,19 @@
         By default this function includes a fail-safe check that assumes folded domains
         really shouldn't be less than 35 or 20 residues. However, for some approaches we
         may wish to over-ride these thresholds to match the passed minimum_folded_domain
         value. If this flag is set to True this override occurs. This is generally not 
         recommended unless you expect there to be well-defined sharp boundaries which could
         define small (20-30) residue folded domains. Default = False.
 
+
+    use_python : bool
+        Flag which, if set to True means we use the Python implementation used for metapredict V2. Default is set
+        to False so we use the Cython implementation, which is default in metapredict V2-FF.
+
     Returns
     ------------
 
     list 
 
         This function takes an amino acid sequence, a disorder score, and returns a 4-position tiple with
         the following information:
@@ -361,26 +383,43 @@
 
     if polynomial_order >= window_size:
         polynomial_order = window_size - 1
 
     # smoothe!!!!
     smoothed_disorder = savgol_filter(disorder, window_size, polynomial_order)
 
-
+    # V2-FF implementation
     # bound 0 and 1
-    smoothed_disorder = np.where(smoothed_disorder<0, 0, smoothed_disorder)
-    smoothed_disorder = np.where(smoothed_disorder>1, 1, smoothed_disorder)    
+    smoothed_disorder = np.clip(smoothed_disorder, a_min=0, a_max=1)
+
+    # v2 implementation
+    #smoothed_disorder = np.where(smoothed_disorder<0, 0, smoothed_disorder)
+    #smoothed_disorder = np.where(smoothed_disorder>1, 1, smoothed_disorder)    
 
     # Using smoothed disorder extract out domains
-    disordered_domain_info = __build_domains_from_values(smoothed_disorder,
-                                                         disorder_threshold,
-                                                         minimum_IDR_size=minimum_IDR_size,
-                                                         minimum_folded_domain=minimum_folded_domain,
-                                                         gap_closure=gap_closure,
-                                                         override_folded_domain_minsize=override_folded_domain_minsize)
+    if use_python:
+        disordered_domain_info = __build_domains_from_values(smoothed_disorder,
+                                                             disorder_threshold,
+                                                             minimum_IDR_size=minimum_IDR_size,
+                                                             minimum_folded_domain=minimum_folded_domain,
+                                                             gap_closure=gap_closure,
+                                                             override_folded_domain_minsize=override_folded_domain_minsize)
+    else:
+
+        # if needed, cast smoothed disorder to be double (bcause the Cython function requires this).
+        if smoothed_disorder.dtype != np.float64:
+            smoothed_disorder = smoothed_disorder.astype(np.float64)
+        
+        disordered_domain_info = CYTHON_build_domains_from_values(smoothed_disorder,
+                                                                  np.double(disorder_threshold),
+                                                                  minimum_IDR_size=minimum_IDR_size,
+                                                                  minimum_folded_domain=minimum_folded_domain,
+                                                                  gap_closure=gap_closure,
+                                                                  override_folded_domain_minsize=override_folded_domain_minsize)
+                                         
                                                          
 
     # finally cycle through and get the actual IDR and FD sequences. Note the if len(d) ==2 means we
     # skip over cases where no FDs or no IDRs were found
     idrs = []
     for d in disordered_domain_info[0]:
         if len(d) == 2:
```

### Comparing `metapredict-2.51/metapredict/backend/encode_sequence.py` & `metapredict-2.61/metapredict/backend/encode_sequence.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/meta_graph.py` & `metapredict-2.61/metapredict/backend/meta_graph.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/meta_predict_disorder.py` & `metapredict-2.61/metapredict/backend/meta_predict_disorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 predictor = "{}/networks/meta_predict_disorder_100e_v1.pt".format(PATH)
 
 # V2 network holds slight increases in accuracy but is still undergoing testing.
 # so far, 0.5% increase in accuracy has been consistently seen. V1 is the published
 # network though, so leaving fo the time being.
 # predictor = "{}/networks/metapredict_network_v2_200epochs_nl1_hs20.pt".format(PATH)
 
-# v3 network has significant increase in accuracy of predicting the actual consensus
+# V3 network has significant increase in accuracy of predicting the actual consensus
 # score values. Actual accuracy from predicting disorder values using the Disprot-PDB
 # testing (as in the paper) were negligent. Therefore, we will not use it as the
 # main network and will continue using V1. 
 
 
 ##################################################################################################
 # hyperparameters used by when metapredict was trained. Manually setting them here for clarity.
```

### Comparing `metapredict-2.51/metapredict/backend/meta_tools.py` & `metapredict-2.61/metapredict/backend/meta_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import protfasta
 import re
 from metapredict.metapredict_exceptions import MetapredictError
+import numpy as np
 
 
 def valid_range(inval, minval, maxval):
     if inval < minval or inval > maxval:
         raise MetapredictError(f'Value {inval:1.3f} is outside of range [{minval:1.3f}, {maxval:1.3f}]')
 
 
@@ -226,45 +227,66 @@
             cur_binary = get_binary_prediction(cur_score, cutoff_value=0.5)
             # write as tsv the caid formatted info
             current_output.write(f'{res_and_score_index+1}\t{cur_residue}\t{cur_score}\t{cur_binary}\n')
     
     current_output.close()
 
 
-def split_fasta(protfasta_fasta_list, number_splits):
+def split_fasta(fasta_list, number_splits):
     '''
     function to split the dict returned from
     a fasta file read in by protfasta to make
     a specific number of dictionaries with
     approximately equal numbers of proteins. 
+
+    Parameters
+    -----------
+    protfasta_fasta_list : list
+        List of amino acid sequences
+
+    number_splits : int
+        Number of lists to split this list into 
+
+    Returns
+    -----------
+    list
+        Returns a list where each sublist within
+        the list contains either the same number
+        number of sequences or +/- 1 number of 
+        sequences to all other lists, and there
+        are number_splits sublists in the main
+        return list.
+          
     '''
-    all_nums=[num for num in range(0, len(protfasta_fasta_list))]
-    num_per_split=int(len(protfasta_fasta_list)/number_splits)
-    all_vals=[]
-    for val in range(0, number_splits):
-        temp_list=[]
-        for subval in range(0, num_per_split):
-            temp_list.append(all_nums.pop())
-        if val==number_splits-1:
-            for val in all_nums:
-                temp_list.append(val)
-        all_vals.append(temp_list)
-    # keep track of added prots
-    num_prots=0
-    split_lists=[]
-    for val in all_vals:
-        temp_list=[]
-        for prot in val:
-            num_prots+=1
-            temp_list.append([protfasta_fasta_list[prot][0], protfasta_fasta_list[prot][1]])
-        split_lists.append(temp_list)
-    # make sure all proteins added
-    if num_prots!= len(protfasta_fasta_list):
+    
+    # Calculate the number of protein sequences per sublist
+    seqs_per_sublist = len(fasta_list) // num_sublists
+
+    # also count remainder
+    remainder = len(fasta_list) % num_sublists
+
+    # Create the sublists
+    sublists = []
+    start = 0
+    for i in range(num_sublists):
+
+        # note: saying 1 if 1 < remainder else 0 means we distribute
+        # the remainder evenly across the sublists
+        sublist_size = seqs_per_sublist + (1 if i < remainder else 0)
+
+        # create a sublist between start and sublist_size position
+        sublist = strings[start:start+sublist_size]
+        sublists.append(sublist)
+        start = start + sublist_size
+
+    # sanity check - good to be sure!
+    if np.sum([len(s) for s in sublist]) != len(fasta_list):
         raise Exception('splitting of fasta file did not get all proteins')
-    return split_lists
+
+    return sublists
 
 
 def append_to_file(outpath, idrs, mode):
     # Open file to append to.
     fh = open(outpath, 'a')
     # depending on mode...
     # dict to hold vals...
```

### Comparing `metapredict-2.51/metapredict/backend/metameta_hybrid_predict.py` & `metapredict-2.61/metapredict/backend/metameta_hybrid_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     # select the chosen network, kept as separate line of code in 
     used_predictor = predictor_string
     
     # set location of chosen network
     predictor_path = f'{PATH}/networks/{used_predictor}'
     
     # set predictor value using py_predictor_V2
-    my_predictor = py_predictor_v2.Predictor(predictor_path, 
-                                            dtype="residues")    
+    my_predictor = py_predictor_v2.Predictor(predictor_path, dtype="residues")    
+                                             
     # get values of prediction
     output_values = my_predictor.predict(sequence)
     
     # if normalized=True (defualt)
     if normalized == True:
         # initialize empty list to populate normalized values
         normalized_IDR_values = []
```

### Comparing `metapredict-2.51/metapredict/backend/networks/.DS_Store` & `metapredict-2.61/metapredict/backend/networks/.DS_Store`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/networks/metaDisorder.pt` & `metapredict-2.61/metapredict/backend/networks/metaDisorder.pt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/networks/meta_predict_disorder_100e_v1.pt` & `metapredict-2.61/metapredict/backend/networks/meta_predict_disorder_100e_v1.pt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/networks/metameta_2_7_22_nl2_hs20_b32_V3.pt` & `metapredict-2.61/metapredict/backend/networks/metameta_2_7_22_nl2_hs20_b32_V3.pt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/networks/metapredict_network_v2_200epochs_nl1_hs20.pt` & `metapredict-2.61/metapredict/backend/networks/metapredict_network_v2_200epochs_nl1_hs20.pt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/networks/metapredict_network_v3_200epochs_nl2_hs20.pt` & `metapredict-2.61/metapredict/backend/networks/metapredict_network_v3_200epochs_nl2_hs20.pt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/backend/py_predictor_v2.py` & `metapredict-2.61/metapredict/backend/py_predictor_v2.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     >>> my_predictor = py_predictor.Predictor(</path/to/saved_network.pt>, 
                                                 dtype={"sequence" or "residues"})
     >>> value = my_predictor.predict(AA_sequence)
     ***
     NOTE:   Assumes all sequences are composed of canonical amino acids and 
             that all networks were implemented using one-hot encoding.
     ***
-    Attributes
+    Attributesb
     ----------
     dtype : str
             Data format that the network was trained for. Either "sequence" or 
             "residues".
     num_layers : int
             Number of hidden layers in the trained network.
     hidden_vector_size : int
@@ -53,30 +53,50 @@
             task with n_classes.
     task : str
             Designates if network is designed for "classification" or "regression".
     network : PyTorch object
             Initialized PARROT network with loaded weights.
     """
 
-    def __init__(self, saved_weights, dtype):
+    def __init__(self, saved_weights, dtype, gpuid='cpu'):
         """
         Parameters
         ----------
         saved_weghts : str or Path
                 Location of the saved network weights. If a valid file is provided,
                 network parameters will be dynamically read in an network will be 
                 initialized.
         dtype : str
                 Data format that the network was trained for. Either "sequence" or 
                 "residues".
+
+        gpuid : str
+            By default set to 'cpu', but if a value is passed will try and override 
+        
         """
 
         self.dtype = dtype
-  
-        loaded_model = torch.load(saved_weights, map_location=torch.device('cpu'))
+
+        # if gpuid is not set to cpu
+        if gpuid != 'cpu':
+            if torch.cuda.is_available():
+                device_string = f"cuda:{gpuid}"
+                device = torch.device(device_string)
+            else:
+                device_string = "cpu"
+                device = torch.device(device_string)
+        else:
+            device_string = "cpu"
+            device = torch.device(device_string)
+
+        self.device = device
+        self.device_string = device_string
+
+        # load using the requested device
+        loaded_model = torch.load(saved_weights, map_location=device)
 
         # Dynamically read in correct network size:
         self.num_layers = 0
         while True:
             s = f'lstm.weight_ih_l{self.num_layers}'
             try:
                 temp = loaded_model[s]
@@ -89,21 +109,22 @@
         self.n_classes = np.shape(loaded_model['fc.bias'])[0]
 
         if self.n_classes > 1:
             self.task = "classification"
         else:
             self.task = "regression"
 
-        # Instantiate network weights into Predictor() object
+        # Instantiate network weights into Predictor() object - note we have to ensure the network
+        # is loaded onto the same model as the device type
         if self.dtype == "sequence":
             self.network = brnn_architecture.BRNN_MtO(20, self.hidden_vector_size, 
-                                            self.num_layers, self.n_classes, 'cpu')
+                                                      self.num_layers, self.n_classes, device_string)
         elif self.dtype == "residues":
             self.network = brnn_architecture.BRNN_MtM(20, self.hidden_vector_size, 
-                                            self.num_layers, self.n_classes, 'cpu')
+                                                      self.num_layers, self.n_classes, device_string)
         else:
             raise ValueError("dtype must equal 'residues' or 'sequence'")
                                         
         self.network.load_state_dict(loaded_model)
 
 
     def predict(self, seq):
```

### Comparing `metapredict-2.51/metapredict/backend/uniprot_predictions.py` & `metapredict-2.61/metapredict/backend/uniprot_predictions.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,17 +38,26 @@
     s = "".join(str(r.data).split('\\n')[1:]).replace("'", "")
     
     # make sure that the last character is not a " due to a ' in protein name
     # Thank you to Github user keithchev for pointing out this bug!
 
     # if this fails the entire return string will be "b''" (len==3). We probably
     # need a more robust way to test for failure but this'll do for now...
+    # Update May 2023; it stopped doing
     if len(str(r.data)) == 3:
         raise MetapredictError(f'Error: unable to fetch UniProt sequence with accession {uniprot_id:s}')
 
+    # added as as second sanity check to handle poorly formatted uniprot accessions. Uniprot appears to
+    # now pass an error message if it fails that includes the term 'Error message', so this catch
+    # checks for that.
+    if str(r.data).find('Error messages') > -1:
+        raise MetapredictError(f'Error: unable to fetch UniProt sequence with accession {uniprot_id:s}')
+
+    print(r.data)
+
     if s[len(s)-1] == '"':
         s = s[:len(s)-1]
 
     if return_full_id == False:
         return s
 
     else:
```

### Comparing `metapredict-2.51/metapredict/data/test_data.fasta` & `metapredict-2.61/metapredict/data/test_data.fasta`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/meta.py` & `metapredict-2.61/metapredict/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## meta.py contains all the user-facing function associated with metapredict. If a new function is added it should be included
 ## here and added to the __all__ list
 ## 
 
 ##Handles the primary functions
 
 # NOTE - any new functions must be added to this list!
-__all__ =  ['predict_disorder_domains', 'predict_disorder', 'graph_disorder', 'predict_all', 'percent_disorder', 'predict_disorder_fasta', 'graph_disorder_fasta', 'predict_disorder_uniprot', 'graph_disorder_uniprot', 'predict_disorder_domains_uniprot', 'predict_disorder_domains_from_external_scores', 'graph_pLDDT_uniprot', 'predict_pLDDT_uniprot', 'graph_pLDDT_fasta', 'predict_pLDDT_fasta', 'graph_pLDDT', 'predict_pLDDT', 'predict_disorder_caid', 'predict_for_multithread']
+__all__ =  ['predict_disorder_domains', 'predict_disorder', 'graph_disorder', 'predict_all', 'percent_disorder', 'predict_disorder_fasta', 'graph_disorder_fasta', 'predict_disorder_uniprot', 'graph_disorder_uniprot', 'predict_disorder_domains_uniprot', 'predict_disorder_domains_from_external_scores', 'graph_pLDDT_uniprot', 'predict_pLDDT_uniprot', 'graph_pLDDT_fasta', 'predict_pLDDT_fasta', 'graph_pLDDT', 'predict_pLDDT', 'predict_disorder_caid', 'predict_disorder_batch']
  
 import os
 import sys
 import numpy as np
 
 # note - we import packages below with a leading _ which means they are ignored in the import
 
@@ -24,14 +24,15 @@
 from metapredict import parameters
 
 # import stuff for IDR predictor from backend. Note the 'as _*' hides the imported
 # module from the user
 from metapredict.backend.meta_predict_disorder import meta_predict as _meta_predict
 from metapredict.backend.metameta_hybrid_predict import metameta_predict as _metameta_predict
 from metapredict.backend import meta_tools as _meta_tools
+from metapredict.backend.batch_predict import batch_predict as _batch_predict
 
 #import stuff for graphing from backend
 from metapredict.backend.meta_graph import graph as _graph
 from metapredict.backend import domain_definition as _domain_definition
 
 # stuff for uniprot from backend
 from metapredict.backend.uniprot_predictions import fetch_sequence as _fetch_sequence
@@ -422,18 +423,19 @@
     Function to return all three types of predictions (legacy_metapredict,
     metapredict, and ppLDDT). Returns as a tuple of numpy 
     arrays, with ppLDDT returned as normalized between 0 and 1 
     (rather than 0 and 100) so can be plotted on same axis easily.
 
     Parameters
     ------------
-
     sequence : str 
         Input amino acid sequence (as string) to be predicted.
 
+    
+
     Returns
     --------
      
     tuple with three np.ndarrays:
 
         [0] - metapredict disorder scores (updated metapredict disorder)
         [1] - legacy metapredict disorder (original metapredict disorder)
@@ -455,14 +457,189 @@
 
     return (meta_disorder, legacy_disorder, ppLDDT)
 
 
 
 # ..........................................................................................
 #
+def predict_disorder_batch(input_sequences,
+                           gpuid=0,
+                           return_domains=False,
+                           disorder_threshold=0.5,
+                           minimum_IDR_size=12,
+                           minimum_folded_domain=50,
+                           gap_closure=10,
+                           show_progress_bar = True,
+                           batch_mode = None):
+
+    """
+    Batch mode predictor which takes advantage of PyTorch
+    parallelization such that whether it's on a GPU or a 
+    CPU, predictions for a set of sequences are performed
+    rapidly.
+
+    Batch mode was implemented in metapredict V2-FF, as is 
+    optimized for the hybrid network first released in V2.
+    As such a few options are not available for batch mode
+    which include:
+
+    * legacy - you cannot predict legacy metapredict scores with batch_mode
+             
+    * normalize - all predictions are automatically normalized to fall between 0 and 1
+            
+    * return_numpy - all disorder scores are returned as numpy arrays.
+                   
+
+    Note also that batch mode uses 32-bit float vectors
+    whereas non-batch uses 64-bit float vectors, so the
+    precise values in batch vs. non-batch may differ 
+    slighly, however this is a numerical precision difference,
+    such that values by both methods are always within
+    1e-3 of one another.
+
+    Parameters
+    --------------
+    input_sequences : list or dictionary
+        A collection of sequences that are presented either
+        as a list of sequences or a dictionary of key-value
+        pairs where values are sequences.
+
+    gpuid : int 
+        Identifier for the GPU being requested. Note that if
+        this is left unset the code will use the first GPU available
+        and if none is available will default back to CPU; in 
+        general it is recommended to not try and set this unless
+        there's a specific reason why a specific GPU should be
+        used
+
+    return_domains : bool
+        Flag which, if set to true, means we return DisorderDomain
+        objects instead of simply the disorder scores. These
+        domain objects include the boundaries between IDRs and 
+        folded domains, the disorder scores, and the individual
+        sequences for IDRs and folded domains. This adds a small
+        amount of overhead to the prediction, but typically only
+        increase prediction time by 10-15%.
+    
+    disorder_threshold : float
+        Used only if return_domains = True.
+
+        Threshold used to deliniate between folded and disordered
+        regions. We use a value of 0.5 because predict_disorder_batch
+        does not support legacy. 
+
+    minimum_IDR_size : int
+        Used only if return_domains = True.
+
+        Defines the smallest possible IDR. This is a hard limit - 
+        i.e. we CANNOT get IDRs smaller than this. Default = 12.
+
+    minimum_folded_domain : int
+        Used only if return_domains = True.
+
+        Defines where we expect the limit of small folded domains 
+        to be. This is NOT a hard limit and functions to modulate
+        the removal of large gaps (i.e. gaps less than this size 
+        are treated less strictly). Note that, in addition, 
+        gaps < 35 are evaluated with a threshold of 
+        0.35*disorder_threshold and gaps < 20 are evaluated with 
+        a threshold of 0.25*disorder_threshold. These two 
+        lengthscales were decided based on the fact that 
+        coiled-coiled regions (which are IDRs in isolation) 
+        often show up with reduced apparent disorder within IDRs, 
+        and but can be as short as 20-30 residues. 
+        The folded_domain_threshold is used based on the 
+        idea that it allows a 'shortest reasonable' folded domain 
+        to be identified. Default=50.
+
+    gap_closure : int
+        Used only if return_domains = True.
+
+        Defines the largest gap that would be 'closed'. Gaps here 
+        refer to a scenario in which you have two groups of 
+        disordered residues seprated by a 'gap' of un-disordered 
+        residues. In general large gap sizes will favour larger 
+        contigous IDRs. It's worth noting that gap_closure becomes 
+        relevant only when minimum_region_size becomes very small 
+        (i.e. < 5) because really gaps emerge when the smoothed 
+        disorder fit is "noisy", but when smoothed gaps
+        are increasingly rare. Default=10.
+
+    show_progress_bar : bool
+        Flag which, if set to True, means a progress bar is printed as 
+        predictions are made, while if False no progress bar is printed.
+        Default  =  True
+
+    batch_mode : string
+        Indictor which, if set to 'pack-n-pad', 'size-collect' 
+        will FORCE the batch algorithm to use mode 'pack-n-pad', 
+        'size-collect' for batch decomposition.
+
+        Mode 'size-collect'  means we pre-filter sequences into 
+        groups where they're all the same length, avoiding padding/packing. 
+        This works in all versions of torch, and will be faster
+        if you have very large datasets or have many copies of 
+        the same sequence.
+
+        Mode 'pack-n-pad' involves padding/packing the sequences so that 
+        all sequences can be passed in a batchsize of 32. This 
+        is only available if pytorch 1.11 or higher is available.
+        In testing, we found that pack-n-pad is about 2x faster than
+        size-collect if running on CPU with variable length sequence
+        if fewer 5000 sequences. On GPU, size-collect was consistently faster.
+
+        Default = None, which means dynamic selection occurs. Default
+        is to use size-collect because it is faster.
+
+    Returns
+    -------------
+    dict or list
+
+        IF RETURN DOMAINS == FALSE: this function returns either
+        a list or a dictionary.
+    
+        If a list was provided as input, the function returns a list
+        of the same length as the input list, where each element is 
+        itself a sublist where element 0 = sequence and element 1 is
+        a numpy array of disorder scores. The order of the return list
+        matches the order of the input list.
+
+        If a dictionary was provided as input, the function returns
+        a dictionary, where the same input keys map to values which are
+        lists of 2 elements, where element 0 = sequence and element 1 is
+        a numpy array of disorder scores.
+
+        IF RETURN DOMAINS == TRUE: this function returns either a list
+        or a dictionary.
+
+        If a list was provided as input, the function returns a list
+        of the same length as the input list, where each element is 
+        a DisorderDomain object. The order of the return list matches 
+        the order of the input list.
+
+        If a dictionary was provided as input, the function returns
+        a dictionary, where the same input keys map to a DisorderDomain
+        object that corresponds to the input dictionary sequence.
+
+    """
+
+    return _batch_predict(input_sequences,
+                          gpuid = gpuid,
+                          return_domains = return_domains,                          
+                          disorder_threshold = disorder_threshold,
+                          minimum_IDR_size = minimum_IDR_size,
+                          minimum_folded_domain = minimum_folded_domain,
+                          gap_closure = gap_closure,
+                          show_progress_bar = show_progress_bar,
+                          force_mode = batch_mode)
+
+
+
+# ..........................................................................................
+#
 def graph_disorder(sequence, 
                    title = 'Predicted protein disorder', 
                    disorder_threshold = None,
                    pLDDT_scores=False,
                    shaded_regions = None,
                    shaded_region_color = 'red',
                    DPI=150, 
@@ -861,17 +1038,18 @@
         Whether to use the legacy metapredict predictor. Default = False.
 
     Returns
     --------
 
     dict or None
         If output_file is set to None (as default) then this fiction returns 
-        a dictionary of sequence ID to disorder vector. If output_file is set 
-        to a filename then a .csv file will instead be written and         
-        no return data will be provided.
+        a dictionary of sequence ID to disorder np.ndarrays(dtype=np.float32). 
+
+        If output_file is set to a filename then a .csv file will instead 
+        be written and no return data will be provided.         
 
     """
 
     # Importantly, by default this function corrects invalid residue
     # values using protfasta.read_fasta() because the disorder predictor
     # cannot have non-amino acid values as an input.
 
@@ -879,51 +1057,73 @@
     test_data_file = os.path.abspath(filepath)
 
     if not os.path.isfile(test_data_file):
         raise FileNotFoundError(f'Datafile [{filepath}] does not exist.')
 
     protfasta_seqs = _protfasta.read_fasta(filepath, invalid_sequence_action = invalid_sequence_action, return_list = True)
 
-    # initialize empty dictionary to be populated with the the fasta headers (key) 
-    # and the predicted disorder values (value)
+
+    # initialize return dictionary
     disorder_dict = {}
+    
+    # Batch mode only supports normalized=True and legacy=False, so if
+    # either of these are set use the slower non batch mode
+    # 
+    if normalized is False or legacy is True:
 
-    # for the sequences in the protffasta_seqs list:
-    for seqs in protfasta_seqs:
+        # initialize empty dictionary to be populated with the the fasta headers (key) 
+        # and the predicted disorder values (value)
+        
 
-        # set cur_header equal to the fasta header
-        cur_header = seqs[0]
+        # for the sequences in the protffasta_seqs list:
+        for seqs in protfasta_seqs:
 
-        # set cur_seq equal to the sequence associated with the fasta header
-        cur_seq = seqs[1]
+            # set cur_header equal to the fasta header
+            cur_header = seqs[0]
 
-        # make all values for curSeq uppercase so they work with predictor
-        cur_seq = cur_seq.upper()
+            # set cur_seq equal to the sequence associated with the fasta header
+            cur_seq = seqs[1]
 
-        # set cur_disorder equal to the predicted values for cur_seq
-        cur_disorder = predict_disorder(cur_seq, normalized=normalized, legacy=legacy)
+            # make all values for curSeq uppercase so they work with predictor
+            cur_seq = cur_seq.upper()
 
-        disorder_dict[cur_header] = cur_disorder
+            # set cur_disorder equal to the predicted values for cur_seq
+            cur_disorder = predict_disorder(cur_seq, normalized=normalized, legacy=legacy, return_numpy=True)
 
+            disorder_dict[cur_header] = cur_disorder
+            
+    else:
+
+        # clean dict will be a dictionary of mapping from header
+        # to sequence, but will overwrite entries where the same
+        # header is present
+        clean_dict = {}
+        for k in protfasta_seqs:
+            clean_dict[k[0]] = k[1]
+
+        tmp_dict = _batch_predict(clean_dict)
+        for k in tmp_dict:
+            disorder_dict[k] = tmp_dict[k][1]
+    
     # if we did not request an output file 
     if output_file is None:
         return disorder_dict
 
     # else write to disk 
     else:
         _meta_tools.write_csv(disorder_dict, output_file)
 
 
 
 
 # ..........................................................................................
 #
 def predict_pLDDT_fasta(filepath, 
-                           output_file = None,
-                           invalid_sequence_action='convert'):
+                        output_file = None,
+                        invalid_sequence_action='convert'):
     """
     Function to read in a .fasta file from a specified filepath.
     Returns a dictionary of pLDDT values where the key is the 
     fasta header and the values are the predicted pLDDT values.
     
     Parameters
     -------------
@@ -1608,22 +1808,7 @@
         # now add all to output_dict
         output_dict[cur_id] = [[cur_sequence], cur_disorder]
 
     # write the output file
     _meta_tools.write_caid_format(output_dict, output_file)
 
 
-def predict_for_multithread(nested_list_of_seqs, 
-    outpath, mode, threshold_val, legacy):
-    '''
-    not multithreaded itself. Just a function
-    needed to predicted batches of sequences
-    for ultimately using in metapredict-multipredict
-    '''
-    all_vals={}
-    for name_seq in nested_list_of_seqs:
-        all_vals[name_seq[0]] = predict_disorder_domains(name_seq[1], disorder_threshold=threshold_val, legacy=legacy, return_list=True)
-    
-    # append vals to outpath
-    _meta_tools.append_to_file(outpath, all_vals, mode=mode)
-
-
```

### Comparing `metapredict-2.51/metapredict/tests/.DS_Store` & `metapredict-2.61/metapredict/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/input_data/DisorderPredictionssp_P04637_P53_HUMANC.txt` & `metapredict-2.61/metapredict/tests/input_data/DisorderPredictionssp_P04637_P53_HUMANC.txt`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/input_data/three_seqs.fasta` & `metapredict-2.61/metapredict/tests/cli_tests/input/three_seqs.fasta`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/local_data.py` & `metapredict-2.61/metapredict/tests/local_data.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/output/test.csv` & `metapredict-2.61/metapredict/tests/output/test.csv`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/test_domain_functions.py` & `metapredict-2.61/metapredict/tests/test_domain_functions.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/test_graph_disorder.py` & `metapredict-2.61/metapredict/tests/test_graph_disorder.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/test_graph_fasta.py` & `metapredict-2.61/metapredict/tests/test_graph_fasta.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict/tests/test_metapredict.py` & `metapredict-2.61/metapredict/tests/test_metapredict.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,20 +13,26 @@
 import sys
 import os
 from . import local_data
 import random
 import string
 import numpy as np
 
+import protfasta
+
 from metapredict.metapredict_exceptions import MetapredictError
 
 
 current_filepath = os.getcwd()
 fasta_filepath = "{}/input_data/testing.fasta".format(current_filepath)
 
+onehundred_seqs = "{}/input_data/test_seqs_100.fasta".format(current_filepath)
+onehundred_scores = "{}/input_data/test_scores_100.npy".format(current_filepath)
+
+
 def test_metapredict_imported():
     """Sample test, will always pass so long as import statement worked"""
     assert "metapredict" in sys.modules
 
 
 # test the legacy metapredict predictor
 def test_legacy_metapredict_predictor():
@@ -98,20 +104,20 @@
                 0.3 : 70.7}
     
     for thresh in [0.05, 0.1, 0.2, 0.3]:
         assert round(meta.percent_disorder(ARFGAP1, disorder_threshold=thresh, mode='disorder_domains'), 1) == expected[thresh]
 
     
     # make sure fasta stuff works for legacy
-    assert meta.predict_disorder_fasta(fasta_filepath, legacy=True) == {'Q8N6T3': local_data.disorder_Q8N6T3_legacy}
-
-    # make sure fasta stuff works for new predictor
-    assert meta.predict_disorder_fasta(fasta_filepath, legacy=False) == {'Q8N6T3': local_data.disorder_Q8N6T3}
-
+    # updated May 2023 to deal with the fact that predict_disorder_fasta now returns a dictionary where values are np.ndarrays
+    assert np.allclose(meta.predict_disorder_fasta(fasta_filepath, legacy=True)['Q8N6T3'], np.array(local_data.disorder_Q8N6T3_legacy, dtype=np.float32))
 
+    # make sure FASTA stuff works for non-legacy predictions
+    # updated May 2023 to deal with the fact that predict_disorder_fasta now returns a dictionary where values are np.ndarrays
+    assert np.allclose(meta.predict_disorder_fasta(fasta_filepath, legacy=False)['Q8N6T3'], np.array(local_data.disorder_Q8N6T3, dtype=np.float32))
 
 
 def test_predict_disorder_fail():
 
     # make sure we get gracefull fail on empty string
     with pytest.raises(MetapredictError):
         DisObj = meta.predict_disorder('')
@@ -175,35 +181,67 @@
         DisObj = meta.predict_disorder_domains(testseq, return_numpy=False, disorder_threshold=2)
 
 
 
 def test_predict_disorder_domains_random_seqs():
 
     N = 200
-    n_seqs = 5
+    n_seqs = 500
 
     for i in range(n_seqs):
         local_seq = ''.join(random.choices(['A','C','D','E','F','G','H','I','K','L','M','N','P','Q','R','S','T','V','W','Y'], k=N))
         DisObj = meta.predict_disorder_domains(local_seq, return_numpy=False, disorder_threshold=1)        
 
         # check no residues are in any IDR
         assert len(DisObj.disordered_domains) == 0
-
         assert meta.percent_disorder(local_seq, mode='disorder_domains', disorder_threshold=1) == 0
 
 
     for i in range(n_seqs):
         local_seq = ''.join(random.choices(['A','C','D','E','F','G','H','I','K','L','M','N','P','Q','R','S','T','V','W','Y'], k=N))
-        DisObj = meta.predict_disorder_domains(local_seq, return_numpy=False, disorder_threshold=0)        
+        DisObj = meta.predict_disorder_domains(local_seq, return_numpy=False, disorder_threshold=0)
 
-        # check all residues are in one IDR
-        assert len(DisObj.disordered_domains[0]) == N
+        # technically we can have non-IDRs with a threshold of 0 if there is a region where disorder score is
+        # literally 0
+        if len(DisObj.disordered_domains[0]) != N:
+            print(f'If this fails we have a weird bug; sequence: {local_seq}')
+            assert np.sum(np.array(DisObj.disorder) > 0) < N
+        else:
+            # check all residues are in one IDR
+            assert len(DisObj.disordered_domains[0]) == N
 
-        assert meta.percent_disorder(local_seq, mode='disorder_domains', disorder_threshold=0) == 100
+            assert meta.percent_disorder(local_seq, mode='disorder_domains', disorder_threshold=0) == 100
 
 
 def test_percent_disorder_fail():
 
     # make sure we get gracefull fail on empty string
     with pytest.raises(MetapredictError):
         DisObj = meta.percent_disorder('')
 
+
+def test_big_test():
+    """
+    Big tests that compares previously computed disordered scores for 100 sequences
+    with the current testable version. This is the most robust test to ensure that
+    the current version reproduces scores of other versions of metapredict
+
+    ## update may 2023
+    Note; we had to pull the atol down to 0.0001 for Py310 which probably reflects
+    some changes under the hood in how floats are dealt with in the C/python/Cython
+    exchange and/or in PyTorch. This is not an issue, but we're just documenting it
+    in case this comes up in the future
+    
+
+    """
+
+    scores = np.load(onehundred_scores, allow_pickle=True).tolist()
+    seqs = protfasta.read_fasta(onehundred_seqs)
+
+    for idx, k in enumerate(seqs):
+        local_score = meta.predict_disorder(seqs[k])
+        assert np.allclose(scores[idx], meta.predict_disorder(seqs[k], return_numpy=True), atol=0.0001)
+
+
+
+        
+
```

### Comparing `metapredict-2.51/metapredict/tests/test_uniprot_functionality.py` & `metapredict-2.61/metapredict/tests/test_uniprot_functionality.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
 
     # checks that when we pull p53 we get 393 residues of sweet,
     # sweet disorder prediction
     assert len(meta.predict_disorder_uniprot(P53_UID)) == 393
 
     # check summed disorder is right
-    assert np.sum(meta.predict_disorder_uniprot(P53_UID)) == 181.7708
+    assert np.isclose(np.sum(meta.predict_disorder_uniprot(P53_UID)),181.7708, 0.0001)
 
     # check legacy disorder is right
-    assert np.sum(meta.predict_disorder_uniprot(P53_UID, legacy=True)) == 172.9651
+    assert np.isclose(np.sum(meta.predict_disorder_uniprot(P53_UID, legacy=True)),  172.9651, 0.0001)
 
     # check summed disorder is right when we don't normalize (these are not magic values,
     # just the expected 'truth' for the 1.0 release
-    assert np.isclose(np.sum(meta.predict_disorder_uniprot(P53_UID, normalized=False, legacy=True)),173.5245)
+    assert np.isclose(np.sum(meta.predict_disorder_uniprot(P53_UID, normalized=False, legacy=True)),173.5245, 0.0001)
 
 
 # ....................................................................................
 #
 def test_graph_disorder_uniprot_():
 
     # checks that this fails when an invalid uniprot accession is passed
@@ -69,15 +69,15 @@
 
 
     # checks that when we pull p53 we get 393 residues of sweet,
     # sweet disorder prediction
 
     dis_domains = meta.predict_disorder_domains_uniprot(P53_UID) 
     assert len(dis_domains.sequence) == 393
-    assert np.sum(dis_domains.disorder) == 181.7708
+    assert np.isclose(np.sum(dis_domains.disorder), 181.7708, 0.001)
 
     # did we find 2 IDRs
     assert len(dis_domains.disordered_domains) == 2
 
     # get IDRs
     IDRs = dis_domains.disordered_domains
     #get idr boundaries
```

### Comparing `metapredict-2.51/metapredict/tests/test_write_fasta.py` & `metapredict-2.61/metapredict/tests/test_write_fasta.py`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/metapredict.egg-info/SOURCES.txt` & `metapredict-2.61/metapredict.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,48 +42,60 @@
 metapredict/parameters.py
 metapredict.egg-info/PKG-INFO
 metapredict.egg-info/SOURCES.txt
 metapredict.egg-info/dependency_links.txt
 metapredict.egg-info/requires.txt
 metapredict.egg-info/top_level.txt
 metapredict/backend/.DS_Store
+metapredict/backend/batch_predict.py
 metapredict/backend/brnn_architecture.py
 metapredict/backend/data_structures.py
 metapredict/backend/domain_definition.py
 metapredict/backend/encode_sequence.py
 metapredict/backend/meta_graph.py
 metapredict/backend/meta_predict_disorder.py
 metapredict/backend/meta_tools.py
 metapredict/backend/metameta_hybrid_predict.py
 metapredict/backend/py_predictor_v2.py
 metapredict/backend/uniprot_predictions.py
+metapredict/backend/cython/domain_definition.c
+metapredict/backend/cython/domain_definition.pyx
 metapredict/backend/networks/.DS_Store
 metapredict/backend/networks/metaDisorder.pt
 metapredict/backend/networks/meta_predict_disorder_100e_v1.pt
 metapredict/backend/networks/metameta_2_7_22_nl2_hs20_b32_V3.pt
 metapredict/backend/networks/metapredict_network_v2_200epochs_nl1_hs20.pt
 metapredict/backend/networks/metapredict_network_v3_200epochs_nl2_hs20.pt
 metapredict/data/README.md
 metapredict/data/test_data.fasta
 metapredict/tests/.DS_Store
 metapredict/tests/__init__.py
 metapredict/tests/local_data.py
+metapredict/tests/pytest.ini
+metapredict/tests/test_batch_vs_single.py
+metapredict/tests/test_cython_v_python.py
 metapredict/tests/test_domain_functions.py
 metapredict/tests/test_graph_disorder.py
 metapredict/tests/test_graph_fasta.py
 metapredict/tests/test_metapredict.py
 metapredict/tests/test_uniprot_functionality.py
 metapredict/tests/test_write_fasta.py
+metapredict/tests/cli_tests/__init__.py
+metapredict/tests/cli_tests/test_metapredict-predict-disorder.py
+metapredict/tests/cli_tests/test_metapredict-predict-idrs.py
+metapredict/tests/cli_tests/input/three_seqs.fasta
 metapredict/tests/input_data/DisorderPredictionssp_P04637_P53_HUMANC.txt
+metapredict/tests/input_data/build_data.ipynb
+metapredict/tests/input_data/test_scores_100.npy
+metapredict/tests/input_data/test_seqs_100.fasta
 metapredict/tests/input_data/testing.fasta
 metapredict/tests/input_data/three_seqs.fasta
 metapredict/tests/output/test.csv
 scripts/metapredict-graph-disorder
 scripts/metapredict-graph-pLDDT
-scripts/metapredict-multipredict
 scripts/metapredict-name
 scripts/metapredict-predict-disorder
 scripts/metapredict-predict-idrs
 scripts/metapredict-predict-pLDDT
 scripts/metapredict-quick-graph
 scripts/metapredict-quick-predict
 scripts/metapredict-uniprot
```

### Comparing `metapredict-2.51/readthedocs.yml` & `metapredict-2.61/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-graph-disorder` & `metapredict-2.61/scripts/metapredict-graph-disorder`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-graph-pLDDT` & `metapredict-2.61/scripts/metapredict-graph-pLDDT`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-name` & `metapredict-2.61/scripts/metapredict-name`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-predict-disorder` & `metapredict-2.61/scripts/metapredict-predict-disorder`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-predict-pLDDT` & `metapredict-2.61/scripts/metapredict-predict-pLDDT`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-quick-graph` & `metapredict-2.61/scripts/metapredict-quick-graph`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-quick-predict` & `metapredict-2.61/scripts/metapredict-quick-predict`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/scripts/metapredict-uniprot` & `metapredict-2.61/scripts/metapredict-uniprot`

 * *Files identical despite different names*

### Comparing `metapredict-2.51/versioneer.py` & `metapredict-2.61/versioneer.py`

 * *Files identical despite different names*

