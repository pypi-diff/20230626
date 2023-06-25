# Comparing `tmp/amid-0.9.0.tar.gz` & `tmp/amid-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amid-0.9.0.tar", last modified: Sat Feb 25 09:44:44 2023, max compression
+gzip compressed data, was "amid-0.9.1.tar", last modified: Sun Apr  9 20:28:33 2023, max compression
```

## Comparing `amid-0.9.0.tar` & `amid-0.9.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-25 09:44:42.000000 amid-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-25 09:44:42.000000 amid-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-02-25 09:44:44.806084 amid-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-02-25 09:44:42.000000 amid-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.802084 amid-0.9.0/amid/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-25 09:44:42.000000 amid-0.9.0/amid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 09:44:42.000000 amid-0.9.0/amid/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.802084 amid-0.9.0/amid/amos/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-25 09:44:42.000000 amid-0.9.0/amid/amos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-25 09:44:42.000000 amid-0.9.0/amid/amos/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-25 09:44:42.000000 amid-0.9.0/amid/amos/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-25 09:44:42.000000 amid-0.9.0/amid/amos/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-02-25 09:44:42.000000 amid-0.9.0/amid/bimcv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.802084 amid-0.9.0/amid/cancer_500/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cancer_500/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cancer_500/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cancer_500/nodules.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cancer_500/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.802084 amid-0.9.0/amid/cc359/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cc359/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cc359/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-25 09:44:42.000000 amid-0.9.0/amid/cc359/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-02-25 09:44:42.000000 amid-0.9.0/amid/covid_1110.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-02-25 09:44:42.000000 amid-0.9.0/amid/crossmoda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-02-25 09:44:42.000000 amid-0.9.0/amid/ct_ich.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/data/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/.bev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/amos.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/bimcv_covid19.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/cancer_500.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/cc359.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/covid_1110.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/crossmoda2022.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/ct_ich.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/egd.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/flare2022.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/lidc.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/lits.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/liver_medseg.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/medseg9.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/midrc.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/mood.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/nlst.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/nsclc.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/rsna-breast-cancer.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/stanford_coca.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/totalsegmentator.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/verse.hash
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 09:44:42.000000 amid-0.9.0/amid/data/vs_seg.hash
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-02-25 09:44:42.000000 amid-0.9.0/amid/egd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-02-25 09:44:42.000000 amid-0.9.0/amid/flare2022.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-02-25 09:44:42.000000 amid-0.9.0/amid/internals/yandex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/lidc/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lidc/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lidc/nodules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lidc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lidc/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/lits/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lits/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-25 09:44:42.000000 amid-0.9.0/amid/lits/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-25 09:44:42.000000 amid-0.9.0/amid/liver_medseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-02-25 09:44:42.000000 amid-0.9.0/amid/medseg9.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-02-25 09:44:42.000000 amid-0.9.0/amid/midrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-02-25 09:44:42.000000 amid-0.9.0/amid/mood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-25 09:44:42.000000 amid-0.9.0/amid/nlst.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-02-25 09:44:42.000000 amid-0.9.0/amid/nsclc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/rsna_bc/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 09:44:42.000000 amid-0.9.0/amid/rsna_bc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-25 09:44:42.000000 amid-0.9.0/amid/rsna_bc/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-25 09:44:42.000000 amid-0.9.0/amid/rsna_bc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-02-25 09:44:42.000000 amid-0.9.0/amid/stanford_coca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/totalsegmentator/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 09:44:42.000000 amid-0.9.0/amid/totalsegmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-25 09:44:42.000000 amid-0.9.0/amid/totalsegmentator/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-02-25 09:44:42.000000 amid-0.9.0/amid/totalsegmentator/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-25 09:44:42.000000 amid-0.9.0/amid/totalsegmentator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-25 09:44:42.000000 amid-0.9.0/amid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-02-25 09:44:42.000000 amid-0.9.0/amid/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-02-25 09:44:42.000000 amid-0.9.0/amid/verse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.806084 amid-0.9.0/amid/vs_seg/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-25 09:44:42.000000 amid-0.9.0/amid/vs_seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-02-25 09:44:42.000000 amid-0.9.0/amid/vs_seg/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-25 09:44:42.000000 amid-0.9.0/amid/vs_seg/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:44:44.802084 amid-0.9.0/amid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-25 09:44:44.000000 amid-0.9.0/amid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-02-25 09:44:42.000000 amid-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-25 09:44:42.000000 amid-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 09:44:44.806084 amid-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-02-25 09:44:42.000000 amid-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-09 20:28:31.000000 amid-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 20:28:31.000000 amid-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-09 20:28:33.734574 amid-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-09 20:28:31.000000 amid-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.730574 amid-0.9.1/amid/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 20:28:31.000000 amid-0.9.1/amid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 20:28:31.000000 amid-0.9.1/amid/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.730574 amid-0.9.1/amid/amos/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 20:28:31.000000 amid-0.9.1/amid/amos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-09 20:28:31.000000 amid-0.9.1/amid/amos/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-09 20:28:31.000000 amid-0.9.1/amid/amos/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-09 20:28:31.000000 amid-0.9.1/amid/amos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-04-09 20:28:31.000000 amid-0.9.1/amid/bimcv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.730574 amid-0.9.1/amid/cancer_500/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cancer_500/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cancer_500/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cancer_500/nodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cancer_500/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.730574 amid-0.9.1/amid/cc359/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cc359/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cc359/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-09 20:28:31.000000 amid-0.9.1/amid/cc359/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-09 20:28:31.000000 amid-0.9.1/amid/covid_1110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-09 20:28:31.000000 amid-0.9.1/amid/crossmoda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-09 20:28:31.000000 amid-0.9.1/amid/ct_ich.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/.bev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/amos.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/bimcv_covid19.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/cancer_500.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/cc359.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/covid_1110.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/crossmoda2022.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/ct_ich.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/egd.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/flare2022.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/lidc.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/lits.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/liver_medseg.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/medseg9.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/midrc.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/mood.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/nlst.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/nsclc.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/rsna-breast-cancer.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/stanford_coca.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/totalsegmentator.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/verse.hash
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 20:28:31.000000 amid-0.9.1/amid/data/vs_seg.hash
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-09 20:28:31.000000 amid-0.9.1/amid/egd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-09 20:28:31.000000 amid-0.9.1/amid/flare2022.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-09 20:28:31.000000 amid-0.9.1/amid/internals/yandex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/lidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lidc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lidc/nodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lidc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lidc/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/lits/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lits/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 20:28:31.000000 amid-0.9.1/amid/lits/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-09 20:28:31.000000 amid-0.9.1/amid/liver_medseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-09 20:28:31.000000 amid-0.9.1/amid/medseg9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-09 20:28:31.000000 amid-0.9.1/amid/midrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-09 20:28:31.000000 amid-0.9.1/amid/mood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-09 20:28:31.000000 amid-0.9.1/amid/nlst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-09 20:28:31.000000 amid-0.9.1/amid/nsclc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/rsna_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:28:31.000000 amid-0.9.1/amid/rsna_bc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-09 20:28:31.000000 amid-0.9.1/amid/rsna_bc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-09 20:28:31.000000 amid-0.9.1/amid/rsna_bc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-04-09 20:28:31.000000 amid-0.9.1/amid/stanford_coca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/totalsegmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:28:31.000000 amid-0.9.1/amid/totalsegmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-09 20:28:31.000000 amid-0.9.1/amid/totalsegmentator/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-09 20:28:31.000000 amid-0.9.1/amid/totalsegmentator/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-09 20:28:31.000000 amid-0.9.1/amid/totalsegmentator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-09 20:28:31.000000 amid-0.9.1/amid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-09 20:28:31.000000 amid-0.9.1/amid/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-09 20:28:31.000000 amid-0.9.1/amid/verse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.734574 amid-0.9.1/amid/vs_seg/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 20:28:31.000000 amid-0.9.1/amid/vs_seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-04-09 20:28:31.000000 amid-0.9.1/amid/vs_seg/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-09 20:28:31.000000 amid-0.9.1/amid/vs_seg/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:28:33.730574 amid-0.9.1/amid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 20:28:33.000000 amid-0.9.1/amid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-09 20:28:31.000000 amid-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-09 20:28:31.000000 amid-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:28:33.734574 amid-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-09 20:28:31.000000 amid-0.9.1/setup.py
```

### Comparing `amid-0.9.0/LICENSE` & `amid-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/PKG-INFO` & `amid-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: amid
-Version: 0.9.0
+Version: 0.9.1
 Summary: A curated list of medical imaging datasets with unified interfaces
 Home-page: https://github.com/neuro-ml/amid
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/amid/archive/v0.9.0.tar.gz
+Download-URL: https://github.com/neuro-ml/amid/archive/v0.9.1.tar.gz
 Keywords: medical imaging,dataset
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -68,15 +68,15 @@
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.lits.dataset.LiTS">LiTS</a>                                     |       201 | Abdominal                           | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.liver_medseg.LiverMedseg">LiverMedseg</a>                       |        50 | Chest, Abdomen                      | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.midrc.MIDRC">MIDRC</a>                                          |       155 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.mood.MOOD">MOOD</a>                                             |      1358 | Head, Abdominal                     | MRI, CT                         |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.medseg9.Medseg9">Medseg9</a>                                    |         9 | Chest                               | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.cancer_500.dataset.MoscowCancer500">MoscowCancer500</a>         |       979 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.covid_1110.MoscowCovid1110">MoscowCovid1110</a>                 |      1110 | Thorax                              | CT                              |
-| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13623 | Thorax                              | CT                              |
+| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13624 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nsclc.NSCLC">NSCLC</a>                                          |       422 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.rsna_bc.dataset.RSNABreastCancer">RSNABreastCancer</a>          |     54710 | Thorax                              | MG                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.stanford_coca.StanfordCoCa">StanfordCoCa</a>                    |       971 | Coronary, Chest                     | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.totalsegmentator.dataset.Totalsegmentator">Totalsegmentator</a> |      1204 | Head, Thorax, Abdomen, Pelvis, Legs | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.vs_seg.dataset.VSSEG">VSSEG</a>                                 |       484 | Head                                | MRI T1c, MRI T2                 |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.verse.VerSe">VerSe</a>                                          |       374 | Thorax, Abdomen                     | CT                              |
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: amid Version: 0.9.0 Summary: A curated list of
+Metadata-Version: 2.1 Name: amid Version: 0.9.1 Summary: A curated list of
 medical imaging datasets with unified interfaces Home-page: https://github.com/
 neuro-ml/amid License: UNKNOWN Download-URL: https://github.com/neuro-ml/amid/
-archive/v0.9.0.tar.gz Keywords: medical imaging,dataset Platform: UNKNOWN
+archive/v0.9.1.tar.gz Keywords: medical imaging,dataset Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3 :: Only Requires-Python: >=3.6 Description-
@@ -29,15 +29,15 @@
 | | AMOS | 600 | Abdomen | CT, MRI | | BIMCVCovid19 | 16335 | Chest | CT | |
 CC359 | 359 | Head | MRI T1 | | CT_ICH | 75 | Head | CT | | CrossMoDA | 484 |
 Head | MRI T1c, MRI T2hr | | EGD | 3096 | Head | FLAIR, MRI T1, MRI T1GD, MRI
 T2 | | FLARE2022 | 2100 | Abdomen | CT | | LIDC | 1018 | Chest | CT | | LiTS |
 201 | Abdominal | CT | | LiverMedseg | 50 | Chest, Abdomen | CT | | MIDRC | 155
 | Thorax | CT | | MOOD | 1358 | Head, Abdominal | MRI, CT | | Medseg9 | 9 |
 Chest | CT | | MoscowCancer500 | 979 | Thorax | CT | | MoscowCovid1110 | 1110 |
-Thorax | CT | | NLST | 13623 | Thorax | CT | | NSCLC | 422 | Thorax | CT | |
+Thorax | CT | | NLST | 13624 | Thorax | CT | | NSCLC | 422 | Thorax | CT | |
 RSNABreastCancer | 54710 | Thorax | MG | | StanfordCoCa | 971 | Coronary, Chest
 | CT | | Totalsegmentator | 1204 | Head, Thorax, Abdomen, Pelvis, Legs | CT | |
 VSSEG | 484 | Head | MRI T1c, MRI T2 | | VerSe | 374 | Thorax, Abdomen | CT |
 Check out [our docs](https://neuro-ml.github.io/amid/) for a more detailed list
 of available datasets and their fields. # Install Just get it from PyPi:
 ```shell pip install amid ``` Or if you want to use version control features:
 ```shell git clone https://github.com/neuro-ml/amid.git cd amid && pip install
```

### Comparing `amid-0.9.0/README.md` & `amid-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.lits.dataset.LiTS">LiTS</a>                                     |       201 | Abdominal                           | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.liver_medseg.LiverMedseg">LiverMedseg</a>                       |        50 | Chest, Abdomen                      | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.midrc.MIDRC">MIDRC</a>                                          |       155 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.mood.MOOD">MOOD</a>                                             |      1358 | Head, Abdominal                     | MRI, CT                         |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.medseg9.Medseg9">Medseg9</a>                                    |         9 | Chest                               | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.cancer_500.dataset.MoscowCancer500">MoscowCancer500</a>         |       979 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.covid_1110.MoscowCovid1110">MoscowCovid1110</a>                 |      1110 | Thorax                              | CT                              |
-| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13623 | Thorax                              | CT                              |
+| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13624 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nsclc.NSCLC">NSCLC</a>                                          |       422 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.rsna_bc.dataset.RSNABreastCancer">RSNABreastCancer</a>          |     54710 | Thorax                              | MG                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.stanford_coca.StanfordCoCa">StanfordCoCa</a>                    |       971 | Coronary, Chest                     | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.totalsegmentator.dataset.Totalsegmentator">Totalsegmentator</a> |      1204 | Head, Thorax, Abdomen, Pelvis, Legs | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.vs_seg.dataset.VSSEG">VSSEG</a>                                 |       484 | Head                                | MRI T1c, MRI T2                 |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.verse.VerSe">VerSe</a>                                          |       374 | Thorax, Abdomen                     | CT                              |
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 |:--------------------------------| | AMOS | 600 | Abdomen | CT, MRI | |
 BIMCVCovid19 | 16335 | Chest | CT | | CC359 | 359 | Head | MRI T1 | | CT_ICH |
 75 | Head | CT | | CrossMoDA | 484 | Head | MRI T1c, MRI T2hr | | EGD | 3096 |
 Head | FLAIR, MRI T1, MRI T1GD, MRI T2 | | FLARE2022 | 2100 | Abdomen | CT | |
 LIDC | 1018 | Chest | CT | | LiTS | 201 | Abdominal | CT | | LiverMedseg | 50 |
 Chest, Abdomen | CT | | MIDRC | 155 | Thorax | CT | | MOOD | 1358 | Head,
 Abdominal | MRI, CT | | Medseg9 | 9 | Chest | CT | | MoscowCancer500 | 979 |
-Thorax | CT | | MoscowCovid1110 | 1110 | Thorax | CT | | NLST | 13623 | Thorax
+Thorax | CT | | MoscowCovid1110 | 1110 | Thorax | CT | | NLST | 13624 | Thorax
 | CT | | NSCLC | 422 | Thorax | CT | | RSNABreastCancer | 54710 | Thorax | MG |
 | StanfordCoCa | 971 | Coronary, Chest | CT | | Totalsegmentator | 1204 | Head,
 Thorax, Abdomen, Pelvis, Legs | CT | | VSSEG | 484 | Head | MRI T1c, MRI T2 | |
 VerSe | 374 | Thorax, Abdomen | CT | Check out [our docs](https://neuro-
 ml.github.io/amid/) for a more detailed list of available datasets and their
 fields. # Install Just get it from PyPi: ```shell pip install amid ``` Or if
 you want to use version control features: ```shell git clone https://
```

### Comparing `amid-0.9.0/amid/amos/dataset.py` & `amid-0.9.1/amid/amos/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/bimcv.py` & `amid-0.9.1/amid/bimcv.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/cancer_500/dataset.py` & `amid-0.9.1/amid/cancer_500/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/cancer_500/nodules.py` & `amid-0.9.1/amid/cancer_500/nodules.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/cancer_500/typing.py` & `amid-0.9.1/amid/cancer_500/typing.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/cc359/dataset.py` & `amid-0.9.1/amid/cc359/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,8 +172,8 @@
             if Path(zipinfo.filename).name.startswith(_id) and not zipinfo.is_dir():
                 return zipfile.Path(str(archive), zipinfo.filename)
 
     raise KeyError(f'Id "{_id}" not found')
 
 
 def zipfile2meta(zf):
-    return {k: v for k, v in zip(['id', 'vendor', 'field', 'age', 'gender'], zf.name[: -len('.nii.gz')].split('_'))}
+    return dict(zip(['id', 'vendor', 'field', 'age', 'gender'], zf.name[: -len('.nii.gz')].split('_')))
```

### Comparing `amid-0.9.0/amid/cc359/transforms.py` & `amid-0.9.1/amid/cc359/transforms.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/covid_1110.py` & `amid-0.9.1/amid/covid_1110.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/crossmoda.py` & `amid-0.9.1/amid/crossmoda.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/ct_ich.py` & `amid-0.9.1/amid/ct_ich.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/egd.py` & `amid-0.9.1/amid/egd.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/flare2022.py` & `amid-0.9.1/amid/flare2022.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/internals/cache.py` & `amid-0.9.1/amid/internals/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,52 +2,55 @@
 from pathlib import Path
 from typing import Dict, Sequence, Union
 
 import numpy as np
 from bev import Repository
 from connectome import CacheColumns as Columns, CacheToDisk as Disk
 from connectome.utils import StringsLike
-from tarn import ReadError, Storage
-from tarn.cache import ChainSerializer, DictSerializer, JsonSerializer, PickleSerializer, Serializer, SerializerError
+from tarn import HashKeyStorage, ReadError
+from tarn.serializers import (
+    ChainSerializer,
+    DictSerializer,
+    JsonSerializer,
+    PickleSerializer,
+    Serializer,
+    SerializerError,
+)
 
 
 class CacheToDisk(Disk):
     def __init__(
         self,
         names: StringsLike,
         serializer: Union[Serializer, Sequence[Serializer]] = None,
-        fetch: bool = False,
         **kwargs,
     ):
         repo = Repository.from_here('../data')
         cache = repo.cache
         super().__init__(
             [x.root for x in cache.local[0].locations],
             cache.storage,
-            remote=cache.remote if fetch else [],
             serializer=default_serializer(serializer),
             names=names,
             **kwargs,
         )
 
 
 class CacheColumns(Columns):
     def __init__(
         self,
         names: StringsLike,
         serializer: Union[Serializer, Sequence[Serializer]] = None,
-        fetch: bool = False,
         **kwargs,
     ):
         repo = Repository.from_here('../data')
         cache = repo.cache
         super().__init__(
             [x.root for x in cache.local[0].locations],
             cache.storage,
-            remote=cache.remote if fetch else [],
             serializer=default_serializer(serializer),
             names=names,
             **kwargs,
         )
 
 
 def default_serializer(serializers):
@@ -85,15 +88,15 @@
             assert isinstance(compression, int)
             with GzipFile(folder / 'value.npy.gz', 'wb', compresslevel=compression, mtime=0) as file:
                 np.save(file, value, allow_pickle=False)
 
         else:
             np.save(folder / 'value.npy', value, allow_pickle=False)
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         paths = list(folder.iterdir())
         if len(paths) != 1:
             raise SerializerError
 
         (path,) = paths
         if path.name == 'value.npy':
             loader = np.load
@@ -112,9 +115,9 @@
             raise ReadError from e
 
 
 class CleanInvalid(Serializer):
     def save(self, value, folder: Path):
         raise SerializerError
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         raise ReadError
```

### Comparing `amid-0.9.0/amid/internals/checksum.py` & `amid-0.9.1/amid/internals/checksum.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             self._serializer.save(value, base)
             tree = {}
             # TODO: this is basically `mirror to storage`
             for file in base.glob('**/*'):
                 if file.is_dir():
                     continue
 
-                tree[str(file.relative_to(base))] = self._storage.write(file)
+                tree[str(file.relative_to(base))] = self._storage.write(file).hex()
 
             return tree
 
 
 # source: https://stackoverflow.com/a/61027781
 class ProgressParallel(Parallel):
     def __init__(self, *args, tqdm_kwargs=None, **kwargs):
```

### Comparing `amid-0.9.0/amid/internals/cli.py` & `amid-0.9.1/amid/internals/cli.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/internals/licenses.py` & `amid-0.9.1/amid/internals/licenses.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/internals/registry.py` & `amid-0.9.1/amid/internals/registry.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/internals/yandex.py` & `amid-0.9.1/amid/internals/yandex.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lidc/dataset.py` & `amid-0.9.1/amid/lidc/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lidc/nodules.py` & `amid-0.9.1/amid/lidc/nodules.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lidc/transforms.py` & `amid-0.9.1/amid/lidc/transforms.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lidc/typing.py` & `amid-0.9.1/amid/lidc/typing.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lits/dataset.py` & `amid-0.9.1/amid/lits/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/lits/transforms.py` & `amid-0.9.1/amid/lits/transforms.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/liver_medseg.py` & `amid-0.9.1/amid/liver_medseg.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,26 +56,31 @@
     ----------
     """
 
     _root: str = None
 
     @meta
     def ids(_root: Silent):
-        result = set()
+        if _root is None:
+            raise ValueError('Please provide the `root` argument')
 
+        result = set()
         with ZipFile(Path(_root) / 'img.zip') as zf:
             for zipinfo in zf.infolist():
                 if zipinfo.is_dir():
                     continue
                 file_stem = Path(zipinfo.filename).stem
                 result.add('liver_medseg_' + re.findall(r'\d+', file_stem)[0])
 
         return tuple(sorted(result))
 
     def _file(i: str, _root: Silent):
+        if _root is None:
+            raise ValueError('Please provide the `root` argument')
+
         num_id = i.split('_')[-1]
         return zipfile.Path(Path(_root) / 'img.zip', f'img{num_id}.nii.gz')
 
     def image(_file) -> np.ndarray:
         with open_nii_gz_file(_file) as nii_file:
             return np.asarray(nii_file.dataobj)
```

### Comparing `amid-0.9.0/amid/medseg9.py` & `amid-0.9.1/amid/medseg9.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/midrc.py` & `amid-0.9.1/amid/midrc.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/mood.py` & `amid-0.9.1/amid/mood.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/nlst.py` & `amid-0.9.1/amid/nlst.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/nsclc.py` & `amid-0.9.1/amid/nsclc.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/rsna_bc/dataset.py` & `amid-0.9.1/amid/rsna_bc/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/rsna_bc/utils.py` & `amid-0.9.1/amid/rsna_bc/utils.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/stanford_coca.py` & `amid-0.9.1/amid/stanford_coca.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/totalsegmentator/const.py` & `amid-0.9.1/amid/totalsegmentator/const.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/totalsegmentator/dataset.py` & `amid-0.9.1/amid/totalsegmentator/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/totalsegmentator/utils.py` & `amid-0.9.1/amid/totalsegmentator/utils.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/transforms.py` & `amid-0.9.1/amid/transforms.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/utils.py` & `amid-0.9.1/amid/utils.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/verse.py` & `amid-0.9.1/amid/verse.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/vs_seg/dataset.py` & `amid-0.9.1/amid/vs_seg/dataset.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid/vs_seg/transforms.py` & `amid-0.9.1/amid/vs_seg/transforms.py`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/amid.egg-info/PKG-INFO` & `amid-0.9.1/amid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: amid
-Version: 0.9.0
+Version: 0.9.1
 Summary: A curated list of medical imaging datasets with unified interfaces
 Home-page: https://github.com/neuro-ml/amid
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/amid/archive/v0.9.0.tar.gz
+Download-URL: https://github.com/neuro-ml/amid/archive/v0.9.1.tar.gz
 Keywords: medical imaging,dataset
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -68,15 +68,15 @@
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.lits.dataset.LiTS">LiTS</a>                                     |       201 | Abdominal                           | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.liver_medseg.LiverMedseg">LiverMedseg</a>                       |        50 | Chest, Abdomen                      | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.midrc.MIDRC">MIDRC</a>                                          |       155 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.mood.MOOD">MOOD</a>                                             |      1358 | Head, Abdominal                     | MRI, CT                         |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.medseg9.Medseg9">Medseg9</a>                                    |         9 | Chest                               | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.cancer_500.dataset.MoscowCancer500">MoscowCancer500</a>         |       979 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.covid_1110.MoscowCovid1110">MoscowCovid1110</a>                 |      1110 | Thorax                              | CT                              |
-| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13623 | Thorax                              | CT                              |
+| <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nlst.NLST">NLST</a>                                             |     13624 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.nsclc.NSCLC">NSCLC</a>                                          |       422 | Thorax                              | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.rsna_bc.dataset.RSNABreastCancer">RSNABreastCancer</a>          |     54710 | Thorax                              | MG                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.stanford_coca.StanfordCoCa">StanfordCoCa</a>                    |       971 | Coronary, Chest                     | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.totalsegmentator.dataset.Totalsegmentator">Totalsegmentator</a> |      1204 | Head, Thorax, Abdomen, Pelvis, Legs | CT                              |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.vs_seg.dataset.VSSEG">VSSEG</a>                                 |       484 | Head                                | MRI T1c, MRI T2                 |
 | <a href="https://neuro-ml.github.io/amid/latest/datasets-api/#amid.verse.VerSe">VerSe</a>                                          |       374 | Thorax, Abdomen                     | CT                              |
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: amid Version: 0.9.0 Summary: A curated list of
+Metadata-Version: 2.1 Name: amid Version: 0.9.1 Summary: A curated list of
 medical imaging datasets with unified interfaces Home-page: https://github.com/
 neuro-ml/amid License: UNKNOWN Download-URL: https://github.com/neuro-ml/amid/
-archive/v0.9.0.tar.gz Keywords: medical imaging,dataset Platform: UNKNOWN
+archive/v0.9.1.tar.gz Keywords: medical imaging,dataset Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3 :: Only Requires-Python: >=3.6 Description-
@@ -29,15 +29,15 @@
 | | AMOS | 600 | Abdomen | CT, MRI | | BIMCVCovid19 | 16335 | Chest | CT | |
 CC359 | 359 | Head | MRI T1 | | CT_ICH | 75 | Head | CT | | CrossMoDA | 484 |
 Head | MRI T1c, MRI T2hr | | EGD | 3096 | Head | FLAIR, MRI T1, MRI T1GD, MRI
 T2 | | FLARE2022 | 2100 | Abdomen | CT | | LIDC | 1018 | Chest | CT | | LiTS |
 201 | Abdominal | CT | | LiverMedseg | 50 | Chest, Abdomen | CT | | MIDRC | 155
 | Thorax | CT | | MOOD | 1358 | Head, Abdominal | MRI, CT | | Medseg9 | 9 |
 Chest | CT | | MoscowCancer500 | 979 | Thorax | CT | | MoscowCovid1110 | 1110 |
-Thorax | CT | | NLST | 13623 | Thorax | CT | | NSCLC | 422 | Thorax | CT | |
+Thorax | CT | | NLST | 13624 | Thorax | CT | | NSCLC | 422 | Thorax | CT | |
 RSNABreastCancer | 54710 | Thorax | MG | | StanfordCoCa | 971 | Coronary, Chest
 | CT | | Totalsegmentator | 1204 | Head, Thorax, Abdomen, Pelvis, Legs | CT | |
 VSSEG | 484 | Head | MRI T1c, MRI T2 | | VerSe | 374 | Thorax, Abdomen | CT |
 Check out [our docs](https://neuro-ml.github.io/amid/) for a more detailed list
 of available datasets and their fields. # Install Just get it from PyPi:
 ```shell pip install amid ``` Or if you want to use version control features:
 ```shell git clone https://github.com/neuro-ml/amid.git cd amid && pip install
```

### Comparing `amid-0.9.0/amid.egg-info/SOURCES.txt` & `amid-0.9.1/amid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amid-0.9.0/pyproject.toml` & `amid-0.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amid"
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 description = "A curated list of medical imaging datasets with unified interfaces"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { file = "LICENSE" }
 keywords = ["medical imaging", "dataset"]
 authors = [
     { name = "NeuroML Group", email = "maxs987@gmail.com" }
@@ -17,36 +17,14 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
-dependencies = [
-    "connectome>=0.4.2,<1.0.0",
-    "bev>=0.5.3,<1.0.0",
-    "tarn>=0.2.0,<1.0.0",
-    "numpy",
-    "nibabel",
-    "more-itertools",
-    "dicom-csv",
-    "tqdm",
-    "pandas",
-    "pylidc",
-    "pyyaml",
-    "requests",
-    "mdai",
-    "joblib",
-    "deli<1.0.0",
-    "typer<1.0.0",
-    "scipy",
-    "scikit-image",
-    "pydicom",
-    "imops"
-]
 
 [project.urls]
 "Homepage" = "https://github.com/neuro-ml/amid"
 "Issues" = "https://github.com/neuro-ml/amid/issues"
 "Source" = "https://github.com/neuro-ml/amid"
 "Docs" = "https://neuro-ml.github.io/amid"
 
@@ -60,14 +38,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["amid"]
 
 [tool.setuptools.dynamic]
 version = { attr = "amid.__version__.__version__" }
+dependencies = { file = "requirements.txt" }
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 
 [tool.isort]
 line_length = 120
```

### Comparing `amid-0.9.0/setup.py` & `amid-0.9.1/setup.py`

 * *Files identical despite different names*

