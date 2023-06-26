# Comparing `tmp/tradingcomdados-1.1.0.tar.gz` & `tmp/tradingcomdados-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.1.0.tar", last modified: Tue Jun 20 01:26:24 2023, max compression
+gzip compressed data, was "tradingcomdados-1.1.1.tar", last modified: Mon Jun 26 18:45:41 2023, max compression
```

## Comparing `tradingcomdados-1.1.0.tar` & `tradingcomdados-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:26:24.009292 tradingcomdados-1.1.0/
--rw-rw-rw-   0        0        0     1173 2023-06-20 01:26:24.008288 tradingcomdados-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-06-20 00:24:03.000000 tradingcomdados-1.1.0/README.md
--rw-rw-rw-   0        0        0      301 2023-06-20 01:23:45.000000 tradingcomdados-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 01:26:24.009292 tradingcomdados-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:26:23.997772 tradingcomdados-1.1.0/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.1.0/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     7732 2023-06-20 00:37:56.000000 tradingcomdados-1.1.0/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.1.0/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:26:24.007774 tradingcomdados-1.1.0/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1173 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-20 01:26:23.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.744973 tradingcomdados-1.1.1/
+-rw-rw-rw-   0        0        0     1702 2023-06-26 18:45:41.744973 tradingcomdados-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.1.1/README.md
+-rw-rw-rw-   0        0        0      452 2023-06-26 00:54:22.000000 tradingcomdados-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:45:41.745973 tradingcomdados-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.735842 tradingcomdados-1.1.1/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.1.1/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0    12162 2023-06-26 00:40:07.000000 tradingcomdados-1.1.1/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.1.1/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.743971 tradingcomdados-1.1.1/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.1.0/setup.py` & `tradingcomdados-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.1.0/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.1.1/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

