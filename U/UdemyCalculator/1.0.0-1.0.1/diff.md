# Comparing `tmp/UdemyCalculator-1.0.0.tar.gz` & `tmp/UdemyCalculator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\UdemyCalculator-1.0.0.tar", last modified: Mon Jun 26 18:39:51 2023, max compression
+gzip compressed data, was "dist\UdemyCalculator-1.0.1.tar", last modified: Mon Jun 26 18:43:40 2023, max compression
```

## Comparing `UdemyCalculator-1.0.0.tar` & `UdemyCalculator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:39:51.474877 UdemyCalculator-1.0.0/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:16:06.000000 UdemyCalculator-1.0.0/LICENCE
--rw-rw-rw-   0        0        0       61 2023-06-26 18:37:39.000000 UdemyCalculator-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      301 2023-06-26 18:39:51.474877 UdemyCalculator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-06-26 18:33:46.000000 UdemyCalculator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 18:39:51.472878 UdemyCalculator-1.0.0/UdemyCalculator.egg-info/
--rw-rw-rw-   0        0        0      301 2023-06-26 18:39:51.000000 UdemyCalculator-1.0.0/UdemyCalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-26 18:39:51.000000 UdemyCalculator-1.0.0/UdemyCalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:39:51.000000 UdemyCalculator-1.0.0/UdemyCalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:39:51.000000 UdemyCalculator-1.0.0/UdemyCalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 18:39:51.474877 UdemyCalculator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-06-26 18:37:39.000000 UdemyCalculator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:39:51.473878 UdemyCalculator-1.0.0/udemycalculator/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:15:24.000000 UdemyCalculator-1.0.0/udemycalculator/__init__.py
--rw-rw-rw-   0        0        0      422 2023-06-26 18:22:55.000000 UdemyCalculator-1.0.0/udemycalculator/calculator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:43:40.626594 UdemyCalculator-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-06-26 18:16:06.000000 UdemyCalculator-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0       61 2023-06-26 18:37:39.000000 UdemyCalculator-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      301 2023-06-26 18:43:40.625595 UdemyCalculator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-06-26 18:33:46.000000 UdemyCalculator-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:43:40.623594 UdemyCalculator-1.0.1/UdemyCalculator.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-06-26 18:43:40.000000 UdemyCalculator-1.0.1/UdemyCalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-26 18:43:40.000000 UdemyCalculator-1.0.1/UdemyCalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:43:40.000000 UdemyCalculator-1.0.1/UdemyCalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:43:40.000000 UdemyCalculator-1.0.1/UdemyCalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:43:40.626594 UdemyCalculator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-06-26 18:43:32.000000 UdemyCalculator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:43:40.625595 UdemyCalculator-1.0.1/udemycalculator/
+-rw-rw-rw-   0        0        0       34 2023-06-26 18:43:25.000000 UdemyCalculator-1.0.1/udemycalculator/__init__.py
+-rw-rw-rw-   0        0        0      422 2023-06-26 18:22:55.000000 UdemyCalculator-1.0.1/udemycalculator/calculator.py
```

