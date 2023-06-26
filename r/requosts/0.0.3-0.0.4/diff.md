# Comparing `tmp/requosts-0.0.3.tar.gz` & `tmp/requosts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requosts-0.0.3.tar", last modified: Mon Jun 26 09:34:36 2023, max compression
+gzip compressed data, was "requosts-0.0.4.tar", last modified: Mon Jun 26 10:18:35 2023, max compression
```

## Comparing `requosts-0.0.3.tar` & `requosts-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.741703 requosts-0.0.3/
--rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:34:36.741353 requosts-0.0.3/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.3/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.739597 requosts-0.0.3/request/
--rw-r--r--   0 a          (501) staff       (20)       29 2023-06-26 09:32:58.000000 requosts-0.0.3/request/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)      377 2023-06-26 09:30:41.000000 requosts-0.0.3/request/request.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 09:34:36.740987 requosts-0.0.3/requosts.egg-info/
--rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      216 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)        9 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 09:34:36.000000 requosts-0.0.3/requosts.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 09:34:36.741795 requosts-0.0.3/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)      300 2023-06-26 09:34:03.000000 requosts-0.0.3/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 10:18:35.677418 requosts-0.0.4/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 10:18:35.677017 requosts-0.0.4/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)        0 2023-06-26 07:57:33.000000 requosts-0.0.4/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 10:18:35.674936 requosts-0.0.4/request/
+-rw-r--r--   0 a          (501) staff       (20)       23 2023-06-26 10:18:29.000000 requosts-0.0.4/request/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)      377 2023-06-26 09:30:41.000000 requosts-0.0.4/request/requests.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 10:18:35.676588 requosts-0.0.4/requosts.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)      191 2023-06-26 10:18:35.000000 requosts-0.0.4/requosts.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      217 2023-06-26 10:18:35.000000 requosts-0.0.4/requosts.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 10:18:35.000000 requosts-0.0.4/requosts.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)        9 2023-06-26 10:18:35.000000 requosts-0.0.4/requosts.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)        8 2023-06-26 10:18:35.000000 requosts-0.0.4/requosts.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 10:18:35.677527 requosts-0.0.4/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)      300 2023-06-26 09:45:39.000000 requosts-0.0.4/setup.py
```

