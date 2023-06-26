# Comparing `tmp/requosts-0.0.2.tar.gz` & `tmp/requosts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requosts-0.0.2.tar", last modified: Mon Jun 26 09:01:41 2023, max compression
+gzip compressed data, was "requosts-0.0.3.tar", last modified: Mon Jun 26 09:34:36 2023, max compression
```

## Comparing `requosts-0.0.2.tar` & `requosts-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.092818 requosts-0.0.2/
--rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:01:41.092502 requosts-0.0.2/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.2/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.090526 requosts-0.0.2/request/
--rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 08:59:27.000000 requosts-0.0.2/request/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)      117 2023-06-26 08:58:25.000000 requosts-0.0.2/request/request.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:01:41.092171 requosts-0.0.2/requosts.egg-info/
--rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      216 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)        9 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 09:01:41.000000 requosts-0.0.2/requosts.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 09:01:41.092906 requosts-0.0.2/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)      300 2023-06-26 09:00:56.000000 requosts-0.0.2/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.741703 requosts-0.0.3/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:34:36.741353 requosts-0.0.3/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.3/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.739597 requosts-0.0.3/request/
+-rw-r--r--   0 a          (501) staff       (20)       29 2023-06-26 09:32:58.000000 requosts-0.0.3/request/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)      377 2023-06-26 09:30:41.000000 requosts-0.0.3/request/request.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.740987 requosts-0.0.3/requosts.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      216 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)        9 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 09:34:36.741795 requosts-0.0.3/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)      300 2023-06-26 09:34:03.000000 requosts-0.0.3/setup.py
```

