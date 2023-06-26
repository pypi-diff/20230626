# Comparing `tmp/earthcube_utilities-0.1.14.tar.gz` & `tmp/earthcube_utilities-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthcube_utilities-0.1.14.tar", last modified: Thu Apr 13 19:48:49 2023, max compression
+gzip compressed data, was "earthcube_utilities-0.1.15.tar", last modified: Mon Jun 26 16:38:59 2023, max compression
```

## Comparing `earthcube_utilities-0.1.14.tar` & `earthcube_utilities-0.1.15.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.335801 earthcube_utilities-0.1.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-13 19:48:49.000000 earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/ec/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/check_sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/ec/collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/collection/rocrate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/collection/rocrate_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/ec/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/datastore/s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2799 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/generate_graph_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/ec/gleanerio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/gleanerio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/gleanerio/gleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.339801 earthcube_utilities-0.1.14/src/ec/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/manageGraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.343801 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_types_top_level.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_graph_sizes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/org_all_org_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/org_all_returns_properties.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/org_all_returns_urns.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_graph_sizes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/select_one.sparql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/sparql_static/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/graph/sparql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/logger/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/missing_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/notebook/geocodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/notebook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/ec_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/ecobjectmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/objects/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/query_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/reporting/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/sitemap/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sitemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sitemap/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/sos_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sos_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sos_json/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/sos_json/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sos_json/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/sos_json/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:48:49.347801 earthcube_utilities-0.1.14/src/ec/summarize/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-13 19:48:37.000000 earthcube_utilities-0.1.14/src/ec/summarize/summarize_materializedview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.480760 earthcube_utilities-0.1.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/check_sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/rocrate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/rocrate_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/datastore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/ec_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/generate_graph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/gleanerio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/gleanerio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/gleanerio/gleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/manageGraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_types_top_level.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_org_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_urns.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_types_top_level.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/select_one.sparql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/logger/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/missing_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/geocodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/ec_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/ecobjectmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/query_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sitemap/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sitemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sitemap/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sos_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sos_json/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/src/ec/summarize/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize/summarize_materializedview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize_identifier_metadata.py
```

### Comparing `earthcube_utilities-0.1.14/PKG-INFO` & `earthcube_utilities-0.1.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: earthcube_utilities
-Version: 0.1.14
+Version: 0.1.15
 Summary: A package of utilities for NSF Earthcube Geocodes Project
-Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
-Maintainer-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
+Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>, Ya-Lan Yang <ylyang@illinois.edu>
+Maintainer-email: Ya-Lan Yang <ylyang@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,16 +16,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Earthcube Utilities
 
 
+## Users
 
-## Proposed use
 ### Earthcube Utilities:
 https://pypi.org/project/earthcube-utilities/
 
 
 ### Manual Install
 `python3 -m pip install  earthcube-utilities`
```

### Comparing `earthcube_utilities-0.1.14/README.md` & `earthcube_utilities-0.1.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Earthcube Utilities
 
 
+## Users
 
-## Proposed use
 ### Earthcube Utilities:
 https://pypi.org/project/earthcube-utilities/
 
 
 ### Manual Install
 `python3 -m pip install  earthcube-utilities`
```

### Comparing `earthcube_utilities-0.1.14/pyproject.toml` & `earthcube_utilities-0.1.15/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "earthcube_utilities"
-version = "0.1.14"
+version = "0.1.15"
 dynamic = ["dependencies"]
 description = "A package of utilities for NSF Earthcube Geocodes Project"
 readme =  "README.md"
 
 authors = [
     {name = "Mike Bobak", email = "mbobak@illinois.edu"},
-    {name= "David Valentine", email="dwvalentine@ucsd.edu"}
+    {name= "David Valentine", email="dwvalentine@ucsd.edu"},
+    {name = "Ya-Lan Yang", email = "ylyang@illinois.edu"}
 ]
 maintainers = [
-    {name = "Mike Bobak", email = "mbobak@illinois.edu"},
+    {name = "Ya-Lan Yang", email = "ylyang@illinois.edu"},
     {name= "David Valentine", email="dwvalentine@ucsd.edu"}
 ]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -33,14 +34,15 @@
 # if the name of the module is the same as the name of the script, then you get
 #    'module' object is not callable
 [project.scripts]
 generategraphstats = "ec.generate_graph_stats:start"
 check_sitemap = "ec.check_sitemap:start"
 query_graph = "ec.query_graph:start"
 missing_report = "ec.missing_report:start"
+summarize_identifier_metadata = "ec.summarize_identifier_metadata:start"
 
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
```

### Comparing `earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/PKG-INFO` & `earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: earthcube-utilities
-Version: 0.1.14
+Version: 0.1.15
 Summary: A package of utilities for NSF Earthcube Geocodes Project
-Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
-Maintainer-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
+Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>, Ya-Lan Yang <ylyang@illinois.edu>
+Maintainer-email: Ya-Lan Yang <ylyang@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,16 +16,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Earthcube Utilities
 
 
+## Users
 
-## Proposed use
 ### Earthcube Utilities:
 https://pypi.org/project/earthcube-utilities/
 
 
 ### Manual Install
 `python3 -m pip install  earthcube-utilities`
```

### Comparing `earthcube_utilities-0.1.14/src/earthcube_utilities.egg-info/SOURCES.txt` & `earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 src/earthcube_utilities.egg-info/PKG-INFO
 src/earthcube_utilities.egg-info/SOURCES.txt
 src/earthcube_utilities.egg-info/dependency_links.txt
 src/earthcube_utilities.egg-info/entry_points.txt
 src/earthcube_utilities.egg-info/requires.txt
 src/earthcube_utilities.egg-info/top_level.txt
 src/ec/check_sitemap.py
+src/ec/ec_reports.py
 src/ec/generate_graph_stats.py
 src/ec/missing_report.py
 src/ec/query_graph.py
+src/ec/summarize_identifier_metadata.py
 src/ec/collection/__init__.py
 src/ec/collection/rocrate_archive.py
 src/ec/collection/rocrate_collection.py
 src/ec/datastore/__init__.py
 src/ec/datastore/s3.py
 src/ec/gleanerio/__init__.py
 src/ec/gleanerio/gleaner.py
@@ -49,14 +51,15 @@
 src/ec/graph/sparql_files/repo_count_datasets.sparql
 src/ec/graph/sparql_files/repo_count_graphs.sparql
 src/ec/graph/sparql_files/repo_count_keywords.sparql
 src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
 src/ec/graph/sparql_files/repo_count_triples.sparql
 src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
 src/ec/graph/sparql_files/repo_count_types.sparql
+src/ec/graph/sparql_files/repo_count_types_top_level.sparql
 src/ec/graph/sparql_files/repo_count_variablename.sparql
 src/ec/graph/sparql_files/repo_graph_sizes.sparql
 src/ec/graph/sparql_files/repo_graphs_startwith.sparql
 src/ec/graph/sparql_files/repo_select_datasets.sparql
 src/ec/graph/sparql_files/repo_select_graphs.sparql
 src/ec/graph/sparql_files/repo_summary_query.sparql
 src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
```

### Comparing `earthcube_utilities-0.1.14/src/ec/check_sitemap.py` & `earthcube_utilities-0.1.15/src/ec/check_sitemap.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/collection/rocrate_collection.py` & `earthcube_utilities-0.1.15/src/ec/collection/rocrate_collection.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/datastore/s3.py` & `earthcube_utilities-0.1.15/src/ec/datastore/s3.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import json
+from datetime import datetime
 from io import BytesIO
 
 import minio
+import pandas
 import pydash
+from minio.commonconfig import CopySource, REPLACE
 from pydash.collections import find
 
 def shaFroms3Path(path, extension=None):
     split = path.split("/")
     sha = split[len(split)-1]
     if extension is not None:
         sha = pydash.strings.replace_end(sha, extension, '')
@@ -35,25 +39,36 @@
         self.default_bucket = default_bucket
 
     def listPath(self, bucket, path, include_user_meta=False):
         pass
     def countPath(self, bucket, path):
         count = len(list(self.listPath(bucket,path)))
 
+    def DataframeFromPath(self, bucket, path, include_user_meta=False):
+        pass
 # who knows, we might implement on disk, or in a database. This just separates the data from the annotated metadata
     def getFileFromStore(self, s3ObjectInfo):
         pass
     def getFileMetadataFromStore(self, s3ObjectInfo):
         pass
     def putTextFileToStore(self,data, s3ObjectInfo ):
         f = BytesIO()
         length = f.write(bytes(data, 'utf-8'))
         f.seek(0)
         resp = self.s3client.put_object(s3ObjectInfo.bucket_name, s3ObjectInfo.object_name, f,length=length)
         return resp.bucket_name, resp.object_name
+    def copyObject(self,s3ObjectInfoToCopy, ObjectPath ):
+        ''' Server Side Copy, eg upload report to latest, make copy to today'''
+        self.s3client.copy_object(
+            s3ObjectInfoToCopy.bucket_name,
+            ObjectPath,
+            CopySource(s3ObjectInfoToCopy.bucket_name, s3ObjectInfoToCopy.object_name),
+           # metadata=metadata,
+            metadata_directive=REPLACE,
+        )
 
     #### Methods for a getting information using infrastructure information
 
     """ Method for gleaner store"""
     def listJsonld(self,bucket, repo,include_user_meta=False):
         """ urllist returns list of urn;s with urls"""
         # include user meta not working.
@@ -120,15 +135,16 @@
 
     def listReportFile(self,bucket, repo,include_user_meta=False):
         """ urllist returns list of urn;s with urls"""
         # include user meta not working.
         path = f"{self.paths['report']}/{repo}/"
         return self.listPath(bucket, path,include_user_meta=include_user_meta)
 
-    def putReportFile(self, bucket, repo, filename, json_str, date="latest"):
+    def putReportFile(self, bucket, repo, filename, json_str,  date="latest", copy_to_date=True):
+
         pass
 
     def getReportFile(self, bucket, repo, filename):
         path = f"{self.paths['report']}/{repo}/filename"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         resp = self.getFileFromStore(s3ObjectInfo)
         return resp
@@ -194,33 +210,49 @@
         """ get an s3 file from teh store
         Parameters:
           s3ObjectInfo: {"bucket_name":obj.bucket_name, "object_name":obj.object_name }
 
         """
         resp = self.s3client.get_object(s3ObjectInfo["bucket_name"], s3ObjectInfo["object_name"])
         return resp.data
+    def DataframeFromPath(self, bucket, path, include_user_meta=False):
+        pathFiles = list(self.listPath(bucket,path,include_user_meta=include_user_meta))
+
+        objs = map(lambda f: self.s3client.stat_object(f.bucket_name, f.object_name), pathFiles)
+        data = map(lambda f: { "metadata": f.metadata, "bucket_name":f.bucket_name, "object_name":f.object_name}, objs )
+        # does not work... should, but does not
+        # data = list(map(lambda f:
+        #                 pick(f,  'bucket_name', 'object_name')
+        #                 , objs ))
+
+        df = pandas.DataFrame(data=data)
+        return df
 
     def getFileMetadataFromStore(self, s3ObjectInfo):
         """ get metadata s3 file from teh store
                Parameters:
                  s3ObjectInfo: {"bucket_name":obj.bucket_name, "object_name":obj.object_name }
 
                """
         s3obj = self.s3client.stat_object(s3ObjectInfo.bucket_name, s3ObjectInfo.object_name)
         for o in s3obj:
             user_meta = pydash.collections.filter_(o,lambda m: m.startswith("X-Amz-Meta") )
         # this needs to return the metadata
         return user_meta
 
-    def putReportFile(self, bucket, repo, filename, json_str, date="latest"):
+    def putReportFile(self, bucket, repo, filename, json_str, date="latest", copy_to_date=True):
         path = f"{self.paths['report']}/{repo}/{date}/{filename}"
         f = BytesIO()
         length = f.write(bytes(json_str, 'utf-8'))
         f.seek(0)
         resp = self.s3client.put_object(bucket, path, f,length=length)
+        if copy_to_date:
+            today_str = datetime.now().strftime("%Y%m%d")
+            path = f"{self.paths['report']}/{repo}/{today_str}/{filename}"
+            self.copyObject(resp,path)
         return resp.bucket_name, resp.object_name
 
     def getReportFile(self, bucket, repo, filename):
         path = f"{self.paths['report']}/{repo}/{filename}"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         resp = self.getFileFromStore(s3ObjectInfo)
         return resp
```

### Comparing `earthcube_utilities-0.1.14/src/ec/generate_graph_stats.py` & `earthcube_utilities-0.1.15/src/ec/generate_graph_stats.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,35 +12,40 @@
 
 log = config_app()
 
 def graphStats(args):
     """query an endpoint, store results as a json file in an s3 store"""
     log.info(f"Querying {args.graphendpoint} for graph statisitcs  ")
 ### more work needed before detailed works
-    if args.repo == "all":
+    if args.source == "all":
          # report_json = generateGraphReportsRepo("all",
          #      args.graphendpoint, reportTypes=reportTypes)
 
         if (args.detailed):
             report_json = generateGraphReportsRepo("all", args.graphendpoint, reportList=reportTypes["all_detailed"] )
         else:
             report_json = generateGraphReportsRepo("all",
                                                        args.graphendpoint,reportList=reportTypes["all"])
     else:
         # report_json = generateGraphReportsRepo(args.repo,
         #   args.graphendpoint,reportTypes=reportTypes)
 
         if (args.detailed):
-            report_json = generateGraphReportsRepo(args.repo, args.graphendpoint,reportList=reportTypes["repo_detailed"] )
+            report_json = generateGraphReportsRepo(args.source, args.graphendpoint,reportList=reportTypes["repo_detailed"] )
         else:
-            report_json = generateGraphReportsRepo(args.repo,
+            report_json = generateGraphReportsRepo(args.source,
                                                        args.graphendpoint, reportList=reportTypes["repo"] )
     s3Minio = s3.MinioDatastore( args.s3server, None)
     #data = f.getvalue()
-    bucketname, objectname = s3Minio.putReportFile(args.s3bucket,args.repo,"graph_report.json",report_json)
+
+    if (args.output):  # just append the json files to one filem, for now.
+        logging.info(f" report for {args.source} appended to file")
+        args.output.write(report_json)
+    if not args.no_upload:
+        bucketname, objectname = s3Minio.putReportFile(args.s3bucket,args.source,"graph_report.json",report_json)
     return 0
 def start():
     """
         Run the generate_repo_stats program.
         query an endpoint, store results as a json file in an s3 store.
         Arguments:
             args: Arguments passed from the command line.
@@ -51,19 +56,23 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('--graphendpoint', dest='graphendpoint',
                         help='graph endpoint' ,default="https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/")
     parser.add_argument('--s3', dest='s3server',
                         help='s3 server address (localhost:9000)', default='localhost:9000')
     parser.add_argument('--s3bucket', dest='s3bucket',
                         help='s3 server address (localhost:9000)', default='gleaner')
-    parser.add_argument('--repo', dest='repo',
+    parser.add_argument('--source', dest='source',
                         help='repository', default='all')
 
     parser.add_argument("--detailed",action='store_true',
                         dest="detailed" ,help='run the detailed version of the reports', default=False)
+    parser.add_argument('--no_upload', dest = 'no_upload',action='store_true', default=False,
+                        help = 'do not upload to s3 bucket ')
+    parser.add_argument('--output',  type=argparse.FileType('w'), dest="output", help="dump to file")
 
     args = parser.parse_args()
 
     exitcode = graphStats(args)
+    exit(exitcode)
 
 if __name__ == '__main__':
     start()
```

### Comparing `earthcube_utilities-0.1.14/src/ec/gleanerio/gleaner.py` & `earthcube_utilities-0.1.15/src/ec/gleanerio/gleaner.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/manageGraph.py` & `earthcube_utilities-0.1.15/src/ec/graph/manageGraph.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_repo_count_graphs.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_graphs.sparql`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## double dollar signes are to escape to a single dollar sign when using string template
 ## Graphs do not always equal datasets. Especially in non-Earthcube graph stores
 SELECT   ?repo (COUNT(distinct ?g) as ?graphs) (COUNT(*) as ?triples)
 WHERE     {
   GRAPH ?g {
       ?s ?p ?o .
-      bind(  REPLACE(REPLACE( STR(?g) ,"urn:(?:\\w+):?(?:\\w+)?:" ,"" ), ":\\w+$$" , "")   as ?repo )
+       bind(  REPLACE(REPLACE( STR(?g) ,"urn:(?:\\w+):" ,"" ), ":\\w+$$" , "")   as ?repo )
    }
 }
 group by ?repo
 
 ## the regesx replace grabs the first portioon, replaces it with nothing,
 ## then grabs the last part and replaces it with nothing,
 ## NOTE: double \\ the escape sequeqnce akd \w+ becomes \\w+
 #((\w+):(\w+))$$
 #(?2)(:(\w+))
 
 ##<urn:gleaner:summoned:opentopography:0024e35144d902d8b413ffd400ede6a27efe2146>
 # urn:\w+:summoned:(\w+)
-#urn:(?:\w+):summoned:(\w+)
+#urn:(?:\w+):summoned:(\w+)
```

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_summary_query.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_summary_query.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/org_all_returns_properties.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_properties.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/repo_summary_query.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_summary_query.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/graph/sparql_query.py` & `earthcube_utilities-0.1.15/src/ec/graph/sparql_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,13 +57,13 @@
     files = filter( lambda f: ends_with(f, ".sparql"), resource)
     files = map(lambda f: replace_end(f,".sparql",""), files)
     files = sort(list(files))
     return files
 
 def getAGraph(  g, endpoint: str) -> pandas.DataFrame:
     """Query a SPARQL endpoint and return a Pandas Dataframe for a geocodes object"""
-    query = _getSparqlFileFromResources('get_triples_for_a_graph')
+    query = _getSparqlFileFromResources('urn_triples_for_a_graph')
     q_template = Template(query)
     thsGraphQuery = q_template.substitute(urn=g)
     g_df = sparqldataframe.query(endpoint, thsGraphQuery)
 
-    return g_df
+    return g_df
```

### Comparing `earthcube_utilities-0.1.14/src/ec/logger/log.py` & `earthcube_utilities-0.1.15/src/ec/logger/log.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/missing_report.py` & `earthcube_utilities-0.1.15/src/ec/missing_report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,85 @@
 #!  python3
-import argparse
+import click
 import logging
 import json
 import sys
 
+from pydash.collections import find
 from pydash import is_empty
 from ec.gleanerio.gleaner import getSitemapSourcesFromGleaner, getGleaner
 from ec.reporting.report import missingReport
 from ec.datastore import s3
 
-def writeMissingReport(args):
-    if (args.cfgfile):
-        s3endpoint,  bucket, glnr= getGleaner(args.cfgfile)
+@click.command()
+@click.option('--cfgfile', help='gleaner config file', type=click.Path(exists=True))
+@click.option('--graphendpoint', help='graph endpoint'
+              )
+# no default for s3 parameters here. read from gleaner. if provided, these override the gleaner config
+@click.option('--s3server', help='s3 server address')
+@click.option('--s3bucket', help='s3 bucket')
+@click.option('--no_upload', help='do not upload to s3 bucket',is_flag=True, default=False)
+@click.option('--output', help='dump to file', type=click.File('wb'))
+@click.option('--source', help='gone or more repositories (--source a --source b)', multiple=True)
+@click.option('--milled', help='include milled', is_flag=True,default=False)
+@click.option('--summon', help='check summon only',is_flag=True, default=False)
+
+def writeMissingReport(cfgfile, graphendpoint, s3server, s3bucket, no_upload, output, source, milled, summon):
+    if cfgfile:
+        s3endpoint, bucket, glnr = getGleaner(cfgfile)
         minio = glnr.get("minio")
         # passed paramters override the config parameters
-        s3server = args.s3server if args.s3server  else  s3endpoint
-        bucket = args.s3bucket if args.s3bucket else bucket
+        s3server = s3server if s3server else s3endpoint
+        bucket = s3bucket if s3bucket else bucket
     else:
-        s3server = args.s3server
-        bucket = args.s3bucket
-    graphendpoint = args.graphendpoint  # not in gleaner file, at present
-    if is_empty(graphendpoint) or is_empty(s3server) or is_empty(bucket):
-        logging.fatal(f" must provide graphendpoint and [a gleaner config or (s3endpoint and s3bucket)]")
+        s3server = s3server
+        bucket = s3bucket
+    graphendpoint = graphendpoint  # not in gleaner file, at present
+    if is_empty(s3server) or is_empty(bucket):
+        logging.fatal(f" must provide a gleaner config or (s3endpoint and s3bucket)]")
+        return 1
+    if is_empty(graphendpoint) and not summon:
+        logging.fatal(f" must provide graphendpoint if you are checking milled")
         return 1
     logging.info(f" s3server: {s3server} bucket:{bucket} graph:{graphendpoint}")
     s3Minio = s3.MinioDatastore(s3server, None)
-    sources = getSitemapSourcesFromGleaner(args.cfgfile)
+    sources = getSitemapSourcesFromGleaner(cfgfile)
     sources = list(filter(lambda source: source.get('active'), sources))
+    sources_to_run = source  # optional if null, run all
 
     for i in sources:
-        url = i.get('url')
-        repo = i.get('name')
-
+        source_url = i.get('url')
+        source_name = i.get('name')
+        if sources_to_run is not None and len(sources_to_run) >0:
+            if not find (sources_to_run, lambda x: x == source_name ):
+                continue
         try:
-            report = missingReport(url, bucket, repo, s3Minio, graphendpoint)
+            report = missingReport(source_url, bucket, source_name, s3Minio, graphendpoint, milled=milled, summon=summon)
             report = json.dumps(report,  indent=2)
-            if (args.output): # just append the json files to one filem, for now.
-                logging.info(f" report for {repo} appended to file")
-                args.output.write(report)
-            if not args.no_upload:
-                s3Minio.putReportFile(bucket, repo, "missing_report.json", report)
+            if output:  # just append the json files to one filem, for now.
+                logging.info(f" report for {source_name} appended to file")
+                output.write(report)
+            if not no_upload:
+                s3Minio.putReportFile(bucket, source_name, "missing_report.json", report)
         except Exception as e:
-            logging.error(f"could not write missing report for {repo} to s3server:{s3server}:{bucket} error:{e}", repo,s3server,bucket, e)
-            return 1
+            logging.error(f"could not write missing report for {source_name} to s3server:{s3server}:{bucket} error:{e}",
+                          source_name, s3server, bucket, e)
     return 0
 
+
 def start():
     """
         Run the write_missing_report program.
         Get a list of active repositories from the gleaner file.
         For each repository, generate missing reports and write these information to a json file and upload it to s3.
         Arguments:
             args: Arguments passed from the command line.
         Returns:
             An exit code.
     """
-    parser = argparse.ArgumentParser()
-    # source of sources, and default s3 store.
-    #   at present, graph endpoint is no longer in gleaner
-    parser.add_argument('--cfgfile', dest='cfgfile',
-                        help='gleaner config file', default='gleaner')
-    parser.add_argument('--graphendpoint', dest = 'graphendpoint',
-                        help = 'graph endpoint', default = "https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/")
-# no default for s3 parameters here. read from gleaner. if provided, these override the gleaner config
-    parser.add_argument('--s3', dest = 's3server',
-                        help = 's3 server address ')
-    parser.add_argument('--s3bucket', dest = 's3bucket',
-                        help = 's3 bucket ')
-    parser.add_argument('--no_upload', dest = 'no_upload',action='store_true', default=False,
-                        help = 'do not upload to s3 bucket ')
-    parser.add_argument('--output',  type=argparse.FileType('w'), dest="output", help="dump to file")
-
-
-    args = parser.parse_args()
-    exitcode = writeMissingReport(args)
+    exitcode = writeMissingReport()
     sys.exit(exitcode)
 
+
 if __name__ == '__main__':
     start()
+
```

### Comparing `earthcube_utilities-0.1.14/src/ec/notebook/utils.py` & `earthcube_utilities-0.1.15/src/ec/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/objects/ecobjectmanager.py` & `earthcube_utilities-0.1.15/src/ec/objects/ecobjectmanager.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/query_graph.py` & `earthcube_utilities-0.1.15/src/ec/query_graph.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/reporting/report.py` & `earthcube_utilities-0.1.15/src/ec/reporting/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import logging
 from datetime import date, datetime
+import time
+from typing import Any
 
 import pandas
 import pydash
 
 import ec.sitemap
 from ec.graph.sparql_query import queryWithSparql
 
@@ -64,40 +66,54 @@
 
 """
 def get_url_from_sha_list(shas: list,  bucket, repo, datastore: bucketDatastore):
     """if a repo has issues with milling or loading to a graph, then get the summoned file"""
 
     pass
 
-def missingReport(valid_sitemap_url :str , bucket, repo, datastore: bucketDatastore, graphendpoint, milled=True):
+def missingReport(valid_sitemap_url :str , bucket, repo, datastore: bucketDatastore, graphendpoint, milled=True, summon=False):
     today = date.today().strftime("%Y-%m-%d")
-    response = {"repo":repo,"graph":graphendpoint,"sitemap":valid_sitemap_url,
+    response = {"source":repo,"graph":graphendpoint,"sitemap":valid_sitemap_url,
                 "date": today, "bucket": bucket, "s3store": datastore.endpoint }
+    t = time.time()
     sitemap = ec.sitemap.Sitemap(valid_sitemap_url)
     sitemap_urls = sitemap.uniqueUrls()
+    response["sitemap_geturls_time"] = time.time() - t
     sitemap_count = pydash.collections.size(sitemap_urls)
+    t = time.time()
     summoned_list = datastore.listSummonedUrls(bucket, repo)
+    response["s3_geturls_time"] = time.time() - t
     summoned_count = pydash.collections.size(summoned_list)
     summoned_urls = list(map(lambda s: s.get("url"), summoned_list))
     dif_sm_summon = pydash.arrays.difference(sitemap_urls, summoned_urls)
     response["sitemap_count"] = sitemap_count
     response["summoned_count"] = summoned_count
+    response["missing_sitemap_summon_count"] = len(dif_sm_summon)
     response["missing_sitemap_summon"] = dif_sm_summon
+    if summon:
+        return response
     ##### summmon to graph
+    t = time.time()
     summoned_sha_list = datastore.listSummonedSha(bucket, repo)
+    response["summon_list_s3_sha_time"] = time.time() - t
+    t = time.time()
     graph_urns = ec.graph.sparql_query.queryWithSparql("repo_select_graphs", graphendpoint, {"repo": repo})
     graph_shas = list(map(lambda u: pydash.strings.substr_right_end(u, ":"), graph_urns['g']))
+    response["graph_sha_urn_time"] = time.time() - t
     dif_summon_graph = pydash.arrays.difference(summoned_sha_list, graph_shas)
-    response["milled_count"] = pydash.collections.size(graph_shas)
+    response["graph_urn_count"] = pydash.collections.size(graph_shas)
+    response["missing_summon_graph_count"] = len(dif_summon_graph)
     response["missing_summon_graph"] = dif_summon_graph
     if milled:
+        t = time.time()
         milled_list = datastore.listMilledSha(bucket, repo)
-
+        response["milled_sha_time"] = time.time() - t
         dif_summon_milled = pydash.arrays.difference(summoned_sha_list, milled_list)
         response["milled_count"] = pydash.collections.size(milled_list)
+        response["missing_summon_milled"] = len(dif_summon_milled)
         response["missing_summon_milled"] = dif_summon_milled
     return response
 
 def compareSitemap2Summoned(valid_sitemap_url :str , bucket, repo, datastore: bucketDatastore):
     #Grab list of metadater-Url from Datastore, ec.datastore.s3.listSummonedUrls
     sitemap = ec.sitemap.Sitemap(valid_sitemap_url)
     sitemap_urls = sitemap.uniqueUrls()
@@ -137,51 +153,43 @@
     return {
         "summoned_count": pydash.collections.size(summoned_list),
         "milled_count": pydash.collections.size(graph_shas),
             "missing": difference
             }
 
 
-def putProcessingReports4Repo(repo, date,  json_str, datastore: bucketDatastore, reportname='processing.json',):
-    """put reports about the processing into reports store
-    this should be items like the sitemap count, summoned counts, and 'milled' counts if apprporate"""
-    # store twice. latest and date
-    bucket_name, object_name= bucketDatastore.putReportFile(datastore.default_bucket, repo, reportname, json_str, date=date)
-    # might return a url...
-    return bucket_name, object_name
-
 ##################################
 #  REPORT GENERATION USING SPARQL QUERIES
 #   this uses defined spaql queries to return counts for reports
 ###################################
 reportTypes = {
     "all": [
         {"code": "triple_count", "name": "all_count_triples"},
             {"code": "graph_count_by_repo", "name": "all_repo_count_graphs"},
         {"code": "dataset_count", "name": "all_count_datasets"},
         {"code": "dataset_count_by_repo", "name": "all_repo_count_datasets"},
+        {"code": "types_count", "name": "all_count_types"},
+        {"code": "types_count_by_repo", "name": "all_repo_count_types"},
         {"code": "mutilple_version_count", "name": "all_count_multiple_versioned_datasets"},
         {"code": "mutilple_version_count_by_repo", "name": "all_repo_count_versioned_datasets"},
         {"code": "repos_with_keywords", "name": "all_repo_with_keywords"},
-        {"code": "types_count", "name": "all_count_types"},
-        {"code": "types_count_by_repo", "name": "all_repo_count_types"},
-     ],
+    ],
     # add the triple count by graph, and graph sizes
     # this will need to be added, managed in the generate_graph
     # add a basic by default, detailed if requested with a flag
     "all_detailed": [
         {"code": "triple_count", "name": "all_count_triples"},
         {"code": "graph_count_by_repo", "name": "all_repo_count_graphs"},
         {"code": "dataset_count", "name": "all_count_datasets"},
-        {"code": "dataset_count_by_repo", "name": "all_repo_count_dataset"},
+        {"code": "dataset_count_by_repo", "name": "all_repo_count_datasets"},
+        {"code": "types_count", "name": "all_count_types"},
+        {"code": "types_count_by_repo", "name": "all_repo_count_types"},
         {"code": "mutilple_version_count", "name": "all_count_multiple_versioned_datasets"},
         {"code": "mutilple_version_count_by_repo", "name": "all_repo_count_versioned_datasets"},
         {"code": "keywords_counts_by_repo", "name": "all_repo_count_keywords"},
-
-        {"code": "types_count", "name": "all_count_types"},
         {"code": "keywords_count", "name": "all_count_keywords"},
         {"code": "variablename_count", "name": "all_count_variablename"},
         {"code": "graph_sizes", "name": "all_graph_sizes"},
 
     ],
     "repo": [
         {"code": "triple_count", "name": "repo_count_triples"},
@@ -211,46 +219,52 @@
 def _get_report_type(reports, code) -> str:
     report = pydash.find(reports, lambda r: r["code"] == code)
     return report["name"]
 
 ##  for the 'object reports, we should have a set.these could probably be make a set of methos with (ObjectType[triples,keywords, types, authors, etc], repo, endpoint/datastore)
 def generateGraphReportsRepo(repo, graphendpoint, reportList=reportTypes["all"]) -> str:
     current_dateTime = datetime.now().strftime("%Y-%m-%d")
-    reports = map (lambda r:   {"report": r["code"],
-                                "data": generateAGraphReportsRepo(repo, r["code"],
-                                 graphendpoint, reportList).to_dict('records')
-                                   }   ,
+    reports = map (lambda r:    generateAGraphReportsRepo(repo, r,
+                                 graphendpoint, reportList)
+                                      ,
                                 reportList)
 
     reports = list(reports)
     return json.dumps({"version": 0, "repo": repo, "date": current_dateTime, "reports": reports }, indent=4)
 
-def generateAGraphReportsRepo(repo, code, graphendpoint, reportList) -> pandas.DataFrame:
+
+def generateAGraphReportsRepo(repo, r, graphendpoint, reportList) -> Any:
     #queryWithSparql("repo_count_types", graphendpoint)
     parameters = {"repo": repo}
     try:
-        report =   queryWithSparql(_get_report_type(reportList, code), graphendpoint, parameters=parameters)
-
-        return report
+        t = time.time()
+        report =   queryWithSparql(_get_report_type(reportList, r['code']), graphendpoint, parameters=parameters)
+        elapsed_time = time.time() - t
+        data = report.to_dict('records')
+        return  {"report": r["code"],
+                 "processing_time": elapsed_time,
+                 "length": len(data),
+         "data": report.to_dict('records')
+         }
     except Exception as ex:
-        logging.error(f"query with sparql failed: report:{code}  repo:{repo}   {ex}")
-        return pandas.DataFrame()
+        logging.error(f"query with sparql failed: report:{r['code']}  repo:{repo}   {ex}")
+        elapsed_time = time.time() - t
+        return {"report": r["code"],
+                "errpr": f"{ex}",
+                 "processing_time": elapsed_time,
+         "data": []
+         }
 
 def getGraphReportsLatestRepoReports(repo,  datastore: bucketDatastore):
     """get the latest for a dashboard"""
     date="latest"
     path = f"{datastore.paths['reports']}/{repo}/{date}/sparql.json"
     filelist = datastore.getReportFile(datastore.default_bucket, repo, path)
 
 def listGraphReportDates4Repo(repo,  datastore: bucketDatastore):
     """get the latest for a dashboard"""
     path = f"{datastore.paths['reports']}/{repo}/"
     filelist = datastore.listPath(path)
     return filelist
 
-def putGraphReports4RepoReport(repo, json_str, datastore: bucketDatastore, date='latest', reportname='sparql.json'):
-    """put the latest for a dashboard. report.GetLastDate to store"""
-    # store twice. latest and date
-    bucket_name, object_name= datastore.putReportFile(datastore.default_bucket, repo, reportname, json_str, date=date)
-    # might return a url...
-    return bucket_name, object_name
+
```

### Comparing `earthcube_utilities-0.1.14/src/ec/sitemap/sitemap.py` & `earthcube_utilities-0.1.15/src/ec/sitemap/sitemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     If the sitemap URL does not exist, then it will return a Sitemap, with an
     len(errors) > 0.
 
     """
     sitemapurl = None
     _validSitemap = True
     sitemap_df = pandas.DataFrame()
-    errors=[]
     _checkedUrls=False
     def __init__(self, sitemapurl, repoName="", no_progress_bar=False):
+        self.errors=[]
         self.sitemapurl = sitemapurl
         self.no_progress_bar = no_progress_bar
         if _urlExists(sitemapurl):
             self.sitemap_df = adv.sitemap_to_df(sitemapurl)
             self._validSitemap = True
         else:
             self.errors.append(f"sitemap url invalid: {sitemapurl}")
@@ -110,8 +110,8 @@
         self.self.source = source
         if source["sourcetype"] !=  "sitemap":
             return Exception("source is Not a sitemap")
         super.__init__(source.url, reponame= source.name)
 
     def get_status(self):
         s = self.source
-        return  { 'name': s.name , 'code': _urlResponse( s.get("url") ), 'description': "res", 'url': s.get("description"), 'type': s.get("sourcetype")}
+        return  { 'name': s.name , 'code': _urlResponse( s.get("url") ), 'description': "res", 'url': s.get("description"), 'type': s.get("sourcetype")}
```

### Comparing `earthcube_utilities-0.1.14/src/ec/sos_json/rdf.py` & `earthcube_utilities-0.1.15/src/ec/sos_json/rdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,8 @@
     """retrieves a release from the url"""
     g= Dataset()
     g.parse(releaseurl, format='nquads')
     return g
 #  using https://github.com/cadmiumkitty/rdfpandas
     #g = Graph()
 #    g.parse(releaseurl, format='nt')
-#    df = to_dataframe(g)
+#    df = to_dataframe(g)
```

### Comparing `earthcube_utilities-0.1.14/src/ec/sos_json/utils.py` & `earthcube_utilities-0.1.15/src/ec/sos_json/utils.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.14/src/ec/summarize/summarize_materializedview.py` & `earthcube_utilities-0.1.15/src/ec/summarize/summarize_materializedview.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,35 +14,37 @@
 HTTP_SCHEMA_ORG = "http://schema.org/"
 BASE_SHCEMA_ORG = HTTPS_SCHEMA_ORG
 context = f"@prefix : <{BASE_SHCEMA_ORG}> ."
 
 ### BLAZEGRAPH
 '''original fetch all from temporary namespace'''
 def get_summary4repo(endpoint: str) -> pandas.DataFrame:
+    logging.INFO("Running Summary Query to Get all records")
     df = queryWithSparql("all_summary_query", endpoint)
     return df
     # file = '../resources/sparql/summary_query.txt'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # df = sparqldataframe.query(endpoint,lines)
     # return df
 
 ''' fetch all from graph namespace'''
 def get_summary4graph(endpoint : str) -> pandas.DataFrame:
+    logging.INFO("Running Summary Query to Get all records")
     df= queryWithSparql("all_summary_query",endpoint)
     return df
     # file = '../resources/sparql/all_summary_query.sparql'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # df = sparqldataframe.query(endpoint,lines)
     # return df
 
 ''' fetch subset  from graph namespace'''
 def get_summary4repoSubset(endpoint: str, repo : str) -> pandas.DataFrame:
-
+    logging.INFO(f"Running Summary Query to Get {repo} records")
     df = queryWithSparql("repo_summary_query",endpoint, parameters={"repo":repo})
     return df
     # file = '../resources/sparql/repo_summary_query.sparql'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # #query = getFileFromResources(f"{template_name}")
     # #q_template = Template(query)
```

