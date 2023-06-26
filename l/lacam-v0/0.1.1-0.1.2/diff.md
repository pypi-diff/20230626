# Comparing `tmp/lacam_v0-0.1.1.tar.gz` & `tmp/lacam_v0-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacam_v0-0.1.1.tar", last modified: Mon Jun 26 20:43:59 2023, max compression
+gzip compressed data, was "lacam_v0-0.1.2.tar", last modified: Mon Jun 26 20:56:08 2023, max compression
```

## Comparing `lacam_v0-0.1.1.tar` & `lacam_v0-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:43:59.458349 lacam_v0-0.1.1/
--rw-rw-rw-   0        0        0      264 2023-06-26 20:43:59.458349 lacam_v0-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 20:43:59.458349 lacam_v0-0.1.1/lacam_v0.egg-info/
--rw-rw-rw-   0        0        0      264 2023-06-26 20:43:59.000000 lacam_v0-0.1.1/lacam_v0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-06-26 20:43:59.000000 lacam_v0-0.1.1/lacam_v0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:43:59.000000 lacam_v0-0.1.1/lacam_v0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-26 20:43:59.000000 lacam_v0-0.1.1/lacam_v0.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 20:43:59.458349 lacam_v0-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      430 2023-06-26 20:43:30.000000 lacam_v0-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:56:08.626975 lacam_v0-0.1.2/
+-rw-rw-rw-   0        0        0      264 2023-06-26 20:56:08.626975 lacam_v0-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:56:08.626975 lacam_v0-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-06-26 20:55:35.000000 lacam_v0-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:56:08.580151 lacam_v0-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:56:08.580151 lacam_v0-0.1.2/src/lacam_v0/
+-rw-rw-rw-   0        0        0       37 2023-06-26 19:59:07.000000 lacam_v0-0.1.2/src/lacam_v0/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-06-26 19:59:13.000000 lacam_v0-0.1.2/src/lacam_v0/datasets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:56:08.626975 lacam_v0-0.1.2/src/lacam_v0.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-06-26 20:56:08.000000 lacam_v0-0.1.2/src/lacam_v0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-26 20:56:08.000000 lacam_v0-0.1.2/src/lacam_v0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:56:08.000000 lacam_v0-0.1.2/src/lacam_v0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 20:56:08.000000 lacam_v0-0.1.2/src/lacam_v0.egg-info/top_level.txt
```

