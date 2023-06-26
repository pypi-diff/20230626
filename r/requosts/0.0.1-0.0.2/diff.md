# Comparing `tmp/requosts-0.0.1.tar.gz` & `tmp/requosts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requosts-0.0.1.tar", last modified: Mon Jun 26 08:10:08 2023, max compression
+gzip compressed data, was "requosts-0.0.2.tar", last modified: Mon Jun 26 09:01:41 2023, max compression
```

## Comparing `requosts-0.0.1.tar` & `requosts-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 08:10:08.907409 requosts-0.0.1/
--rw-r--r--   0 a          (501) staff       (20)      189 2023-06-26 08:10:08.907138 requosts-0.0.1/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.1/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 08:10:08.904533 requosts-0.0.1/request/
--rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 08:01:07.000000 requosts-0.0.1/request/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)      116 2023-06-26 08:00:05.000000 requosts-0.0.1/request/requests.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 08:10:08.906670 requosts-0.0.1/requosts.egg-info/
--rw-r--r--   0 a          (501) staff       (20)      189 2023-06-26 08:10:08.000000 requosts-0.0.1/requosts.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      221 2023-06-26 08:10:08.000000 requosts-0.0.1/requosts.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 08:10:08.000000 requosts-0.0.1/requosts.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)       20 2023-06-26 08:10:08.000000 requosts-0.0.1/requosts.egg-info/entry_points.txt
--rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 08:10:08.000000 requosts-0.0.1/requosts.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 08:10:08.907513 requosts-0.0.1/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)      344 2023-06-26 08:10:02.000000 requosts-0.0.1/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.092818 requosts-0.0.2/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:01:41.092502 requosts-0.0.2/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.2/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.090526 requosts-0.0.2/request/
+-rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 08:59:27.000000 requosts-0.0.2/request/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)      117 2023-06-26 08:58:25.000000 requosts-0.0.2/request/request.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.092171 requosts-0.0.2/requosts.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      216 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)        9 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 09:01:41.092906 requosts-0.0.2/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)      300 2023-06-26 09:00:56.000000 requosts-0.0.2/setup.py
```

