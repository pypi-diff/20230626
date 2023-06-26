# Comparing `tmp/nomenklatura-2.9.5.tar.gz` & `tmp/nomenklatura-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-2.9.5.tar", last modified: Tue Apr 25 08:10:40 2023, max compression
+gzip compressed data, was "nomenklatura-3.0.0.tar", last modified: Mon Jun 26 14:45:37 2023, max compression
```

## Comparing `nomenklatura-2.9.5.tar` & `nomenklatura-3.0.0.tar`

### file list

```diff
@@ -1,90 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.014672 nomenklatura-2.9.5/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/data/match-regression.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/judgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/matching/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:09:53.000000 nomenklatura-2.9.5/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.874036 nomenklatura-3.0.0/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.874036 nomenklatura-3.0.0/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.878036 nomenklatura-3.0.0/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:45:37.874036 nomenklatura-3.0.0/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:45:14.000000 nomenklatura-3.0.0/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 14:45:37.000000 nomenklatura-3.0.0/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:45:37.882036 nomenklatura-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 14:43:41.000000 nomenklatura-3.0.0/setup.py
```

### Comparing `nomenklatura-2.9.5/LICENSE` & `nomenklatura-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/PKG-INFO` & `nomenklatura-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.5
+Version: 3.0.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
 
 ![screenshot](./docs/screenshot.png)
@@ -47,15 +47,15 @@
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
-* `nomenklatura.Loader` - a general purpose access mechanism for entities. By default, a `nomenklatura.FileLoader` is used to access entity data stored in files, but the loader can be subclassed to work with entities from a database system.
+* `nomenklatura.Store` - a general purpose access mechanism for entities. By default, a store is used to access entity data stored in files as an in-memory cache, but the store can be subclassed to work with entities from a database system.
 * `nomenklatura.Index` - a full-text in-memory search index for FtM entities. In the application, this is used to block de-duplication candidates, but the index can also be used to drive an API etc.
 * `nomenklatura.Resolver` - the core of the de-duplication process, the resolver is essentially a graph with edges made out of entity judgements. The resolver can be used to store judgements or get the canonical ID for a given entity.
 
 All of the API classes have extensive type annotations, which should make their integration in any modern Python API simpler.
 
 ## Design
 
@@ -91,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-2.9.5/README.md` & `nomenklatura-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
-* `nomenklatura.Loader` - a general purpose access mechanism for entities. By default, a `nomenklatura.FileLoader` is used to access entity data stored in files, but the loader can be subclassed to work with entities from a database system.
+* `nomenklatura.Store` - a general purpose access mechanism for entities. By default, a store is used to access entity data stored in files as an in-memory cache, but the store can be subclassed to work with entities from a database system.
 * `nomenklatura.Index` - a full-text in-memory search index for FtM entities. In the application, this is used to block de-duplication candidates, but the index can also be used to drive an API etc.
 * `nomenklatura.Resolver` - the core of the de-duplication process, the resolver is essentially a graph with edges made out of entity judgements. The resolver can be used to store judgements or get the canonical ID for a given entity.
 
 All of the API classes have extensive type annotations, which should make their integration in any modern Python API simpler.
 
 ## Design
```

### Comparing `nomenklatura-2.9.5/nomenklatura/cli.py` & `nomenklatura-3.0.0/nomenklatura/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from pathlib import Path
 from typing import Generator, Iterable, List, Optional, Tuple
 from followthemoney.cli.util import path_writer, InPath, OutPath
 from followthemoney.cli.util import path_entities, write_entity
 from followthemoney.cli.aggregate import sorted_aggregate
 
 from nomenklatura.cache import Cache
-from nomenklatura.matching.train import train_matcher
-from nomenklatura.loader import FileLoader
+from nomenklatura.matching import train_v2_matcher, train_v1_matcher
+from nomenklatura.store import load_entity_file_store
 from nomenklatura.resolver import Resolver
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CompositeEntity as Entity
 from nomenklatura.enrich import Enricher, make_enricher, match, enrich
 from nomenklatura.statement import Statement, CSV, FORMATS
+from nomenklatura.matching import get_algorithm, DefaultAlgorithm
 from nomenklatura.statement import write_statements, read_path_statements
 from nomenklatura.senzing import senzing_record
 from nomenklatura.xref import xref as run_xref
 from nomenklatura.tui import dedupe_ui
 
 
 log = logging.getLogger(__name__)
@@ -53,28 +54,33 @@
 
 
 @cli.command("xref", help="Generate dedupe candidates")
 @click.argument("path", type=InPath)
 @click.option("-r", "--resolver", type=ResPath)
 @click.option("-a", "--auto-threshold", type=click.FLOAT, default=None)
 @click.option("-l", "--limit", type=click.INT, default=5000)
+@click.option("--algorithm", default=DefaultAlgorithm.NAME)
 @click.option("--scored/--unscored", is_flag=True, type=click.BOOL, default=True)
 def xref_file(
     path: Path,
     resolver: Optional[Path] = None,
     auto_threshold: Optional[float] = None,
+    algorithm: str = DefaultAlgorithm.NAME,
     limit: int = 5000,
     scored: bool = True,
 ) -> None:
     resolver_ = _get_resolver(path, resolver)
-    loader = FileLoader(path, resolver=resolver_)
+    store = load_entity_file_store(path, resolver=resolver_)
+    algorithm_type = get_algorithm(algorithm)
+    if algorithm_type is None:
+        raise click.Abort(f"Unknown algorithm: {algorithm}")
     run_xref(
-        loader,
-        resolver_,
+        store,
         auto_threshold=auto_threshold,
+        algorithm=algorithm_type,
         scored=scored,
         limit=limit,
     )
     resolver_.save()
     log.info("Xref complete in: %s", resolver_.path)
 
 
@@ -127,36 +133,42 @@
 
 @cli.command("dedupe", help="Interactively judge xref candidates")
 @click.argument("path", type=InPath)
 @click.option("-x", "--xref", is_flag=True, default=False)
 @click.option("-r", "--resolver", type=ResPath)
 def dedupe(path: Path, xref: bool = False, resolver: Optional[Path] = None) -> None:
     resolver_ = _get_resolver(path, resolver)
-    loader = FileLoader(path, resolver=resolver_)
+    store = load_entity_file_store(path, resolver=resolver_)
     if xref:
-        run_xref(loader, resolver_)
+        run_xref(store)
 
-    dedupe_ui(resolver_, loader)
+    dedupe_ui(store)
     resolver_.save()
 
 
 @cli.command("merge-resolver", help="Merge resolver configs")
 @click.argument("outpath", type=OutPath)
 @click.option("-i", "--inputs", type=InPath, multiple=True)
 def merge_resolver(outpath: Path, inputs: Iterable[Path]) -> None:
     resolver = Resolver[Entity].load(outpath)
     for path in inputs:
         resolver.merge(path)
     resolver.save()
 
 
-@cli.command("train-matcher", help="Train a matching model from judgement pairs")
+@cli.command("train-v1-matcher", help="Train a matching model from judgement pairs")
 @click.argument("pairs_file", type=InPath)
-def train_matcher_(pairs_file: Path) -> None:
-    train_matcher(pairs_file)
+def train_v1_matcher_(pairs_file: Path) -> None:
+    train_v1_matcher(pairs_file)
+
+
+@cli.command("train-v2-matcher", help="Train a matching model from judgement pairs")
+@click.argument("pairs_file", type=InPath)
+def train_v2_matcher_(pairs_file: Path) -> None:
+    train_v2_matcher(pairs_file)
 
 
 @cli.command("match", help="Generate matches from an enrichment source")
 @click.argument("config", type=InPath)
 @click.argument("entities", type=InPath)
 @click.option("-o", "--outpath", type=OutPath, default="-")
 @click.option("-r", "--resolver", type=ResPath)
```

### Comparing `nomenklatura-2.9.5/nomenklatura/data/match-regression.pkl` & `nomenklatura-3.0.0/nomenklatura/data/regression-v1.pkl`

 * *Files 16% similar despite different names*

```diff
@@ -12,53 +12,53 @@
 000000b0: 0e6e 5f66 6561 7475 7265 735f 696e 5f94  .n_features_in_.
 000000c0: 4b11 8c0f 6e5f 7361 6d70 6c65 735f 7365  K...n_samples_se
 000000d0: 656e 5f94 8c15 6e75 6d70 792e 636f 7265  en_...numpy.core
 000000e0: 2e6d 756c 7469 6172 7261 7994 8c06 7363  .multiarray...sc
 000000f0: 616c 6172 9493 948c 056e 756d 7079 948c  alar.....numpy..
 00000100: 0564 7479 7065 9493 948c 0269 3894 8988  .dtype.....i8...
 00000110: 8794 5294 284b 038c 013c 944e 4e4e 4aff  ..R.(K...<.NNNJ.
-00000120: ffff ff4a ffff ffff 4b00 7494 6243 08c4  ...J....K.t.bC..
-00000130: 8004 0000 0000 0094 8694 5294 8c05 6d65  ..........R...me
+00000120: ffff ff4a ffff ffff 4b00 7494 6243 08a9  ...J....K.t.bC..
+00000130: 6d04 0000 0000 0094 8694 5294 8c05 6d65  m.........R...me
 00000140: 616e 5f94 6814 8c0c 5f72 6563 6f6e 7374  an_.h..._reconst
 00000150: 7275 6374 9493 9468 178c 076e 6461 7272  ruct...h...ndarr
 00000160: 6179 9493 944b 0085 9443 0162 9487 9452  ay...K...C.b...R
 00000170: 9428 4b01 4b11 8594 6819 8c02 6638 9489  .(K.K...h...f8..
 00000180: 8887 9452 9428 4b03 681d 4e4e 4e4a ffff  ...R.(K.h.NNNJ..
-00000190: ffff 4aff ffff ff4b 0074 9462 8943 88b4  ..J....K.t.b.C..
-000001a0: cf8e 2ba7 7f2e 40ce d0ea 414b b6e6 3ff9  ..+...@...AK..?.
-000001b0: faf8 96fb a645 3fdb 1928 0a01 81e9 3f70  .....E?..(....?p
-000001c0: 10af acba fa4e 3fd9 8f10 4baf ca64 3f01  .....N?...K..d?.
-000001d0: 02ef f0d5 a87f 3ffa b0d5 701a fcd2 3ff8  ......?...p...?.
-000001e0: a579 6e42 e7c9 3f9b c46c ee18 1fbe 3fd7  .ynB..?..l....?.
-000001f0: e6c2 47e7 13b8 3f76 ea8e 1cbb 70b7 3f97  ..G...?v....p.?.
-00000200: c910 3a42 1262 3f7e 3468 81f2 009f 3f5d  ..:B.b?~4h....?]
-00000210: 8e7c 4846 b1af 3f73 306b 3e49 c5ae 3f56  .|HF..?s0k>I..?V
-00000220: 063e bdd6 e2a3 bf94 7494 628c 0476 6172  .>......t.b..var
+00000190: ffff 4aff ffff ff4b 0074 9462 8943 8801  ..J....K.t.b.C..
+000001a0: 8c32 81ae 4328 4020 0746 c6a2 82e7 3fe7  .2..C(@ .F....?.
+000001b0: 6fbb 06b0 4e43 3f61 acad f841 0ae7 3f40  o...NC?a...A..?@
+000001c0: 5bda fa52 e157 3f0f 927b 212a be62 3ffe  [..R.W?..{!*.b?.
+000001d0: e8aa b68d 8965 3f72 b9ba ee82 17d2 3f80  .....e?r......?.
+000001e0: 19c2 ed87 f7c8 3ffc 9fe1 4af6 34bf 3fe6  ......?...J.4.?.
+000001f0: a60c d1d9 beb8 3f30 98e5 5655 19b3 3fb9  ......?0..VU..?.
+00000200: bab9 1695 885a 3f27 ac04 37fc 8a96 3fdf  .....Z?'..7...?.
+00000210: 8037 465e 7d9b 3f14 1013 1c5f 66a3 3ff7  .7F^}.?...._f.?.
+00000220: 3eb3 dc01 59a8 bf94 7494 628c 0476 6172  >...Y...t.b..var
 00000230: 5f94 6824 6826 4b00 8594 6828 8794 5294  _.h$h&K...h(..R.
-00000240: 284b 014b 1185 9468 2e89 4388 53ab bc30  (K.K...h..C.S..0
-00000250: 9d00 6c40 1694 ddee e6c0 bf3f 8deb 94f2  ..l@.......?....
-00000260: 51a3 453f 3a2b d878 46af bb3f d6de 9ffc  Q.E?:+.xF..?....
-00000270: c42a 6e3f ec84 e7e8 71b4 803f bf2c 1acd  .*n?....q..?.,..
-00000280: 522c b23f 5cc4 3944 720d d33f 1a78 68a9  R,.?\.9Dr..?.xh.
-00000290: 4aa9 c43f ffd9 9e29 728d c23f 7b6d b9d6  J..?...)r..?{m..
-000002a0: 218a bc3f 1f5c f9d2 4aba b03f 4f22 24a5  !..?.\..J..?O"$.
-000002b0: 0d08 623f 6f7f 59d2 a310 9e3f c053 1c8d  ..b?o.Y....?.S..
-000002c0: 82b8 bc3f 9a5f f82c 6854 a63f fb81 184a  ...?._.,hT.?...J
-000002d0: 6217 da3f 9474 9462 8c06 7363 616c 655f  b..?.t.b..scale_
+00000240: 284b 014b 1185 9468 2e89 4388 a074 018d  (K.K...h..C..t..
+00000250: e030 6c40 9d46 749b c9bb bb3f b8ac 197a  .0l@.Ft....?...z
+00000260: c64b 433f a076 b7a3 8808 bd3f 0fa5 d025  .KC?.v.....?...%
+00000270: 1c62 6e3f d4e2 0e7b f381 713f 962f 76d4  .bn?...{..q?./v.
+00000280: 452d a93f fe95 745e 3e87 d13f f283 6f45  E-.?..t^>..?..oE
+00000290: d618 c43f cd9b 3351 17b0 c23f 31e4 d415  ...?..3Q...?1...
+000002a0: 450e bd3f 8d86 9d86 786b ab3f c0bb 1bfa  E..?....xk.?....
+000002b0: 947d 5a3f 2c0c 6f83 f00b 963f 338f c731  .}Z?,.o....?3..1
+000002c0: 8023 ac3f 3255 043b 2272 9c3f 2619 b933  .#.?2U.;"r.?&..3
+000002d0: 0879 d43f 9474 9462 8c06 7363 616c 655f  .y.?.t.b..scale_
 000002e0: 9468 2468 264b 0085 9468 2887 9452 9428  .h$h&K...h(..R.(
-000002f0: 4b01 4b11 8594 682e 8943 88fd 7886 163e  K.K...h..C..x..>
-00000300: ef2d 40ec cea3 6344 8ad6 3f67 7b6d e153  .-@...cD..?g{m.S
-00000310: 509a 3f05 d754 b6e6 0bd5 3ffe 950c e0ec  P.?..T....?.....
-00000320: 11af 3f45 9414 65d6 1eb7 3f4c a0bc ee4e  ..?E..e...?L...N
-00000330: 0dd1 3f28 2be8 88ad 75e1 3f79 6f16 1a8b  ..?(+...u.?yo...
-00000340: b6d9 3f9f 4909 a695 5dd8 3f6d 6790 6775  ..?.I...].?mg.gu
-00000350: 5ed5 3f1c 99cc 461c 5cd0 3f4d 117f d45d  ^.?...F.\.?M...]
-00000360: 05a8 3fd5 9c4b 72c0 eec5 3fa1 02a5 36cb  ..?..Kr...?...6.
-00000370: 6fd5 3fd9 73f4 5628 bbca 3f8b f01f 548f  o.?.s.V(..?...T.
-00000380: 6ee4 3f94 7494 628c 105f 736b 6c65 6172  n.?.t.b.._sklear
+000002f0: 4b01 4b11 8594 682e 8943 88c5 61eb f1fe  K.K...h..C..a...
+00000300: 082e 40a8 f1d0 b8a7 10d5 3f04 6f77 e456  ..@.......?.ow.V
+00000310: d998 3f76 15d2 c393 8dd5 3fb2 55c8 745f  ..?v......?.U.t_
+00000320: 2eaf 3ffe 9e2a cda1 bcb0 3fab 110e a556  ..?..*....?....V
+00000330: 62cc 3fdb c7d6 3a29 bfe0 3ff0 704c b008  b.?...:)..?.pL..
+00000340: 5cd9 3ffd f2e7 1f4b 74d8 3fe4 8cb4 b6b4  \.?....Kt.?.....
+00000350: 8fd5 3f8f b255 461b 9fcd 3f60 4726 506c  ..?..UF...?`G&Pl
+00000360: 96a4 3f02 a7ec f512 c8c2 3f2d c38b e9dd  ..?.......?-....
+00000370: 01ce 3f57 edb0 8077 55c5 3f8d 959e 3a47  ..?W...wU.?...:G
+00000380: 19e2 3f94 7494 628c 105f 736b 6c65 6172  ..?.t.b.._sklear
 00000390: 6e5f 7665 7273 696f 6e94 8c05 312e 322e  n_version...1.2.
 000003a0: 3294 7562 8694 8c12 6c6f 6769 7374 6963  2.ub....logistic
 000003b0: 7265 6772 6573 7369 6f6e 948c 1e73 6b6c  regression...skl
 000003c0: 6561 726e 2e6c 696e 6561 725f 6d6f 6465  earn.linear_mode
 000003d0: 6c2e 5f6c 6f67 6973 7469 6394 8c12 4c6f  l._logistic...Lo
 000003e0: 6769 7374 6963 5265 6772 6573 7369 6f6e  gisticRegression
 000003f0: 9493 9429 8194 7d94 288c 0770 656e 616c  ...)..}.(..penal
@@ -79,64 +79,64 @@
 000004e0: 7365 735f 9468 2468 264b 0085 9468 2887  ses_.h$h&K...h(.
 000004f0: 9452 9428 4b01 4b02 8594 681c 8943 1000  .R.(K.K...h..C..
 00000500: 0000 0000 0000 0001 0000 0000 0000 0094  ................
 00000510: 7494 628c 076e 5f69 7465 725f 9468 2468  t.b..n_iter_.h$h
 00000520: 264b 0085 9468 2887 9452 9428 4b01 4b01  &K...h(..R.(K.K.
 00000530: 8594 6819 8c02 6934 9489 8887 9452 9428  ..h...i4.....R.(
 00000540: 4b03 681d 4e4e 4e4a ffff ffff 4aff ffff  K.h.NNNJ....J...
-00000550: ff4b 0074 9462 8943 041f 0000 0094 7494  .K.t.b.C......t.
+00000550: ff4b 0074 9462 8943 041e 0000 0094 7494  .K.t.b.C......t.
 00000560: 628c 0563 6f65 665f 9468 2468 264b 0085  b..coef_.h$h&K..
 00000570: 9468 2887 9452 9428 4b01 4b01 4b11 8694  .h(..R.(K.K.K...
-00000580: 682e 8943 8835 2e64 3b1b faec 3f00 8e32  h..C.5.d;...?..2
-00000590: c158 45b2 3f0e 7f68 1ce5 e5d0 bfaf 593a  .XE.?..h......Y:
-000005a0: a175 01eb 3ff1 0bc1 2ade cc96 3f69 2abd  .u..?...*...?i*.
-000005b0: 0a33 38a4 3fda c5fb d8b0 c6ca 3f85 d679  .38.?.......?..y
-000005c0: 2fa9 8af1 3f1a 9a9c e0c5 12d1 3fe1 4c75  /...?.......?.Lu
-000005d0: 8dfc d5a4 3f34 b3e1 26b4 68c1 3ff6 cef0  ....?4..&.h.?...
-000005e0: 48bf eaa6 bfe1 09ba 536a 92ce bf9b d957  H.......Sj.....W
-000005f0: 3f35 5bd2 bf9d a7fb a273 14e3 3ff5 21e3  ?5[......s..?.!.
-00000600: ae18 52ed 3ff5 3150 3a3a 40ae 3f94 7494  ..R.?.1P::@.?.t.
+00000580: 682e 8943 88e6 5779 856d fce6 3f72 a4f0  h..C..Wy.m..?r..
+00000590: 689a 39e9 3fd3 15e8 9085 50d0 bf7a 295c  h.9.?.....P..z)\
+000005a0: d0e7 a5bd 3fae b3c4 e06d 38a1 3f13 c113  ....?....m8.?...
+000005b0: c92b 4aaf 3f76 3285 7849 3cc3 3faf b079  .+J.?v2.xI<.?..y
+000005c0: ca45 7cf1 3fff 5702 4743 9ad4 3fe8 2512  .E|.?.W.GC..?.%.
+000005d0: 7b2d af31 3fd3 e4b1 5a90 38bf 3fb5 9448  {-.1?...Z.8.?..H
+000005e0: 762d 45ab bfae f9e3 a843 8aca bf98 9407  v-E......C......
+000005f0: 259c a6cb bfb7 b994 3d76 51de 3f86 76da  %.......=vQ.?.v.
+00000600: 8dc6 a8e2 3f2d 4c34 a6ca d3a4 3f94 7494  ....?-L4....?.t.
 00000610: 628c 0a69 6e74 6572 6365 7074 5f94 6824  b..intercept_.h$
 00000620: 6826 4b00 8594 6828 8794 5294 284b 014b  h&K...h(..R.(K.K
-00000630: 0185 9468 2e89 4308 ad0d f310 190a 0240  ...h..C........@
+00000630: 0185 9468 2e89 4308 6927 bcba 15f9 0040  ...h..C.i'.....@
 00000640: 9474 9462 6840 6841 7562 8694 658c 066d  .t.bh@hAub..e..m
 00000650: 656d 6f72 7994 4e68 5789 6840 6841 7562  emory.NhW.h@hAub
 00000660: 8c0c 636f 6566 6669 6369 656e 7473 947d  ..coefficients.}
 00000670: 9428 8c0a 6e61 6d65 5f6d 6174 6368 9468  .(..name_match.h
-00000680: 1668 2e43 0835 2e64 3b1b faec 3f94 8694  .h.C.5.d;...?...
+00000680: 1668 2e43 08e6 5779 856d fce6 3f94 8694  .h.C..Wy.m..?...
 00000690: 5294 8c12 6e61 6d65 5f74 6f6b 656e 5f6f  R...name_token_o
-000006a0: 7665 726c 6170 9468 1668 2e43 0800 8e32  verlap.h.h.C...2
-000006b0: c158 45b2 3f94 8694 5294 8c0c 6e61 6d65  .XE.?...R...name
-000006c0: 5f6e 756d 6265 7273 9468 1668 2e43 080e  _numbers.h.h.C..
-000006d0: 7f68 1ce5 e5d0 bf94 8694 5294 8c10 6e61  .h........R...na
+000006a0: 7665 726c 6170 9468 1668 2e43 0872 a4f0  verlap.h.h.C.r..
+000006b0: 689a 39e9 3f94 8694 5294 8c0c 6e61 6d65  h.9.?...R...name
+000006c0: 5f6e 756d 6265 7273 9468 1668 2e43 08d3  _numbers.h.h.C..
+000006d0: 15e8 9085 50d0 bf94 8694 5294 8c10 6e61  ....P.....R...na
 000006e0: 6d65 5f6c 6576 656e 7368 7465 696e 9468  me_levenshtein.h
-000006f0: 1668 2e43 08af 593a a175 01eb 3f94 8694  .h.C..Y:.u..?...
+000006f0: 1668 2e43 087a 295c d0e7 a5bd 3f94 8694  .h.C.z)\....?...
 00000700: 5294 8c0b 7068 6f6e 655f 6d61 7463 6894  R...phone_match.
-00000710: 6816 682e 4308 f10b c12a decc 963f 9486  h.h.C....*...?..
+00000710: 6816 682e 4308 aeb3 c4e0 6d38 a13f 9486  h.h.C.....m8.?..
 00000720: 9452 948c 0b65 6d61 696c 5f6d 6174 6368  .R...email_match
-00000730: 9468 1668 2e43 0869 2abd 0a33 38a4 3f94  .h.h.C.i*..38.?.
+00000730: 9468 1668 2e43 0813 c113 c92b 4aaf 3f94  .h.h.C.....+J.?.
 00000740: 8694 5294 8c10 6964 656e 7469 6669 6572  ..R...identifier
-00000750: 5f6d 6174 6368 9468 1668 2e43 08da c5fb  _match.h.h.C....
-00000760: d8b0 c6ca 3f94 8694 5294 8c0b 646f 625f  ....?...R...dob_
-00000770: 6d61 7463 6865 7394 6816 682e 4308 85d6  matches.h.h.C...
-00000780: 792f a98a f13f 9486 9452 948c 1064 6f62  y/...?...R...dob
+00000750: 5f6d 6174 6368 9468 1668 2e43 0876 3285  _match.h.h.C.v2.
+00000760: 7849 3cc3 3f94 8694 5294 8c0b 646f 625f  xI<.?...R...dob_
+00000770: 6d61 7463 6865 7394 6816 682e 4308 afb0  matches.h.h.C...
+00000780: 79ca 457c f13f 9486 9452 948c 1064 6f62  y.E|.?...R...dob
 00000790: 5f79 6561 725f 6d61 7463 6865 7394 6816  _year_matches.h.
-000007a0: 682e 4308 1a9a 9ce0 c512 d13f 9486 9452  h.C........?...R
+000007a0: 682e 4308 ff57 0247 439a d43f 9486 9452  h.C..W.GC..?...R
 000007b0: 948c 1066 6972 7374 5f6e 616d 655f 6d61  ...first_name_ma
-000007c0: 7463 6894 6816 682e 4308 e14c 758d fcd5  tch.h.h.C..Lu...
-000007d0: a43f 9486 9452 948c 1166 616d 696c 795f  .?...R...family_
+000007c0: 7463 6894 6816 682e 4308 e825 127b 2daf  tch.h.h.C..%.{-.
+000007d0: 313f 9486 9452 948c 1166 616d 696c 795f  1?...R...family_
 000007e0: 6e61 6d65 5f6d 6174 6368 9468 1668 2e43  name_match.h.h.C
-000007f0: 0834 b3e1 26b4 68c1 3f94 8694 5294 8c0b  .4..&.h.?...R...
+000007f0: 08d3 e4b1 5a90 38bf 3f94 8694 5294 8c0b  ....Z.8.?...R...
 00000800: 6269 7274 685f 706c 6163 6594 6816 682e  birth_place.h.h.
-00000810: 4308 f6ce f048 bfea a6bf 9486 9452 948c  C....H.......R..
+00000810: 4308 b594 4876 2d45 abbf 9486 9452 948c  C...Hv-E.....R..
 00000820: 0f67 656e 6465 725f 6d69 736d 6174 6368  .gender_mismatch
-00000830: 9468 1668 2e43 08e1 09ba 536a 92ce bf94  .h.h.C....Sj....
+00000830: 9468 1668 2e43 08ae f9e3 a843 8aca bf94  .h.h.C.....C....
 00000840: 8694 5294 8c10 636f 756e 7472 795f 6d69  ..R...country_mi
-00000850: 736d 6174 6368 9468 1668 2e43 089b d957  smatch.h.h.C...W
-00000860: 3f35 5bd2 bf94 8694 5294 8c14 6f72 675f  ?5[.....R...org_
+00000850: 736d 6174 6368 9468 1668 2e43 0898 9407  smatch.h.h.C....
+00000860: 259c a6cb bf94 8694 5294 8c14 6f72 675f  %.......R...org_
 00000870: 6964 656e 7469 6669 6572 5f6d 6174 6368  identifier_match
-00000880: 9468 1668 2e43 089d a7fb a273 14e3 3f94  .h.h.C.....s..?.
+00000880: 9468 1668 2e43 08b7 b994 3d76 51de 3f94  .h.h.C....=vQ.?.
 00000890: 8694 5294 8c0d 6164 6472 6573 735f 6d61  ..R...address_ma
-000008a0: 7463 6894 6816 682e 4308 f521 e3ae 1852  tch.h.h.C..!...R
-000008b0: ed3f 9486 9452 948c 0f61 6464 7265 7373  .?...R...address
-000008c0: 5f6e 756d 6265 7273 9468 1668 2e43 08f5  _numbers.h.h.C..
-000008d0: 3150 3a3a 40ae 3f94 8694 5294 7575 2e    1P::@.?...R.uu.
+000008a0: 7463 6894 6816 682e 4308 8676 da8d c6a8  tch.h.h.C..v....
+000008b0: e23f 9486 9452 948c 0f61 6464 7265 7373  .?...R...address
+000008c0: 5f6e 756d 6265 7273 9468 1668 2e43 082d  _numbers.h.h.C.-
+000008d0: 4c34 a6ca d3a4 3f94 8694 5294 7575 2e    L4....?...R.uu.
```

### Comparing `nomenklatura-2.9.5/nomenklatura/dataset/catalog.py` & `nomenklatura-3.0.0/nomenklatura/dataset/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     def has(self, name: str) -> bool:
         return name in self.names
 
     @property
     def names(self) -> Set[str]:
         return {d.name for d in self.datasets}
 
+    def __repr__(self) -> str:
+        return f"<DataCatalog[{self.dataset_type.__name__}]({self.names!r})>"  # pragma: no cover
+
     def to_dict(self) -> Dict[str, Any]:
         return {
             "datasets": [d.to_dict() for d in self.datasets],
             "updated_at": self.updated_at,
         }
 
     @classmethod
```

### Comparing `nomenklatura-2.9.5/nomenklatura/dataset/coverage.py` & `nomenklatura-3.0.0/nomenklatura/dataset/publisher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-from typing import List, Any, Dict
+from banal import as_bool
+from typing import Optional, Dict, Any
 from followthemoney.types import registry
 
-from nomenklatura.dataset.util import type_check, type_require, cleanup
+from nomenklatura.dataset.util import Named, cleanup
+from nomenklatura.dataset.util import type_check, type_require
 
 
-class DataCoverage(object):
-    """Details on the temporal and geographic scope of a dataset."""
+class DataPublisher(Named):
+    """Publisher information, eg. the government authority."""
 
-    def __init__(self, data: Dict[str, Any]) -> None:
-        self.start = type_check(registry.date, data.get("start"))
-        self.end = type_check(registry.date, data.get("end"))
-        self.countries: List[str] = []
-        for country in data.get("countries", []):
-            self.countries.append(type_require(registry.country, country))
+    def __init__(self, data: Dict[str, Any]):
+        name = type_require(registry.string, data.get("name"))
+        super().__init__(name)
+        self.url = type_require(registry.url, data.get("url"))
+        self.description = type_check(registry.string, data.get("description"))
+        self.country = type_check(registry.country, data.get("country"))
+        self.official = as_bool(data.get("official", False))
+        self.logo_url = type_check(registry.url, data.get("logo_url"))
+
+    @property
+    def country_label(self) -> Optional[str]:
+        if self.country is None:
+            return None
+        return registry.country.caption(self.country)
 
     def to_dict(self) -> Dict[str, Any]:
-        data = {"start": self.start, "end": self.end, "countries": self.countries}
+        data = {
+            "name": self.name,
+            "url": self.url,
+            "description": self.description,
+            "country": self.country,
+            "country_label": self.country_label,
+            "official": self.official,
+            "logo_url": self.logo_url,
+        }
         return cleanup(data)
-
-    def __repr__(self) -> str:
-        return f"<DataCoverage({self.start!r}>{self.end!r}, {self.countries!r})>"
```

### Comparing `nomenklatura-2.9.5/nomenklatura/dataset/dataset.py` & `nomenklatura-3.0.0/nomenklatura/dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-import yaml
 from functools import cached_property
-from typing import TYPE_CHECKING
-from typing import Any, Dict, TypeVar, Type, List, Optional, Set
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Type, TypeVar
+
+import yaml
 from followthemoney.types import registry
 
-from nomenklatura.dataset.resource import DataResource
-from nomenklatura.dataset.publisher import DataPublisher
 from nomenklatura.dataset.coverage import DataCoverage
-from nomenklatura.dataset.util import Named, cleanup, string_list
-from nomenklatura.dataset.util import type_check, type_require
-from nomenklatura.util import iso_to_version, PathLike
+from nomenklatura.dataset.publisher import DataPublisher
+from nomenklatura.dataset.resource import DataResource
+from nomenklatura.dataset.util import (
+    Named,
+    cleanup,
+    string_list,
+    type_check,
+    type_require,
+)
+from nomenklatura.util import PathLike, iso_to_version
 
 if TYPE_CHECKING:
     from nomenklatura.dataset.catalog import DataCatalog
 
 DS = TypeVar("DS", bound="Dataset")
 
 
@@ -27,14 +32,15 @@
         self.title = type_require(registry.string, data["title"])
         self.license = type_check(registry.url, data.get("license"))
         self.summary = type_check(registry.string, data.get("summary"))
         self.description = type_check(registry.string, data.get("description"))
         self.url = type_check(registry.url, data.get("url"))
         self.updated_at = type_check(registry.date, data.get("updated_at"))
         self.version = type_check(registry.string, data.get("version"))
+        self.category = type_check(registry.string, data.get("category"))
         if self.version is None and self.updated_at is not None:
             self.version = iso_to_version(self.updated_at)
 
         pdata = data.get("publisher")
         self.publisher = DataPublisher(pdata) if pdata is not None else None
 
         cdata = data.get("coverage")
@@ -79,24 +85,36 @@
             current.remove(self)
         return current
 
     @property
     def dataset_names(self) -> List[str]:
         return [d.name for d in self.datasets]
 
+    @cached_property
+    def scope_names(self) -> Set[str]:
+        """This is based on the premise that collections (ie. datasets which have children)
+        never contain entities themselves that need to be queried."""
+        if len(self.children):
+            return {d.name for d in self.children}
+        return {self.name}
+
+    def __repr__(self) -> str:
+        return f"<Dataset({self.name})>"  # pragma: no cover
+
     def to_dict(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {
             "name": self.name,
             "title": self.title,
             "license": self.license,
             "summary": self.summary,
             "description": self.description,
             "url": self.url,
             "version": self.version,
             "updated_at": self.updated_at,
+            "category": self.category,
             "resources": [r.to_dict() for r in self.resources],
             "children": [c.name for c in self.children],
         }
         if self.coverage is not None:
             data["coverage"] = self.coverage.to_dict()
         if self.publisher is not None:
             data["publisher"] = self.publisher.to_dict()
```

### Comparing `nomenklatura-2.9.5/nomenklatura/dataset/publisher.py` & `nomenklatura-3.0.0/nomenklatura/dataset/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,66 @@
-from banal import as_bool
-from typing import Optional, Dict, Any
+from typing import Any, Dict, Iterable, List, Optional
+
 from followthemoney.types import registry
+from followthemoney.types.common import PropertyType
+from normality import stringify
+
+from nomenklatura.exceptions import MetadataException
+
 
-from nomenklatura.dataset.util import Named, cleanup
-from nomenklatura.dataset.util import type_check, type_require
+def type_check(
+    type_: PropertyType, value: Any, options: Iterable[str] = []
+) -> Optional[str]:
+    text = stringify(value)
+    if text is None:
+        return None
+    cleaned = type_.clean_text(text)
+    if cleaned is None:
+        raise MetadataException("Invalid %s: %r" % (type_.name, value))
+    if options and cleaned not in options:
+        raise MetadataException(
+            "Invalid %s: %r not in %s" % (type_.name, value, ",".join(options))
+        )
+    return cleaned
+
+
+def type_require(type_: PropertyType, value: Any) -> str:
+    text = stringify(value)
+    if text is None:
+        raise MetadataException("Invalid %s: %r" % (type_.name, value))
+    cleaned = type_.clean_text(text)
+    if cleaned is None:
+        raise MetadataException("Invalid %s: %r" % (type_.name, value))
+    return cleaned
+
+
+def string_list(value: Any) -> List[str]:
+    if value is None:
+        return []
+    return [type_require(registry.string, s) for s in value]
+
+
+def cleanup(data: Dict[str, Any]) -> Dict[str, Any]:
+    for key, value in list(data.items()):
+        if value is None:
+            data.pop(key)
+    return data
+
+
+class Named(object):
+    def __init__(self, name: str) -> None:
+        self.name = name
+
+    def __eq__(self, other: Any) -> bool:
+        try:
+            return not not self.name == other.name
+        except AttributeError:
+            return False
 
+    def __lt__(self, other: Any) -> bool:
+        return self.name.__lt__(other.name)
 
-class DataPublisher(Named):
-    """Publisher information, eg. the government authority."""
+    def __hash__(self) -> int:
+        return hash(self.name)
 
-    def __init__(self, data: Dict[str, Any]):
-        name = type_require(registry.string, data.get("name"))
-        super().__init__(name)
-        self.url = type_require(registry.url, data.get("url"))
-        self.description = type_check(registry.string, data.get("description"))
-        self.country = type_check(registry.country, data.get("country"))
-        self.official = as_bool(data.get("official", False))
-
-    @property
-    def country_label(self) -> Optional[str]:
-        if self.country is None:
-            return None
-        return registry.country.caption(self.country)
-
-    def to_dict(self) -> Dict[str, Any]:
-        data = {
-            "name": self.name,
-            "url": self.url,
-            "description": self.description,
-            "country": self.country,
-            "country_label": self.country_label,
-            "official": self.official,
-        }
-        return cleanup(data)
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}({self.name!r})>"
```

### Comparing `nomenklatura-2.9.5/nomenklatura/dataset/resource.py` & `nomenklatura-3.0.0/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/db.py` & `nomenklatura-3.0.0/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/__init__.py` & `nomenklatura-3.0.0/nomenklatura/enrich/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from importlib import import_module
 from typing import Iterable, Generator, Optional, Type, cast
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
-from nomenklatura.matching import compare_scored
+from nomenklatura.matching import DefaultAlgorithm
 from nomenklatura.enrich.common import Enricher, EnricherConfig
 from nomenklatura.enrich.common import EnrichmentAbort, EnrichmentException
 from nomenklatura.judgement import Judgement
 from nomenklatura.resolver import Resolver
 
 log = logging.getLogger(__name__)
 __all__ = [
@@ -43,15 +43,15 @@
             for match in enricher.match_wrapped(entity):
                 if entity.id is None or match.id is None:
                     continue
                 if not resolver.check_candidate(entity.id, match.id):
                     continue
                 if not entity.schema.can_match(match.schema):
                     continue
-                result = compare_scored(entity, match)
+                result = DefaultAlgorithm.compare(entity, match)
                 score = result["score"]
                 log.info("Match [%s]: %.2f -> %s", entity, score, match)
                 resolver.suggest(entity.id, match.id, score)
                 match.datasets.add(enricher.dataset.name)
                 match = resolver.apply(match)
                 yield match
         except EnrichmentException:
```

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/aleph.py` & `nomenklatura-3.0.0/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/common.py` & `nomenklatura-3.0.0/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.0.0/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.0.0/nomenklatura/enrich/opencorporates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,74 @@
+import json
 import logging
 from normality import slugify
 from typing import cast, Any, Dict, Generator, Optional
 from urllib.parse import urlparse
 from banal import ensure_dict
 from followthemoney.types import registry
-from requests.exceptions import HTTPError
+from requests.exceptions import RequestException
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.enrich.common import Enricher, EnricherConfig
-from nomenklatura.enrich.common import EnrichmentAbort
+from nomenklatura.enrich.common import EnrichmentAbort, EnrichmentException
+from nomenklatura.util import normalize_url, ParamsType
 
 
 log = logging.getLogger(__name__)
 
 
+def parse_date(raw: Any) -> Optional[str]:
+    return registry.date.clean(raw)
+
+
 class OpenCorporatesEnricher(Enricher):
     COMPANY_SEARCH_API = "https://api.opencorporates.com/v0.4/companies/search"
     OFFICER_SEARCH_API = "https://api.opencorporates.com/v0.4/officers/search"
     UI_PART = "://opencorporates.com/"
     API_PART = "://api.opencorporates.com/v0.4/"
 
     def __init__(self, dataset: DS, cache: Cache, config: EnricherConfig):
         super().__init__(dataset, cache, config)
         token_var = "${OPENCORPORATES_API_TOKEN}"
         self.api_token: Optional[str] = self.get_config_expand("api_token", token_var)
+        self.quota_exceeded = False
         if self.api_token == token_var:
             self.api_token = None
         if self.api_token is None:
             log.warning("OpenCorporates has no API token (%s)" % token_var)
         self.cache.preload(f"{self.COMPANY_SEARCH_API}%")
 
+    def oc_get_cached(self, url: str, params: ParamsType = None) -> Optional[Any]:
+        url = normalize_url(url, params=params)
+        response = self.cache.get(url, max_age=self.cache_days)
+        if response is None:
+            if self.quota_exceeded:
+                return None
+            hidden_url = normalize_url(url, params={"api_token": self.api_token})
+            try:
+                resp = self.session.get(hidden_url)
+                resp.raise_for_status()
+            except RequestException as rex:
+                if rex.response is not None:
+                    if rex.response.status_code == 403:
+                        log.info("OpenCorporates quota exceeded; using only cache now.")
+                        self.quota_exceeded = True
+                        return None
+                    elif rex.response.status_code == 401:
+                        raise EnrichmentAbort(
+                            "Authorization failure: %s" % url
+                        ) from rex
+                msg = "HTTP fetch failed [%s]: %s" % (url, rex)
+                raise EnrichmentException(msg) from rex
+            response = resp.text
+            self.cache.set(url, response)
+        return json.loads(response)
+
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
 
         if entity.schema.name in ["Company", "Organization", "LegalEntity"]:
             yield from self.search_companies(entity)
         if entity.schema.name in ["Person", "LegalEntity", "Company", "Organization"]:
@@ -77,23 +110,25 @@
 
         juris = self.jurisdiction_to_country(data.get("jurisdiction_code"))
         entity.add("jurisdiction", juris)
         entity.add("alias", data.get("alternative_names"))
         entity.add("address", data.get("registered_address_in_full"))
         entity.add("sourceUrl", data.get("registry_url"))
         entity.add("legalForm", data.get("company_type"))
-        entity.add("incorporationDate", data.get("incorporation_date"))
-        entity.add("dissolutionDate", data.get("dissolution_date"))
+        inc_date = data.get("incorporation_date")
+        entity.add("incorporationDate", parse_date(inc_date))
+        dis_date = data.get("dissolution_date")
+        entity.add("dissolutionDate", parse_date(dis_date))
         entity.add("status", data.get("current_status"))
         entity.add("registrationNumber", data.get("company_number"))
         entity.add("opencorporatesUrl", oc_url)
         source = data.get("source", {})
         entity.add("publisher", source.get("publisher"))
         entity.add("publisherUrl", source.get("url"))
-        entity.add("retrievedAt", source.get("retrieved_at"))
+        entity.add("retrievedAt", parse_date(source.get("retrieved_at")))
         for code in data.get("industry_codes", []):
             code = code.get("industry_code", code)
             entity.add("sector", code.get("description"))
         for previous in data.get("previous_names", []):
             entity.add("previousName", previous.get("company_name"))
         for alias in data.get("alternative_names", []):
             entity.add("alias", alias.get("company_name"))
@@ -115,31 +150,22 @@
     #     entity.add("opencorporatesUrl", data.get("opencorporates_url"))
     #     source = data.get("source", {})
     #     entity.add("publisher", source.get("publisher"))
     #     entity.add("publisherUrl", source.get("url"))
     #     entity.add("retrievedAt", source.get("retrieved_at"))
     #     return entity
 
-    def names_query(self, entity: CE) -> str:
-        # names = entity.get_type_values(registry.name)
-        # names = set([n.lower() for n in names])
-        # print(names)
-        return entity.caption
-
     def search_companies(self, entity: CE) -> Generator[CE, None, None]:
         countries = entity.get_type_values(registry.country)
-        q = self.names_query(entity)
-        params = {"q": q, "sparse": True, "country_codes": countries}
+        params = {"q": entity.caption, "sparse": True, "country_codes": countries}
         for page in range(1, 9):
             params["page"] = page
-            results = self.http_get_json_cached(
-                self.COMPANY_SEARCH_API,
-                params=params,
-                hidden={"api_token": self.api_token},
-            )
+            results = self.oc_get_cached(self.COMPANY_SEARCH_API, params=params)
+            if results is None:
+                break
 
             # print(results)
             for company in results.get("results", {}).get("companies", []):
                 proxy = self.company_entity(entity, company)
                 yield proxy
             if page >= results.get("total_pages", 0):
                 break
```

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.0.0/nomenklatura/enrich/wikidata/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from functools import cache
 from typing import cast, Generator, Any, Dict, Optional, Set
 from followthemoney.helpers import check_person_cutoff
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
-from nomenklatura.enrich.wikidata.lang import pick_obj_lang
+from nomenklatura.enrich.wikidata.lang import LangText, pick_obj_lang
 from nomenklatura.enrich.wikidata.qualified import qualify_value
 from nomenklatura.enrich.wikidata.props import (
     PROPS_ASSOCIATION,
     PROPS_DIRECT,
     PROPS_FAMILY,
     PROPS_QUALIFIED,
     PROPS_TOPICS,
 )
 from nomenklatura.enrich.wikidata.model import Claim, Item
 from nomenklatura.enrich.common import Enricher, EnricherConfig
 from nomenklatura.util import is_qid
 
 WD_API = "https://www.wikidata.org/w/api.php"
-LABEL_PREFIX = "wd:label"
+LABEL_PREFIX = "wd:lb:"
 log = logging.getLogger(__name__)
 
 
 class WikidataEnricher(Enricher):
     def __init__(self, dataset: DS, cache: Cache, config: EnricherConfig):
         super().__init__(dataset, cache, config)
         self.depth = self.get_config_int("depth", 1)
@@ -107,30 +107,31 @@
         data = self.wikibase_getentities(qid, cache_days=cache_days)
         entity = data.get("entities", {}).get(qid)
         if entity is None:
             return None
         return Item(entity)
 
     @cache
-    def get_label(self, qid: str) -> Optional[str]:
-        cache_key = f"{LABEL_PREFIX}:{qid}"
-        cached = self.cache.get(cache_key, max_age=self.label_cache_days)
+    def get_label(self, qid: str) -> LangText:
+        cache_key = f"{LABEL_PREFIX}{qid}"
+        cached = self.cache.get_json(cache_key, max_age=self.label_cache_days)
         if cached is not None:
-            return cached
+            return LangText.parse(cached)
         data = self.wikibase_getentities(
             qid,
             cache_days=self.cache_days,
             props="labels",
         )
         entity = data.get("entities", {}).get(qid)
         label = pick_obj_lang(entity.get("labels", {}))
-        if label is not None:
-            self.cache.set(cache_key, label.text)
-            return label.text
-        return None
+        if label.text is None:
+            label.text = qid
+        label.original = qid
+        self.cache.set_json(cache_key, label.pack())
+        return label
 
     def make_link(
         self,
         proxy: CE,
         claim: Claim,
         depth: int,
         seen: Set[str],
@@ -155,45 +156,46 @@
         if "role.pep" in proxy.get("topics", quiet=True):
             if "role.pep" not in other.get("topics"):
                 other.add("topics", "role.rca")
         yield other
         yield from self.item_graph(other, item, depth=depth - 1, seen=seen)
         link = self.make_entity(proxy, schema)
         min_id, max_id = sorted((proxy.id, other.id))
+        # FIXME: doesn't lead to collisions because claim.property has an inverse:
         link.id = f"wd-{claim.property}-{min_id}-{max_id}"
         link.id = link.id.lower()
         link.add(source_prop, proxy.id)
         link.add(target_prop, item.id)
         rel = claim.property_label(self)
-        link.add("relationship", rel)
+        rel.apply(link, "relationship")
 
         for qual in claim.get_qualifier("P580"):
             text = qual.text(self)
-            link.add("startDate", text)
+            text.apply(link, "startDate")
 
         for qual in claim.get_qualifier("P582"):
             text = qual.text(self)
-            link.add("endDate", text)
+            text.apply(link, "endDate")
 
         for qual in claim.get_qualifier("P585"):
             text = qual.text(self)
-            link.add("date", text)
+            text.apply(link, "date")
 
         for qual in claim.get_qualifier("P1039"):
             text = qual.text(self)
-            link.set("relationship", text)
+            text.apply(link, "relationship")
 
         for qual in claim.get_qualifier("P2868"):
             text = qual.text(self)
-            link.set("relationship", text)
+            text.apply(link, "relationship")
 
         for ref in claim.references:
             for snak in ref.get("P854"):
                 text = snak.text(self)
-                link.add("sourceUrl", text)
+                text.apply(link, "sourceUrl")
         yield link
 
     def item_graph(
         self,
         proxy: CE,
         item: Item,
         depth: Optional[int] = None,
@@ -234,17 +236,18 @@
     def item_proxy(self, ref: CE, item: Item, schema: str = "Person") -> Optional[CE]:
         proxy = self.make_entity(ref, schema)
         proxy.id = item.id
         if item.modified is None:
             return None
         proxy.add("modifiedAt", item.modified)
         proxy.add("wikidataId", item.id)
-        proxy.add("name", item.label)
-        proxy.add("notes", item.description)
-        proxy.add("alias", item.aliases)
+        item.label.apply(proxy, "name")
+        item.description.apply(proxy, "notes")
+        for alias in item.aliases:
+            alias.apply(proxy, "alias")
 
         if proxy.schema.is_a("Person") and not item.is_instance("Q5"):
             log.debug("Person is not a Q5 [%s]: %s", item.id, item.label)
             return None
 
         for claim in item.claims:
             if claim.property is None:
@@ -252,13 +255,16 @@
             ftm_prop = PROPS_DIRECT.get(claim.property)
             if ftm_prop is None:
                 continue
             if ftm_prop not in proxy.schema.properties:
                 log.info("Entity %s does not have property: %s", proxy.id, ftm_prop)
                 continue
             value = claim.text(self)
-            if ftm_prop in PROPS_QUALIFIED and value is not None:
+            if ftm_prop in PROPS_QUALIFIED:
                 value = qualify_value(self, value, claim)
-            if ftm_prop == "topics" and claim.qid is not None:
-                value = PROPS_TOPICS.get(claim.qid)
-            proxy.add(ftm_prop, value)
+            if ftm_prop == "topics":
+                topic = PROPS_TOPICS.get(claim.qid or "")
+                if topic is None:
+                    continue
+                value = LangText(topic, original=claim.qid)
+            value.apply(proxy, ftm_prop)
         return proxy
```

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.0.0/nomenklatura/enrich/wikidata/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from normality import stringify
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 
 from nomenklatura.enrich.wikidata.value import snak_value_to_string
-from nomenklatura.enrich.wikidata.lang import pick_obj_lang
+from nomenklatura.enrich.wikidata.lang import pick_obj_lang, LangText
 
 if TYPE_CHECKING:
     from nomenklatura.enrich.wikidata import WikidataEnricher
 
 
 class Snak(object):
     """Some Notation About Knowledge (TM)."""
@@ -17,24 +17,24 @@
         self._value = datavalue.pop("value", None)
         data.pop("hash", None)
         self.type = data.pop("datatype", None)
         self.property: Optional[str] = data.pop("property", None)
         self.snaktype = data.pop("snaktype", None)
         # self._data = data
 
-    def property_label(self, enricher: "WikidataEnricher") -> Optional[str]:
+    def property_label(self, enricher: "WikidataEnricher") -> LangText:
         return enricher.get_label(self.property)
 
     @property
     def qid(self) -> Optional[str]:
         if self.value_type == "wikibase-entityid":
             return stringify(self._value.get("id"))
         return None
 
-    def text(self, enricher: "WikidataEnricher") -> Optional[str]:
+    def text(self, enricher: "WikidataEnricher") -> LangText:
         return snak_value_to_string(enricher, self.value_type, self._value)
 
 
 class Reference(object):
     def __init__(self, data: Dict[str, Any]) -> None:
         self.snaks: Dict[str, List[Snak]] = {}
         for prop, snak_data in data.pop("snaks", {}).items():
@@ -64,35 +64,28 @@
     """A wikidata item (or entity)."""
 
     def __init__(self, data: Dict[str, Any]) -> None:
         self.id: str = data.pop("id")
         self.modified: Optional[str] = data.pop("modified", None)
 
         labels: Dict[str, Dict[str, str]] = data.pop("labels", {})
-        self.label: Optional[str] = None
-        label = pick_obj_lang(labels)
-        if label is not None:
-            self.label = label.text
-        self.aliases: Set[str] = set()
+        self.label: LangText = pick_obj_lang(labels)
+        self.aliases: Set[LangText] = set()
         for obj in labels.values():
-            self.aliases.add(obj["value"])
+            self.aliases.add(LangText(obj["value"], obj["language"]))
 
         aliases: Dict[str, List[Dict[str, str]]] = data.pop("aliases", {})
         for lang in aliases.values():
             for obj in lang:
-                self.aliases.add(obj["value"])
+                self.aliases.add(LangText(obj["value"], obj["language"]))
 
-        if self.label is not None:
-            self.aliases.discard(self.label)
+        self.aliases.discard(self.label)
 
         descriptions: Dict[str, Dict[str, str]] = data.pop("descriptions", {})
-        self.description: Optional[str] = None
-        description = pick_obj_lang(descriptions)
-        if description is not None:
-            self.description = description.text
+        self.description = pick_obj_lang(descriptions)
 
         self.claims: List[Claim] = []
         claims: Dict[str, List[Dict[str, Any]]] = data.pop("claims", {})
         for prop, values in claims.items():
             for value in values:
                 self.claims.append(Claim(value, prop))
```

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.0.0/nomenklatura/enrich/wikidata/props.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,8 +60,11 @@
 
 PROPS_TOPICS = {
     "Q82955": "role.pep",
     "Q193391": "role.diplo",
     "Q392651": "role.spy",
     "Q14886050": "crime.terror",
     "Q16533": "role.judge",
+    "Q17276321": "role.pep",  # member of the state duma
+    "Q189290": "mil",  # military officer
+    "Q47064": "mil",  # military personnel
 }
```

### Comparing `nomenklatura-2.9.5/nomenklatura/enrich/yente.py` & `nomenklatura-3.0.0/nomenklatura/enrich/yente.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
+import time
 import logging
 from banal import ensure_list
 from typing import Any, Generator, Optional, Dict, List
 from urllib.parse import urljoin
 from followthemoney.types import registry
 from followthemoney.namespace import Namespace
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.enrich.common import Enricher, EnricherConfig
+from nomenklatura.enrich.common import EnrichmentException
 from nomenklatura.util import normalize_url
 
 log = logging.getLogger(__name__)
 
 
 class YenteEnricher(Enricher):
     """Uses the `yente` match API to look up entities in a specific dataset."""
@@ -58,15 +60,23 @@
             "queries": {
                 "entity": {
                     "schema": entity.schema.name,
                     "properties": props,
                 }
             }
         }
-        response = self.http_post_json_cached(url, cache_key, query)
+        for retry in range(4):
+            try:
+                response = self.http_post_json_cached(url, cache_key, query)
+            except EnrichmentException as exc:
+                log.info("Error matching %r: %s", entity, exc)
+                if retry == 3:
+                    raise
+                time.sleep((retry + 1) ** 2)
+
         inner_resp = response.get("responses", {}).get("entity", {})
         for result in inner_resp.get("results", []):
             proxy = self.load_entity(entity, result)
             proxy.add("sourceUrl", self.make_url(proxy))
             if self._ns is not None:
                 proxy = self._ns.apply(proxy)
             yield proxy
```

### Comparing `nomenklatura-2.9.5/nomenklatura/entity.py` & `nomenklatura-3.0.0/nomenklatura/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from hashlib import sha1
-from banal import hash_data
-from datetime import datetime
 from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 from typing import Generator, Iterable, Tuple, Type, TypeVar
 from followthemoney import model
 from followthemoney.model import Model
 from followthemoney.exc import InvalidData
 from followthemoney.types.common import PropertyType
@@ -13,66 +11,61 @@
 from followthemoney.proxy import P
 from followthemoney.types import registry
 from followthemoney.proxy import EntityProxy
 
 from nomenklatura.dataset import DS
 from nomenklatura.publish.names import pick_name
 from nomenklatura.statement.statement import Statement
+from nomenklatura.util import BASE_ID
 
 if TYPE_CHECKING:
-    from nomenklatura.loader import Loader
+    from nomenklatura.store import View
 
 CE = TypeVar("CE", bound="CompositeEntity")
+DEFAULT_DATASET = "default"
 
 
 class CompositeEntity(EntityProxy):
     """An entity object that can link to a set of datasets that it is sourced from."""
 
     __slots__ = (
         "schema",
         "id",
         "_caption",
-        "target",
-        "external",
-        "referents",
-        "datasets",
+        "extra_referents",
         "default_dataset",
         "statement_type",
         "_statements",
     )
 
     def __init__(
         self,
         model: "Model",
         data: Dict[str, Any],
         cleaned: bool = True,
-        default_dataset: str = "default",
+        default_dataset: str = DEFAULT_DATASET,
     ):
         data = dict(data or {})
         schema = model.get(data.pop("schema", None))
         if schema is None:
             raise InvalidData(gettext("No schema for entity."))
         self.schema = schema
 
         self._caption: Optional[str] = None
         """A pre-computed label for this entity."""
 
-        self.target: Optional[bool] = data.pop("target", None)
-        self.external: Optional[bool] = data.pop("external", None)
-        self.referents: Set[str] = set(data.pop("referents", []))
+        self.extra_referents: Set[str] = set(data.pop("referents", []))
         """The IDs of all entities which are included in this canonical entity."""
 
-        self.datasets: Set[str] = set(data.pop("datasets", []))
-        """The set of datasets from which information in this entity is derived."""
-
         self.default_dataset = default_dataset
         self.id: Optional[str] = data.pop("id", None)
         self._statements: Dict[str, Set[Statement]] = {}
 
         properties = data.pop("properties", None)
+        # external = data.pop("external", None)
         if isinstance(properties, Mapping):
             for key, value in properties.items():
                 self.add(key, value, cleaned=cleaned, quiet=True)
 
     @property
     def _properties(self) -> Dict[str, List[str]]:  # type: ignore
         return {p: [s.value for s in v] for p, v in self._statements.items()}
@@ -93,39 +86,62 @@
 
     @property
     def statements(self) -> Generator[Statement, None, None]:
         if self.id is not None:
             yield Statement(
                 canonical_id=self.id,
                 entity_id=self.id,
-                prop=Statement.BASE,
-                prop_type=Statement.BASE,
+                prop=BASE_ID,
+                prop_type=BASE_ID,
                 schema=self.schema.name,
                 value=self.checksum(),
                 dataset=self.default_dataset,
             )
         yield from self._iter_stmt()
 
     @property
-    def first_seen(self) -> Optional[datetime]:
+    def first_seen(self) -> Optional[str]:
         seen = (s.first_seen for s in self._iter_stmt() if s.first_seen is not None)
         return min(seen, default=None)
 
     @property
-    def last_seen(self) -> Optional[datetime]:
+    def last_seen(self) -> Optional[str]:
         seen = (s.last_seen for s in self._iter_stmt() if s.last_seen is not None)
         return max(seen, default=None)
 
     @property
+    def target(self) -> Optional[bool]:
+        target: Optional[bool] = None
+        for stmt in self._iter_stmt():
+            if stmt.target is not None:
+                target = target or stmt.target
+        return target
+
+    @property
+    def datasets(self) -> Set[str]:
+        datasets: Set[str] = set()
+        for stmt in self._iter_stmt():
+            datasets.add(stmt.dataset)
+        return datasets
+
+    @property
+    def referents(self) -> Set[str]:
+        referents: Set[str] = set(self.extra_referents)
+        for stmt in self._iter_stmt():
+            if stmt.entity_id is not None and stmt.entity_id != self.id:
+                referents.add(stmt.entity_id)
+        return referents
+
+    @property
     def key_prefix(self) -> Optional[str]:
         return self.default_dataset
 
     @key_prefix.setter
-    def key_prefix(self, dataset: Optional[str]) -> None:
-        raise NotImplemented
+    def key_prefix(self, dataset: str) -> None:
+        self.default_dataset = dataset
 
     def _pick_caption(self) -> str:
         is_thing = self.schema.is_a("Thing")
         for prop in self.schema.caption:
             values = self.get(prop)
             if is_thing and len(values) > 1:
                 name = pick_name(values)
@@ -147,20 +163,15 @@
     def add_statement(self, stmt: Statement) -> None:
         # TODO: change target, schema etc. based on data
         if not self.schema.is_a(stmt.schema):
             try:
                 self.schema = model.common_schema(self.schema, stmt.schema)
             except InvalidData as exc:
                 raise InvalidData(f"{self.id}: {exc}") from exc
-        if stmt.target is not None:
-            self.target = self.target or stmt.target
-        self.datasets.add(stmt.dataset)
-        if stmt.entity_id != self.id and stmt.entity_id is not None:
-            self.referents.add(stmt.entity_id)
-        if stmt.prop != Statement.BASE:
+        if stmt.prop != BASE_ID:
             self._statements.setdefault(stmt.prop, set())
             self._statements[stmt.prop].add(stmt)
 
     def clean_value(
         self,
         prop: Property,
         value: Optional[str],
@@ -179,15 +190,15 @@
 
     def claim(
         self,
         prop: P,
         value: Optional[str],
         schema: Optional[str] = None,
         dataset: Optional[str] = None,
-        seen: Optional[datetime] = None,
+        seen: Optional[str] = None,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
         cleaned: bool = False,
         quiet: bool = False,
         fuzzy: bool = False,
         format: Optional[str] = None,
     ) -> None:
@@ -231,15 +242,15 @@
 
     def claim_many(
         self,
         prop: P,
         values: Iterable[Optional[str]],
         schema: Optional[str] = None,
         dataset: Optional[str] = None,
-        seen: Optional[datetime] = None,
+        seen: Optional[str] = None,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
         cleaned: bool = False,
         quiet: bool = False,
         fuzzy: bool = False,
         format: Optional[str] = None,
     ) -> None:
@@ -412,44 +423,48 @@
             data["last_seen"] = self.last_seen
         return data
 
     def __len__(self) -> int:
         return len(list(self._iter_stmt())) + 1
 
     def _to_nested_dict(
-        self: CE, loader: "Loader[DS, CE]", depth: int, path: List[str]
+        self: CE, view: "View[DS, CE]", depth: int, path: List[str]
     ) -> Dict[str, Any]:
         next_depth = depth if self.schema.edge else depth - 1
         next_path = list(path)
         if self.id is not None:
             next_path.append(self.id)
         data = self.to_dict()
         if next_depth < 0:
             return data
-        nested: Dict[str, Any] = {}
-        for prop, adjacent in loader.get_adjacent(self):
+        nested: Dict[str, List[Any]] = {}
+        for prop, adjacent in view.get_adjacent(self):
             if adjacent.id in next_path:
                 continue
-            value = adjacent._to_nested_dict(loader, next_depth, next_path)
+            value = adjacent._to_nested_dict(view, next_depth, next_path)
             if prop.name not in nested:
                 nested[prop.name] = []
             nested[prop.name].append(value)
         data["properties"].update(nested)
         return data
 
     def to_nested_dict(
-        self: CE, loader: "Loader[DS, CE]", depth: int = 1
+        self: CE, view: "View[DS, CE]", depth: int = 1
     ) -> Dict[str, Any]:
-        return self._to_nested_dict(loader, depth=depth, path=[])
+        return self._to_nested_dict(view, depth=depth, path=[])
 
     @classmethod
     def from_dict(
-        cls: Type[CE], model: Model, data: Dict[str, Any], cleaned: bool = True
+        cls: Type[CE],
+        model: Model,
+        data: Dict[str, Any],
+        cleaned: bool = True,
+        default_dataset: str = DEFAULT_DATASET,
     ) -> CE:
-        return super().from_dict(model, data, cleaned=cleaned)
+        return cls(model, data, cleaned=cleaned, default_dataset=default_dataset)
 
     @classmethod
     def from_statements(cls: Type[CE], statements: Iterable[Statement]) -> CE:
         obj: Optional[CE] = None
         for stmt in statements:
             if obj is None:
                 data = {"schema": stmt.schema, "id": stmt.canonical_id}
```

### Comparing `nomenklatura-2.9.5/nomenklatura/index/entry.py` & `nomenklatura-3.0.0/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/judgement.py` & `nomenklatura-3.0.0/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/matching/features/dates.py` & `nomenklatura-3.0.0/nomenklatura/matching/v1/dates.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-from typing import Iterable, Set
 from prefixdate import Precision
+from followthemoney.proxy import E
 
-from nomenklatura.entity import CompositeEntity as Entity
-from nomenklatura.matching.features.util import props_pair, has_overlap
-
-
-def with_precision(values: Iterable[str], precision: Precision) -> Set[str]:
-    dates = set()
-    for value in values:
-        if len(value) >= precision.value:
-            dates.add(value[: precision.value])
-    return dates
+from nomenklatura.matching.v1.util import has_overlap
+from nomenklatura.matching.util import props_pair, dates_precision
 
 
 def flip_day_month(value: str) -> str:
     # This is such a common mistake we just consider flips as matches.
     year, month, day = value.split("-", 2)
     return f"{year}-{day}-{month}"
 
 
-def dob_matches(left: Entity, right: Entity) -> float:
+def dob_matches(left: E, right: E) -> float:
     """The birth date or incorporation date of the two entities is the same."""
     left_dates, right_dates = props_pair(left, right, ["birthDate"])
-    left_days = with_precision(left_dates, Precision.DAY)
+    left_days = dates_precision(left_dates, Precision.DAY)
     left_days.update([flip_day_month(d) for d in left_days])
-    right_days = with_precision(right_dates, Precision.DAY)
+    right_days = dates_precision(right_dates, Precision.DAY)
     return has_overlap(left_days, right_days)
 
 
-def dob_year_matches(left: Entity, right: Entity) -> float:
+def dob_year_matches(left: E, right: E) -> float:
     """The birth date or incorporation year of the two entities is the same."""
     left_dates, right_dates = props_pair(left, right, ["birthDate"])
-    left_years = with_precision(left_dates, Precision.YEAR)
-    right_years = with_precision(right_dates, Precision.YEAR)
+    left_years = dates_precision(left_dates, Precision.YEAR)
+    right_years = dates_precision(right_dates, Precision.YEAR)
     if len(left_years.intersection(right_dates)) > 0:
         return 1.0
     if len(right_years.intersection(left_dates)) > 0:
         return 1.0
     return 0.0
```

### Comparing `nomenklatura-2.9.5/nomenklatura/matching/features/misc.py` & `nomenklatura-3.0.0/nomenklatura/matching/v1/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,75 @@
+from followthemoney.proxy import E
 from followthemoney.types import registry
-from nomenklatura.entity import CompositeEntity as Entity
 
-from nomenklatura.matching.features.util import normalize_text, tokenize_pair
-from nomenklatura.matching.features.util import has_disjoint, has_overlap, has_schema
-from nomenklatura.matching.features.util import compare_levenshtein, compare_sets
-from nomenklatura.matching.features.util import props_pair, type_pair, extract_numbers
+from nomenklatura.matching.v1.util import has_disjoint, has_overlap
+from nomenklatura.matching.v1.util import compare_levenshtein, tokenize_pair
+from nomenklatura.matching.util import extract_numbers, props_pair, type_pair
+from nomenklatura.matching.util import compare_sets, has_schema
+from nomenklatura.util import normalize_name
 
 
-def birth_place(left: Entity, right: Entity) -> float:
+def birth_place(left: E, right: E) -> float:
     """Same place of birth."""
     lv, rv = tokenize_pair(props_pair(left, right, ["birthPlace"]))
     tokens = min(len(lv), len(rv))
     return float(len(lv.intersection(rv))) / float(max(2.0, tokens))
 
 
-def address_match(left: Entity, right: Entity) -> float:
+def address_match(left: E, right: E) -> float:
     """Text similarity between addresses."""
     lv, rv = type_pair(left, right, registry.address)
-    lvn = [normalize_text(v) for v in lv]
-    rvn = [normalize_text(v) for v in rv]
+    lvn = [normalize_name(v) for v in lv]
+    rvn = [normalize_name(v) for v in rv]
     return compare_sets(lvn, rvn, compare_levenshtein)
 
 
-def address_numbers(left: Entity, right: Entity) -> float:
+def address_numbers(left: E, right: E) -> float:
     """Find if names contain numbers, score if the numbers are different."""
     lv, rv = type_pair(left, right, registry.address)
     lvn = extract_numbers(lv)
     rvn = extract_numbers(rv)
     common = len(lvn.intersection(rvn))
     disjoint = len(lvn.difference(rvn))
     return common - disjoint
 
 
-def gender_mismatch(left: Entity, right: Entity) -> float:
+def gender_mismatch(left: E, right: E) -> float:
     """Both entities have a different gender associated with them."""
     lv, rv = props_pair(left, right, ["gender"])
     return has_disjoint(lv, rv)
 
 
-def phone_match(left: Entity, right: Entity) -> float:
+def phone_match(left: E, right: E) -> float:
     """Matching phone numbers between the two entities."""
     lv, rv = type_pair(left, right, registry.phone)
     return has_overlap(set(lv), set(rv))
 
 
-def email_match(left: Entity, right: Entity) -> float:
+def email_match(left: E, right: E) -> float:
     """Matching email addresses between the two entities."""
     lv, rv = type_pair(left, right, registry.email)
     return has_overlap(set(lv), set(rv))
 
 
-def identifier_match(left: Entity, right: Entity) -> float:
+def identifier_match(left: E, right: E) -> float:
     """Matching identifiers (e.g. passports, national ID cards, registration or
     tax numbers) between the two entities."""
     if has_schema(left, right, "Organization"):
         return 0.0
     lv, rv = type_pair(left, right, registry.identifier)
     return has_overlap(set(lv), set(rv))
 
 
-def org_identifier_match(left: Entity, right: Entity) -> float:
+def org_identifier_match(left: E, right: E) -> float:
     """Matching identifiers (e.g. registration or tax numbers) between two
     organizations or companies."""
     if not has_schema(left, right, "Organization"):
         return 0.0
     lv, rv = type_pair(left, right, registry.identifier)
     return has_overlap(set(lv), set(rv))
 
 
-def country_mismatch(left: Entity, right: Entity) -> float:
+def country_mismatch(left: E, right: E) -> float:
     """Both entities are linked to different countries."""
     lv, rv = type_pair(left, right, registry.country)
     return has_disjoint(set(lv), set(rv))
```

### Comparing `nomenklatura-2.9.5/nomenklatura/matching/features/util.py` & `nomenklatura-3.0.0/nomenklatura/matching/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,60 @@
 import re
-import math
-import Levenshtein
+from pathlib import Path
 from itertools import product
-from normality import slugify
-from functools import lru_cache
-from normality.constants import WS
-from typing import Callable, Iterable, List
-from typing import Optional, Set, Tuple, TypeVar
+from prefixdate import Precision
+from typing import List, Set, TypeVar, Tuple, Iterable, Optional, Callable, Any
+from followthemoney.proxy import E
 from followthemoney.types.common import PropertyType
 
-from nomenklatura.entity import CompositeEntity as Entity
+from nomenklatura import __version__
+from nomenklatura.util import DATA_PATH
 
 V = TypeVar("V")
-FIND_NUM = re.compile("\d{2,}")
+FIND_NUM = re.compile(r"\d{2,}")
+BASE_URL = "https://github.com/opensanctions/nomenklatura/blob/%s/nomenklatura/%s#L%s"
+CODE_PATH = DATA_PATH.joinpath("..").resolve()
 
 
-def has_intersection(left: Iterable[str], right: Iterable[str]) -> float:
-    """Returns 1.0 if there is any overlap between the iterables, else 0.0."""
-    if len(set(left).intersection(right)) > 0:
-        return 1.0
-    return 0.0
-
-
-def has_disjoint(left: Set[str], right: Set[str]) -> float:
-    """Returns 1.0 if both sequences are non-empty but have no common values."""
-    if len(left) and len(right):
-        if set(left).isdisjoint(right):
-            return 1.0
-    return 0.0
+def extract_numbers(values: List[str]) -> Set[str]:
+    numbers: Set[str] = set()
+    for value in values:
+        numbers.update(FIND_NUM.findall(value))
+    return numbers
 
 
-def has_overlap(left: Set[str], right: Set[str]) -> float:
-    """Returns 1.0 if both sequences overlap, -1.0 if they're non-empty but disjoint."""
-    if not len(left) or not len(right):
-        return 0.0
-    if set(left).isdisjoint(right):
-        return -1.0
-    return 1.0
+def dates_precision(values: Iterable[str], precision: Precision) -> Set[str]:
+    dates = set()
+    for value in values:
+        if len(value) >= precision.value:
+            dates.add(value[: precision.value])
+    return dates
 
 
-def has_schema(left: Entity, right: Entity, schema: str) -> bool:
+def has_schema(left: E, right: E, schema: str) -> bool:
     """Check if one of the entities has the required schema."""
     if left.schema.is_a(schema) or right.schema.is_a(schema):
         if not left.schema.can_match(right.schema):
             return False
         return True
     return False
 
 
-def extract_numbers(values: List[str]) -> Set[str]:
-    numbers: Set[str] = set()
-    for value in values:
-        numbers.update(FIND_NUM.findall(value))
-    return numbers
-
-
-def compare_levenshtein(left: str, right: str) -> float:
-    distance = Levenshtein.distance(left, right)
-    base = max((1, len(left), len(right)))
-    return 1.0 - (distance / float(base))
-    # return math.sqrt(distance)
-
-
-def props_pair(
-    left: Entity, right: Entity, props: List[str]
-) -> Tuple[Set[str], Set[str]]:
+def props_pair(left: E, right: E, props: List[str]) -> Tuple[Set[str], Set[str]]:
     left_values: Set[str] = set()
     right_values: Set[str] = set()
     for prop in props:
         left_values.update(left.get(prop, quiet=True))
         right_values.update(right.get(prop, quiet=True))
     return left_values, right_values
 
 
-def type_pair(
-    left: Entity, right: Entity, type_: PropertyType
-) -> Tuple[List[str], List[str]]:
-    left_values = left.get_type_values(type_)
-    right_values = right.get_type_values(type_)
+def type_pair(left: E, right: E, type_: PropertyType) -> Tuple[List[str], List[str]]:
+    left_values = left.get_type_values(type_, matchable=True)
+    right_values = right.get_type_values(type_, matchable=True)
     return left_values, right_values
 
 
 def compare_sets(
     left: Iterable[Optional[V]],
     right: Iterable[Optional[V]],
     compare_func: Callable[[V, V], float],
@@ -94,29 +67,12 @@
             continue
         results.append(compare_func(l, r))
     if not len(results):
         return 0.0
     return select_func(results)
 
 
-@lru_cache(maxsize=1000)
-def normalize_text(text: str) -> Optional[str]:
-    return slugify(text, sep=WS)
-
-
-def tokenize(texts: Iterable[str]) -> Set[str]:
-    tokens: Set[str] = set()
-    for text in texts:
-        cleaned = normalize_text(text)
-        if cleaned is None:
-            continue
-        for token in cleaned.split(WS):
-            token = token.strip()
-            if len(token) > 2:
-                tokens.add(token)
-    return tokens
-
-
-def tokenize_pair(
-    pair: Tuple[Iterable[str], Iterable[str]]
-) -> Tuple[Set[str], Set[str]]:
-    return tokenize(pair[0]), tokenize(pair[1])
+def make_github_url(func: Callable[..., Any]) -> str:
+    """Make a URL to the source code of a matching function."""
+    code_path = Path(func.__code__.co_filename).relative_to(CODE_PATH)
+    line_no = func.__code__.co_firstlineno
+    return BASE_URL % (__version__, code_path, line_no)
```

### Comparing `nomenklatura-2.9.5/nomenklatura/matching/pairs.py` & `nomenklatura-3.0.0/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/matching/train.py` & `nomenklatura-3.0.0/nomenklatura/matching/v1/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 from sklearn.model_selection import train_test_split  # type: ignore
 from sklearn.linear_model import LogisticRegression  # type: ignore
 from sklearn import metrics  # type: ignore
 from concurrent.futures import ThreadPoolExecutor
 
 from nomenklatura.judgement import Judgement
 from nomenklatura.matching.pairs import read_pairs, JudgedPair
-from nomenklatura.matching.features import FEATURES, encode_pair
-from nomenklatura.matching.model import explain_matcher, save_matcher, compare_scored
+from nomenklatura.matching.v1.model import MatcherV1
 from nomenklatura.util import PathLike
 
 log = logging.getLogger(__name__)
 
 
 def pair_convert(pair: JudgedPair) -> Tuple[List[float], int]:
     """Encode a pair of training data into features and target."""
     judgement = 1 if pair.judgement == Judgement.POSITIVE else 0
-    features = encode_pair(pair.left, pair.right)
+    features = MatcherV1.encode_pair(pair.left, pair.right)
     return features, judgement
 
 
 def pairs_to_arrays(
     pairs: Iterable[JudgedPair],
 ) -> Tuple[NDArray[np.float32], NDArray[np.float32]]:
     """Parallelize feature computation for training data"""
@@ -67,16 +66,16 @@
     # logreg = LogisticRegression(class_weight={0: 95, 1: 1})
     # logreg = LogisticRegression(penalty="l1", solver="liblinear")
     logreg = LogisticRegression(penalty="l2")
     log.info("Training model...")
     pipe = make_pipeline(StandardScaler(), logreg)
     pipe.fit(X_train, y_train)
     coef = logreg.coef_[0]
-    coefficients = {n.__name__: c for n, c in zip(FEATURES, coef)}
-    save_matcher(pipe, coefficients)
+    coefficients = {n.__name__: c for n, c in zip(MatcherV1.FEATURES, coef)}
+    MatcherV1.save(pipe, coefficients)
     print("Coefficients:")
     pprint(coefficients)
     y_pred = pipe.predict(X_test)
     cnf_matrix = metrics.confusion_matrix(y_test, y_pred)
     print("Confusion matrix:\n", cnf_matrix)
     print("Accuracy:", metrics.accuracy_score(y_test, y_pred))
     print("Precision:", metrics.precision_score(y_test, y_pred))
```

### Comparing `nomenklatura-2.9.5/nomenklatura/publish/dates.py` & `nomenklatura-3.0.0/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/publish/edges.py` & `nomenklatura-3.0.0/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/publish/names.py` & `nomenklatura-3.0.0/nomenklatura/publish/names.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import string
 import logging
-import Levenshtein
 from itertools import combinations
 from collections import defaultdict
-from normality import normalize
 from typing import Dict, Optional, List, Tuple
+from nomenklatura.util import normalize_name, levenshtein
 
 log = logging.getLogger(__name__)
 ASCII = set(string.ascii_letters + string.digits + string.whitespace)
 
 
 def ascii_share(text: str) -> float:
     """Determine the percentage of a string that's in pure ASCII."""
@@ -18,25 +17,22 @@
         return 0.0
     return float(len(asciis)) / float(len(chars))
 
 
 def pick_name(names: List[str]) -> Optional[str]:
     forms: List[Tuple[str, str, float]] = []
     for name in sorted(names):
-        norm = normalize(name, ascii=True, lowercase=False)
+        norm = normalize_name(name)
         if norm is not None:
             weight = 2 - ascii_share(name)
             forms.append((norm, name, weight))
             forms.append((norm.title(), name, weight))
 
     edits: Dict[str, float] = defaultdict(float)
-    cache: Dict[Tuple[str, str], int] = {}
     for ((l_norm, left, l_weight), (r_norm, right, r_weight)) in combinations(forms, 2):
-        pair = (l_norm[:128], r_norm[:128])
-        if pair not in cache:
-            cache[pair] = Levenshtein.distance(*pair)
-        edits[left] += cache[pair] * l_weight
-        edits[right] += cache[pair] * r_weight
+        distance = levenshtein(l_norm, r_norm)
+        edits[left] += distance * l_weight
+        edits[right] += distance * r_weight
 
     for cand, _ in sorted(edits.items(), key=lambda x: x[1]):
         return cand
     return None
```

### Comparing `nomenklatura-2.9.5/nomenklatura/resolver/edge.py` & `nomenklatura-3.0.0/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/resolver/identifier.py` & `nomenklatura-3.0.0/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/resolver/resolver.py` & `nomenklatura-3.0.0/nomenklatura/resolver/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         for edge in self.nodes.get(node, []):
             if edge.judgement == Judgement.POSITIVE:
                 other = edge.other(node)
                 rec = self._traverse(other, seen)
                 connected.update(rec)
         return connected
 
-    @lru_cache(maxsize=500000)
+    @lru_cache(maxsize=200000)
     def connected(self, node: Identifier) -> Set[Identifier]:
         return self._traverse(node, set())
 
     def get_canonical(self, entity_id: StrIdent) -> str:
         """Return the canonical identifier for the given entity ID."""
         node = Identifier.get(entity_id)
         best = max(self.connected(node))
```

### Comparing `nomenklatura-2.9.5/nomenklatura/senzing.py` & `nomenklatura-3.0.0/nomenklatura/senzing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This format can then be used to perform record linkage against other datasets.
 # As a next step, the matching results could be converted back into a
 # nomenklatura resolver file and then used to generate integrated FtM entities.
 import logging
 from typing import Dict, Generator, List, Optional, TypedDict, Union
 from followthemoney.types import registry
 
-from nomenklatura.loader import Loader
+from nomenklatura.store import View
 from nomenklatura.dataset import DS
 from nomenklatura.entity import CE
 from nomenklatura.util import is_qid
 
 log = logging.getLogger(__name__)
 
 Feature = Union[str, Dict[str, str]]
@@ -27,17 +27,17 @@
 
 def map_feature(entity: CE, features: List[Feature], prop: str, attr: str) -> None:
     for value in entity.get(prop, quiet=True):
         features.append({attr: value})
 
 
 def senzing_adjacent_features(
-    entity: CE, loader: Loader[DS, CE]
+    entity: CE, view: View[DS, CE]
 ) -> Generator[Feature, None, None]:
-    for _, adj in loader.get_adjacent(entity):
+    for _, adj in view.get_adjacent(entity):
         adj_data: Optional[Dict[str, Optional[str]]] = None
         if adj.schema.name == "Address":
             adj_data = {
                 "ADDR_FULL": adj.first("full"),
                 "ADDR_LINE1": adj.first("street"),
                 "ADDR_LINE2": adj.first("street2"),
                 "ADDR_CITY": adj.first("city"),
@@ -58,15 +58,15 @@
         if adj_data is not None:
             values = {k: v for k, v in adj_data.items() if v is not None}
             if len(values):
                 yield values
 
 
 def senzing_record(
-    data_source: str, entity: CE, loader: Optional[Loader[DS, CE]] = None
+    data_source: str, entity: CE, view: Optional[View[DS, CE]] = None
 ) -> Optional[SenzingRecord]:
     if not entity.schema.matchable or entity.schema.name == "Address":
         return None
     if entity.id is None:
         return None
     record: SenzingRecord = {
         "DATA_SOURCE": data_source,
@@ -105,16 +105,16 @@
     map_feature(entity, features, "ogrnCode", "NATIONAL_ID_NUMBER")
     map_feature(entity, features, "taxNumber", "TAX_ID_NUMBER")
     map_feature(entity, features, "innCode", "TAX_ID_NUMBER")
     map_feature(entity, features, "vatCode", "TAX_ID_NUMBER")
     map_feature(entity, features, "leiCode", "LEI_NUMBER")
     map_feature(entity, features, "dunsCode", "DUNS_NUMBER")
 
-    if loader is not None:
-        for adj_feature in senzing_adjacent_features(entity, loader):
+    if view is not None:
+        for adj_feature in senzing_adjacent_features(entity, view):
             features.append(adj_feature)
 
     for wd_id in (entity.id, entity.first("wikidataId")):
         if wd_id is not None and is_qid(wd_id):
             features.append(
                 {
                     "TRUSTED_ID_TYPE": "WIKIDATA",
```

### Comparing `nomenklatura-2.9.5/nomenklatura/statement/serialize.py` & `nomenklatura-3.0.0/nomenklatura/statement/serialize.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import csv
 import click
 import orjson
 from pathlib import Path
 from io import TextIOWrapper
-from typing import BinaryIO, Generator, Iterable, Type
+from typing import BinaryIO, Generator, Iterable, Type, Dict, Any
 from followthemoney.cli.util import MAX_LINE
 
 from nomenklatura.statement.statement import S
+from nomenklatura.util import pack_prop, unpack_prop, bool_text
 
 JSON = "json"
 CSV = "csv"
-FORMATS = [JSON, CSV]
+PACK = "pack"
+FORMATS = [JSON, CSV, PACK]
 
 CSV_COLUMNS = [
     "canonical_id",
     "entity_id",
     "prop",
     "prop_type",
     "schema",
@@ -25,14 +27,28 @@
     "target",
     "external",
     "first_seen",
     "last_seen",
     "id",
 ]
 
+PACK_COLUMNS = [
+    "entity_id",
+    "prop",
+    "value",
+    "dataset",
+    "lang",
+    "original_value",
+    "target",
+    "external",
+    "first_seen",
+    "last_seen",
+    "id",
+]
+
 
 def read_json_statements(
     fh: BinaryIO,
     statement_type: Type[S],
     max_line: int = MAX_LINE,
 ) -> Generator[S, None, None]:
     while line := fh.readline(max_line):
@@ -44,19 +60,34 @@
     fh: BinaryIO, statement_type: Type[S]
 ) -> Generator[S, None, None]:
     wrapped = TextIOWrapper(fh, encoding="utf-8")
     for row in csv.DictReader(wrapped, dialect=csv.unix_dialect):
         yield statement_type.from_row(row)
 
 
+def read_pack_statements(
+    fh: BinaryIO, statement_type: Type[S]
+) -> Generator[S, None, None]:
+    wrapped = TextIOWrapper(fh, encoding="utf-8")
+    for row in csv.DictReader(wrapped, dialect=csv.unix_dialect):
+        row["canonical_id"] = row["entity_id"]
+        schema, prop_type, prop = unpack_prop(row["prop"])
+        row["schema"] = schema
+        row["prop"] = prop
+        row["prop_type"] = prop_type
+        yield statement_type.from_row(row)
+
+
 def read_statements(
     fh: BinaryIO, format: str, statement_type: Type[S]
 ) -> Generator[S, None, None]:
     if format == CSV:
         yield from read_csv_statements(fh, statement_type)
+    elif format == PACK:
+        yield from read_pack_statements(fh, statement_type)
     else:
         yield from read_json_statements(fh, statement_type)
 
 
 def read_path_statements(
     path: Path, format: str, statement_type: Type[S]
 ) -> Generator[S, None, None]:
@@ -84,12 +115,39 @@
         writer = csv.writer(wrapped, dialect=csv.unix_dialect)
         writer.writerow(CSV_COLUMNS)
         for stmt in statements:
             row = stmt.to_row()
             writer.writerow([row.get(c) for c in CSV_COLUMNS])
 
 
+def pack_statement(stmt: S) -> Dict[str, Any]:
+    row = stmt.to_row()
+    row.pop("canonical_id", None)
+    row.pop("prop_type", None)
+    prop = row.pop("prop")
+    schema = row.pop("schema")
+    if prop is None or schema is None:
+        raise ValueError("Cannot pack statement without prop and schema")
+    row["prop"] = pack_prop(prop, schema)
+    return row
+
+
+def write_pack_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
+    with TextIOWrapper(fh, encoding="utf-8") as wrapped:
+        writer = csv.writer(
+            wrapped,
+            dialect=csv.unix_dialect,
+            quoting=csv.QUOTE_MINIMAL,
+        )
+        writer.writerow(PACK_COLUMNS)
+        for stmt in statements:
+            row = pack_statement(stmt)
+            writer.writerow([row.get(c) for c in PACK_COLUMNS])
+
+
 def write_statements(fh: BinaryIO, format: str, statements: Iterable[S]) -> None:
     if format == CSV:
         write_csv_statements(fh, statements)
+    elif format == PACK:
+        write_pack_statements(fh, statements)
     else:
         write_json_statements(fh, statements)
```

### Comparing `nomenklatura-2.9.5/nomenklatura/statement/statement.py` & `nomenklatura-3.0.0/nomenklatura/statement/statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import hashlib
-from datetime import datetime
 from sqlalchemy.engine import Row
 from typing import cast, TYPE_CHECKING
 from typing import Any, Dict, Generator, Optional, Type, TypeVar, TypedDict
 
-from nomenklatura.util import (
-    bool_text,
-    datetime_iso,
-    iso_datetime,
-    text_bool,
-)
+from nomenklatura.util import bool_text, datetime_iso, text_bool, BASE_ID
 
 if TYPE_CHECKING:
     from nomenklatura.entity import CE
 
 S = TypeVar("S", bound="Statement")
 
 
@@ -26,30 +20,30 @@
     schema: str
     value: str
     dataset: str
     lang: Optional[str]
     original_value: Optional[str]
     target: Optional[bool]
     external: Optional[bool]
-    first_seen: Optional[datetime]
-    last_seen: Optional[datetime]
+    first_seen: Optional[str]
+    last_seen: Optional[str]
 
 
 class Statement(object):
     """A single statement about a property relevant to an entity.
 
     For example, this could be useddocker to say: "In dataset A, entity X has the
     property `name` set to 'John Smith'. I first observed this at K, and last
     saw it at L."
 
     Null property values are not supported. This might need to change if we
     want to support making property-less entities.
     """
 
-    BASE = "id"
+    BASE = BASE_ID
 
     __slots__ = [
         "id",
         "entity_id",
         "canonical_id",
         "prop",
         "prop_type",
@@ -70,20 +64,20 @@
         prop: str,
         prop_type: str,
         schema: str,
         value: str,
         dataset: str,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
-        first_seen: Optional[datetime] = None,
+        first_seen: Optional[str] = None,
         target: Optional[bool] = False,
         external: Optional[bool] = False,
         id: Optional[str] = None,
         canonical_id: Optional[str] = None,
-        last_seen: Optional[datetime] = None,
+        last_seen: Optional[str] = None,
     ):
         self.entity_id = entity_id
         self.canonical_id = canonical_id or entity_id
         self.prop = prop
         self.prop_type = prop_type
         self.schema = schema
         self.value = value
@@ -118,32 +112,32 @@
             "id": self.id,
         }
 
     def to_row(self) -> Dict[str, Optional[str]]:
         data = cast(Dict[str, str], self.to_dict())
         return {
             **data,
-            "first_seen": datetime_iso(self.first_seen),
-            "last_seen": datetime_iso(self.last_seen),
+            "first_seen": self.first_seen,
+            "last_seen": self.last_seen,
             "target": bool_text(self.target),
             "external": bool_text(self.external),
         }
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __repr__(self) -> str:
         return "<Statement(%r, %r, %r)>" % (self.entity_id, self.prop, self.value)
 
     def __eq__(self, other: Any) -> bool:
         return not self.id != other.id
 
     def __lt__(self, other: Any) -> bool:
-        self_key = (self.prop != self.BASE, self.id or "")
-        other_key = (other.prop != self.BASE, other.id or "")
+        self_key = (self.prop != BASE_ID, self.id or "")
+        other_key = (other.prop != BASE_ID, other.id or "")
         return self_key < other_key
 
     def clone(self: S) -> S:
         """Make a deep copy of the given statement."""
         return type(self).from_dict(self.to_dict())
 
     def generate_key(self) -> Optional[str]:
@@ -192,65 +186,53 @@
             id=data.get("id", None),
             canonical_id=data.get("canonical_id", None),
             last_seen=data.get("last_seen", None),
         )
 
     @classmethod
     def from_row(cls: Type[S], data: Dict[str, str]) -> S:
-        return cls(
-            id=data.get("id", None),
-            canonical_id=data.get("canonical_id", None),
-            entity_id=data["entity_id"],
-            prop=data["prop"],
-            prop_type=data["prop_type"],
-            schema=data["schema"],
-            value=data["value"],
-            dataset=data["dataset"],
-            lang=data.get("lang", None),
-            original_value=data.get("original_value", None),
-            first_seen=iso_datetime(data.get("first_seen", None)),
-            target=text_bool(data.get("target")),
-            external=text_bool(data.get("external")),
-            last_seen=iso_datetime(data.get("last_seen", None)),
-        )
+        typed_data = cast(StatementDict, data)
+        typed_data["target"] = text_bool(data.get("target"))
+        typed_data["external"] = text_bool(data.get("external"))
+        return cls.from_dict(typed_data)
 
     @classmethod
     def from_db_row(cls: Type[S], row: Row) -> S:
         return cls(
             id=row.id,
             canonical_id=row.canonical_id,
             entity_id=row.entity_id,
             prop=row.prop,
             prop_type=row.prop_type,
             schema=row.schema,
             value=row.value,
             dataset=row.dataset,
             lang=row.lang,
             original_value=row.original_value,
-            first_seen=row.first_seen,
+            first_seen=datetime_iso(row.first_seen),
             target=row.target,
             external=row.external,
-            last_seen=row.last_seen,
+            last_seen=datetime_iso(row.last_seen),
         )
 
     @classmethod
     def from_entity(
         cls: Type[S],
         entity: "CE",
         dataset: str,
-        first_seen: Optional[datetime] = None,
-        last_seen: Optional[datetime] = None,
+        first_seen: Optional[str] = None,
+        last_seen: Optional[str] = None,
         target: Optional[bool] = None,
         external: Optional[bool] = None,
     ) -> Generator[S, None, None]:
         if entity.id is not None:
             yield cls(
                 entity_id=entity.id,
-                prop=cls.BASE,
-                prop_type=cls.BASE,
+                prop=BASE_ID,
+                prop_type=BASE_ID,
                 schema=entity.schema.name,
                 value=entity.id,
                 dataset=dataset,
                 target=target,
                 external=external,
                 first_seen=first_seen,
                 last_seen=last_seen,
```

### Comparing `nomenklatura-2.9.5/nomenklatura/tui/app.py` & `nomenklatura-3.0.0/nomenklatura/tui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 from rich.text import Text
 from rich.console import RenderableType
 from textual.app import App, ComposeResult
 from textual.widget import Widget
 from textual.widgets import Footer
 
 from nomenklatura.judgement import Judgement
-from nomenklatura.loader import Loader
-from nomenklatura.resolver import Resolver
+from nomenklatura.store import Store
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.tui.comparison import render_comparison
 
 
 class DedupeState(object):
     def __init__(
         self,
-        resolver: Resolver[CE],
-        loader: Loader[DS, CE],
+        store: Store[DS, CE],
         url_base: Optional[str] = None,
     ):
-        self.resolver = resolver
-        self.loader = loader
+        self.store = store
+        self.resolver = store.resolver
+        self.view = store.default_view(external=True)
         self.url_base = url_base
         self.latinize = False
         self.message: Optional[str] = None
         self.ignore: Set[Tuple[str, str]] = set()
         self.left: Optional[CE] = None
         self.right: Optional[CE] = None
         self.score = 0.0
@@ -39,29 +38,34 @@
                 continue
             if score is None:
                 self.ignore.add((left_id, right_id))
                 continue
             if not self.resolver.check_candidate(left_id, right_id):
                 self.ignore.add((left_id, right_id))
                 continue
-            self.left = self.loader.get_entity(left_id)
-            self.right = self.loader.get_entity(right_id)
+            self.left = self.view.get_entity(left_id)
+            self.right = self.view.get_entity(right_id)
             self.score = score
             if self.left is not None and self.right is not None:
                 if self.left.schema == self.right.schema:
                     return True
                 if self.left.schema.can_match(self.right.schema):
                     return True
             self.ignore.add((left_id, right_id))
         return False
 
     def decide(self, judgement: Judgement) -> None:
         if self.left is not None and self.left.id is not None:
             if self.right is not None and self.right.id is not None:
-                self.resolver.decide(self.left.id, self.right.id, judgement=judgement)
+                canonical_id = self.resolver.decide(
+                    self.left.id,
+                    self.right.id,
+                    judgement=judgement,
+                )
+                self.store.update(canonical_id)
         self.load()
 
     def save(self) -> None:
         self.resolver.save()
 
 
 class DedupeWidget(Widget):
@@ -73,15 +77,15 @@
         return cast(DedupeApp, self.app).dedupe
 
     def render(self) -> RenderableType:
         if self.dedupe.message is not None:
             return Text(self.dedupe.message, justify="center")
         if self.dedupe.left and self.dedupe.right:
             return render_comparison(
-                self.dedupe.loader,
+                self.dedupe.view,
                 self.dedupe.left,
                 self.dedupe.right,
                 self.dedupe.score,
                 latinize=self.dedupe.latinize,
                 url_base=self.dedupe.url_base,
             )
         return Text("No candidates.", justify="center")
```

### Comparing `nomenklatura-2.9.5/nomenklatura/tui/comparison.py` & `nomenklatura-3.0.0/nomenklatura/tui/comparison.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from rich.table import Table
 from rich.text import Text
 from followthemoney.types import registry
 from followthemoney.property import Property
 
 from nomenklatura.dataset import DS
 from nomenklatura.entity import CE
-from nomenklatura.loader import Loader
+from nomenklatura.store import View
 from nomenklatura.tui.util import comparison_props
 
 
 def render_column(entity: CE) -> Text:
     return Text.assemble(
         (entity.schema.label, "blue"), " [%s]" % entity.id, no_wrap=True
     )
 
 
 def render_values(
-    loader: Loader[DS, CE], prop: Property, entity: CE, other: CE, latinize: bool
+    view: View[DS, CE], prop: Property, entity: CE, other: CE, latinize: bool
 ) -> Text:
     values = entity.get(prop, quiet=True)
     other_values = other.get_type_values(prop.type)
     text = Text()
     for i, value in enumerate(sorted(values)):
         caption = prop.type.caption(value)
         if prop.type == registry.entity:
-            sub = loader.get_entity(value)
+            sub = view.get_entity(value)
             if sub is not None:
                 caption = sub.caption
         score = prop.type.compare_sets([value], other_values)
         if latinize:
             caption = latinize_text(caption) or caption
         if prop.name == "wikidataId":
             caption = f"https://wikidata.org/wiki/{value}"
@@ -43,15 +43,15 @@
             if i > 0:
                 text.append(" · ", "gray")
             text.append(caption, style)
     return text
 
 
 def render_comparison(
-    loader: Loader[DS, CE],
+    view: View[DS, CE],
     left: CE,
     right: CE,
     score: float,
     latinize: bool = False,
     url_base: Optional[str] = None,
 ) -> Table:
     if left is None or right is None:
@@ -61,16 +61,16 @@
     score_text = "Score: %.3f" % score
     table.add_column(score_text, justify="right", no_wrap=True, ratio=2)
     table.add_column(render_column(left), ratio=5)
     table.add_column(render_column(right), ratio=5)
 
     for prop in comparison_props(left, right):
         label = Text(prop.label, "white bold")
-        left_text = render_values(loader, prop, left, right, latinize)
-        right_text = render_values(loader, prop, right, left, latinize)
+        left_text = render_values(view, prop, left, right, latinize)
+        right_text = render_values(view, prop, right, left, latinize)
         table.add_row(label, left_text, right_text)
 
     ds_label = Text("Sources", "grey bold")
     ds_left = Text(", ".join(left.datasets))
     ds_right = Text(", ".join(right.datasets))
     table.add_row(ds_label, ds_left, ds_right)
```

### Comparing `nomenklatura-2.9.5/nomenklatura/tui/util.py` & `nomenklatura-3.0.0/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.5/nomenklatura/xref.py` & `nomenklatura-3.0.0/nomenklatura/xref.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
-from typing import List, Optional
+from typing import List, Optional, Type
 from followthemoney.schema import Schema
 
 from nomenklatura.dataset import DS
 from nomenklatura.entity import CE
-from nomenklatura.loader import Loader
-from nomenklatura.resolver import Resolver
+from nomenklatura.store import Store
 from nomenklatura.judgement import Judgement
 from nomenklatura.index import Index
-from nomenklatura.matching import compare_scored
-from nomenklatura.util import is_qid
+from nomenklatura.matching import DefaultAlgorithm, ScoringAlgorithm
 
 log = logging.getLogger(__name__)
 
 
 def _print_stats(pairs: int, suggested: int, scores: List[float]) -> None:
     matches = len(scores)
     log.info(
@@ -23,83 +21,74 @@
         sum(scores) / max(1, matches),
         min(scores, default=0.0),
         max(scores, default=0.0),
     )
 
 
 def xref(
-    loader: Loader[DS, CE],
-    resolver: Resolver[CE],
+    store: Store[DS, CE],
     limit: int = 5000,
     scored: bool = True,
-    adjacent: bool = False,
+    external: bool = True,
     range: Optional[Schema] = None,
     auto_threshold: Optional[float] = None,
     focus_dataset: Optional[str] = None,
+    algorithm: Type[ScoringAlgorithm] = DefaultAlgorithm,
     user: Optional[str] = None,
 ) -> None:
-    log.info("Begin xref: %r, resolver: %s", loader, resolver)
-    index = Index(loader)
-    index.build(adjacent=adjacent)
+    log.info("Begin xref: %r, resolver: %s", store, store.resolver)
+    view = store.default_view(external=external)
+    index = Index(view)
+    index.build()
     try:
         scores: List[float] = []
         suggested = 0
         idx = 0
         for idx, ((left_id, right_id), score) in enumerate(index.pairs()):
             if idx % 1000 == 0 and idx > 0:
                 _print_stats(idx, suggested, scores)
 
-            if not resolver.check_candidate(left_id, right_id):
+            if not store.resolver.check_candidate(left_id, right_id):
                 continue
 
-            if is_qid(left_id.id) and is_qid(right_id.id):
-                continue
-
-            left = loader.get_entity(left_id.id)
-            right = loader.get_entity(right_id.id)
+            left = view.get_entity(left_id.id)
+            right = view.get_entity(right_id.id)
             if left is None or left.id is None or right is None or right.id is None:
                 continue
 
             if not left.schema.can_match(right.schema):
                 continue
 
             if range is not None:
                 if not left.schema.is_a(range) and not right.schema.is_a(range):
                     continue
 
             if scored:
-                result = compare_scored(left, right)
+                result = algorithm.compare(left, right)
                 score = result["score"]
             scores.append(score)
 
-            # if score > 0.985:
-            #     if is_qid(left.id) and right.id.startswith("acf-"):
-            #         print("LEFT", left, right)
-            #         resolver.decide(left_id, right_id, Judgement.POSITIVE)
-            #         continue
-            #     if is_qid(right.id) and left.id.startswith("acf-"):
-            #         print("RIGHT", left, right)
-            #         resolver.decide(left_id, right_id, Judgement.POSITIVE)
-            #         continue
-
             # Not sure this is globally a good idea.
             if len(left.datasets.intersection(right.datasets)) > 0:
                 score = score * 0.7
 
             if auto_threshold is not None and score > auto_threshold:
                 log.info("Auto-merge [%.2f]: %s <> %s", score, left, right)
-                resolver.decide(left_id, right_id, Judgement.POSITIVE, user=user)
+                canonical_id = store.resolver.decide(
+                    left_id, right_id, Judgement.POSITIVE, user=user
+                )
+                store.update(canonical_id)
                 continue
 
             if focus_dataset in left.datasets and focus_dataset not in right.datasets:
                 score = (score + 1.0) / 2.0
             if focus_dataset not in left.datasets and focus_dataset in right.datasets:
                 score = (score + 1.0) / 2.0
 
-            resolver.suggest(left.id, right.id, score, user=user)
-            if suggested > limit:
+            store.resolver.suggest(left.id, right.id, score, user=user)
+            if suggested >= limit:
                 break
             suggested += 1
         _print_stats(idx, suggested, scores)
 
     except KeyboardInterrupt:
         log.info("User cancelled, xref will end gracefully.")
```

### Comparing `nomenklatura-2.9.5/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.0.0/nomenklatura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.5
+Version: 3.0.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
 
 ![screenshot](./docs/screenshot.png)
@@ -47,15 +47,15 @@
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
-* `nomenklatura.Loader` - a general purpose access mechanism for entities. By default, a `nomenklatura.FileLoader` is used to access entity data stored in files, but the loader can be subclassed to work with entities from a database system.
+* `nomenklatura.Store` - a general purpose access mechanism for entities. By default, a store is used to access entity data stored in files as an in-memory cache, but the store can be subclassed to work with entities from a database system.
 * `nomenklatura.Index` - a full-text in-memory search index for FtM entities. In the application, this is used to block de-duplication candidates, but the index can also be used to drive an API etc.
 * `nomenklatura.Resolver` - the core of the de-duplication process, the resolver is essentially a graph with edges made out of entity judgements. The resolver can be used to store judgements or get the canonical ID for a given entity.
 
 All of the API classes have extensive type annotations, which should make their integration in any modern Python API simpler.
 
 ## Design
 
@@ -91,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-2.9.5/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.0.0/nomenklatura.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 nomenklatura/__init__.py
 nomenklatura/cache.py
 nomenklatura/cli.py
 nomenklatura/db.py
 nomenklatura/entity.py
 nomenklatura/exceptions.py
 nomenklatura/judgement.py
-nomenklatura/loader.py
 nomenklatura/py.typed
 nomenklatura/senzing.py
 nomenklatura/util.py
 nomenklatura/xref.py
 nomenklatura.egg-info/PKG-INFO
 nomenklatura.egg-info/SOURCES.txt
 nomenklatura.egg-info/dependency_links.txt
 nomenklatura.egg-info/entry_points.txt
 nomenklatura.egg-info/namespace_packages.txt
 nomenklatura.egg-info/not-zip-safe
 nomenklatura.egg-info/requires.txt
 nomenklatura.egg-info/top_level.txt
-nomenklatura/data/match-regression.pkl
+nomenklatura/data/regression-v1.pkl
+nomenklatura/data/regression-v2.pkl
 nomenklatura/dataset/__init__.py
 nomenklatura/dataset/catalog.py
 nomenklatura/dataset/coverage.py
 nomenklatura/dataset/dataset.py
 nomenklatura/dataset/publisher.py
 nomenklatura/dataset/resource.py
 nomenklatura/dataset/util.py
@@ -43,32 +43,47 @@
 nomenklatura/enrich/wikidata/qualified.py
 nomenklatura/enrich/wikidata/value.py
 nomenklatura/index/__init__.py
 nomenklatura/index/entry.py
 nomenklatura/index/index.py
 nomenklatura/index/tokenizer.py
 nomenklatura/matching/__init__.py
-nomenklatura/matching/model.py
 nomenklatura/matching/pairs.py
-nomenklatura/matching/train.py
 nomenklatura/matching/types.py
-nomenklatura/matching/features/__init__.py
-nomenklatura/matching/features/dates.py
-nomenklatura/matching/features/misc.py
-nomenklatura/matching/features/names.py
-nomenklatura/matching/features/util.py
+nomenklatura/matching/util.py
+nomenklatura/matching/heuristic/__init__.py
+nomenklatura/matching/heuristic/logic.py
+nomenklatura/matching/v1/__init__.py
+nomenklatura/matching/v1/dates.py
+nomenklatura/matching/v1/misc.py
+nomenklatura/matching/v1/model.py
+nomenklatura/matching/v1/names.py
+nomenklatura/matching/v1/train.py
+nomenklatura/matching/v1/util.py
+nomenklatura/matching/v2/__init__.py
+nomenklatura/matching/v2/dates.py
+nomenklatura/matching/v2/misc.py
+nomenklatura/matching/v2/model.py
+nomenklatura/matching/v2/names.py
+nomenklatura/matching/v2/train.py
+nomenklatura/matching/v2/util.py
 nomenklatura/publish/__init__.py
 nomenklatura/publish/dates.py
 nomenklatura/publish/edges.py
 nomenklatura/publish/names.py
 nomenklatura/resolver/__init__.py
 nomenklatura/resolver/common.py
 nomenklatura/resolver/edge.py
 nomenklatura/resolver/identifier.py
 nomenklatura/resolver/resolver.py
 nomenklatura/statement/__init__.py
 nomenklatura/statement/serialize.py
 nomenklatura/statement/statement.py
+nomenklatura/store/__init__.py
+nomenklatura/store/base.py
+nomenklatura/store/level.py
+nomenklatura/store/memory.py
+nomenklatura/store/util.py
 nomenklatura/tui/__init__.py
 nomenklatura/tui/app.py
 nomenklatura/tui/comparison.py
 nomenklatura/tui/util.py
```

### Comparing `nomenklatura-2.9.5/setup.py` & `nomenklatura-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="2.9.5",
+    version="3.0.0",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
@@ -19,16 +19,17 @@
     namespace_packages=[],
     include_package_data=True,
     package_data={"": ["nomenklatura/data/*", "nomenklatura/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.3.0, < 4.0.0",
         "shortuuid >= 1.0.11, < 2.0.0",
+        "jellyfish == 1.0.0",
         "rich >= 10.9.0, < 14.0.0",
-        "textual >= 0.19.0, < 0.21.0",
+        "textual >= 0.19.0, < 0.29.0",
         "scikit-learn == 1.2.2",
         "click >= 8.0.0, < 9.0.0",
     ],
     tests_require=[],
     entry_points={
         "console_scripts": [
             "nk = nomenklatura.cli:cli",
@@ -42,10 +43,12 @@
             "mypy",
             "flake8>=2.6.0",
             "pytest",
             "pytest-cov",
             "coverage>=4.1",
             "types-setuptools",
             "types-requests",
-        ]
+            "plyvel",
+        ],
+        "leveldb": ["plyvel"],
     },
 )
```

