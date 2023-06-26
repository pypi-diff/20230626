# Comparing `tmp/y0-0.1.0.tar.gz` & `tmp/y0-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y0-0.1.0.tar", last modified: Tue Jun 15 01:36:19 2021, max compression
+gzip compressed data, was "y0-0.2.0.tar", last modified: Mon Jun 26 21:57:06 2023, max compression
```

## Comparing `y0-0.1.0.tar` & `y0-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,144 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.990349 y0-0.1.0/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1536 2021-06-15 01:01:46.000000 y0-0.1.0/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      360 2021-01-14 17:13:52.000000 y0-0.1.0/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     8024 2021-06-15 01:36:19.990517 y0-0.1.0/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     5512 2021-06-15 01:34:55.000000 y0-0.1.0/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.954233 y0-0.1.0/docs/
--rw-r--r--   0 cthoyt     (501) staff       (20)      605 2021-05-17 17:24:23.000000 y0-0.1.0/docs/Makefile
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.962297 y0-0.1.0/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      191 2021-05-14 22:59:07.000000 y0-0.1.0/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     6934 2021-06-15 01:36:19.000000 y0-0.1.0/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)       63 2021-01-11 18:23:32.000000 y0-0.1.0/docs/source/dsl.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       72 2021-05-14 22:59:07.000000 y0-0.1.0/docs/source/examples.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       51 2021-05-14 22:59:07.000000 y0-0.1.0/docs/source/graph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       72 2021-06-15 00:49:27.000000 y0-0.1.0/docs/source/identification.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      312 2021-05-14 22:59:07.000000 y0-0.1.0/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      505 2021-01-11 17:48:32.000000 y0-0.1.0/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7328 2021-01-11 22:44:31.000000 y0-0.1.0/docs/source/logo.png
--rw-r--r--   0 cthoyt     (501) staff       (20)       58 2021-05-14 22:59:07.000000 y0-0.1.0/docs/source/mutation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       54 2021-01-11 18:24:39.000000 y0-0.1.0/docs/source/parser.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     2120 2021-06-15 01:36:19.991251 y0-0.1.0/setup.cfg
--rw-r--r--   0 cthoyt     (501) staff       (20)      129 2021-06-10 14:19:56.000000 y0-0.1.0/setup.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.950749 y0-0.1.0/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.968902 y0-0.1.0/src/y0/
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2021-01-11 18:04:36.000000 y0-0.1.0/src/y0/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      319 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/__main__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.973327 y0-0.1.0/src/y0/algorithm/
--rw-r--r--   0 cthoyt     (501) staff       (20)       71 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/algorithm/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     6739 2021-06-10 14:10:04.000000 y0-0.1.0/src/y0/algorithm/conditional_independencies.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3209 2021-06-10 14:28:57.000000 y0-0.1.0/src/y0/algorithm/falsification.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5695 2021-06-10 14:10:04.000000 y0-0.1.0/src/y0/algorithm/simplify_latent.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    10985 2021-06-15 00:49:27.000000 y0-0.1.0/src/y0/algorithm/taheri_design.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      775 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      830 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    31212 2021-06-15 00:49:27.000000 y0-0.1.0/src/y0/dsl.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    16440 2021-06-15 00:49:27.000000 y0-0.1.0/src/y0/examples.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11206 2021-06-15 00:49:27.000000 y0-0.1.0/src/y0/graph.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3621 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/identify.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.974363 y0-0.1.0/src/y0/mutate/
--rw-r--r--   0 cthoyt     (501) staff       (20)      284 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/mutate/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5543 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/mutate/canonicalize_expr.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3513 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/mutate/chain.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.975213 y0-0.1.0/src/y0/parser/
--rw-r--r--   0 cthoyt     (501) staff       (20)      237 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/parser/__init__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.976665 y0-0.1.0/src/y0/parser/ce/
--rw-r--r--   0 cthoyt     (501) staff       (20)      108 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/parser/ce/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2062 2021-06-10 14:28:57.000000 y0-0.1.0/src/y0/parser/ce/grammar.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1395 2021-06-10 14:28:57.000000 y0-0.1.0/src/y0/parser/ce/utils.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.977775 y0-0.1.0/src/y0/parser/craig/
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/parser/craig/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1893 2021-06-10 14:28:57.000000 y0-0.1.0/src/y0/parser/craig/grammar.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2800 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/parser/craig/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1293 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/parser/internal.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1077 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/predicates.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1831 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/r_utils.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.980046 y0-0.1.0/src/y0/resources/
--rw-r--r--   0 cthoyt     (501) staff       (20)      226 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/resources/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   242724 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/resources/asia.csv
--rw-r--r--   0 cthoyt     (501) staff       (20)    72805 2021-05-14 22:59:07.000000 y0-0.1.0/src/y0/resources/viral_pathogenesis.json
--rw-r--r--   0 cthoyt     (501) staff       (20)     2768 2021-06-10 14:19:56.000000 y0-0.1.0/src/y0/struct.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.981769 y0-0.1.0/src/y0/util/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2021-06-10 16:02:25.000000 y0-0.1.0/src/y0/util/combinatorics.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    23647 2021-06-15 00:49:27.000000 y0-0.1.0/src/y0/util/stat_utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      971 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.970844 y0-0.1.0/src/y0.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     8024 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1977 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       36 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2021-01-11 18:25:31.000000 y0-0.1.0/src/y0.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      184 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        3 2021-06-15 01:36:19.000000 y0-0.1.0/src/y0.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.984943 y0-0.1.0/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       52 2021-01-11 17:48:32.000000 y0-0.1.0/tests/__init__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.987036 y0-0.1.0/tests/test_algorithm/
--rw-r--r--   0 cthoyt     (501) staff       (20)       53 2021-05-14 22:59:07.000000 y0-0.1.0/tests/test_algorithm/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7984 2021-06-10 14:10:04.000000 y0-0.1.0/tests/test_algorithm/test_conditional_independencies.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1121 2021-05-14 22:59:07.000000 y0-0.1.0/tests/test_algorithm/test_falsification.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3609 2021-06-10 14:10:04.000000 y0-0.1.0/tests/test_algorithm/test_simplify_latent.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2404 2021-06-10 14:28:57.000000 y0-0.1.0/tests/test_causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    10915 2021-06-10 14:10:04.000000 y0-0.1.0/tests/test_dsl.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2714 2021-06-15 00:49:27.000000 y0-0.1.0/tests/test_graph.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7283 2021-06-10 14:10:04.000000 y0-0.1.0/tests/test_is_identifiable.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.988684 y0-0.1.0/tests/test_mutate/
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2021-05-14 22:59:07.000000 y0-0.1.0/tests/test_mutate/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5804 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_mutate/test_canonicalize.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2233 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_mutate/test_chain.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1095 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_mutate/test_simplify.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2021-06-15 01:36:19.990055 y0-0.1.0/tests/test_parser/
--rw-r--r--   0 cthoyt     (501) staff       (20)       78 2021-05-14 22:59:07.000000 y0-0.1.0/tests/test_parser/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1512 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_parser/test_causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3881 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_parser/test_craig.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      905 2021-06-10 14:19:56.000000 y0-0.1.0/tests/test_parser/test_internal.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1928 2021-06-10 14:10:04.000000 y0-0.1.0/tests/test_predicates.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.992371 y0-0.2.0/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1509 2022-08-17 22:51:48.000000 y0-0.2.0/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      359 2022-08-17 22:51:48.000000 y0-0.2.0/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10209 2023-06-26 21:57:06.992592 y0-0.2.0/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8761 2023-06-26 21:42:49.000000 y0-0.2.0/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.924059 y0-0.2.0/docs/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      605 2021-07-06 18:38:06.000000 y0-0.2.0/docs/Makefile
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.931495 y0-0.2.0/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-06-21 14:43:48.000000 y0-0.2.0/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6945 2023-06-26 21:57:06.000000 y0-0.2.0/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)       63 2021-01-11 18:23:32.000000 y0-0.2.0/docs/source/dsl.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       72 2021-07-06 18:18:06.000000 y0-0.2.0/docs/source/examples.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       51 2021-05-14 22:59:07.000000 y0-0.2.0/docs/source/graph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       72 2021-06-23 12:26:24.000000 y0-0.2.0/docs/source/identification.rst
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.933282 y0-0.2.0/docs/source/img/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    87578 2022-03-04 18:55:06.000000 y0-0.2.0/docs/source/img/simulation_graph_algorithm.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)    29002 2022-03-04 18:55:06.000000 y0-0.2.0/docs/source/img/simulation_graph_diagram.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)      312 2023-06-21 14:43:46.000000 y0-0.2.0/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      505 2021-01-11 17:48:32.000000 y0-0.2.0/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7328 2021-01-11 22:44:31.000000 y0-0.2.0/docs/source/logo.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)       58 2021-07-06 18:38:06.000000 y0-0.2.0/docs/source/mutation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       54 2021-01-11 18:24:39.000000 y0-0.2.0/docs/source/parser.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      350 2022-03-04 18:55:06.000000 y0-0.2.0/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2517 2023-06-26 21:57:06.993772 y0-0.2.0/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.917465 y0-0.2.0/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.941036 y0-0.2.0/src/y0/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2021-01-11 18:04:36.000000 y0-0.2.0/src/y0/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      319 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/__main__.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.945971 y0-0.2.0/src/y0/algorithm/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       71 2021-07-06 18:18:06.000000 y0-0.2.0/src/y0/algorithm/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7498 2023-05-26 08:34:43.000000 y0-0.2.0/src/y0/algorithm/conditional_independencies.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3764 2023-05-26 08:34:43.000000 y0-0.2.0/src/y0/algorithm/falsification.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.949722 y0-0.2.0/src/y0/algorithm/identify/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      413 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7930 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/_extras.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    19698 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/cg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2156 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/id_c.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12042 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12432 2023-06-22 08:02:11.000000 y0-0.2.0/src/y0/algorithm/identify/id_std.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8718 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/algorithm/identify/idc_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12247 2022-08-18 23:01:18.000000 y0-0.2.0/src/y0/algorithm/identify/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5784 2022-03-04 18:55:06.000000 y0-0.2.0/src/y0/algorithm/simplify_latent.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11752 2023-06-24 07:28:07.000000 y0-0.2.0/src/y0/algorithm/taheri_design.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      775 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      830 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2401 2022-03-04 18:55:06.000000 y0-0.2.0/src/y0/complexity.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    51893 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/dsl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    38158 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/examples.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    22027 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/graph.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3745 2023-05-26 08:34:43.000000 y0-0.2.0/src/y0/identify.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.952260 y0-0.2.0/src/y0/mutate/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      334 2021-07-10 05:19:53.000000 y0-0.2.0/src/y0/mutate/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7103 2023-05-16 16:49:41.000000 y0-0.2.0/src/y0/mutate/canonicalize_expr.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3475 2023-05-16 17:48:58.000000 y0-0.2.0/src/y0/mutate/chain.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.953686 y0-0.2.0/src/y0/parser/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      237 2021-07-06 18:18:06.000000 y0-0.2.0/src/y0/parser/__init__.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.955354 y0-0.2.0/src/y0/parser/ce/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      108 2021-07-06 18:18:06.000000 y0-0.2.0/src/y0/parser/ce/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2088 2021-07-10 05:19:53.000000 y0-0.2.0/src/y0/parser/ce/grammar.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1395 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/parser/ce/utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.957425 y0-0.2.0/src/y0/parser/craig/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2021-07-06 18:18:06.000000 y0-0.2.0/src/y0/parser/craig/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1893 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/parser/craig/grammar.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2889 2022-03-04 19:51:19.000000 y0-0.2.0/src/y0/parser/craig/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1293 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/parser/internal.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1055 2022-03-04 19:51:19.000000 y0-0.2.0/src/y0/predicates.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1831 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/r_utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.961360 y0-0.2.0/src/y0/resources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      226 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/resources/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)   242724 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/resources/asia.csv
+-rw-r--r--   0 cthoyt     (501) staff       (20)    72805 2021-10-24 17:26:19.000000 y0-0.2.0/src/y0/resources/viral_pathogenesis.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6465 2023-04-27 15:39:25.000000 y0-0.2.0/src/y0/simulation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4199 2023-06-26 21:42:45.000000 y0-0.2.0/src/y0/struct.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.963922 y0-0.2.0/src/y0/util/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2021-07-06 18:38:06.000000 y0-0.2.0/src/y0/util/combinatorics.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    23460 2023-04-20 12:00:10.000000 y0-0.2.0/src/y0/util/stat_utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      984 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.943452 y0-0.2.0/src/y0.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10209 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3494 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       35 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2021-01-11 18:25:31.000000 y0-0.2.0/src/y0.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      215 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        3 2023-06-26 21:57:06.000000 y0-0.2.0/src/y0.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.970983 y0-0.2.0/tests/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.972782 y0-0.2.0/tests/.pytest_cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-04-04 16:03:05.000000 y0-0.2.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-04-04 16:03:05.000000 y0-0.2.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-04-04 16:03:05.000000 y0-0.2.0/tests/.pytest_cache/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.919681 y0-0.2.0/tests/.pytest_cache/v/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.974388 y0-0.2.0/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      504 2023-05-17 13:49:37.000000 y0-0.2.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12871 2023-06-26 21:07:53.000000 y0-0.2.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-06-26 21:07:53.000000 y0-0.2.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 cthoyt     (501) staff       (20)       52 2021-01-11 17:48:32.000000 y0-0.2.0/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    33224 2023-05-30 07:11:18.000000 y0-0.2.0/tests/id_star.log
+-rw-r--r--   0 cthoyt     (501) staff       (20)    19892 2023-05-30 07:11:18.000000 y0-0.2.0/tests/idc_star.log
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.980273 y0-0.2.0/tests/test_algorithm/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.982059 y0-0.2.0/tests/test_algorithm/.pytest_cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-04-04 16:06:28.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/.gitignore
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-04-04 16:06:28.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-04-04 16:06:28.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.920179 y0-0.2.0/tests/test_algorithm/.pytest_cache/v/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.983676 y0-0.2.0/tests/test_algorithm/.pytest_cache/v/cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      131 2023-05-22 07:33:26.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4188 2023-05-31 10:07:59.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-05-31 10:07:59.000000 y0-0.2.0/tests/test_algorithm/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 cthoyt     (501) staff       (20)       53 2021-07-06 18:18:06.000000 y0-0.2.0/tests/test_algorithm/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1831 2023-04-18 22:09:31.000000 y0-0.2.0/tests/test_algorithm/cases.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    16612 2023-05-30 10:37:27.000000 y0-0.2.0/tests/test_algorithm/id_star.log
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9946 2023-05-30 10:37:27.000000 y0-0.2.0/tests/test_algorithm/idc_star.log
+-rw-r--r--   0 cthoyt     (501) staff       (20)    33399 2023-06-26 21:42:45.000000 y0-0.2.0/tests/test_algorithm/test_cg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8996 2023-05-02 15:49:33.000000 y0-0.2.0/tests/test_algorithm/test_conditional_independencies.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1092 2022-08-18 22:59:51.000000 y0-0.2.0/tests/test_algorithm/test_falsification.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12320 2023-06-26 21:42:45.000000 y0-0.2.0/tests/test_algorithm/test_id_alg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    23264 2023-06-26 21:42:45.000000 y0-0.2.0/tests/test_algorithm/test_id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    21609 2023-06-26 21:42:45.000000 y0-0.2.0/tests/test_algorithm/test_original_id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4026 2022-03-04 18:55:06.000000 y0-0.2.0/tests/test_algorithm/test_simplify_latent.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2318 2021-10-26 22:29:31.000000 y0-0.2.0/tests/test_causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2972 2022-03-04 18:55:06.000000 y0-0.2.0/tests/test_complexity.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    20314 2023-05-16 17:48:54.000000 y0-0.2.0/tests/test_dsl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9650 2023-04-18 22:23:53.000000 y0-0.2.0/tests/test_graph.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7233 2022-03-04 19:51:19.000000 y0-0.2.0/tests/test_is_identifiable.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.985979 y0-0.2.0/tests/test_mutate/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.987750 y0-0.2.0/tests/test_mutate/.pytest_cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-05-10 12:59:01.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/.gitignore
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-05-10 12:59:01.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-05-10 12:59:01.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.920762 y0-0.2.0/tests/test_mutate/.pytest_cache/v/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.989379 y0-0.2.0/tests/test_mutate/.pytest_cache/v/cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-05-16 15:40:49.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 cthoyt     (501) staff       (20)      736 2023-05-16 15:40:49.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-05-16 15:40:49.000000 y0-0.2.0/tests/test_mutate/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2021-07-06 18:18:06.000000 y0-0.2.0/tests/test_mutate/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8785 2023-05-11 15:27:03.000000 y0-0.2.0/tests/test_mutate/test_canonicalize.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2145 2021-07-06 18:38:06.000000 y0-0.2.0/tests/test_mutate/test_chain.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1638 2022-03-04 10:47:26.000000 y0-0.2.0/tests/test_mutate/test_simplify.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-26 21:57:06.991912 y0-0.2.0/tests/test_parser/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       78 2021-07-06 18:18:06.000000 y0-0.2.0/tests/test_parser/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1474 2021-07-06 18:38:06.000000 y0-0.2.0/tests/test_parser/test_causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3823 2021-07-06 18:38:06.000000 y0-0.2.0/tests/test_parser/test_craig.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      905 2021-07-06 18:38:06.000000 y0-0.2.0/tests/test_parser/test_internal.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1928 2021-07-06 18:38:06.000000 y0-0.2.0/tests/test_predicates.py
```

### Comparing `y0-0.1.0/LICENSE` & `y0-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Y0 Causal Inference Engine
-Copyright (c) 2021 Charles Tapley Hoyt and Battelle Memorial Institute
+Copyright (c) 2022 Charles Tapley Hoyt and Battelle Memorial Institute
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
 following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
    disclaimer.
```

### Comparing `y0-0.1.0/PKG-INFO` & `y0-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,171 +1,285 @@
 Metadata-Version: 2.1
 Name: y0
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python code for causal modeling.
 Home-page: https://github.com/y0-causal-inference/y0
+Download-URL: https://github.com/y0-causal-inference/y0/releases
 Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: BSD-3-Clause
-Download-URL: https://github.com/y0-causal-inference/y0/releases
 Project-URL: Bug Tracker, https://github.com/y0-causal-inference/y0/issues
 Project-URL: Source Code, https://github.com/y0-causal-inference/y0
-Description: <p align="center">
-          <img src="docs/source/logo.png" height="120">
-        </p>
-        
-        <h1 align="center">
-          y0
-        </h1>
-        
-        <p align="center">
-            <a href="https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests">
-                <img alt="Tests" src="https://github.com/y0-causal-inference/y0/workflows/Tests/badge.svg" />
-            </a>
-           <a href="https://github.com/cthoyt/cookiecutter-python-package">
-              <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-python--package-yellow" /> 
-           </a>
-            <a href="https://pypi.org/project/y0">
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/y0" />
-            </a>
-            <a href="https://pypi.org/project/y0">
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/y0" />
-            </a>
-            <a href="https://github.com/y0-causal-inference/y0/blob/main/LICENSE">
-                <img alt="PyPI - License" src="https://img.shields.io/pypi/l/y0" />
-            </a>
-            <a href='https://y0.readthedocs.io/en/latest/?badge=latest'>
-                <img src='https://readthedocs.org/projects/y0/badge/?version=latest' alt='Documentation Status' />
-            </a>
-            <a href="https://zenodo.org/badge/latestdoi/328745468">
-                <img src="https://zenodo.org/badge/328745468.svg" alt="DOI">
-            </a>
-            <a href="https://github.com/psf/black">
-                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
-            </a>
-        </p>
-        
-        `y0` (pronounced "why not?") is Python code for causal inferencing.
-        
-        ## 💪 Getting Started
-        
-        > TODO show in a very small amount of space the **MOST** useful thing your package can do.
-        Make it as short as possible! You have an entire set of docs for later.
-        
-        ## ⬇️ Installation
-        
-        The most recent release can be installed from
-        [PyPI](https://pypi.org/project/y0/) with:
-        
-        ```bash
-        $ pip install y0
-        ```
-        
-        The most recent code and data can be installed directly from GitHub with:
-        
-        ```bash
-        $ pip install git+https://github.com/y0-causal-inference/y0.git
-        ```
-        
-        To install in development mode, use the following:
-        
-        ```bash
-        $ git clone git+https://github.com/y0-causal-inference/y0.git
-        $ cd y0
-        $ pip install -e .
-        ```
-        
-        ## ⚖️ License
-        
-        The code in this package is licensed under the [BSD-3-Clause
-        license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
-        
-        ## 🙏 Contributing
-        
-        Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
-        [CONTRIBUTING.rst](https://github.com/y0-causal-inference/y0/blob/master/CONTRIBUTING.rst) for more information on getting
-        involved.
-        
-        ## Acknowledgements
-        
-        ### Supporters
-        
-        This project has been supported by several organizations (in alphabetical order):
-        
-        - [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/)
-        - [Pacific Northwest National Laboratory](https://www.pnnl.org/)
-        
-        ### 💰 Funding
-        
-        The development of the Y0 Causal Inference Engine has been funded by the following grants:
-        
-        | Funding Body                                             | Program                                                                                                                       | Grant           |
-        |----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------|
-        | DARPA                                                    | [Automating Scientific Knowledge Extraction (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction) | HR00111990009   |
-        | PNNL Data Model Convergence Initiative    | [Causal Inference and Machine Learning Methods for Analysis of Security Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/converged-applications-projects) | 90001   |
-        
-        ### 🍪 Cookiecutter
-        
-        This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-        [cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
-        [cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-package) template.
-        
-        ## 🛠️ Development
-        
-        The final section of the README is for if you want to get involved by making a code contribution.
-        
-        ### ❓ Testing
-        
-        After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
-        run reproducibly with:
-        
-        ```shell
-        $ tox
-        ```
-        
-        Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests).
-        
-        ### 📦 Making a Release
-        
-        After installing the package in development mode and installing
-        `tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
-        in `tox.ini`. Run the following from the shell:
-        
-        ```shell
-        $ tox -e finish
-        ```
-        
-        This script does the following:
-        
-        1. Uses BumpVersion to switch the version number in the `setup.cfg` and
-           `src/y0/version.py` to not have the `-dev` suffix
-        2. Packages the code in both a tar archive and a wheel
-        3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
-           step
-        4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
-        5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
-           use `tox -e bumpversion minor` after.
-        
 Keywords: cthoyt,cookiecutter,structural causal modeling
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: r
+Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE
+
+<p align="center">
+  <img src="docs/source/logo.png" height="120">
+</p>
+
+<h1 align="center">
+  y0
+</h1>
+
+<p align="center">
+    <a href="https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests">
+        <img alt="Tests" src="https://github.com/y0-causal-inference/y0/workflows/Tests/badge.svg" />
+    </a>
+   <a href="https://github.com/cthoyt/cookiecutter-python-package">
+      <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
+   </a>
+    <a href="https://pypi.org/project/y0">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/y0" />
+    </a>
+    <a href="https://pypi.org/project/y0">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/y0" />
+    </a>
+    <a href="https://github.com/y0-causal-inference/y0/blob/main/LICENSE">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/y0" />
+    </a>
+    <a href='https://y0.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/y0/badge/?version=latest' alt='Documentation Status' />
+    </a>
+    <a href="https://zenodo.org/badge/latestdoi/328745468">
+        <img src="https://zenodo.org/badge/328745468.svg" alt="DOI">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+    </a>
+</p>
+
+`y0` (pronounced "why not?") is Python code for causal inference.
+
+## 💪 Getting Started
+
+### Representing Probability Expressions
+
+`y0` has a fully featured internal domain specific language for representing
+probability expressions:
+
+```python
+from y0.dsl import P, A, B
+
+# The probability of A given B
+expr_1 = P(A | B)
+
+# The probability of A given not B
+expr_2 = P(A | ~B)
+
+# The joint probability of A and B
+expr_3 = P(A, B)
+```
+
+It can also be used to manipulate expressions:
+
+```python
+from y0.dsl import P, A, B, Sum
+
+P(A, B).marginalize(A) == Sum[A](P(A, B))
+P(A, B).conditional(A) == P(A, B) / Sum[A](P(A, B))
+```
+
+DSL objects can be converted into strings with `str()` and parsed back
+using `y0.parser.parse_y0()`.
+
+A full demo of the DSL can be found in this
+[Jupyter Notebook](https://github.com/y0-causal-inference/y0/blob/main/notebooks/DSL%20Demo.ipynb)
+
+### Representing Causality
+
+`y0` has a notion of acyclic directed mixed graphs built on top of
+`networkx` that can be used to model causality:
+
+```python
+from y0.graph import NxMixedGraph
+from y0.dsl import X, Y, Z1, Z2
+
+# Example from:
+#   J. Pearl and D. Mackenzie (2018)
+#   The Book of Why: The New Science of Cause and Effect.
+#   Basic Books, p. 240.
+napkin = NxMixedGraph.from_edges(
+    directed=[
+        (Z2, Z1),
+        (Z1, X),
+        (X, Y),
+    ],
+    undirected=[
+        (Z2, X),
+        (Z2, Y),
+    ],
+)
+```
+
+`y0` has many pre-written examples in `y0.examples` from Pearl, Shpitser,
+Bareinboim, and others.
+
+### do Calculus
+
+`y0` provides _actual_ implementations of many algorithms that have remained
+unimplemented for the last 15 years of publications including:
+
+| Algorithm | Reference                                                                   |
+|-----------|-----------------------------------------------------------------------------|
+| ID        | [Shpitser and Pearl, 2006](https://dl.acm.org/doi/10.5555/1597348.1597382)  |
+| IDC       | [Shpitser and Pearl, 2008](https://www.jmlr.org/papers/v9/shpitser08a.html) |
+| ID*       | [Shpitser and Pearl, 2012](https://arxiv.org/abs/1206.5294)                 |
+| IDC*      | [Shpitser and Pearl, 2012](https://arxiv.org/abs/1206.5294)                 |
+
+Apply an algorithm to an ADMG and a causal query to generate an estimand
+represented in the DSL like:
+
+```python
+from y0.dsl import P, X, Y
+from y0.examples import napkin
+from y0.algorithm.identify import Identification, identify
+
+# TODO after ID* and IDC* are done, we'll update this interface
+query = Identification.from_expression(graph=napkin, query=P(Y @ X))
+estimand = identify(query)
+assert estimand == P(Y @ X)
+```
+
+## 🚀 Installation
+
+The most recent release can be installed from
+[PyPI](https://pypi.org/project/y0/) with:
+
+```bash
+$ pip install y0
+```
+
+The most recent code and data can be installed directly from GitHub with:
+
+```bash
+$ pip install git+https://github.com/y0-causal-inference/y0.git
+```
+
+## 👐 Contributing
+
+Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
+[CONTRIBUTING.md](https://github.com/y0-causal-inference/y0/blob/master/.github/CONTRIBUTING.md) for more information on getting
+involved.
+
+## 👋 Attribution
+
+### ⚖️ License
+
+The code in this package is licensed under the [BSD-3-Clause
+license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
+
+### 📖 Citation
+
+Before we publish an application note on `y0`, you can cite this software
+via our Zenodo record (also see the badge above):
+
+```bibtex
+@software{y0,
+  author       = {Charles Tapley Hoyt and
+                  Jeremy Zucker and
+                  Marc-Antoine Parent},
+  title        = {y0-causal-inference/y0},
+  month        = jun,
+  year         = 2021,
+  publisher    = {Zenodo},
+  version      = {v0.1.0},
+  doi          = {10.5281/zenodo.4950768},
+  url          = {https://doi.org/10.5281/zenodo.4950768}
+}
+```
+
+### 🙏 Supporters
+
+This project has been supported by several organizations (in alphabetical order):
+
+- [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/)
+- [Pacific Northwest National Laboratory](https://www.pnnl.org/)
+
+### 💰 Funding
+
+The development of the Y0 Causal Inference Engine has been funded by the following grants:
+
+| Funding Body                                             | Program                                                                                                                       | Grant           |
+|----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------|
+| DARPA                                                    | [Automating Scientific Knowledge Extraction (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction) | HR00111990009   |
+| PNNL Data Model Convergence Initiative    | [Causal Inference and Machine Learning Methods for Analysis of Security Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/converged-applications-projects) | 90001   |
+| DARPA                                                    |  [Automating Scientific Knowledge Extraction and Modeling (ASKEM)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction-and-modeling) |  HR00112220036  |
+
+### 🍪 Cookiecutter
+
+This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
+[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-package) template.
+
+## 🛠️ Development
+
+<details>
+  <summary>See developer instructions</summary>
+
+The final section of the README is for if you want to get involved by making a code contribution.
+
+### Developer Installation
+
+To install in development mode, use the following:
+
+```bash
+$ git clone git+https://github.com/y0-causal-inference/y0.git
+$ cd y0
+$ pip install -e .
+```
+
+### ❓ Testing
+
+After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
+run reproducibly with:
+
+```shell
+$ tox
+```
+
+Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests).
+
+### 📦 Making a Release
+
+After installing the package in development mode and installing
+`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell:
+
+```shell
+$ tox -e finish
+```
+
+This script does the following:
+
+1. Uses BumpVersion to switch the version number in the `setup.cfg` and
+   `src/y0/version.py` to not have the `-dev` suffix
+2. Packages the code in both a tar archive and a wheel
+3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
+   step
+4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
+5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
+   use `tox -e bumpversion minor` after.
+
+</details>
```

#### html2text {}

```diff
@@ -1,74 +1,112 @@
-Metadata-Version: 2.1 Name: y0 Version: 0.1.0 Summary: Python code for causal
-modeling. Home-page: https://github.com/y0-causal-inference/y0 Author: Jeremy
-Zucker Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
-Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Download-URL: https://
-github.com/y0-causal-inference/y0/releases Project-URL: Bug Tracker, https://
-github.com/y0-causal-inference/y0/issues Project-URL: Source Code, https://
-github.com/y0-causal-inference/y0 Description:
+Metadata-Version: 2.1 Name: y0 Version: 0.2.0 Summary: Python code for causal
+modeling. Home-page: https://github.com/y0-causal-inference/y0 Download-URL:
+https://github.com/y0-causal-inference/y0/releases Author: Jeremy Zucker
+Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
+Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Project-URL: Bug
+Tracker, https://github.com/y0-causal-inference/y0/issues Project-URL: Source
+Code, https://github.com/y0-causal-inference/y0 Keywords:
+cthoyt,cookiecutter,structural causal modeling Classifier: Development Status
+:: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: BSD License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Information Analysis Classifier: Topic :: Software Development
+:: Compilers Classifier: Framework :: Pytest Classifier: Framework :: tox
+Classifier: Framework :: Sphinx Requires-Python: >=3.10 Description-Content-
+Type: text/markdown Provides-Extra: r Provides-Extra: tests Provides-Extra:
+docs License-File: LICENSE
                             [docs/source/logo.png]
                                ****** y0 ******
  [Tests] [Cookiecutter_template_from_@cthoyt] [PyPI] [PyPI_-_Python_Version]
        [PyPI_-_License] [Documentation_Status] [DOI] [Code_style:_black]
-`y0` (pronounced "why not?") is Python code for causal inferencing. ## ðª
-Getting Started > TODO show in a very small amount of space the **MOST** useful
-thing your package can do. Make it as short as possible! You have an entire set
-of docs for later. ## â¬ï¸ Installation The most recent release can be
-installed from [PyPI](https://pypi.org/project/y0/) with: ```bash $ pip install
-y0 ``` The most recent code and data can be installed directly from GitHub
-with: ```bash $ pip install git+https://github.com/y0-causal-inference/y0.git
-``` To install in development mode, use the following: ```bash $ git clone
-git+https://github.com/y0-causal-inference/y0.git $ cd y0 $ pip install -e .
-``` ## âï¸ License The code in this package is licensed under the [BSD-3-
-Clause license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
-## ð Contributing Contributions, whether filing an issue, making a pull
-request, or forking, are appreciated. See [CONTRIBUTING.rst](https://
-github.com/y0-causal-inference/y0/blob/master/CONTRIBUTING.rst) for more
-information on getting involved. ## Acknowledgements ### Supporters This
+`y0` (pronounced "why not?") is Python code for causal inference. ## ðª
+Getting Started ### Representing Probability Expressions `y0` has a fully
+featured internal domain specific language for representing probability
+expressions: ```python from y0.dsl import P, A, B # The probability of A given
+B expr_1 = P(A | B) # The probability of A given not B expr_2 = P(A | ~B) # The
+joint probability of A and B expr_3 = P(A, B) ``` It can also be used to
+manipulate expressions: ```python from y0.dsl import P, A, B, Sum P(A,
+B).marginalize(A) == Sum[A](P(A, B)) P(A, B).conditional(A) == P(A, B) / Sum[A]
+(P(A, B)) ``` DSL objects can be converted into strings with `str()` and parsed
+back using `y0.parser.parse_y0()`. A full demo of the DSL can be found in this
+[Jupyter Notebook](https://github.com/y0-causal-inference/y0/blob/main/
+notebooks/DSL%20Demo.ipynb) ### Representing Causality `y0` has a notion of
+acyclic directed mixed graphs built on top of `networkx` that can be used to
+model causality: ```python from y0.graph import NxMixedGraph from y0.dsl import
+X, Y, Z1, Z2 # Example from: # J. Pearl and D. Mackenzie (2018) # The Book of
+Why: The New Science of Cause and Effect. # Basic Books, p. 240. napkin =
+NxMixedGraph.from_edges( directed=[ (Z2, Z1), (Z1, X), (X, Y), ], undirected=[
+(Z2, X), (Z2, Y), ], ) ``` `y0` has many pre-written examples in `y0.examples`
+from Pearl, Shpitser, Bareinboim, and others. ### do Calculus `y0` provides
+_actual_ implementations of many algorithms that have remained unimplemented
+for the last 15 years of publications including: | Algorithm | Reference | |---
+--------|----------------------------------------------------------------------
+-------| | ID | [Shpitser and Pearl, 2006](https://dl.acm.org/doi/10.5555/
+1597348.1597382) | | IDC | [Shpitser and Pearl, 2008](https://www.jmlr.org/
+papers/v9/shpitser08a.html) | | ID* | [Shpitser and Pearl, 2012](https://
+arxiv.org/abs/1206.5294) | | IDC* | [Shpitser and Pearl, 2012](https://
+arxiv.org/abs/1206.5294) | Apply an algorithm to an ADMG and a causal query to
+generate an estimand represented in the DSL like: ```python from y0.dsl import
+P, X, Y from y0.examples import napkin from y0.algorithm.identify import
+Identification, identify # TODO after ID* and IDC* are done, we'll update this
+interface query = Identification.from_expression(graph=napkin, query=P(Y @ X))
+estimand = identify(query) assert estimand == P(Y @ X) ``` ## ð Installation
+The most recent release can be installed from [PyPI](https://pypi.org/project/
+y0/) with: ```bash $ pip install y0 ``` The most recent code and data can be
+installed directly from GitHub with: ```bash $ pip install git+https://
+github.com/y0-causal-inference/y0.git ``` ## ð Contributing Contributions,
+whether filing an issue, making a pull request, or forking, are appreciated.
+See [CONTRIBUTING.md](https://github.com/y0-causal-inference/y0/blob/
+master/.github/CONTRIBUTING.md) for more information on getting involved. ##
+ð Attribution ### âï¸ License The code in this package is licensed under
+the [BSD-3-Clause license](https://github.com/y0-causal-inference/y0/blob/
+master/LICENSE). ### ð Citation Before we publish an application note on
+`y0`, you can cite this software via our Zenodo record (also see the badge
+above): ```bibtex @software{y0, author = {Charles Tapley Hoyt and Jeremy Zucker
+and Marc-Antoine Parent}, title = {y0-causal-inference/y0}, month = jun, year =
+2021, publisher = {Zenodo}, version = {v0.1.0}, doi = {10.5281/zenodo.4950768},
+url = {https://doi.org/10.5281/zenodo.4950768} } ``` ### ð Supporters This
 project has been supported by several organizations (in alphabetical order): -
 [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology]
 (https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/) -
 [Pacific Northwest National Laboratory](https://www.pnnl.org/) ### ð° Funding
 The development of the Y0 Causal Inference Engine has been funded by the
 following grants: | Funding Body | Program | Grant | |-------------------------
 ---------------------------------|---------------------------------------------
 -------------------------------------------------------------------------------
 ---|-----------------| | DARPA | [Automating Scientific Knowledge Extraction
 (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-
 extraction) | HR00111990009 | | PNNL Data Model Convergence Initiative |
 [Causal Inference and Machine Learning Methods for Analysis of Security
 Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/
-converged-applications-projects) | 90001 | ### ðª Cookiecutter This package
-was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using
-[@cthoyt](https://github.com/cthoyt)'s [cookiecutter-python-package](https://
-github.com/cthoyt/cookiecutter-python-package) template. ## ð ï¸ Development
-The final section of the README is for if you want to get involved by making a
-code contribution. ### â Testing After cloning the repository and installing
-`tox` with `pip install tox`, the unit tests in the `tests/` folder can be run
-reproducibly with: ```shell $ tox ``` Additionally, these tests are
-automatically re-run with each commit in a [GitHub Action](https://github.com/
-y0-causal-inference/y0/actions?query=workflow%3ATests). ### ð¦ Making a
-Release After installing the package in development mode and installing `tox`
-with `pip install tox`, the commands for making a new release are contained
-within the `finish` environment in `tox.ini`. Run the following from the shell:
-```shell $ tox -e finish ``` This script does the following: 1. Uses
-BumpVersion to switch the version number in the `setup.cfg` and `src/y0/
+converged-applications-projects) | 90001 | | DARPA | [Automating Scientific
+Knowledge Extraction and Modeling (ASKEM)](https://www.darpa.mil/program/
+automating-scientific-knowledge-extraction-and-modeling) | HR00112220036 | ###
+ðª Cookiecutter This package was created with [@audreyfeldroy](https://
+github.com/audreyfeldroy)'s [cookiecutter](https://github.com/cookiecutter/
+cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-
+package) template. ## ð ï¸ Development  See developer instructions The final
+section of the README is for if you want to get involved by making a code
+contribution. ### Developer Installation To install in development mode, use
+the following: ```bash $ git clone git+https://github.com/y0-causal-inference/
+y0.git $ cd y0 $ pip install -e . ``` ### â Testing After cloning the
+repository and installing `tox` with `pip install tox`, the unit tests in the
+`tests/` folder can be run reproducibly with: ```shell $ tox ``` Additionally,
+these tests are automatically re-run with each commit in a [GitHub Action]
+(https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests). ###
+ð¦ Making a Release After installing the package in development mode and
+installing `tox` with `pip install tox`, the commands for making a new release
+are contained within the `finish` environment in `tox.ini`. Run the following
+from the shell: ```shell $ tox -e finish ``` This script does the following: 1.
+Uses BumpVersion to switch the version number in the `setup.cfg` and `src/y0/
 version.py` to not have the `-dev` suffix 2. Packages the code in both a tar
 archive and a wheel 3. Uploads to PyPI using `twine`. Be sure to have a
 `.pypirc` file configured to avoid the need for manual input at this step 4.
 Push to GitHub. You'll need to make a release going with the commit where the
 version was bumped. 5. Bump the version to the next patch. If you made big
 changes and want to bump the version by minor, you can use `tox -e bumpversion
-minor` after. Keywords: cthoyt,cookiecutter,structural causal modeling
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-Environment :: Console Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Compilers Classifier: Framework ::
-Pytest Classifier: Framework :: tox Classifier: Framework :: Sphinx Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: r
-Provides-Extra: docs
+minor` after.
```

### Comparing `y0-0.1.0/docs/Makefile` & `y0-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/docs/source/conf.py` & `y0-0.2.0/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 #
 
 import os
 import re
 import sys
 from datetime import date
 
-sys.path.insert(0, os.path.abspath('../../src'))
+sys.path.insert(0, os.path.abspath("../../src"))
 
 # -- Project information -----------------------------------------------------
 
-project = 'y0'
-copyright = f'{date.today().year}, Jeremy Zucker and Charles Tapley Hoyt'
-author = 'Jeremy Zucker and Charles Tapley Hoyt'
+project = "y0"
+copyright = f"{date.today().year}, Jeremy Zucker and Charles Tapley Hoyt"
+author = "Jeremy Zucker and Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = '0.1.0'
+release = "0.2.0"
 
 # The short X.Y version.
 parsed_version = re.match(
-    '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
+    "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
-version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
+version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
 
-if parsed_version.group('release'):
-    tags.add('prerelease')
+if parsed_version.group("release"):
+    tags.add("prerelease")
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -52,63 +52,63 @@
 # A list of prefixes that are ignored when creating the module index. (new in Sphinx 0.6)
 modindex_common_prefix = ["y0."]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autosummary',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.intersphinx',
+    "sphinx.ext.autosummary",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
-    'sphinx_autodoc_typehints',
-    'sphinx_click.ext',
-    'sphinx_automodapi.automodapi',
-    'texext',
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
+    "sphinx_autodoc_typehints",
+    "sphinx_click.ext",
+    "sphinx_automodapi.automodapi",
+    "texext",
 ]
 
 # generate autosummary pages
 autosummary_generate = True
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -126,21 +126,21 @@
 # 'searchbox.html']``.
 #
 # html_sidebars = {}
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 #
-if os.path.exists('logo.png'):
-    html_logo = 'logo.png'
+if os.path.exists("logo.png"):
+    html_logo = "logo.png"
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'y0doc'
+htmlhelp_basename = "y0doc"
 
 # -- Options for LaTeX output ------------------------------------------------
 
 # latex_elements = {
 #     The paper size ('letterpaper' or 'a4paper').
 #
 #     'papersize': 'letterpaper',
@@ -174,35 +174,35 @@
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         master_doc,
-        'y0',
-        'y0 Documentation',
+        "y0",
+        "y0 Documentation",
         [author],
         1,
     ),
 ]
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
-        'y0',
-        'y0 Documentation',
+        "y0",
+        "y0 Documentation",
         author,
-        'Jeremy Zucker and Charles Tapley Hoyt',
-        'Python code for causal modeling',
-        'Miscellaneous',
+        "Jeremy Zucker and Charles Tapley Hoyt",
+        "Python code for causal modeling",
+        "Miscellaneous",
     ),
 ]
 
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
 # epub_title = project
@@ -221,14 +221,14 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'https://docs.python.org/3/': None,
-    'networkx': ('https://networkx.org/documentation/latest/', None),
-    'ananke': ('https://ananke.readthedocs.io/en/latest', None),
+    "python": ("https://docs.python.org/3", None),
+    "networkx": ("https://networkx.org/documentation/latest/", None),
+    "ananke": ("https://ananke.readthedocs.io/en/latest", None),
 }
 
-autoclass_content = 'both'
-autodoc_member_order = 'bysource'
+autoclass_content = "both"
+autodoc_member_order = "bysource"
```

### Comparing `y0-0.1.0/docs/source/logo.png` & `y0-0.2.0/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/setup.cfg` & `y0-0.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [metadata]
 name = y0
-version = 0.1.0
+version = 0.2.0
 description = Python code for causal modeling.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/y0-causal-inference/y0
 download_url = https://github.com/y0-causal-inference/y0/releases
 project_urls = 
 	Bug Tracker = https://github.com/y0-causal-inference/y0/issues
 	Source Code = https://github.com/y0-causal-inference/y0
 author = Jeremy Zucker
 author_email = jeremy.zucker@pnnl.gov
 maintainer = Charles Tapley Hoyt
 maintainer_email = cthoyt@gmail.com
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = 
+	LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering :: Mathematics
 	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Software Development :: Compilers
 	Framework :: Pytest
 	Framework :: tox
 	Framework :: Sphinx
@@ -40,30 +41,34 @@
 [options]
 install_requires = 
 	more_itertools
 	tqdm
 	click
 	more_click
 	pyparsing
-	ananke-causal
 	networkx
 	tabulate
+	pandas
+	scikit-learn
 zip_safe = false
 include_package_data = True
-python_requires = >=3.8
+python_requires = >=3.10
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 r = 
 	rpy2
+tests = 
+	pytest
+	coverage
 docs = 
 	sphinx
 	sphinx-rtd-theme
 	sphinx-click
 	sphinx-autodoc-typehints
 	sphinx_automodapi
 	texext
@@ -77,14 +82,15 @@
 
 [coverage:run]
 branch = True
 source = y0
 omit = 
 	tests/*
 	docs/*
+	src/y0/algorithm/identify/_extras.py
 
 [coverage:paths]
 source = 
 	src/y0
 	.tox/*/lib/python*/site-packages/y0
 
 [coverage:report]
@@ -96,11 +102,39 @@
 	def __str__
 	def __repr__
 
 [darglint]
 docstring_style = sphinx
 strictness = short
 
+[flake8]
+ignore = 
+	W503
+	D105
+	S404
+	S603
+	E203
+exclude = 
+	.tox,
+	.git,
+	__pycache__,
+	docs/source/conf.py,
+	build,
+	dist,
+	tests/fixtures/*,
+	*.pyc,
+	*.egg-info,
+	.cache,
+	.eggs,
+	data
+	.ipynb_checkpoints
+max-line-length = 120
+max-complexity = 20
+import-order-style = pycharm
+application-import-names = 
+	y0
+	tests
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `y0-0.1.0/src/y0/algorithm/conditional_independencies.py` & `y0-0.2.0/src/y0/algorithm/conditional_independencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 # -*- coding: utf-8 -*-
 
 """An implementation to get conditional independencies of an ADMG."""
 
 import copy
 from functools import partial
 from itertools import chain, combinations, groupby
-from typing import Iterable, List, Optional, Set, Tuple, Union
+from typing import Callable, Iterable, List, Optional, Sequence, Set, Tuple
 
 import networkx as nx
-from ananke.graphs import ADMG, SG
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
+from ..dsl import Variable
 from ..graph import NxMixedGraph
 from ..struct import DSeparationJudgement
 from ..util.combinatorics import powerset
 
 __all__ = [
     "are_d_separated",
     "minimal",
     "get_conditional_independencies",
 ]
 
 
 def get_conditional_independencies(
-    graph: Union[NxMixedGraph, SG],
+    graph: NxMixedGraph,
     *,
     policy=None,
     **kwargs,
 ) -> Set[DSeparationJudgement]:
     """Get the conditional independencies from the given ADMG.
 
-    Conditional independencies is the minmal set of d-separation judgements to cover
+    Conditional independencies is the minimal set of d-separation judgements to cover
     the unique left/right combinations in all valid d-separation.
 
     :param graph: An acyclic directed mixed graph
     :param policy: Retention policy when more than one conditional independency option exists (see minimal for details)
-    :param kwargs: Other keyword arguments are passed to d_separations
+    :param kwargs: Other keyword arguments are passed to :func:`d_separations`
     :return: A set of conditional dependencies
 
     .. seealso:: Original issue https://github.com/y0-causal-inference/y0/issues/24
     """
-    if isinstance(graph, NxMixedGraph):
-        graph = graph.to_admg()
     if policy is None:
-        policy = topological_policy(graph)
+        policy = get_topological_policy(graph)
     return minimal(
         d_separations(graph, **kwargs),
         policy=policy,
     )
 
 
-def minimal(
-    judgements: Iterable[DSeparationJudgement], policy=None
-) -> Set[DSeparationJudgement]:
+def minimal(judgements: Iterable[DSeparationJudgement], policy=None) -> Set[DSeparationJudgement]:
     """Given some d-separations, reduces to a 'minimal' collection.
 
-    For indepdencies of the form A _||_ B | {C1, C2, ...} the minimal collection will::
+    For independencies of the form A _||_ B | {C1, C2, ...} the minimal collection will::
 
     - Have only one independency with the same A/B nodes.
     - If there are multiples sets of C-nodes, the kept d-separation will be the first/minimal
       element in the group sorted according to `policy` argument.
 
     The default policy is to sort by the shortest set of conditions & then lexicographic.
 
@@ -69,127 +65,148 @@
     """
     if policy is None:
         policy = _len_lex
     judgements = sorted(judgements, key=_judgement_grouper)
     return {min(vs, key=policy) for k, vs in groupby(judgements, _judgement_grouper)}
 
 
-def topological_policy(graph: ADMG):
+def get_topological_policy(
+    graph: NxMixedGraph,
+) -> Callable[[DSeparationJudgement], Tuple[int, int]]:
     """Sort d-separations by condition length and topological order.
 
     This policy will prefers small collections, and collections with variables earlier
     in topological order for collections of the same size.
 
-    :param graph: ADMG
+    :param graph: a mixed graph
     :return: A function suitable for use as a sort key on d-separations
     """
-    order = graph.topological_sort()
+    order = list(graph.topological_sort())
     return partial(_topological_policy, order=order)
 
 
-def _topological_policy(judgement: DSeparationJudgement, order):
+def _topological_policy(
+    judgement: DSeparationJudgement, order: Sequence[Variable]
+) -> Tuple[int, int]:
     return (
         len(judgement.conditions),
         sum((order.index(v) for v in judgement.conditions)),
     )
 
 
-def _judgement_grouper(judgement: DSeparationJudgement) -> Tuple[str, str]:
+def _judgement_grouper(judgement: DSeparationJudgement) -> Tuple[Variable, Variable]:
     """Simplify d-separation to just left & right element (for grouping left/right pairs)."""
     return judgement.left, judgement.right
 
 
 def _len_lex(judgement: DSeparationJudgement) -> Tuple[int, str]:
     """Sort by length of conditions & the lexicography a d-separation."""
-    return len(judgement.conditions), ",".join(judgement.conditions)
+    return len(judgement.conditions), ",".join(c.name for c in judgement.conditions)
+
 
+def disorient(graph: NxMixedGraph) -> nx.Graph:
+    """Convert an ADMG into a undirected (networkx) graph.
 
-def disorient(graph: SG) -> nx.Graph:
-    """Convert an :mod:`ananke` mixed directed/undirected into a undirected (networkx) graph."""
+    :param graph: An ADMG
+    :returns: A disoriented graph
+    """
     rv = nx.Graph()
-    rv.add_nodes_from(graph.vertices)
-    rv.add_edges_from(chain(graph.di_edges, graph.ud_edges, graph.bi_edges))
+    rv.add_nodes_from(graph.nodes())
+    rv.add_edges_from(graph.directed.edges())
+    rv.add_edges_from(graph.undirected.edges())
     return rv
 
 
-def get_moral_links(graph: SG) -> List[Tuple[str, str]]:
+def get_moral_links(graph: NxMixedGraph) -> List[Tuple[Variable, Variable]]:
     """Generate links to ensure all co-parents in a graph are linked.
 
     May generate links that already exist as we assume we are not working on a multi-graph.
 
     :param graph: Graph to process
     :return: An collection of edges to add.
     """
-    parents = [graph.parents([v]) for v in graph.vertices]
-    moral_links = [
-        *chain(*[combinations(nodes, 2) for nodes in parents if len(parents) > 1])
-    ]
+    parents = [graph.directed.predecessors(node) for node in graph.nodes()]
+    moral_links = [*chain(*[combinations(nodes, 2) for nodes in parents if len(parents) > 1])]
     return moral_links
 
 
 def are_d_separated(
-    graph: SG, a: str, b: str, *, conditions: Optional[Iterable[str]] = None
+    graph: NxMixedGraph,
+    a: Variable,
+    b: Variable,
+    *,
+    conditions: Optional[Iterable[Variable]] = None,
 ) -> DSeparationJudgement:
     """Test if nodes named by a & b are d-separated in G.
 
     a & b can be provided in either order and the order of conditions does not matter.
     However DSeparationJudgement may put things in canonical order.
 
     :param graph: Graph to test
     :param a: A node in the graph
     :param b: A node in the graph
     :param conditions: A collection of graph nodes
     :return: T/F and the final graph (as evidence)
+    :raises TypeError: if the left/right arguments or any conditions are
+        not Variable instances
     """
-    conditions = set(conditions) if conditions else set()
-    named = {a, b}.union(conditions)
+    if conditions is None:
+        conditions = set()
+    if not isinstance(a, Variable):
+        raise TypeError(f"left argument is not given as a Variable: {type(a)}: {a}")
+    if not isinstance(b, Variable):
+        raise TypeError(f"right argument is not given as a Variable: {type(b)}: {b}")
+    if not all(isinstance(c, Variable) for c in conditions):
+        raise TypeError(f"some conditions are not variables: {conditions}")
+
+    condition_names = {c for c in conditions}
+    named = {a, b}.union(condition_names)
 
     # Filter to ancestors
-    keep = graph.ancestors(named)
-    graph = copy.deepcopy(graph.subgraph(keep))
+    keep = graph.ancestors_inclusive(named)
+    sg = copy.deepcopy(graph.subgraph(keep))
 
     # Moralize (link parents of mentioned nodes)
-    for u, v in get_moral_links(graph):
-        graph.add_udedge(u, v)
+    for u, v in get_moral_links(sg):
+        sg.add_undirected_edge(u, v)
 
     # disorient & remove conditions
-    evidence_graph = disorient(graph)
+    evidence_graph = disorient(sg)
 
-    keep = set(evidence_graph.nodes) - set(conditions)
+    keep = set(evidence_graph.nodes) - set(condition_names)
     evidence_graph = evidence_graph.subgraph(keep)
 
     # check for path....
     separated = not nx.has_path(evidence_graph, a, b)  # If no path, then d-separated!
 
-    return DSeparationJudgement.create(
-        left=a, right=b, conditions=conditions, separated=separated
-    )
+    return DSeparationJudgement.create(left=a, right=b, conditions=conditions, separated=separated)
 
 
 def d_separations(
-    graph: Union[NxMixedGraph, SG],
+    graph: NxMixedGraph,
     *,
     max_conditions: Optional[int] = None,
     verbose: Optional[bool] = False,
     return_all: Optional[bool] = False,
 ) -> Iterable[DSeparationJudgement]:
     """Generate d-separations in the provided graph.
 
     :param graph: Graph to search for d-separations.
     :param max_conditions: Longest set of conditions to investigate
     :param return_all: If false (default) only returns the first d-separation per left/right pair.
     :param verbose: If true, prints extra output with tqdm
     :yields: True d-separation judgements
     """
-    if isinstance(graph, NxMixedGraph):
-        graph = graph.to_admg()
-
-    vertices = set(graph.vertices)
+    vertices = set(graph.nodes())
     for a, b in tqdm(
-        combinations(vertices, 2), disable=not verbose, desc="d-separation check"
+        combinations(vertices, 2),
+        disable=not verbose,
+        desc="Checking d-separations",
+        unit="pair",
+        total=len(vertices) * (len(vertices) - 1) // 2,
     ):
         for conditions in powerset(vertices - {a, b}, stop=max_conditions):
             judgement = are_d_separated(graph, a, b, conditions=conditions)
             if judgement.separated:
                 yield judgement
                 if not return_all:
                     break
```

### Comparing `y0-0.1.0/src/y0/algorithm/falsification.py` & `y0-0.2.0/src/y0/algorithm/falsification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,118 @@
 # -*- coding: utf-8 -*-
 
 """Causal graphs have implications that can be tested in the context of a specific dataset.
 
 This module includes algorithms to perform those tests.
 """
 
-from collections import abc
+from dataclasses import dataclass
 from typing import Iterable, Optional, Union
 
 import pandas as pd
-from ananke.graphs import SG
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from .conditional_independencies import get_conditional_independencies
+from ..graph import NxMixedGraph
 from ..struct import DSeparationJudgement
-from ..util.stat_utils import cressie_read
 
+__all__ = [
+    "get_graph_falsifications",
+    "get_falsifications",
+    "Falsifications",
+]
 
-class Falsifications(abc.Sequence):
+
+@dataclass
+class Falsifications:
     """A list of variables pairs that failed the D-separation and covariance test.
 
     Has an extra 'evidence' property that is a dictionary.
 
     - Keys are the d-separated variable pairs
     - Values are the covariances measured between them.
     """
 
-    def __init__(self, failures, evidence: pd.DataFrame):
-        """Create Falsifications result.
-
-        :param failures: Sequence of implications that did not pass
-        :param evidence: Collection of all implications tested
-        """
-        self._failures = failures
-        self.evidence = evidence
-
-    def __getitem__(self, i):
-        return self._failures[i]
+    #: Sequence of implications that did not pass
+    failures: pd.Series
+    #: Collection of all implications tested
+    evidence: pd.DataFrame
 
-    def __len__(self):
-        return len(self._failures)
 
-    def __repr__(self):
-        return repr(self._failures) + "+evidence"
-
-
-def falsifications(
-    to_test: Union[SG, Iterable[DSeparationJudgement]],
+def get_graph_falsifications(
+    graph: NxMixedGraph,
     df: pd.DataFrame,
-    significance_level: float = 0.05,
+    significance_level: Optional[float] = None,
     max_given: Optional[int] = None,
     verbose: bool = False,
 ) -> Falsifications:
     """Test conditional independencies implied by a graph.
 
-    :param to_test: Either a graph to generate d-separation from or a list of D-separations to check.
+    :param graph: An ADMG
     :param df: Data to check for consistency with a causal implications
     :param significance_level: Significance for p-value test
     :param max_given: The maximum set size in the power set of the vertices minus the d-separable pairs
     :param verbose: If true, use tqdm for status updates.
     :return: Falsifications report
     """
-    if isinstance(to_test, SG):
-        to_test = get_conditional_independencies(
-            to_test, max_conditions=max_given, verbose=verbose
-        )
+    judgements = get_conditional_independencies(graph, max_conditions=max_given, verbose=verbose)
+    return get_falsifications(
+        judgements=judgements,
+        df=df,
+        significance_level=significance_level,
+        verbose=verbose,
+    )
+
+
+HB_LEVEL_NAME = "Holm–Bonferroni level"
 
-    variances = {
-        (left, right, given): cressie_read(left, right, given, df, boolean=False)
-        for _, left, right, given in tqdm(
-            to_test, disable=not verbose, desc="Checking conditionals"
-        )
-    }
 
-    rows = [
-        (left, right, given, chi, p, dof)
-        for (left, right, given), (chi, dof, p) in variances.items()
-    ]
+def get_falsifications(
+    judgements: Union[NxMixedGraph, Iterable[DSeparationJudgement]],
+    df: pd.DataFrame,
+    significance_level: Optional[float] = None,
+    verbose: bool = False,
+) -> Falsifications:
+    """Test conditional independencies implied by a list of D-separation judgements.
 
+    :param judgements: A list of D-separation judgements to check.
+    :param df: Data to check for consistency with a causal implications
+    :param significance_level: Significance for p-value test
+    :param verbose: If true, use tqdm for status updates.
+    :return: Falsifications report
+    """
+    if significance_level is None:
+        significance_level = 0.05
+    variances = {
+        judgement: judgement.cressie_read(df)
+        for judgement in tqdm(judgements, disable=not verbose, desc="Checking conditionals")
+    }
+    evidence = pd.DataFrame(
+        [
+            (
+                judgement.left.name,
+                judgement.right.name,
+                "|".join(c.name for c in judgement.conditions),
+                chi,
+                p,
+                dof,
+            )
+            for judgement, (chi, p, dof) in variances.items()
+        ],
+        columns=["left", "right", "given", "chi^2", "p", "dof"],
+    )
+    evidence.sort_values("p", ascending=True, inplace=True)
     evidence = (
-        pd.DataFrame(rows, columns=["left", "right", "given", "chi^2", "p", "dof"])
-        .sort_values("p")
-        .assign(
-            **{
-                "Holm–Bonferroni level": significance_level
-                / pd.Series(range(len(rows) + 1, 0, -1))
-            }
+        evidence.assign(
+            **{HB_LEVEL_NAME: significance_level / pd.Series(range(len(evidence.index) + 1, 0, -1))}
         )
         .pipe(_assign_flags)
         .sort_values(["flagged", "dof"], ascending=False)
     )
 
-    failures = evidence[evidence["flagged"]][["left", "right", "given"]].apply(
-        tuple, axis="columns"
-    )
+    failures_df = evidence.loc[evidence["flagged"], ["left", "right", "given"]]
+    failures = failures_df.apply(tuple, axis="columns")
     return Falsifications(failures, evidence)
 
 
 def _assign_flags(df: pd.DataFrame) -> pd.DataFrame:
-    return df.assign(flagged=(df["p"] < df["Holm–Bonferroni level"]))
+    return df.assign(flagged=(df["p"] < df[HB_LEVEL_NAME]))
```

### Comparing `y0-0.1.0/src/y0/algorithm/simplify_latent.py` & `y0-0.2.0/src/y0/algorithm/simplify_latent.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import itertools as itt
 import logging
 from typing import Iterable, Mapping, NamedTuple, Optional, Set, Tuple
 
 import networkx as nx
 
+from ..dsl import Variable
 from ..graph import DEFAULT_TAG
 
 __all__ = [
     "simplify_latent_dag",
     "SimplifyResults",
     "remove_widow_latents",
     "transform_latents_with_parents",
@@ -26,16 +27,16 @@
 DEFAULT_SUFFIX = "_prime"
 
 
 class SimplifyResults(NamedTuple):
     """Results from the simplification of a LV-DAG."""
 
     graph: nx.DiGraph
-    widows: Set[str]
-    redundant: Set[str]
+    widows: Set[Variable]
+    redundant: Set[Variable]
 
 
 def simplify_latent_dag(graph: nx.DiGraph, tag: Optional[str] = None):
     """Apply Robin Evans' three algorithms in succession."""
     if tag is None:
         tag = DEFAULT_TAG
 
@@ -46,15 +47,15 @@
     return SimplifyResults(
         graph=graph,
         widows=widows,
         redundant=redundant,
     )
 
 
-def iter_latents(graph: nx.DiGraph, *, tag: Optional[str] = None) -> Iterable[str]:
+def iter_latents(graph: nx.DiGraph, *, tag: Optional[str] = None) -> Iterable[Variable]:
     """Iterate over nodes marked as latent.
 
     :param graph: A latent variable DAG
     :param tag: The tag for which variables are latent
     :yields: Nodes that are latent
     """
     if tag is None:
@@ -63,29 +64,27 @@
     for node in nx.topological_sort(graph):
         if graph.nodes[node][tag]:
             yield node
 
 
 def remove_widow_latents(
     graph: nx.DiGraph, tag: Optional[str] = None
-) -> Tuple[nx.DiGraph, Set[str]]:
+) -> Tuple[nx.DiGraph, Set[Variable]]:
     """Remove latents with no children (in-place).
 
     :param graph: A latent variable DAG
     :param tag: The tag for which variables are latent
     :returns: The graph, modified in place
     """
     remove = set(iter_widow_latents(graph, tag=tag))
     graph.remove_nodes_from(remove)
     return graph, remove
 
 
-def iter_widow_latents(
-    graph: nx.DiGraph, *, tag: Optional[str] = None
-) -> Iterable[str]:
+def iter_widow_latents(graph: nx.DiGraph, *, tag: Optional[str] = None) -> Iterable[Variable]:
     """Iterate over latent variables with no children.
 
     :param graph: A latent variable DAG
     :param tag: The tag for which variables are latent
     :yields: Nodes with no children
     """
     for node in iter_latents(graph, tag=tag):
@@ -109,15 +108,15 @@
         tag = DEFAULT_TAG
     if suffix is None:
         suffix = DEFAULT_SUFFIX
     for latent_node, parents, children in iter_middle_latents(graph, tag=tag):
         graph.remove_node(latent_node)
         graph.add_edges_from(itt.product(parents, children))
 
-        new_node = f"{latent_node}{suffix}"
+        new_node = Variable(f"{latent_node}{suffix}")
         graph.add_node(new_node, **{tag: True})
         for child in children:
             graph.add_edge(new_node, child)
 
     return graph
 
 
@@ -138,15 +137,15 @@
         graph.add_node(new_node, **{tag: True})
         for child in children:
             graph.add_edge(new_node, child)
 
 
 def iter_middle_latents(
     graph: nx.DiGraph, *, tag: Optional[str] = None
-) -> Iterable[Tuple[str, Set[str], Set[str]]]:
+) -> Iterable[Tuple[Variable, Set[Variable], Set[Variable]]]:
     """Iterate over latent nodes that have both parents and children (along with them).
 
     :param graph: A latent variable DAG
     :param tag: The tag for which variables are latent
     :yields: Nodes with both parents and children, along with the set of parents and set of children
     """
     for node in iter_latents(graph, tag=tag):
@@ -157,32 +156,30 @@
         if 0 == len(children):
             continue
         yield node, parents, children
 
 
 def remove_redundant_latents(
     graph: nx.DiGraph, tag: Optional[str] = None
-) -> Tuple[nx.DiGraph, Set[str]]:
+) -> Tuple[nx.DiGraph, Set[Variable]]:
     """Remove redundant latent variables.
 
     :param graph: A latent variable DAG
     :param tag: The tag for which variables are latent
     :returns: The graph, modified in place
     """
     remove = set(_iter_redundant_latents(graph, tag=tag))
     graph.remove_nodes_from(remove)
     return graph, remove
 
 
-def _iter_redundant_latents(graph, *, tag: Optional[str] = None) -> Iterable[str]:
-    latents: Mapping[str, Set[str]] = {
+def _iter_redundant_latents(graph: nx.DiGraph, *, tag: Optional[str] = None) -> Iterable[Variable]:
+    latents: Mapping[Variable, Set[Variable]] = {
         node: set(graph.successors(node)) for node in iter_latents(graph, tag=tag)
     }
-    for (left, left_children), (right, right_children) in itt.product(
-        latents.items(), repeat=2
-    ):
+    for (left, left_children), (right, right_children) in itt.product(latents.items(), repeat=2):
         if left_children == right_children and left > right:
             # if children are the same, keep the lower sort order node
             yield left
         elif left_children < right_children:
             # if left's children are a proper subset of right's children, we don't need left
             yield left
```

### Comparing `y0-0.1.0/src/y0/algorithm/taheri_design.py` & `y0-0.2.0/src/y0/algorithm/taheri_design.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,28 +9,25 @@
 import logging
 import textwrap
 from pathlib import Path
 from typing import Collection, Iterable, List, NamedTuple, Optional, Set, Tuple, Union
 
 import click
 import networkx as nx
-from ananke.graphs import ADMG
 from more_click import verbose_option
 from tabulate import tabulate
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
+from y0.algorithm.identify import Identification, Unidentifiable, identify
 from y0.algorithm.simplify_latent import simplify_latent_dag
+from y0.complexity import complexity
 from y0.dsl import Expression, P, Variable
-from y0.graph import (
-    DEFAULT_TAG,
-    NxMixedGraph,
-    admg_from_latent_variable_dag,
-    admg_to_latent_variable_dag,
-)
+from y0.graph import DEFAULT_TAG, NxMixedGraph
 from y0.identify import is_identifiable
+from y0.mutate import canonicalize
 from y0.util.combinatorics import powerset
 
 __all__ = [
     "taheri_design_admg",
     "taheri_design_dag",
     "Result",
     "draw_results",
@@ -39,29 +36,30 @@
 logger = logging.getLogger(__name__)
 
 
 class Result(NamedTuple):
     """Results from the LV-DAG check."""
 
     identifiable: bool
-    identifiability_expr: Optional[Expression]
+    #: The estimand returned from the related identification algorithm. Is none if not identifiable.
+    estimand: Optional[Expression]
     pre_nodes: int
     pre_edges: int
     post_nodes: int
     post_edges: int
-    latents: List[str]
-    observed: List[str]
+    latents: List[Variable]
+    observed: List[Variable]
     lvdag: nx.DiGraph
-    admg: ADMG
+    admg: NxMixedGraph
 
 
 def taheri_design_admg(
-    graph: Union[ADMG, NxMixedGraph],
-    cause: str,
-    effect: str,
+    graph: NxMixedGraph,
+    cause: Union[str, Variable],
+    effect: Union[str, Variable],
     *,
     tag: Optional[str] = None,
     stop: Optional[int] = None,
 ) -> List[Result]:
     """Run the brute force implementation of the Taheri Design algorithm on an ADMG.
 
     :param graph: An ADMG
@@ -70,33 +68,33 @@
     :param tag: The key for node data describing whether it is latent.
         If None, defaults to :data:`y0.graph.DEFAULT_TAG`.
     :param stop: Largest combination to get (None means length of the list and is the default)
     :return: A list of LV-DAG identifiability results. Will be length 2^(|V| - 2 - # bidirected edges)
     """
     if tag is None:
         tag = DEFAULT_TAG
-    if isinstance(graph, NxMixedGraph):
-        graph = graph.to_admg()
-    dag = admg_to_latent_variable_dag(graph, tag=tag)
+    cause = Variable.norm(cause)
+    effect = Variable.norm(effect)
+    dag = graph.to_latent_variable_dag(tag=tag)
     fixed_latent = {node for node, data in dag.nodes(data=True) if data[tag]}
     return _help(
         graph=dag,
         cause=cause,
         effect=effect,
         fixed_observed={cause, effect},
         fixed_latent=fixed_latent,
         tag=tag,
         stop=stop,
     )
 
 
 def taheri_design_dag(
     graph: nx.DiGraph,
-    cause: str,
-    effect: str,
+    cause: Union[str, Variable],
+    effect: Union[str, Variable],
     *,
     tag: Optional[str] = None,
     stop: Optional[int] = None,
 ) -> List[Result]:
     """Run the brute force implementation of the Taheri Design algorithm on a DAG.
 
     Identify all latent variable configurations inducible over the given DAG that result
@@ -106,31 +104,33 @@
     :param cause: The node that gets perturbed.
     :param effect: The node that we're interested in.
     :param tag: The key for node data describing whether it is latent.
         If None, defaults to :data:`y0.graph.DEFAULT_TAG`.
     :param stop: Largest combination to get (None means length of the list and is the default)
     :return: A list of LV-DAG identifiability results. Will be length 2^(|V| - 2)
     """
+    cause = Variable.norm(cause)
+    effect = Variable.norm(effect)
     return _help(
         graph=graph,
         cause=cause,
         effect=effect,
         fixed_observed={cause, effect},
         tag=tag,
         stop=stop,
     )
 
 
 def _help(
     graph: nx.DiGraph,
-    cause: str,
-    effect: str,
+    cause: Variable,
+    effect: Variable,
     *,
-    fixed_observed: Optional[Collection[str]] = None,
-    fixed_latent: Optional[Collection[str]] = None,
+    fixed_observed: Optional[Collection[Variable]] = None,
+    fixed_latent: Optional[Collection[Variable]] = None,
     tag: Optional[str] = None,
     stop: Optional[int] = None,
 ) -> List[Result]:
     return [
         _get_result(
             lvdag=lvdag,
             latents=latents,
@@ -146,67 +146,72 @@
             tag=tag,
             stop=stop,
         )
     ]
 
 
 def _get_result(
-    lvdag,
-    latents,
-    observed,
-    cause,
-    effect,
+    lvdag: nx.DiGraph,
+    latents: Collection[Variable],
+    observed: Collection[Variable],
+    cause: Variable,
+    effect: Variable,
     *,
     tag: Optional[str] = None,
 ) -> Result:
     # Book keeping
     pre_nodes, pre_edges = lvdag.number_of_nodes(), lvdag.number_of_edges()
 
     # Apply the robin evans algorithms
     simplify_latent_dag(lvdag, tag=tag)
     post_nodes, post_edges = lvdag.number_of_nodes(), lvdag.number_of_edges()
 
     # Convert the latent variable DAG to an ADMG
-    admg = admg_from_latent_variable_dag(lvdag, tag=tag)
+    admg = NxMixedGraph.from_latent_variable_dag(lvdag, tag=tag)
 
-    if cause not in admg.vertices:
+    if cause not in admg.nodes():
         raise KeyError(f"ADMG missing cause: {cause}")
-    if effect not in admg.vertices:
+    if effect not in admg.nodes():
         raise KeyError(f"ADMG missing effect: {effect}")
 
     # Check if the ADMG is identifiable under the (simple) causal query
-    query = P(Variable(effect) @ ~Variable(cause))
+    query = P(effect @ ~cause)
     identifiable = is_identifiable(admg, query)
-    identifiability_expr = None
+    try:
+        estimand: Optional[Expression] = canonicalize(
+            identify(Identification.from_expression(graph=admg, query=query))
+        )
+    except Unidentifiable:
+        estimand = None
 
     return Result(
         identifiable,
-        identifiability_expr=identifiability_expr,
+        estimand=estimand,
         pre_nodes=pre_nodes,
         pre_edges=pre_edges,
         post_nodes=post_nodes,
         post_edges=post_edges,
         latents=sorted(latents),
         observed=sorted(observed),
         lvdag=lvdag,
         admg=admg,
     )
 
 
 def iterate_lvdags(
     graph: nx.DiGraph,
-    fixed_observed: Optional[Collection[str]] = None,
-    fixed_latents: Optional[Collection[str]] = None,
+    fixed_observed: Optional[Collection[Variable]] = None,
+    fixed_latents: Optional[Collection[Variable]] = None,
     *,
     tag: Optional[str] = None,
     stop: Optional[int] = None,
-) -> Iterable[Tuple[Set[str], Set[str], nx.DiGraph]]:
+) -> Iterable[Tuple[Set[Variable], Set[Variable], nx.DiGraph]]:
     """Iterate over all possible latent variable configurations for the given graph.
 
-    :param graph: A regularDAG
+    :param graph: A regular DAG
     :param fixed_observed: Nodes to skip in the power set of all possible latent variables. Often, the cause and
         effect from a causal query will be used here to avoid setting them as latent (since they can not be).
     :param fixed_latents: Nodes to skip in the power set of all possible latent variables. Often, latent nodes
         from ADMG->LV-DAG conversion will go here.
     :param tag: The key for node data describing whether it is latent.
         If None, defaults to :data:`y0.graph.DEFAULT_TAG`.
     :param stop: Largest combination to get (None means length of the list and is the default)
@@ -214,34 +219,37 @@
     """
     if tag is None:
         tag = DEFAULT_TAG
 
     fixed_observed = set() if not fixed_observed else set(fixed_observed)
     fixed_latents = set() if not fixed_latents else set(fixed_latents)
 
-    inducible_nodes = set(graph)
+    inducible_nodes: Set[Variable] = set(graph)
     inducible_nodes.difference_update(fixed_observed)
     inducible_nodes.difference_update(fixed_latents)
 
     if stop is None:
         stop = len(inducible_nodes) - 1
-    it = powerset(
-        sorted(inducible_nodes),
-        stop=stop,
-        reverse=True,
-        use_tqdm=True,
-        tqdm_kwargs=dict(desc="LV powerset"),
+    it: Iterable[Set[Variable]] = map(
+        set,
+        powerset(
+            sorted(inducible_nodes),
+            stop=stop,
+            reverse=True,
+            use_tqdm=True,
+            tqdm_kwargs=dict(desc="LV powerset"),
+        ),
     )
 
     graph = graph.copy()
     for node in fixed_observed:
         graph.nodes[node][tag] = False
     for node in fixed_latents:
         graph.nodes[node][tag] = True
-    for induced_latents in map(set, it):
+    for induced_latents in it:
         yv = graph.copy()
         for node in inducible_nodes:
             yv.nodes[node][tag] = node in induced_latents
         yield induced_latents, inducible_nodes - induced_latents, yv  # type:ignore
 
 
 def draw_results(
@@ -259,32 +267,31 @@
         path = [path]
 
     rendered_results = [result for result in results if result.identifiable]
     if max_size is not None:
         rendered_results = [
             result
             for result in results
-            if len(result.admg.vertices) - len(result.latents) < max_size
+            if len(result.admg.nodes()) - len(result.latents) < max_size
         ]
 
     logger.debug("rendering %s identifiable queries", rendered_results)
 
     nrows = 1 + len(rendered_results) // ncols
-    fig, axes = plt.subplots(
-        ncols=ncols, nrows=nrows, figsize=(ncols * x_ratio, nrows * y_ratio)
-    )
+    fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=(ncols * x_ratio, nrows * y_ratio))
     it = itt.zip_longest(axes.ravel(), tqdm(rendered_results, desc="generating chart"))
     for i, (ax, result) in enumerate(it, start=1):
         if result is None:
             ax.axis("off")
         else:
-            mixed_graph = NxMixedGraph.from_admg(result.admg)
-            title = f"{i}) Latent: " + ", ".join(result.latents)
-            if result.identifiability_expr is not None:
-                title += f"\n${result.identifiability_expr.to_latex()}$"
+            mixed_graph = result.admg
+            title = f"{i}) Latent: " + ", ".join(f"${v.to_latex()}$" for v in result.latents)
+            estimand_complexity = complexity(result.estimand)
+            if result.estimand is not None:
+                title += f"\n${result.estimand.to_latex()}$\n$C={estimand_complexity}$"
             mixed_graph.draw(ax=ax, title="\n".join(textwrap.wrap(title, width=45)))
 
     fig.tight_layout()
 
     for _path in tqdm(path, desc="saving"):
         logger.info("saving to %s", _path)
         fig.savefig(_path, dpi=400)
@@ -295,68 +302,69 @@
     rows = [
         (
             i,
             result.identifiable,
             result.post_nodes - result.pre_nodes,
             result.post_edges - result.pre_edges,
             len(result.latents),
-            ", ".join(result.latents),
+            ", ".join(f"${v.to_latex()}$" for v in result.latents),
         )
         for i, result in enumerate(results, start=1)
     ]
-    print(
-        tabulate(
-            rows, headers=["Row", "ID?", "Node Simp.", "Edge Simp.", "N", "Latents"]
-        ),
+    print(  # noqa:T201
+        tabulate(rows, headers=["Row", "ID?", "Node Simp.", "Edge Simp.", "N", "Latents"]),
         file=file,
     )
 
 
 @click.command()
 @verbose_option
 def main():
     """Run the algorithm on the IGF graph with the PI3K/Erk example."""
     import pystow
-    from y0.resources import VIRAL_PATHOGENESIS_PATH
-    from y0.graph import NxMixedGraph
 
-    viral_pathogenesis_admg = NxMixedGraph.from_causalfusion_path(
-        VIRAL_PATHOGENESIS_PATH
-    )
+    from y0.examples import igf_example
 
-    results = taheri_design_admg(
-        viral_pathogenesis_admg, cause="EGFR", effect="CytokineStorm", stop=5
-    )
+    results = taheri_design_dag(igf_example.graph.directed, cause="PI3K", effect="Erk", stop=3)
+    # print_results(results)
     draw_results(
         results,
         [
-            pystow.join("y0", "viral_pathogenesis_egfr.png"),
-            pystow.join("y0", "viral_pathogenesis_egfr.svg"),
+            pystow.join("y0", name="ifg_identifiable_configs.png"),
+            pystow.join("y0", name="ifg_identifiable_configs.svg"),
         ],
+        ncols=3,
     )
+    import sys
+
+    sys.exit(0)
+
+    from y0.graph import NxMixedGraph
+    from y0.resources import VIRAL_PATHOGENESIS_PATH
+
+    viral_pathogenesis_admg = NxMixedGraph.from_causalfusion_path(VIRAL_PATHOGENESIS_PATH)
 
     results = taheri_design_admg(
-        viral_pathogenesis_admg, cause=r"sIL6R\alpha", effect="CytokineStorm", stop=5
+        viral_pathogenesis_admg, cause="EGFR", effect="CytokineStorm", stop=5
     )
     draw_results(
         results,
         [
-            pystow.join("y0", "viral_pathogenesis_sIL6ra.png"),
-            pystow.join("y0", "viral_pathogenesis_sIL6ra.svg"),
+            pystow.join("y0", name="viral_pathogenesis_egfr.png"),
+            pystow.join("y0", name="viral_pathogenesis_egfr.svg"),
         ],
     )
 
-    from y0.examples import igf_graph
-
-    results = taheri_design_dag(igf_graph, cause="PI3K", effect="Erk")
-    print_results(results)
+    results = taheri_design_admg(
+        viral_pathogenesis_admg, cause=r"sIL6R\alpha", effect="CytokineStorm", stop=5
+    )
     draw_results(
         results,
         [
-            pystow.join("y0", "ifg_identifiable_configs.png"),
-            pystow.join("y0", "ifg_identifiable_configs.svg"),
+            pystow.join("y0", name="viral_pathogenesis_sIL6ra.png"),
+            pystow.join("y0", name="viral_pathogenesis_sIL6ra.svg"),
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `y0-0.1.0/src/y0/causaleffect.py` & `y0-0.2.0/src/y0/causaleffect.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/cli.py` & `y0-0.2.0/src/y0/cli.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/identify.py` & `y0-0.2.0/src/y0/identify.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,67 @@
 # -*- coding: utf-8 -*-
 
 """Implementations of the identify algorithm from Shpitser and Pearl."""
 
 from typing import List, Set, Tuple, Union
 
-from ananke.graphs import ADMG
-from ananke.identification import OneLineID
-
 from .dsl import (
     CounterfactualVariable,
     Distribution,
-    Intervention,
     Probability,
     Variable,
+    _get_outcome_variables,
+    _get_treatment_variables,
 )
 from .graph import NxMixedGraph
 
 __all__ = [
     "is_identifiable",
 ]
 
 
 def _get_treatments(variables: Set[Variable]) -> List[str]:
-    return list(
-        {variable.name for variable in variables if isinstance(variable, Intervention)}
-    )
+    return [variable.name for variable in _get_treatment_variables(variables)]
 
 
 def _get_outcomes(variables: Set[Variable]) -> List[str]:
-    return list(
-        {
-            variable.name
-            for variable in variables
-            if not isinstance(variable, Intervention)
-        }
-    )
+    return [variable.name for variable in _get_outcome_variables(variables)]
 
 
-def _all_counterfactual(distribution: Distribution) -> bool:
-    return all(
-        isinstance(variable, CounterfactualVariable)
-        for variable in distribution.children
-    )
+def _all_counterfactual(distribution: Union[Probability, Distribution]) -> bool:
+    return all(isinstance(variable, CounterfactualVariable) for variable in distribution.children)
 
 
-def _all_intervened_same(distribution: Distribution) -> bool:
+def _all_intervened_same(distribution: Union[Probability, Distribution]) -> bool:
     return 1 == len(
         {
             variable.interventions  # type:ignore
             for variable in distribution.children
         }
     )
 
 
-def _get_to(query: Distribution) -> Tuple[List[str], List[str]]:
+def _get_to(query: Union[Probability, Distribution]) -> Tuple[List[str], List[str]]:
     if not _all_counterfactual(query):
-        raise ValueError(
-            "all variables in input distribution should be counterfactuals"
-        )
+        raise ValueError("all variables in input distribution should be counterfactuals")
 
     if not _all_intervened_same(query):
         raise ValueError("not all variables are invervened on the same")
 
     treatments = [
-        intervention.name
-        for intervention in query.children[0].interventions  # type:ignore
+        intervention.name for intervention in query.children[0].interventions  # type:ignore
     ]
     outcomes = [variable.name for variable in query.children]
     return treatments, outcomes
 
 
-def is_identifiable(
-    graph: Union[ADMG, NxMixedGraph], query: Union[Probability, Distribution]
-) -> bool:
+def is_identifiable(graph: NxMixedGraph, query: Union[Probability, Distribution]) -> bool:
     """Check if the expression is identifiable.
 
-    :param graph: Either an Ananke graph or y0 NxMixedGraph that can be converted to an Ananke graph
+    :param graph: An ADMG
     :param query: A probability distribution with the following properties:
 
         1. There are no conditions
         2. All variables are counterfactuals
         3. The set of interventions on each counterfactual variable are the same
     :raises ValueError: If the given probability distribution does not meet the above properties
     :returns: Whether the graph is identifiable under the causal query.
@@ -109,24 +91,36 @@
         graph.add_directed_edge('X', 'Y')
         graph.add_directed_edge('X', 'Z')
         graph.add_directed_edge('Z', 'Y')
         graph.add_undirected_edge('Y', 'Z')
 
         assert is_identifiable(graph, P(Y @ ~X))
     """
-    if isinstance(graph, NxMixedGraph):
-        graph = graph.to_admg()
-
-    if isinstance(query, Probability):
-        query = query.distribution
-
     if query.is_conditioned():
         raise ValueError("input distribution should not have any conditions")
 
     treatments, outcomes = _get_to(query)
 
-    one_line_id = OneLineID(
-        graph=graph,
-        treatments=treatments,
-        outcomes=outcomes,
-    )
-    return one_line_id.id()
+    try:
+        from ananke.identification import OneLineID
+    except ImportError:
+        from y0.algorithm.identify import Identification, Unidentifiable, identify
+
+        try:
+            identify(
+                Identification.from_expression(
+                    graph=graph,
+                    query=query,
+                )
+            )
+        except Unidentifiable:
+            return False
+        else:
+            return True
+    else:
+        graph = graph.to_admg()
+        one_line_id = OneLineID(
+            graph=graph,
+            treatments=treatments,
+            outcomes=outcomes,
+        )
+        return one_line_id.id()
```

### Comparing `y0-0.1.0/src/y0/mutate/canonicalize_expr.py` & `y0-0.2.0/src/y0/mutate/canonicalize_expr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
 
 """Implementation of the canonicalization algorithm."""
 
-from typing import Mapping, Optional, Sequence, Tuple, Union
+from operator import attrgetter
+from typing import Iterable, Mapping, Optional, Sequence, Tuple, Union
 
 from ..dsl import (
     CounterfactualVariable,
     Distribution,
     Expression,
     Fraction,
-    Intervention,
+    One,
     Probability,
     Product,
     Sum,
     Variable,
+    Zero,
     ensure_ordering,
 )
 
 __all__ = [
     "canonicalize",
+    "canonical_expr_equal",
 ]
 
 
 def canonicalize(
     expression: Expression, ordering: Optional[Sequence[Union[str, Variable]]] = None
 ) -> Expression:
     """Canonicalize an expression that meets the markov condition with respect to the given ordering.
@@ -31,16 +34,16 @@
     :param ordering: A toplogical ordering. If none is given, it is assigned by sort order of the variable names.
     :return: A canonical expression
     """
     canonicalizer = Canonicalizer(ensure_ordering(expression, ordering=ordering))
     return canonicalizer.canonicalize(expression)
 
 
-def _sort_probability_key(probability: Probability) -> str:
-    return probability.distribution.children[0].name
+def _sort_probability_key(probability: Probability) -> Tuple[str, ...]:
+    return tuple(child.name for child in probability.children)
 
 
 class Canonicalizer:
     """A data structure to support application of the canonicalize algorithm."""
 
     ordering: Sequence[Variable]
     ordering_level: Mapping[str, int]
@@ -52,23 +55,21 @@
 
         :raises ValueError: if the ordering has duplicates
         """
         if len(set(ordering)) != len(ordering):
             raise ValueError(f"ordering has duplicates: {ordering}")
 
         self.ordering = ordering
-        self.ordering_level = {
-            variable.name: level for level, variable in enumerate(self.ordering)
-        }
+        self.ordering_level = {variable.name: level for level, variable in enumerate(self.ordering)}
 
     def _canonicalize_probability(self, expression: Probability) -> Probability:
         return Probability(
             Distribution(
-                children=self._sorted(expression.distribution.children),
-                parents=self._sorted(expression.distribution.parents),
+                children=self._sorted(expression.children),
+                parents=self._sorted(expression.parents),
             )
         )
 
     def _sorted(self, variables: Tuple[Variable, ...]) -> Tuple[Variable, ...]:
         return tuple(
             sorted(
                 (self._canonicalize_variable(variable) for variable in variables),
@@ -76,82 +77,112 @@
             )
         )
 
     def _canonicalize_variable(self, variable: Variable) -> Variable:
         if isinstance(variable, CounterfactualVariable):
             return CounterfactualVariable(
                 name=variable.name,
-                interventions=tuple(
-                    sorted(variable.interventions, key=self._intervention_key)
-                ),
+                star=variable.star,
+                interventions=tuple(sorted(variable.interventions)),
             )
         else:
             return variable
 
-    @staticmethod
-    def _intervention_key(intervention: Intervention):
-        return intervention.name, intervention.star
-
     def _sorted_key(self, variable: Variable) -> int:
         return self.ordering_level[variable.name]
 
     def canonicalize(self, expression: Expression) -> Expression:
         """Canonicalize an expression.
 
         :param expression: An uncanonicalized expression
         :return: A canonicalized expression
         :raises TypeError: if an object with an invalid type is passed
         """
         if isinstance(expression, Probability):  # atomic
             return self._canonicalize_probability(expression)
         elif isinstance(expression, Sum):
+            if not expression.ranges:  # flatten unnecessary sum
+                return self.canonicalize(expression.expression)
             return Sum(
                 expression=self.canonicalize(expression.expression),
-                ranges=expression.ranges,
+                ranges=self._sorted(expression.ranges),
             )
         elif isinstance(expression, Product):
+            if 1 == len(expression.expressions):  # flatten unnecessary product
+                return self.canonicalize(expression.expressions[0])
+
             probabilities = []
             other = []
-            for subexpr in expression.expressions:
+            for subexpr in _flatten_product(expression):
                 subexpr = self.canonicalize(subexpr)
                 if isinstance(subexpr, Probability):
                     probabilities.append(subexpr)
+                elif isinstance(subexpr, One):
+                    continue
+                elif isinstance(subexpr, Zero):
+                    return Zero()  # If there's an explicit zero, then return zero
                 else:
                     other.append(subexpr)
-            probabilities = sorted(probabilities, key=_sort_probability_key)
+            if not probabilities and not other:
+                return One()
 
+            probabilities = sorted(probabilities, key=_sort_probability_key)
             # If other is empty, this is also atomic
             other = sorted(other, key=self._nonatomic_key)
-            return Product((*probabilities, *other))
+            expressions = (*probabilities, *other)
+            if len(expressions) == 1:
+                return expressions[0]
+            return Product(expressions)
         elif isinstance(expression, Fraction):
-            return Fraction(
-                numerator=self.canonicalize(expression.numerator),
-                denominator=self.canonicalize(expression.denominator),
-            )
+            numerator = self.canonicalize(expression.numerator)
+            # TODO check if there's a zero in numerator, then return zero if so
+            denominator = self.canonicalize(expression.denominator)
+            if isinstance(denominator, One):
+                return numerator
+            if numerator == denominator:
+                return One()
+            return numerator / denominator  # TODO
+        elif isinstance(expression, (One, Zero)):
+            return expression
         else:
             raise TypeError
 
     def _nonatomic_key(self, expression: Expression):
         """Generate a sort key for a *canonical* expression.
 
         :param expression: A canonical expression
         :returns: A tuple in which the first element is the integer priority for the expression
             and the rest depends on the expression type.
         :raises TypeError: if an invalid expression type is given
         """
         if isinstance(expression, Probability):
-            return 0, expression.distribution.children[0].name
+            return 0, expression.children[0].name
         elif isinstance(expression, Sum):
             return 1, *self._nonatomic_key(expression.expression)
         elif isinstance(expression, Product):
-            inner_keys = (
-                self._nonatomic_key(sexpr) for sexpr in expression.expressions
-            )
+            inner_keys = (self._nonatomic_key(sexpr) for sexpr in expression.expressions)
             return 2, *inner_keys
         elif isinstance(expression, Fraction):
             return (
                 3,
                 self._nonatomic_key(expression.numerator),
                 self._nonatomic_key(expression.denominator),
             )
+        elif isinstance(expression, (One, Zero)):
+            return 4, expression.to_text()
+            # TODO find an example where this happens
         else:
             raise TypeError
+
+
+def _flatten_product(product: Product) -> Iterable[Expression]:
+    for expression in product.expressions:
+        if isinstance(expression, Product):
+            yield from _flatten_product(expression)
+        else:
+            yield expression
+
+
+def canonical_expr_equal(left: Expression, right: Expression) -> bool:
+    """Return True if two expressions are equal after canonicalization."""
+    ordering = sorted(left.get_variables() | right.get_variables(), key=attrgetter("name"))
+    return canonicalize(left, ordering) == canonicalize(right, ordering)
```

### Comparing `y0-0.1.0/src/y0/mutate/chain.py` & `y0-0.2.0/src/y0/mutate/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Operations for mutating and simplifying expressions."""
 
 from ..dsl import (
     Distribution,
+    Expression,
     Fraction,
     OrderingHint,
     P,
     Probability,
     Product,
     ensure_ordering,
 )
@@ -15,17 +16,15 @@
 __all__ = [
     "chain_expand",
     "fraction_expand",
     "bayes_expand",
 ]
 
 
-def chain_expand(
-    p: Probability, *, reorder: bool = True, ordering: OrderingHint = None
-) -> Product:
+def chain_expand(p: Probability, *, reorder: bool = True, ordering: OrderingHint = None) -> Product:
     r"""Expand a probability distribution to a product of conditional probabilities on single variables.
 
     :param p: The given probability expression
     :param reorder: Should the variables be reordered with respect to the ordering before expanding? This is important
         because there are a variety of equivalent expressions that can't be directly matched.
     :param ordering: An ordering to be used if ``reorder`` is true. If none, automatically generates a canonical
         ordering using :func:`y0.dsl.ensure_ordering`.
@@ -35,41 +34,41 @@
 
     Two variables:
 
     .. math::
         P(X,Y)=P(X|Y)*P(Y)
 
     >>> from y0.dsl import P, X, Y
-    >>> assert chain_expand(P(X | Y)) == P(X | Y) * P(Y)
+    >>> assert chain_expand(P(X, Y)) == P(X | Y) * P(Y)
 
     The recurrence relation for many variables is defined as:
 
     .. math::
         P(X_n,\dots,X_1) = P(X_n|X_{n-1},\dots,X_1) \times P(X_{n-1},\dots,X_1)
 
     >>> from y0.dsl import P, A, X, Y, Z
-    >>> chain_expand(P(X, Y, Z)) == P(X | (Y, Z)) * P(Y | Z) * P(Z)
+    >>> assert chain_expand(P(X, Y, Z)) == P(X | Y, Z) * P(Y | Z) * P(Z)
 
     Extra conditions come along for the ride.
 
-    >>> chain_expand(P(X & Y | A)) == P(X | (Y, Z, A)) * P(Y | (Z, A)) * P(Z | A)
+    >>> assert chain_expand(P(X, Y, Z | A)) == P(X | Y, Z, A) * P(Y | Z, A) * P(Z | A)
     """
     if reorder:
         _ordering = ensure_ordering(p, ordering=ordering)
-        if any(v not in _ordering for v in p.distribution.children):
+        if any(v not in _ordering for v in p.children):
             raise ValueError
-        ordered_children = tuple(v for v in _ordering if v in p.distribution.children)
+        ordered_children = tuple(v for v in _ordering if v in p.children)
     else:
-        ordered_children = p.distribution.children
+        ordered_children = p.children
 
     return Product(
         tuple(
             P(
                 Distribution(children=(ordered_children[i],)).given(
-                    ordered_children[i + 1 :] + p.distribution.parents
+                    ordered_children[i + 1 :] + p.parents
                 )
             )
             for i in range(len(ordered_children))
         )
     )
 
 
@@ -85,23 +84,23 @@
         P(A | B) = \frac{P(A,B)}{P(B)}
 
     In general, with many children $Y_i$ and many parents $X_i$:
 
     .. math::
         P(Y_1,\dots,Y_n | X_1, \dots, X_m) = \frac{P(Y_1,\dots,Y_n,X_1,\dots,X_m)}{P(X_1,\dots,X_m)}
     """
-    return p.uncondition() / P(p.distribution.parents)
+    return Fraction(p.uncondition(), P(p.parents))
 
 
-def bayes_expand(p: Probability) -> Fraction:
+def bayes_expand(p: Probability) -> Expression:
     r"""Expand a probability distribution using Bayes' theorem.
 
     :param p: The given probability expression, with arbitrary number of children and parents
     :returns: A fraction representing the joint distribution
 
     .. math::
         P(Y_1,\dots,Y_n|X_1,\dots,X_m)
         = \frac{P(Y_1,\dots,Y_n,X_1,\dots,X_m)}{\sum_{Y_1,\dots,Y_n} P(Y_1,\dots,Y_n,X_1,\dots,X_m)}
 
     .. note:: This expansion will create a different but equal expression to :func:`fraction_expand`.
     """
-    return p.uncondition().marginalize(p.distribution.children)
+    return p.uncondition().normalize_marginalize(p.children)
```

### Comparing `y0-0.1.0/src/y0/parser/ce/grammar.py` & `y0-0.2.0/src/y0/parser/craig/grammar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # -*- coding: utf-8 -*-
 
 """A parser for Craig-like probability expressions based on :mod:`pyparsing`."""
 
-import logging
-
 from pyparsing import (
     Forward,
     Group,
     OneOrMore,
     Optional,
-    ParseException,
     ParseResults,
     StringEnd,
     StringStart,
     Suppress,
 )
 
 from .utils import probability_pe, qfactor_pe, variables_pe
 from ...dsl import Expression, Fraction, Product, Sum
 
 __all__ = [
-    "parse_causaleffect",
+    "parse_craig",
     "grammar",
 ]
 
-logger = logging.getLogger(__name__)
 expr = Forward()
 
 
 def _make_sum(_s, _l, tokens: ParseResults) -> Sum:
     return Sum(
         ranges=tuple(tokens["ranges"].asList()) if "ranges" in tokens else tuple(),
         expression=tokens["expression"],
@@ -50,24 +46,26 @@
         return Product(tuple(tokens))
 
 
 # auto-product
 rr = OneOrMore(probability_pe | qfactor_pe | expr).setParseAction(_make_product)
 
 sum_pe = (
-    Suppress("\\sum_{")
+    Suppress("[")
+    + Suppress("sum_{")
     + Optional(Group(variables_pe).setResultsName("ranges"))
     + Suppress("}")
     + rr.setResultsName("expression")
+    + Suppress("]")
 )
 sum_pe.setName("sum")
 sum_pe.setParseAction(_make_sum)
 
 fraction_pe = (
-    Suppress("\\frac_{")
+    Suppress("frac_{")
     + rr.setResultsName("numerator")
     + Suppress("}{")
     + rr.setResultsName("denominator")
     + Suppress("}")
 )
 fraction_pe.setName("fraction")
 fraction_pe.setParseAction(_make_frac)
@@ -76,16 +74,11 @@
 
 # TODO enable products?
 
 grammar = StringStart() + expr + StringEnd()
 grammar.setName("probabilityGrammar")
 
 
-def parse_causaleffect(s: str) -> Expression:
-    """Parse a causaleffect probability expression."""
-    try:
-        x = grammar.parseString(s)
-    except ParseException:
-        logger.warning("could not parse %s", s)
-        raise
-    else:
-        return x.asList()[0]
+def parse_craig(s: str) -> Expression:
+    """Parse a Craig-like probability expression."""
+    x = grammar.parseString(s)
+    return x.asList()[0]
```

### Comparing `y0-0.1.0/src/y0/parser/ce/utils.py` & `y0-0.2.0/src/y0/parser/ce/utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/parser/craig/grammar.py` & `y0-0.2.0/src/y0/parser/ce/grammar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # -*- coding: utf-8 -*-
 
 """A parser for Craig-like probability expressions based on :mod:`pyparsing`."""
 
+import logging
+
 from pyparsing import (
     Forward,
     Group,
     OneOrMore,
     Optional,
+    ParseException,
     ParseResults,
     StringEnd,
     StringStart,
     Suppress,
 )
 
 from .utils import probability_pe, qfactor_pe, variables_pe
-from ...dsl import Expression, Fraction, Product, Sum
+from ...dsl import Expression, Fraction, Product, Sum, _sorted_variables
 
 __all__ = [
-    "parse_craig",
+    "parse_causaleffect",
     "grammar",
 ]
 
+logger = logging.getLogger(__name__)
 expr = Forward()
 
 
 def _make_sum(_s, _l, tokens: ParseResults) -> Sum:
     return Sum(
-        ranges=tuple(tokens["ranges"].asList()) if "ranges" in tokens else tuple(),
+        ranges=_sorted_variables(tokens["ranges"].asList() if "ranges" in tokens else []),
         expression=tokens["expression"],
     )
 
 
 def _make_frac(_s, _l, tokens: ParseResults) -> Fraction:
     return Fraction(
         numerator=tokens["numerator"],
@@ -46,26 +50,24 @@
         return Product(tuple(tokens))
 
 
 # auto-product
 rr = OneOrMore(probability_pe | qfactor_pe | expr).setParseAction(_make_product)
 
 sum_pe = (
-    Suppress("[")
-    + Suppress("sum_{")
+    Suppress("\\sum_{")
     + Optional(Group(variables_pe).setResultsName("ranges"))
     + Suppress("}")
     + rr.setResultsName("expression")
-    + Suppress("]")
 )
 sum_pe.setName("sum")
 sum_pe.setParseAction(_make_sum)
 
 fraction_pe = (
-    Suppress("frac_{")
+    Suppress("\\frac_{")
     + rr.setResultsName("numerator")
     + Suppress("}{")
     + rr.setResultsName("denominator")
     + Suppress("}")
 )
 fraction_pe.setName("fraction")
 fraction_pe.setParseAction(_make_frac)
@@ -74,11 +76,16 @@
 
 # TODO enable products?
 
 grammar = StringStart() + expr + StringEnd()
 grammar.setName("probabilityGrammar")
 
 
-def parse_craig(s: str) -> Expression:
-    """Parse a Craig-like probability expression."""
-    x = grammar.parseString(s)
-    return x.asList()[0]
+def parse_causaleffect(s: str) -> Expression:
+    """Parse a causaleffect probability expression."""
+    try:
+        x = grammar.parseString(s)
+    except ParseException:
+        logger.warning("could not parse %s", s)
+        raise
+    else:
+        return x.asList()[0]
```

### Comparing `y0-0.1.0/src/y0/parser/craig/utils.py` & `y0-0.2.0/src/y0/parser/craig/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ...dsl import (
     CounterfactualVariable,
     Distribution,
     Intervention,
     Probability,
     QFactor,
     Variable,
+    _sorted_variables,
 )
 
 __all__ = [
     "probability_pe",
     "variables_pe",
     "qfactor_pe",
 ]
@@ -56,32 +57,37 @@
     )
 
 
 def _make_probability(_s, _l, tokens: ParseResults) -> Probability:
     children, parents = tokens["children"].asList(), tokens["parents"].asList()
     if not children:
         raise ValueError
-    return Probability(Distribution(children=tuple(children), parents=tuple(parents)))
+    return Probability(
+        Distribution(
+            children=_sorted_variables(children),
+            parents=_sorted_variables(parents),
+        )
+    )
 
 
 def _make_q(_s, _l, tokens: ParseResults) -> QFactor:
-    codomain, domain = tokens["codomain"].asList(), tokens["domain"].asList()
-    return QFactor(codomain=tuple(codomain), domain=tuple(domain))
+    return QFactor(
+        codomain=_sorted_variables(tokens["codomain"].asList()),
+        domain=_sorted_variables(tokens["domain"].asList()),
+    )
 
 
 # The suffix "pe" refers to :class:`pyparsing.ParserElement`, which is the
 #  class in pyparsing that everything inherits from
 star_pe = Optional("*")("star").setParseAction(_set_star)
 intervention_pe = letter("name") + star_pe
 intervention_pe.setParseAction(_make_intervention)
 interventions_pe = Optional(
     Suppress("_{")
-    + delimitedList(Group(intervention_pe).setParseAction(_unpack)).setResultsName(
-        "interventions"
-    )
+    + delimitedList(Group(intervention_pe).setParseAction(_unpack)).setResultsName("interventions")
     + Suppress("}"),
 )
 variable_pe = letter("name") + interventions_pe
 variable_pe.setParseAction(_make_variable)
 variable_pe.setName("variable")
 
 variables_pe = delimitedList(Group(variable_pe).setParseAction(_unpack))
```

### Comparing `y0-0.1.0/src/y0/parser/internal.py` & `y0-0.2.0/src/y0/parser/internal.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/predicates.py` & `y0-0.2.0/src/y0/predicates.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,16 @@
     :param expression: Any expression
     :return: if the expression satisfies the sum/product of markov kernels condition
     :raises TypeError: if an object with an invalid type is passed
     """
     if isinstance(expression, Probability):
         return expression.distribution.is_markov_kernel()
     elif isinstance(expression, Product):
-        return all(
-            has_markov_postcondition(subexpr) for subexpr in expression.expressions
-        )
+        return all(has_markov_postcondition(subexpr) for subexpr in expression.expressions)
     elif isinstance(expression, Sum):
         return has_markov_postcondition(expression.expression)
     elif isinstance(expression, Fraction):
-        return has_markov_postcondition(
-            expression.numerator
-        ) and has_markov_postcondition(expression.denominator)
+        return has_markov_postcondition(expression.numerator) and has_markov_postcondition(
+            expression.denominator
+        )
     else:
         raise TypeError
```

### Comparing `y0-0.1.0/src/y0/r_utils.py` & `y0-0.2.0/src/y0/r_utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/resources/asia.csv` & `y0-0.2.0/src/y0/resources/asia.csv`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/resources/viral_pathogenesis.json` & `y0-0.2.0/src/y0/resources/viral_pathogenesis.json`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/util/combinatorics.py` & `y0-0.2.0/src/y0/util/combinatorics.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/src/y0/util/stat_utils.py` & `y0-0.2.0/src/y0/util/stat_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #
 # Originally copied from: https://github.com/pgmpy/pgmpy/blob/dev/pgmpy/estimators/CITests.py
 # 20Feb2021
 
 """Statitistical tests for conditional independence with conditions."""
 
 from warnings import warn
+
 from scipy import stats
 
 
 def chi_square(X, Y, Z, data, boolean=True, **kwargs):
     r"""
     Chi-square conditional independence test.
     Tests the null hypothesis that X is independent from Y given Zs.
@@ -96,17 +97,15 @@
     >>> chi_square(X='A', Y='C', Z=[], data=data, boolean=True, significance_level=0.05)
     True
     >>> chi_square(X='A', Y='B', Z=['D'], data=data, boolean=True, significance_level=0.05)
     True
     >>> chi_square(X='A', Y='B', Z=['D', 'E'], data=data, boolean=True, significance_level=0.05)
     False
     """
-    return power_divergence(
-        X=X, Y=Y, Z=Z, data=data, boolean=boolean, lambda_="pearson", **kwargs
-    )
+    return power_divergence(X=X, Y=Y, Z=Z, data=data, boolean=boolean, lambda_="pearson", **kwargs)
 
 
 def g_sq(X, Y, Z, data, boolean=True, **kwargs):
     """
     G squared test for conditional independence. Also commonly known as G-test,
     likelihood-ratio or maximum likelihood statistical significance test.
     Tests the null hypothesis that X is independent of Y given Zs.
@@ -446,17 +445,15 @@
     >>> neyman(X='A', Y='C', Z=[], data=data, boolean=True, significance_level=0.05)
     True
     >>> neyman(X='A', Y='B', Z=['D'], data=data, boolean=True, significance_level=0.05)
     True
     >>> neyman(X='A', Y='B', Z=['D', 'E'], data=data, boolean=True, significance_level=0.05)
     False
     """
-    return power_divergence(
-        X=X, Y=Y, Z=Z, data=data, boolean=boolean, lambda_="neyman", **kwargs
-    )
+    return power_divergence(X=X, Y=Y, Z=Z, data=data, boolean=boolean, lambda_="neyman", **kwargs)
 
 
 def cressie_read(X, Y, Z, data, boolean=True, **kwargs):
     """
     Cressie Read statistic for conditional independence[1].
     Tests the null hypothesis that X is independent of Y given Zs.
 
@@ -606,17 +603,15 @@
     # Step 1: Check if the arguments are valid and type conversions.
     if hasattr(Z, "__iter__"):
         Z = list(Z)
     else:
         raise (f"Z must be an iterable. Got object type: {type(Z)}")
 
     if (X in Z) or (Y in Z):
-        raise ValueError(
-            f"The variables X or Y can't be in Z. Found {X if X in Z else Y} in Z."
-        )
+        raise ValueError(f"The variables X or Y can't be in Z. Found {X if X in Z else Y} in Z.")
 
     # Step 2: Do a simple contingency test if there are no conditional variables.
     if len(Z) == 0:
         chi, p_value, dof, expected = stats.chi2_contingency(
             data.groupby([X, Y]).size().unstack(Y, fill_value=0), lambda_=lambda_
         )
 
@@ -631,24 +626,18 @@
                     df.groupby([X, Y]).size().unstack(Y, fill_value=0), lambda_=lambda_
                 )
                 chi += c
                 dof += d
             except ValueError:
                 # If one of the values is 0 in the 2x2 table.
                 if isinstance(z_state, str):
-                    warn(
-                        f"Skipping the test {X} \u27C2 {Y} | {Z[0]}={z_state}. Not enough samples"
-                    )
+                    warn(f"Skipping the test {X} \u27C2 {Y} | {Z[0]}={z_state}. Not enough samples")
                 else:
-                    z_str = ", ".join(
-                        [f"{var}={state}" for var, state in zip(Z, z_state)]
-                    )
-                    warn(
-                        f"Skipping the test {X} \u27C2 {Y} | {z_str}. Not enough samples"
-                    )
+                    z_str = ", ".join([f"{var}={state}" for var, state in zip(Z, z_state)])
+                    warn(f"Skipping the test {X} \u27C2 {Y} | {z_str}. Not enough samples")
         p_value = 1 - stats.chi2.cdf(chi, df=dof)
 
     # Step 4: Return the values
     if boolean:
         return p_value >= kwargs["significance_level"]
     else:
         return chi, dof, p_value
```

### Comparing `y0-0.1.0/src/y0/version.py` & `y0-0.2.0/src/y0/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`y0` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
@@ -34,8 +34,8 @@
 
 def get_version(with_git_hash: bool = False):
     """Get the :mod:`y0` version string, including a git hash."""
     return f"{VERSION}-{get_git_hash()}" if with_git_hash else VERSION
 
 
 if __name__ == "__main__":
-    print(get_version(with_git_hash=True))
+    print(get_version(with_git_hash=True))  # noqa:T201
```

### Comparing `y0-0.1.0/src/y0.egg-info/PKG-INFO` & `y0-0.2.0/src/y0.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,171 +1,285 @@
 Metadata-Version: 2.1
 Name: y0
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python code for causal modeling.
 Home-page: https://github.com/y0-causal-inference/y0
+Download-URL: https://github.com/y0-causal-inference/y0/releases
 Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: BSD-3-Clause
-Download-URL: https://github.com/y0-causal-inference/y0/releases
 Project-URL: Bug Tracker, https://github.com/y0-causal-inference/y0/issues
 Project-URL: Source Code, https://github.com/y0-causal-inference/y0
-Description: <p align="center">
-          <img src="docs/source/logo.png" height="120">
-        </p>
-        
-        <h1 align="center">
-          y0
-        </h1>
-        
-        <p align="center">
-            <a href="https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests">
-                <img alt="Tests" src="https://github.com/y0-causal-inference/y0/workflows/Tests/badge.svg" />
-            </a>
-           <a href="https://github.com/cthoyt/cookiecutter-python-package">
-              <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-python--package-yellow" /> 
-           </a>
-            <a href="https://pypi.org/project/y0">
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/y0" />
-            </a>
-            <a href="https://pypi.org/project/y0">
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/y0" />
-            </a>
-            <a href="https://github.com/y0-causal-inference/y0/blob/main/LICENSE">
-                <img alt="PyPI - License" src="https://img.shields.io/pypi/l/y0" />
-            </a>
-            <a href='https://y0.readthedocs.io/en/latest/?badge=latest'>
-                <img src='https://readthedocs.org/projects/y0/badge/?version=latest' alt='Documentation Status' />
-            </a>
-            <a href="https://zenodo.org/badge/latestdoi/328745468">
-                <img src="https://zenodo.org/badge/328745468.svg" alt="DOI">
-            </a>
-            <a href="https://github.com/psf/black">
-                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
-            </a>
-        </p>
-        
-        `y0` (pronounced "why not?") is Python code for causal inferencing.
-        
-        ## 💪 Getting Started
-        
-        > TODO show in a very small amount of space the **MOST** useful thing your package can do.
-        Make it as short as possible! You have an entire set of docs for later.
-        
-        ## ⬇️ Installation
-        
-        The most recent release can be installed from
-        [PyPI](https://pypi.org/project/y0/) with:
-        
-        ```bash
-        $ pip install y0
-        ```
-        
-        The most recent code and data can be installed directly from GitHub with:
-        
-        ```bash
-        $ pip install git+https://github.com/y0-causal-inference/y0.git
-        ```
-        
-        To install in development mode, use the following:
-        
-        ```bash
-        $ git clone git+https://github.com/y0-causal-inference/y0.git
-        $ cd y0
-        $ pip install -e .
-        ```
-        
-        ## ⚖️ License
-        
-        The code in this package is licensed under the [BSD-3-Clause
-        license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
-        
-        ## 🙏 Contributing
-        
-        Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
-        [CONTRIBUTING.rst](https://github.com/y0-causal-inference/y0/blob/master/CONTRIBUTING.rst) for more information on getting
-        involved.
-        
-        ## Acknowledgements
-        
-        ### Supporters
-        
-        This project has been supported by several organizations (in alphabetical order):
-        
-        - [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/)
-        - [Pacific Northwest National Laboratory](https://www.pnnl.org/)
-        
-        ### 💰 Funding
-        
-        The development of the Y0 Causal Inference Engine has been funded by the following grants:
-        
-        | Funding Body                                             | Program                                                                                                                       | Grant           |
-        |----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------|
-        | DARPA                                                    | [Automating Scientific Knowledge Extraction (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction) | HR00111990009   |
-        | PNNL Data Model Convergence Initiative    | [Causal Inference and Machine Learning Methods for Analysis of Security Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/converged-applications-projects) | 90001   |
-        
-        ### 🍪 Cookiecutter
-        
-        This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-        [cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
-        [cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-package) template.
-        
-        ## 🛠️ Development
-        
-        The final section of the README is for if you want to get involved by making a code contribution.
-        
-        ### ❓ Testing
-        
-        After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
-        run reproducibly with:
-        
-        ```shell
-        $ tox
-        ```
-        
-        Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests).
-        
-        ### 📦 Making a Release
-        
-        After installing the package in development mode and installing
-        `tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
-        in `tox.ini`. Run the following from the shell:
-        
-        ```shell
-        $ tox -e finish
-        ```
-        
-        This script does the following:
-        
-        1. Uses BumpVersion to switch the version number in the `setup.cfg` and
-           `src/y0/version.py` to not have the `-dev` suffix
-        2. Packages the code in both a tar archive and a wheel
-        3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
-           step
-        4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
-        5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
-           use `tox -e bumpversion minor` after.
-        
 Keywords: cthoyt,cookiecutter,structural causal modeling
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: r
+Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE
+
+<p align="center">
+  <img src="docs/source/logo.png" height="120">
+</p>
+
+<h1 align="center">
+  y0
+</h1>
+
+<p align="center">
+    <a href="https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests">
+        <img alt="Tests" src="https://github.com/y0-causal-inference/y0/workflows/Tests/badge.svg" />
+    </a>
+   <a href="https://github.com/cthoyt/cookiecutter-python-package">
+      <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
+   </a>
+    <a href="https://pypi.org/project/y0">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/y0" />
+    </a>
+    <a href="https://pypi.org/project/y0">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/y0" />
+    </a>
+    <a href="https://github.com/y0-causal-inference/y0/blob/main/LICENSE">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/y0" />
+    </a>
+    <a href='https://y0.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/y0/badge/?version=latest' alt='Documentation Status' />
+    </a>
+    <a href="https://zenodo.org/badge/latestdoi/328745468">
+        <img src="https://zenodo.org/badge/328745468.svg" alt="DOI">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+    </a>
+</p>
+
+`y0` (pronounced "why not?") is Python code for causal inference.
+
+## 💪 Getting Started
+
+### Representing Probability Expressions
+
+`y0` has a fully featured internal domain specific language for representing
+probability expressions:
+
+```python
+from y0.dsl import P, A, B
+
+# The probability of A given B
+expr_1 = P(A | B)
+
+# The probability of A given not B
+expr_2 = P(A | ~B)
+
+# The joint probability of A and B
+expr_3 = P(A, B)
+```
+
+It can also be used to manipulate expressions:
+
+```python
+from y0.dsl import P, A, B, Sum
+
+P(A, B).marginalize(A) == Sum[A](P(A, B))
+P(A, B).conditional(A) == P(A, B) / Sum[A](P(A, B))
+```
+
+DSL objects can be converted into strings with `str()` and parsed back
+using `y0.parser.parse_y0()`.
+
+A full demo of the DSL can be found in this
+[Jupyter Notebook](https://github.com/y0-causal-inference/y0/blob/main/notebooks/DSL%20Demo.ipynb)
+
+### Representing Causality
+
+`y0` has a notion of acyclic directed mixed graphs built on top of
+`networkx` that can be used to model causality:
+
+```python
+from y0.graph import NxMixedGraph
+from y0.dsl import X, Y, Z1, Z2
+
+# Example from:
+#   J. Pearl and D. Mackenzie (2018)
+#   The Book of Why: The New Science of Cause and Effect.
+#   Basic Books, p. 240.
+napkin = NxMixedGraph.from_edges(
+    directed=[
+        (Z2, Z1),
+        (Z1, X),
+        (X, Y),
+    ],
+    undirected=[
+        (Z2, X),
+        (Z2, Y),
+    ],
+)
+```
+
+`y0` has many pre-written examples in `y0.examples` from Pearl, Shpitser,
+Bareinboim, and others.
+
+### do Calculus
+
+`y0` provides _actual_ implementations of many algorithms that have remained
+unimplemented for the last 15 years of publications including:
+
+| Algorithm | Reference                                                                   |
+|-----------|-----------------------------------------------------------------------------|
+| ID        | [Shpitser and Pearl, 2006](https://dl.acm.org/doi/10.5555/1597348.1597382)  |
+| IDC       | [Shpitser and Pearl, 2008](https://www.jmlr.org/papers/v9/shpitser08a.html) |
+| ID*       | [Shpitser and Pearl, 2012](https://arxiv.org/abs/1206.5294)                 |
+| IDC*      | [Shpitser and Pearl, 2012](https://arxiv.org/abs/1206.5294)                 |
+
+Apply an algorithm to an ADMG and a causal query to generate an estimand
+represented in the DSL like:
+
+```python
+from y0.dsl import P, X, Y
+from y0.examples import napkin
+from y0.algorithm.identify import Identification, identify
+
+# TODO after ID* and IDC* are done, we'll update this interface
+query = Identification.from_expression(graph=napkin, query=P(Y @ X))
+estimand = identify(query)
+assert estimand == P(Y @ X)
+```
+
+## 🚀 Installation
+
+The most recent release can be installed from
+[PyPI](https://pypi.org/project/y0/) with:
+
+```bash
+$ pip install y0
+```
+
+The most recent code and data can be installed directly from GitHub with:
+
+```bash
+$ pip install git+https://github.com/y0-causal-inference/y0.git
+```
+
+## 👐 Contributing
+
+Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
+[CONTRIBUTING.md](https://github.com/y0-causal-inference/y0/blob/master/.github/CONTRIBUTING.md) for more information on getting
+involved.
+
+## 👋 Attribution
+
+### ⚖️ License
+
+The code in this package is licensed under the [BSD-3-Clause
+license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
+
+### 📖 Citation
+
+Before we publish an application note on `y0`, you can cite this software
+via our Zenodo record (also see the badge above):
+
+```bibtex
+@software{y0,
+  author       = {Charles Tapley Hoyt and
+                  Jeremy Zucker and
+                  Marc-Antoine Parent},
+  title        = {y0-causal-inference/y0},
+  month        = jun,
+  year         = 2021,
+  publisher    = {Zenodo},
+  version      = {v0.1.0},
+  doi          = {10.5281/zenodo.4950768},
+  url          = {https://doi.org/10.5281/zenodo.4950768}
+}
+```
+
+### 🙏 Supporters
+
+This project has been supported by several organizations (in alphabetical order):
+
+- [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/)
+- [Pacific Northwest National Laboratory](https://www.pnnl.org/)
+
+### 💰 Funding
+
+The development of the Y0 Causal Inference Engine has been funded by the following grants:
+
+| Funding Body                                             | Program                                                                                                                       | Grant           |
+|----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------|
+| DARPA                                                    | [Automating Scientific Knowledge Extraction (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction) | HR00111990009   |
+| PNNL Data Model Convergence Initiative    | [Causal Inference and Machine Learning Methods for Analysis of Security Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/converged-applications-projects) | 90001   |
+| DARPA                                                    |  [Automating Scientific Knowledge Extraction and Modeling (ASKEM)](https://www.darpa.mil/program/automating-scientific-knowledge-extraction-and-modeling) |  HR00112220036  |
+
+### 🍪 Cookiecutter
+
+This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
+[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-package) template.
+
+## 🛠️ Development
+
+<details>
+  <summary>See developer instructions</summary>
+
+The final section of the README is for if you want to get involved by making a code contribution.
+
+### Developer Installation
+
+To install in development mode, use the following:
+
+```bash
+$ git clone git+https://github.com/y0-causal-inference/y0.git
+$ cd y0
+$ pip install -e .
+```
+
+### ❓ Testing
+
+After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
+run reproducibly with:
+
+```shell
+$ tox
+```
+
+Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests).
+
+### 📦 Making a Release
+
+After installing the package in development mode and installing
+`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell:
+
+```shell
+$ tox -e finish
+```
+
+This script does the following:
+
+1. Uses BumpVersion to switch the version number in the `setup.cfg` and
+   `src/y0/version.py` to not have the `-dev` suffix
+2. Packages the code in both a tar archive and a wheel
+3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
+   step
+4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
+5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
+   use `tox -e bumpversion minor` after.
+
+</details>
```

#### html2text {}

```diff
@@ -1,74 +1,112 @@
-Metadata-Version: 2.1 Name: y0 Version: 0.1.0 Summary: Python code for causal
-modeling. Home-page: https://github.com/y0-causal-inference/y0 Author: Jeremy
-Zucker Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
-Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Download-URL: https://
-github.com/y0-causal-inference/y0/releases Project-URL: Bug Tracker, https://
-github.com/y0-causal-inference/y0/issues Project-URL: Source Code, https://
-github.com/y0-causal-inference/y0 Description:
+Metadata-Version: 2.1 Name: y0 Version: 0.2.0 Summary: Python code for causal
+modeling. Home-page: https://github.com/y0-causal-inference/y0 Download-URL:
+https://github.com/y0-causal-inference/y0/releases Author: Jeremy Zucker
+Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
+Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Project-URL: Bug
+Tracker, https://github.com/y0-causal-inference/y0/issues Project-URL: Source
+Code, https://github.com/y0-causal-inference/y0 Keywords:
+cthoyt,cookiecutter,structural causal modeling Classifier: Development Status
+:: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: BSD License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Information Analysis Classifier: Topic :: Software Development
+:: Compilers Classifier: Framework :: Pytest Classifier: Framework :: tox
+Classifier: Framework :: Sphinx Requires-Python: >=3.10 Description-Content-
+Type: text/markdown Provides-Extra: r Provides-Extra: tests Provides-Extra:
+docs License-File: LICENSE
                             [docs/source/logo.png]
                                ****** y0 ******
  [Tests] [Cookiecutter_template_from_@cthoyt] [PyPI] [PyPI_-_Python_Version]
        [PyPI_-_License] [Documentation_Status] [DOI] [Code_style:_black]
-`y0` (pronounced "why not?") is Python code for causal inferencing. ## ðª
-Getting Started > TODO show in a very small amount of space the **MOST** useful
-thing your package can do. Make it as short as possible! You have an entire set
-of docs for later. ## â¬ï¸ Installation The most recent release can be
-installed from [PyPI](https://pypi.org/project/y0/) with: ```bash $ pip install
-y0 ``` The most recent code and data can be installed directly from GitHub
-with: ```bash $ pip install git+https://github.com/y0-causal-inference/y0.git
-``` To install in development mode, use the following: ```bash $ git clone
-git+https://github.com/y0-causal-inference/y0.git $ cd y0 $ pip install -e .
-``` ## âï¸ License The code in this package is licensed under the [BSD-3-
-Clause license](https://github.com/y0-causal-inference/y0/blob/master/LICENSE).
-## ð Contributing Contributions, whether filing an issue, making a pull
-request, or forking, are appreciated. See [CONTRIBUTING.rst](https://
-github.com/y0-causal-inference/y0/blob/master/CONTRIBUTING.rst) for more
-information on getting involved. ## Acknowledgements ### Supporters This
+`y0` (pronounced "why not?") is Python code for causal inference. ## ðª
+Getting Started ### Representing Probability Expressions `y0` has a fully
+featured internal domain specific language for representing probability
+expressions: ```python from y0.dsl import P, A, B # The probability of A given
+B expr_1 = P(A | B) # The probability of A given not B expr_2 = P(A | ~B) # The
+joint probability of A and B expr_3 = P(A, B) ``` It can also be used to
+manipulate expressions: ```python from y0.dsl import P, A, B, Sum P(A,
+B).marginalize(A) == Sum[A](P(A, B)) P(A, B).conditional(A) == P(A, B) / Sum[A]
+(P(A, B)) ``` DSL objects can be converted into strings with `str()` and parsed
+back using `y0.parser.parse_y0()`. A full demo of the DSL can be found in this
+[Jupyter Notebook](https://github.com/y0-causal-inference/y0/blob/main/
+notebooks/DSL%20Demo.ipynb) ### Representing Causality `y0` has a notion of
+acyclic directed mixed graphs built on top of `networkx` that can be used to
+model causality: ```python from y0.graph import NxMixedGraph from y0.dsl import
+X, Y, Z1, Z2 # Example from: # J. Pearl and D. Mackenzie (2018) # The Book of
+Why: The New Science of Cause and Effect. # Basic Books, p. 240. napkin =
+NxMixedGraph.from_edges( directed=[ (Z2, Z1), (Z1, X), (X, Y), ], undirected=[
+(Z2, X), (Z2, Y), ], ) ``` `y0` has many pre-written examples in `y0.examples`
+from Pearl, Shpitser, Bareinboim, and others. ### do Calculus `y0` provides
+_actual_ implementations of many algorithms that have remained unimplemented
+for the last 15 years of publications including: | Algorithm | Reference | |---
+--------|----------------------------------------------------------------------
+-------| | ID | [Shpitser and Pearl, 2006](https://dl.acm.org/doi/10.5555/
+1597348.1597382) | | IDC | [Shpitser and Pearl, 2008](https://www.jmlr.org/
+papers/v9/shpitser08a.html) | | ID* | [Shpitser and Pearl, 2012](https://
+arxiv.org/abs/1206.5294) | | IDC* | [Shpitser and Pearl, 2012](https://
+arxiv.org/abs/1206.5294) | Apply an algorithm to an ADMG and a causal query to
+generate an estimand represented in the DSL like: ```python from y0.dsl import
+P, X, Y from y0.examples import napkin from y0.algorithm.identify import
+Identification, identify # TODO after ID* and IDC* are done, we'll update this
+interface query = Identification.from_expression(graph=napkin, query=P(Y @ X))
+estimand = identify(query) assert estimand == P(Y @ X) ``` ## ð Installation
+The most recent release can be installed from [PyPI](https://pypi.org/project/
+y0/) with: ```bash $ pip install y0 ``` The most recent code and data can be
+installed directly from GitHub with: ```bash $ pip install git+https://
+github.com/y0-causal-inference/y0.git ``` ## ð Contributing Contributions,
+whether filing an issue, making a pull request, or forking, are appreciated.
+See [CONTRIBUTING.md](https://github.com/y0-causal-inference/y0/blob/
+master/.github/CONTRIBUTING.md) for more information on getting involved. ##
+ð Attribution ### âï¸ License The code in this package is licensed under
+the [BSD-3-Clause license](https://github.com/y0-causal-inference/y0/blob/
+master/LICENSE). ### ð Citation Before we publish an application note on
+`y0`, you can cite this software via our Zenodo record (also see the badge
+above): ```bibtex @software{y0, author = {Charles Tapley Hoyt and Jeremy Zucker
+and Marc-Antoine Parent}, title = {y0-causal-inference/y0}, month = jun, year =
+2021, publisher = {Zenodo}, version = {v0.1.0}, doi = {10.5281/zenodo.4950768},
+url = {https://doi.org/10.5281/zenodo.4950768} } ``` ### ð Supporters This
 project has been supported by several organizations (in alphabetical order): -
 [Harvard Program in Therapeutic Science - Laboratory of Systems Pharmacology]
 (https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/) -
 [Pacific Northwest National Laboratory](https://www.pnnl.org/) ### ð° Funding
 The development of the Y0 Causal Inference Engine has been funded by the
 following grants: | Funding Body | Program | Grant | |-------------------------
 ---------------------------------|---------------------------------------------
 -------------------------------------------------------------------------------
 ---|-----------------| | DARPA | [Automating Scientific Knowledge Extraction
 (ASKE)](https://www.darpa.mil/program/automating-scientific-knowledge-
 extraction) | HR00111990009 | | PNNL Data Model Convergence Initiative |
 [Causal Inference and Machine Learning Methods for Analysis of Security
 Constrained Unit Commitment (SCY0)](https://www.pnnl.gov/projects/dmc/
-converged-applications-projects) | 90001 | ### ðª Cookiecutter This package
-was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using
-[@cthoyt](https://github.com/cthoyt)'s [cookiecutter-python-package](https://
-github.com/cthoyt/cookiecutter-python-package) template. ## ð ï¸ Development
-The final section of the README is for if you want to get involved by making a
-code contribution. ### â Testing After cloning the repository and installing
-`tox` with `pip install tox`, the unit tests in the `tests/` folder can be run
-reproducibly with: ```shell $ tox ``` Additionally, these tests are
-automatically re-run with each commit in a [GitHub Action](https://github.com/
-y0-causal-inference/y0/actions?query=workflow%3ATests). ### ð¦ Making a
-Release After installing the package in development mode and installing `tox`
-with `pip install tox`, the commands for making a new release are contained
-within the `finish` environment in `tox.ini`. Run the following from the shell:
-```shell $ tox -e finish ``` This script does the following: 1. Uses
-BumpVersion to switch the version number in the `setup.cfg` and `src/y0/
+converged-applications-projects) | 90001 | | DARPA | [Automating Scientific
+Knowledge Extraction and Modeling (ASKEM)](https://www.darpa.mil/program/
+automating-scientific-knowledge-extraction-and-modeling) | HR00112220036 | ###
+ðª Cookiecutter This package was created with [@audreyfeldroy](https://
+github.com/audreyfeldroy)'s [cookiecutter](https://github.com/cookiecutter/
+cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-python-package](https://github.com/cthoyt/cookiecutter-python-
+package) template. ## ð ï¸ Development  See developer instructions The final
+section of the README is for if you want to get involved by making a code
+contribution. ### Developer Installation To install in development mode, use
+the following: ```bash $ git clone git+https://github.com/y0-causal-inference/
+y0.git $ cd y0 $ pip install -e . ``` ### â Testing After cloning the
+repository and installing `tox` with `pip install tox`, the unit tests in the
+`tests/` folder can be run reproducibly with: ```shell $ tox ``` Additionally,
+these tests are automatically re-run with each commit in a [GitHub Action]
+(https://github.com/y0-causal-inference/y0/actions?query=workflow%3ATests). ###
+ð¦ Making a Release After installing the package in development mode and
+installing `tox` with `pip install tox`, the commands for making a new release
+are contained within the `finish` environment in `tox.ini`. Run the following
+from the shell: ```shell $ tox -e finish ``` This script does the following: 1.
+Uses BumpVersion to switch the version number in the `setup.cfg` and `src/y0/
 version.py` to not have the `-dev` suffix 2. Packages the code in both a tar
 archive and a wheel 3. Uploads to PyPI using `twine`. Be sure to have a
 `.pypirc` file configured to avoid the need for manual input at this step 4.
 Push to GitHub. You'll need to make a release going with the commit where the
 version was bumped. 5. Bump the version to the next patch. If you made big
 changes and want to bump the version by minor, you can use `tox -e bumpversion
-minor` after. Keywords: cthoyt,cookiecutter,structural causal modeling
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-Environment :: Console Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Compilers Classifier: Framework ::
-Pytest Classifier: Framework :: tox Classifier: Framework :: Sphinx Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: r
-Provides-Extra: docs
+minor` after.
```

### Comparing `y0-0.1.0/tests/test_algorithm/test_conditional_independencies.py` & `y0-0.2.0/tests/test_algorithm/test_conditional_independencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,115 +1,116 @@
 # -*- coding: utf-8 -*-
 
 """Test getting conditional independencies (and related)."""
 
 import unittest
-from typing import Iterable, Set, Union
-
-from ananke.graphs import ADMG, SG
+from typing import Iterable, Set
 
 from y0.algorithm.conditional_independencies import (
     are_d_separated,
     get_conditional_independencies,
     get_moral_links,
 )
+from y0.dsl import AA, B, C, D, E, F, G, Variable
 from y0.examples import Example, d_separation_example, examples
 from y0.graph import NxMixedGraph
 from y0.struct import DSeparationJudgement
 
 
 class TestDSeparation(unittest.TestCase):
     """Test the d-separation utility."""
 
     def test_mit_example(self):
         """Test checking D-separation on the MIT example."""
-        graph = d_separation_example.graph.to_admg()
+        graph = d_separation_example.graph
 
-        self.assertFalse(are_d_separated(graph, "AA", "B", conditions=["D", "F"]))
-        self.assertTrue(are_d_separated(graph, "AA", "B"))
-        self.assertTrue(are_d_separated(graph, "D", "E", conditions=["C"]))
-        self.assertFalse(are_d_separated(graph, "AA", "B", conditions=["C"]))
-        self.assertFalse(are_d_separated(graph, "D", "E"))
-        self.assertFalse(are_d_separated(graph, "D", "E", conditions=["AA", "B"]))
-        self.assertFalse(are_d_separated(graph, "G", "G", conditions=["C"]))
+        self.assertFalse(are_d_separated(graph, AA, B, conditions=[D, F]))
+        self.assertTrue(are_d_separated(graph, AA, B))
+        self.assertTrue(are_d_separated(graph, D, E, conditions=[C]))
+        self.assertFalse(are_d_separated(graph, AA, B, conditions=[C]))
+        self.assertFalse(are_d_separated(graph, D, E))
+        self.assertFalse(are_d_separated(graph, D, E, conditions=[AA, B]))
+        self.assertFalse(are_d_separated(graph, G, G, conditions=[C]))
 
     def test_examples(self):
-        """Check that example conditional independencies are d-separations and that conditions (if present) are required.
+        """Check that example conditional independencies are d-separations and conditions (if present) are required.
 
         This test is using convenient examples to ensure that the d-separation algorithm
         isn't just always returning true or false.
         """
         testable = (
-            example
-            for example in examples
-            if example.conditional_independencies is not None
+            example for example in examples if example.conditional_independencies is not None
         )
 
         for example in testable:
             with self.subTest(name=example.name):
-                graph = example.graph.to_admg()
                 for ci in example.conditional_independencies:
+                    self.assertIn(ci.left, example.graph)
+                    self.assertIn(ci.right, example.graph)
+                    judgement = are_d_separated(
+                        example.graph, ci.left, ci.right, conditions=ci.conditions
+                    )
                     self.assertTrue(
-                        are_d_separated(
-                            graph, ci.left, ci.right, conditions=ci.conditions
-                        ),
-                        msg="Expected d-separation not found",
+                        judgement,
+                        msg=f"Expected d-separation not found in {example.name}",
                     )
                     if ci.conditions:
                         self.assertFalse(
-                            are_d_separated(graph, ci.left, ci.right),
+                            are_d_separated(example.graph, ci.left, ci.right),
                             msg="Unexpected d-separation",
                         )
 
     def test_moral_links(self):
         """Test adding 'moral links' (part of the d-separation algorithm).
 
         This test covers several cases around moral links to ensure that they are added when needed.
         """
-        graph = ADMG(
-            vertices=("a", "b", "c"),
-            di_edges=[("a", "b"), ("b", "c")],
-        )
-        links = set(tuple(sorted(e)) for e in get_moral_links(graph))
-        self.assertEqual(set(), links, msg="Unexpected moral links added.")
-
-        graph = ADMG(
-            vertices=("a", "b", "c"),
-            di_edges=[("a", "c"), ("b", "c")],
+        graph = NxMixedGraph.from_str_edges(
+            nodes=("a", "b", "c"),
+            directed=[("a", "b"), ("b", "c")],
+        )
+        links = list(get_moral_links(graph))
+        self.assertEqual([], links, msg="Unexpected moral links added.")
+
+        graph = NxMixedGraph.from_str_edges(
+            nodes=("a", "b", "c"),
+            directed=[("a", "c"), ("b", "c")],
         )
         links = set(tuple(sorted(e)) for e in get_moral_links(graph))
         self.assertEqual(
-            {("a", "b")}, links, msg="Moral links not as expected in single-link case."
+            {(Variable("a"), Variable("b"))},
+            links,
+            msg="Moral links not as expected in single-link case.",
         )
 
-        graph = ADMG(
-            vertices=("a", "b", "aa", "bb", "c"),
-            di_edges=[("a", "c"), ("b", "c"), ("aa", "c"), ("bb", "c")],
+        graph = NxMixedGraph.from_str_edges(
+            nodes=("a", "b", "aa", "bb", "c"),
+            directed=[("a", "c"), ("b", "c"), ("aa", "c"), ("bb", "c")],
         )
         links = set(tuple(sorted(e)) for e in get_moral_links(graph))
         self.assertEqual(
             {
-                ("a", "b"),
-                ("a", "aa"),
-                ("a", "bb"),
-                ("aa", "b"),
-                ("aa", "bb"),
-                ("b", "bb"),
+                (Variable("a"), Variable("b")),
+                (Variable("a"), Variable("aa")),
+                (Variable("a"), Variable("bb")),
+                (Variable("aa"), Variable("b")),
+                (Variable("aa"), Variable("bb")),
+                (Variable("b"), Variable("bb")),
             },
             links,
             msg="Moral links not as expected in multi-link case.",
         )
 
-        graph = ADMG(
-            vertices=("a", "b", "c", "d", "e"),
-            di_edges=[("a", "c"), ("b", "c"), ("c", "e"), ("d", "e")],
+        graph = NxMixedGraph.from_str_edges(
+            nodes=("a", "b", "c", "d", "e"),
+            directed=[("a", "c"), ("b", "c"), ("c", "e"), ("d", "e")],
         )
         links = set(tuple(sorted(e)) for e in get_moral_links(graph))
         self.assertEqual(
-            {("a", "b"), ("c", "d")},
+            {(Variable("a"), Variable("b")), (Variable("c"), Variable("d"))},
             links,
             msg="Moral links not as expected in multi-site case.",
         )
 
 
 class TestGetConditionalIndependencies(unittest.TestCase):
     """Test getting conditional independencies."""
@@ -118,41 +119,54 @@
         """Assert that the example is consistent w.r.t. D-separations."""
         self.assertIsNotNone(example.conditional_independencies)
         self.assert_has_judgements(
             graph=example.graph,
             judgements=example.conditional_independencies,
         )
 
-    def assert_has_judgements(
-        self, graph: Union[NxMixedGraph, SG], judgements: Iterable[DSeparationJudgement]
-    ) -> None:
+    def assert_judgement_types(self, judgements: Iterable[DSeparationJudgement]):
+        """Assert all judgmenets have the right types."""
+        self.assertTrue(
+            all(
+                (
+                    isinstance(judgement.left, Variable)
+                    and isinstance(judgement.right, Variable)
+                    and all(isinstance(c, Variable) for c in judgement.conditions)
+                )
+                for judgement in judgements
+            )
+        )
+
+    def assert_has_judgements(self, graph, judgements: Iterable[DSeparationJudgement]) -> None:
         """Assert that the graph has the correct conditional independencies.
 
         :param graph: the graph to test
+        :type graph: NxMixedGraph or ananke.graphs.SG
         :param judgements: the set of expected conditional independencies
         """
-        asserted_judgements = set(judgements)
-        observed_judgements = get_conditional_independencies(graph)
+        self.assertTrue(all(isinstance(node, Variable) for node in graph))
+        self.assert_judgement_types(judgements)
 
+        asserted_judgements = set(judgements)
         self.assertIsNotNone(asserted_judgements, "Expected independencies is empty.")
+
+        observed_judgements = get_conditional_independencies(graph)
         self.assertIsNotNone(observed_judgements, "Observed independencies is empty.")
+        self.assert_judgement_types(asserted_judgements)
+
         self.assertTrue(
             all(judgement.is_canonical for judgement in observed_judgements),
             msg="one or more of the returned DSeparationJudgement instances are not canonical",
         )
 
         self.assert_valid_judgements(graph, asserted_judgements)
         self.assert_valid_judgements(graph, observed_judgements)
 
-        expected_pairs = {
-            (judgement.left, judgement.right) for judgement in asserted_judgements
-        }
-        observed_pairs = {
-            (judgement.left, judgement.right) for judgement in observed_judgements
-        }
+        expected_pairs = {(judgement.left, judgement.right) for judgement in asserted_judgements}
+        observed_pairs = {(judgement.left, judgement.right) for judgement in observed_judgements}
         self.assertEqual(
             expected_pairs,
             observed_pairs,
             "Judgements do not find same separable pairs",
         )
 
         def _get_match(ref, options):
@@ -169,40 +183,39 @@
                 self.assertGreaterEqual(
                     len(judgement.conditions),
                     len(matching.conditions),
                     msg="Observed conditional independence more complicated than reference.",
                 )
 
     def assert_valid_judgements(
-        self, graph: Union[NxMixedGraph, SG], judgements: Set[DSeparationJudgement]
+        self, graph: NxMixedGraph, judgements: Set[DSeparationJudgement]
     ) -> None:
         """Check that a set of judgments are valid with respect to a graph."""
-        if isinstance(graph, NxMixedGraph):
-            graph = graph.to_admg()
+        self.assertIsInstance(graph, NxMixedGraph)
+
         for judgement in judgements:
             self.assertTrue(
+                all(isinstance(condition, Variable) for condition in judgement.conditions)
+            )
+            self.assertTrue(
                 are_d_separated(
                     graph,
                     judgement.left,
                     judgement.right,
                     conditions=judgement.conditions,
                 ),
                 msg=f"Conditional independency is not a d-separation in {graph}",
             )
 
         pairs = [(judgement.left, judgement.right) for judgement in judgements]
-        self.assertEqual(
-            len(pairs), len(set(pairs)), "Duplicate left/right pair observed"
-        )
+        self.assertEqual(len(pairs), len(set(pairs)), "Duplicate left/right pair observed")
 
     def test_examples(self):
         """Test getting the conditional independencies from the example graphs."""
         testable = (
-            example
-            for example in examples
-            if example.conditional_independencies is not None
+            example for example in examples if example.conditional_independencies is not None
         )
 
         for example in testable:
             with self.subTest(name=example.name):
                 self.maxDiff = None
                 self.assert_example_has_judgements(example)
```

### Comparing `y0-0.1.0/tests/test_algorithm/test_falsification.py` & `y0-0.2.0/tests/test_algorithm/test_falsification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # -*- coding: utf-8 -*-
 
 """Test falsification of testable implications given a graph."""
 
 import unittest
 
 from y0.algorithm.conditional_independencies import get_conditional_independencies
-from y0.algorithm.falsification import falsifications
+from y0.algorithm.falsification import get_falsifications, get_graph_falsifications
 from y0.examples import asia_example
 
 
 class TestFalsification(unittest.TestCase):
     """Test the falsifiable implications."""
 
-    def test_asia_from_graph(self):
+    def test_graph_falsifications(self):
         """Test the asia graph against data generated from it."""
-        graph = asia_example.graph.to_admg()
-        df = asia_example.data
-        issues = falsifications(graph, df)
-        self.assertEqual(0, len(issues))
+        issues = get_graph_falsifications(asia_example.graph, asia_example.data)
+        self.assertEqual(0, len(issues.failures))
         self.assertGreater(len(issues.evidence), 0)
 
-    def test_asia_from_list(self):
+    def test_falsifications(self):
         """Test the asia graph against data generated from it, passing in the implications to test."""
-        graph = asia_example.graph.to_admg()
-        df = asia_example.data
-        implications = get_conditional_independencies(graph)
-        issues = falsifications(implications, df)
-        self.assertEqual(0, len(issues))
+        implications = get_conditional_independencies(asia_example.graph)
+        issues = get_falsifications(implications, asia_example.data)
+        self.assertEqual(0, len(issues.failures))
         self.assertEqual(len(issues.evidence), len(implications))
```

### Comparing `y0-0.1.0/tests/test_causaleffect.py` & `y0-0.2.0/tests/test_causaleffect.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pyparsing
 
 from y0.dsl import P, Q, Sum, Variable
 from y0.examples import examples, verma_1
 
 try:
     from y0.causaleffect import r_get_verma_constraints
-    from y0.struct import VermaConstraint
     from y0.r_utils import CAUSALEFFECT, IGRAPH
+    from y0.struct import VermaConstraint
 except ImportError:  # rpy2 is not installed
     missing_rpy2 = True
 else:
     missing_rpy2 = False
 
 u_1 = Variable("u_1")
 V1 = Variable("V1")
@@ -28,16 +28,15 @@
 @unittest.skipIf(missing_rpy2, "rpy2 is not installed")
 class TestCausalEffect(unittest.TestCase):
     """Tests for the causaleffect wrapper."""
 
     @classmethod
     def setUpClass(cls) -> None:
         """Make imports for the class."""
-        from rpy2.robjects.packages import importr
-        from rpy2.robjects.packages import PackageNotInstalledError
+        from rpy2.robjects.packages import PackageNotInstalledError, importr
 
         try:
             importr(CAUSALEFFECT)
             importr(IGRAPH)
         except PackageNotInstalledError:
             raise unittest.SkipTest("R packages not properly installed.")
 
@@ -60,14 +59,10 @@
 
         expected_rhs_expr = Sum[u_1, V3](P(V4 | u_1 | V3) * P(V3) * P(u_1))
         self.assertEqual(
             expected_rhs_expr,
             verma_constraint.rhs_expr,
             msg=f"Expected: {expected_rhs_expr}\nActual:  {verma_constraint.rhs_expr}",
         )
-        self.assertEqual(
-            Sum[V2](Q[V2, V4](V1, V2, V3, V4)), verma_constraint.lhs_cfactor
-        )
-        self.assertEqual(
-            Sum[V2](P(V4 | (V1, V2, V3)) * P(V2 | V1)), verma_constraint.lhs_expr
-        )
+        self.assertEqual(Sum[V2](Q[V2, V4](V1, V2, V3, V4)), verma_constraint.lhs_cfactor)
+        self.assertEqual(Sum[V2](P(V4 | (V1, V2, V3)) * P(V2 | V1)), verma_constraint.lhs_expr)
         self.assertEqual((V1,), verma_constraint.variables)
```

### Comparing `y0-0.1.0/tests/test_is_identifiable.py` & `y0-0.2.0/tests/test_is_identifiable.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 class TestUtils(unittest.TestCase):
     """Test utility functions for ID algorithms."""
 
     def test_to(self):
         """Test getting treatments and outcomes."""
         with self.assertRaises(ValueError):
-            _get_to(P(X).distribution)
+            _get_to(P(X))
         with self.assertRaises(ValueError):
-            _get_to(P(X, Y).distribution)
+            _get_to(P(X, Y))
         with self.assertRaises(ValueError):
-            _get_to(P(X @ Y, X @ Z).distribution)
+            _get_to(P(X @ Y, X @ Z))
 
-        for expected_t, expected_o, expression in [
+        for expected_t, expected_o, probability in [
             (["X"], ["Y"], P(Y @ X)),
             (["X"], ["Y", "Z"], P(Y @ X, Z @ X)),
         ]:
-            t, o = _get_to(expression.distribution)
+            t, o = _get_to(probability)
             self.assertEqual(expected_t, t)
             self.assertEqual(expected_o, o)
 
 
 class TestNotIdentifiable(unittest.TestCase):
     """Tests for lack of identifiability.
```

### Comparing `y0-0.1.0/tests/test_mutate/test_chain.py` & `y0-0.2.0/tests/test_mutate/test_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,39 @@
 
 class TestChain(unittest.TestCase):
     """Tests for chain mutations."""
 
     def test_chain_expand_automatic_reordering(self):
         """Test expanding a joint probability to a product of conditional probabilities."""
         self.assertEqual(P(X | Y) * P(Y), chain_expand(P(X, Y), reorder=True))
-        self.assertEqual(
-            P(X | (Y, Z)) * P(Y | Z) * P(Z), chain_expand(P(X, Y, Z), reorder=True)
-        )
+        self.assertEqual(P(X | (Y, Z)) * P(Y | Z) * P(Z), chain_expand(P(X, Y, Z), reorder=True))
         self.assertEqual(
             P(W | (X, Y, Z)) * P(X | (Y, Z)) * P(Y | Z) * P(Z),
             chain_expand(P(W, X, Y, Z), reorder=True),
         )
 
         # Test that conditions come along for the ride
-        self.assertEqual(
-            P(X | (Y, A)) * P(Y | A), chain_expand(P(X & Y | A), reorder=True)
-        )
+        self.assertEqual(P(X | (Y, A)) * P(Y | A), chain_expand(P(X & Y | A), reorder=True))
         self.assertEqual(
             P(X | (Y, A, B)) * P(Y | (A, B)),
             chain_expand(P(X & Y | (A, B)), reorder=True),
         )
 
     def test_chain_expand_no_reordering(self):
         """Test expanding a joint probability to a product of conditional probabilities."""
         self.assertEqual(P(X | Y) * P(Y), chain_expand(P(X, Y), reorder=False))
-        self.assertEqual(
-            P(X | (Y, Z)) * P(Y | Z) * P(Z), chain_expand(P(X, Y, Z), reorder=False)
-        )
+        self.assertEqual(P(X | (Y, Z)) * P(Y | Z) * P(Z), chain_expand(P(X, Y, Z), reorder=False))
         self.assertEqual(
             P(W | (X, Y, Z)) * P(X | (Y, Z)) * P(Y | Z) * P(Z),
             chain_expand(P(W, X, Y, Z), reorder=False),
         )
 
     def test_fraction_expand(self):
         """Test expanding a conditional probability with Bayes' Theorem."""
         self.assertEqual(P(A, B) / P(B), fraction_expand(P(A | B)))
         self.assertEqual(P(W, X, Y, Z) / P(X, Y, Z), fraction_expand(P(W | (X, Y, Z))))
 
     def test_bayes_expand(self):
         """Test expanding a conditional using extended Bayes' Theorem."""
         self.assertEqual(P(A, X) / Sum[A](P(A, X)), bayes_expand(P(A | X)))
         self.assertEqual(P(A, X, Y) / Sum[A](P(A, X, Y)), bayes_expand(P(A | (X, Y))))
-        self.assertEqual(
-            P(A, B, X, Y) / Sum[A, B](P(A, B, X, Y)), bayes_expand(P(A & B | (X, Y)))
-        )
+        self.assertEqual(P(A, B, X, Y) / Sum[A, B](P(A, B, X, Y)), bayes_expand(P(A & B | (X, Y))))
```

### Comparing `y0-0.1.0/tests/test_mutate/test_simplify.py` & `y0-0.2.0/tests/test_mutate/test_simplify.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 # -*- coding: utf-8 -*-
 
 """Tests for canceling fractions."""
 
 import unittest
 
-from y0.dsl import A, B, One, P, Sum
+from y0.dsl import A, B, Fraction, One, P, Sum
 
 one = One()
 
 
 class TestCancel(unittest.TestCase):
     """Test cancelling fractions."""
 
     def test_simple_identity(self):
         """Test cancelling when the numerator and denominator are the same."""
         for label, frac in [
-            ("one", one / one),
+            ("one", Fraction(one, one)),
             ("prob", P(A) / P(A)),
             ("sum", Sum(P(A)) / Sum(P(A))),
             ("product", (P(A) * P(B)) / (P(A) * P(B))),
         ]:
             with self.subTest(type=label):
+                self.assertIsInstance(frac, Fraction)
                 self.assertEqual(one, frac.simplify(), msg=f"\n\nActual:{frac}")
 
     def test_fraction_simplify(self):
         """Test cancelling on products."""
         for label, expected, frac in [
             ("leave num.", P(B), (P(A) * P(B)) / P(A)),
             ("leave den.", one / P(B), P(A) / (P(A) * P(B))),
             ("unordered", one, (P(A) * P(B)) / (P(B) * P(A))),
+            ("canonical", one / P(A), one / P(A)),
+            ("flipper", P(A), Fraction(one, Fraction(one, P(A)))),
+            ("prob-redundant-one", P(A), Fraction(P(A), one)),
+            ("sum-redundant-one", Sum(P(A)), Fraction(Sum(P(A)), one)),
+            ("frac-redundant-one", P(A) / P(B), Fraction(Fraction(P(A), P(B)), one)),
+            ("prod-redundant-one", P(A) * P(B), Fraction(P(A) * P(B), one)),
         ]:
             with self.subTest(type=label):
+                self.assertIsInstance(frac, Fraction)
                 self.assertEqual(expected, frac.simplify(), msg=f"\n\nActual:{frac}")
```

### Comparing `y0-0.1.0/tests/test_parser/test_causaleffect.py` & `y0-0.2.0/tests/test_parser/test_causaleffect.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,8 @@
             (
                 Sum[U_1, C](P(D | U_1 | C) * P(C) * P(U_1)),
                 r"\sum_{U_{1},C}P(D|U_{1},C)P(C)P(U_{1})",
             ),
         ]:
             with self.subTest(s=s):
                 actual = parse_causaleffect(s)
-                self.assertEqual(
-                    expr, actual, msg=f"\nExpected: {expr}\nActual:   {actual}"
-                )
+                self.assertEqual(expr, actual, msg=f"\nExpected: {expr}\nActual:   {actual}")
```

### Comparing `y0-0.1.0/tests/test_parser/test_craig.py` & `y0-0.2.0/tests/test_parser/test_craig.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,21 @@
 from y0.parser.craig.grammar import fraction_pe, grammar, sum_pe
 from y0.parser.craig.utils import probability_pe, qfactor_pe, variable_pe
 
 
 class TestGrammar(unittest.TestCase):
     """Tests for parsing probability expressions."""
 
-    def assert_many(
-        self, expressions, parser_element: ParserElement, direct: bool = True
-    ):
+    def assert_many(self, expressions, parser_element: ParserElement, direct: bool = True):
         """Help testing many."""
         for expression in expressions:
-            with self.subTest(
-                expr=expression.to_text(), parser_element=parser_element.name
-            ):
+            with self.subTest(expr=expression.to_text(), parser_element=parser_element.name):
                 self.assert_parse_equal(expression, parser_element, direct=direct)
 
-    def assert_parse_equal(
-        self, expression, parser_element: ParserElement, direct: bool = True
-    ):
+    def assert_parse_equal(self, expression, parser_element: ParserElement, direct: bool = True):
         """Help test parsing works round trip.
 
         :param expression: The DSL object to check
         :param parser_element: The relevant parser element for specific checking
         :param direct: If true, uses object equals checks. If false, uses stringification then string equals checks.
             Switch to false when things aren't working during development.
         """
```

### Comparing `y0-0.1.0/tests/test_parser/test_internal.py` & `y0-0.2.0/tests/test_parser/test_internal.py`

 * *Files identical despite different names*

### Comparing `y0-0.1.0/tests/test_predicates.py` & `y0-0.2.0/tests/test_predicates.py`

 * *Files identical despite different names*

