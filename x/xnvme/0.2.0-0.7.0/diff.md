# Comparing `tmp/xnvme-0.2.0.tar.gz` & `tmp/xnvme-core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnvme-0.2.0.tar", last modified: Thu May 12 12:55:52 2022, max compression
+gzip compressed data, was "xnvme-0.7.0.tar", last modified: Mon Jun 26 07:12:38 2023, max compression
```

## Comparing `xnvme-0.2.0.tar` & `xnvme-core-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:55:52.426841 xnvme-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-12 12:55:52.423809 xnvme-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-12 12:55:52.428254 xnvme-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2696 2022-05-12 12:53:47.000000 xnvme-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:55:52.370331 xnvme-0.2.0/xnvme/
--rw-r--r--   0 root         (0) root         (0)       86 2022-05-12 12:44:19.000000 xnvme-0.2.0/xnvme/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119168 2022-05-12 12:55:47.000000 xnvme-0.2.0/xnvme/libxnvme.pxd
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:55:52.415423 xnvme-0.2.0/xnvme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-12 12:55:49.000000 xnvme-0.2.0/xnvme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2022-05-12 12:55:52.000000 xnvme-0.2.0/xnvme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-12 12:55:50.000000 xnvme-0.2.0/xnvme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-05-12 12:55:51.000000 xnvme-0.2.0/xnvme.egg-info/top_level.txt
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.861208 xnvme-0.7.0/
+-rw-r--r--   0 safl       (501) staff       (20)    11701 2023-06-20 11:05:46.000000 xnvme-0.7.0/LICENSE
+-rw-r--r--   0 safl       (501) staff       (20)     1177 2023-06-26 07:12:38.861096 xnvme-0.7.0/PKG-INFO
+-rw-r--r--   0 safl       (501) staff       (20)      663 2023-06-20 11:05:46.000000 xnvme-0.7.0/README.rst
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.859376 xnvme-0.7.0/bin/
+-rwxr-xr-x   0 safl       (501) staff       (20)     1114 2023-06-20 11:05:46.000000 xnvme-0.7.0/bin/xpy_dev_open
+-rwxr-xr-x   0 safl       (501) staff       (20)      812 2023-06-20 11:05:46.000000 xnvme-0.7.0/bin/xpy_enumerate
+-rwxr-xr-x   0 safl       (501) staff       (20)      267 2023-06-20 11:05:46.000000 xnvme-0.7.0/bin/xpy_libconf
+-rw-r--r--   0 safl       (501) staff       (20)      104 2023-06-20 11:05:46.000000 xnvme-0.7.0/pyproject.toml
+-rw-r--r--   0 safl       (501) staff       (20)       38 2023-06-26 07:12:38.861244 xnvme-0.7.0/setup.cfg
+-rw-r--r--   0 safl       (501) staff       (20)     1057 2023-06-20 11:05:46.000000 xnvme-0.7.0/setup.py
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.858104 xnvme-0.7.0/xnvme/
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.860671 xnvme-0.7.0/xnvme/ctypes_bindings/
+-rw-r--r--   0 safl       (501) staff       (20)       97 2023-06-20 11:05:46.000000 xnvme-0.7.0/xnvme/ctypes_bindings/__init__.py
+-rw-r--r--   0 safl       (501) staff       (20)   189171 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme/ctypes_bindings/api.py
+-rw-r--r--   0 safl       (501) staff       (20)     1504 2023-06-20 11:05:46.000000 xnvme-0.7.0/xnvme/ctypes_bindings/library_loader.py
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.860913 xnvme-0.7.0/xnvme/ctypes_bindings/tests/
+-rw-r--r--   0 safl       (501) staff       (20)        0 2023-06-20 11:05:46.000000 xnvme-0.7.0/xnvme/ctypes_bindings/tests/__init__.py
+-rw-r--r--   0 safl       (501) staff       (20)      784 2023-06-20 11:05:46.000000 xnvme-0.7.0/xnvme/ctypes_bindings/tests/test_loader.py
+drwxr-xr-x   0 safl       (501) staff       (20)        0 2023-06-26 07:12:38.860147 xnvme-0.7.0/xnvme.egg-info/
+-rw-r--r--   0 safl       (501) staff       (20)     1177 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/PKG-INFO
+-rw-r--r--   0 safl       (501) staff       (20)      451 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/SOURCES.txt
+-rw-r--r--   0 safl       (501) staff       (20)        1 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/dependency_links.txt
+-rw-r--r--   0 safl       (501) staff       (20)        1 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/not-zip-safe
+-rw-r--r--   0 safl       (501) staff       (20)       24 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/requires.txt
+-rw-r--r--   0 safl       (501) staff       (20)        6 2023-06-26 07:12:38.000000 xnvme-0.7.0/xnvme.egg-info/top_level.txt
```

