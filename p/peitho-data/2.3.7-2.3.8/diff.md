# Comparing `tmp/peitho_data-2.3.7.tar.gz` & `tmp/peitho_data-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.3.7.tar", last modified: Wed Jun 21 03:36:37 2023, max compression
+gzip compressed data, was "peitho_data-2.3.8.tar", last modified: Mon Jun 26 12:28:24 2023, max compression
```

## Comparing `peitho_data-2.3.7.tar` & `peitho_data-2.3.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.513919 peitho_data-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 03:34:35.000000 peitho_data-2.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 03:34:35.000000 peitho_data-2.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 03:36:37.513919 peitho_data-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-21 03:34:35.000000 peitho_data-2.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/machine_learning/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/machine_learning/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/machine_learning/cnn/image_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.513919 peitho_data-2.3.7/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.513919 peitho_data-2.3.7/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.513919 peitho_data-2.3.7/peitho_data/tests/machine_learning/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/machine_learning/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/machine_learning/cnn/test_image_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-21 03:34:35.000000 peitho_data-2.3.7/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:36:37.509919 peitho_data-2.3.7/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 03:36:37.000000 peitho_data-2.3.7/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-21 03:36:37.000000 peitho_data-2.3.7/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:36:37.000000 peitho_data-2.3.7/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:35:00.000000 peitho_data-2.3.7/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 03:36:37.000000 peitho_data-2.3.7/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 03:36:37.000000 peitho_data-2.3.7/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 03:36:37.513919 peitho_data-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 03:34:35.000000 peitho_data-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 12:26:04.000000 peitho_data-2.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 12:26:04.000000 peitho_data-2.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 12:28:24.206587 peitho_data-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-26 12:26:04.000000 peitho_data-2.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/machine_learning/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/cnn/image_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/test_image_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:26:36.000000 peitho_data-2.3.8/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 12:28:24.206587 peitho_data-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 12:26:04.000000 peitho_data-2.3.8/setup.py
```

### Comparing `peitho_data-2.3.7/LICENSE` & `peitho_data-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/README.md` & `peitho_data-2.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,297 +1,273 @@
 00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a0a 3c61 2068 7265 663d 2268  er">..<a href="h
-00000020: 7474 7073 3a2f 2f77 7777 2e62 696c 6962  ttps://www.bilib
-00000030: 696c 692e 636f 6d2f 7669 6465 6f2f 4256  ili.com/video/BV
-00000040: 316b 6234 7931 6d37 6537 3f70 3d33 223e  1kb4y1m7e7?p=3">
-00000050: 0a20 2020 203c 696d 6720 616c 743d 22e6  .    <img alt=".
-00000060: b0b8 e681 9222 2073 7263 3d22 2e2f 7468  ....." src="./th
-00000070: 656d 652f e99f b6e5 8589 e68a 9ae6 9c88  eme/............
-00000080: 2de5 a4a9 e4b8 8be4 baba e997 b42e 706e  -.............pn
-00000090: 6722 3e0a 2020 2020 5261 6964 656e 2053  g">.    Raiden S
-000000a0: 686f 6775 6e20 28e9 9bb7 e794 b5e5 b086  hogun (.........
-000000b0: e586 9b29 2c20 7468 6520 6368 6172 6163  ...), the charac
-000000c0: 7465 7220 6f66 2065 7465 726e 6974 792c  ter of eternity,
-000000d0: 2074 6865 6d65 7320 6d79 206e 6576 6572   themes my never
-000000e0: 2d65 6e64 696e 6720 666f 6375 7320 6f6e  -ending focus on
-000000f0: 2064 6174 6120 696e 2067 656e 6572 616c   data in general
-00000100: 0a3c 2f61 3e0a 0a3c 6272 3e0a 3c62 723e  .</a>..<br>.<br>
-00000110: 0a0a 5b21 5b50 7950 495d 2868 7474 7073  ..[![PyPI](https
-00000120: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000130: 6f2f 7079 7069 2f76 2f70 6569 7468 6f2d  o/pypi/v/peitho-
-00000140: 6461 7461 3f6c 6f67 6f3d 7079 7069 266c  data?logo=pypi&l
-00000150: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2673  ogoColor=white&s
-00000160: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00000170: 6765 295d 2868 7474 7073 3a2f 2f70 7970  ge)](https://pyp
-00000180: 692e 6f72 672f 7072 6f6a 6563 742f 7065  i.org/project/pe
-00000190: 6974 686f 2d64 6174 612f 290a 5b21 5b52  itho-data/).[![R
-000001a0: 6561 6420 7468 6520 446f 6373 2028 7665  ead the Docs (ve
-000001b0: 7273 696f 6e29 5d28 6874 7470 733a 2f2f  rsion)](https://
-000001c0: 696d 672e 7368 6965 6c64 732e 696f 2f72  img.shields.io/r
-000001d0: 6561 6474 6865 646f 6373 2f70 6569 7468  eadthedocs/peith
-000001e0: 6f2d 6461 7461 2f6c 6174 6573 743f 6c6f  o-data/latest?lo
-000001f0: 676f 3d52 6561 6425 3230 7468 6525 3230  go=Read%20the%20
-00000200: 446f 6373 266c 6f67 6f43 6f6c 6f72 3d77  Docs&logoColor=w
-00000210: 6869 7465 2673 7479 6c65 3d66 6f72 2d74  hite&style=for-t
-00000220: 6865 2d62 6164 6765 295d 2868 7474 7073  he-badge)](https
-00000230: 3a2f 2f70 6569 7468 6f2d 6461 7461 2e72  ://peitho-data.r
-00000240: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000250: 2f6c 6174 6573 742f 290a 5b21 5b47 6974  /latest/).[![Git
-00000260: 4875 6220 576f 726b 666c 6f77 2053 7461  Hub Workflow Sta
-00000270: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
-00000280: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000290: 7562 2f61 6374 696f 6e73 2f77 6f72 6b66  ub/actions/workf
-000002a0: 6c6f 772f 7374 6174 7573 2f51 7562 6974  low/status/Qubit
-000002b0: 5069 2f70 6569 7468 6f2d 6461 7461 2f63  Pi/peitho-data/c
-000002c0: 692d 6364 2e79 6d6c 3f6c 6f67 6f3d 6769  i-cd.yml?logo=gi
-000002d0: 7468 7562 2673 7479 6c65 3d66 6f72 2d74  thub&style=for-t
-000002e0: 6865 2d62 6164 6765 295d 2868 7474 7073  he-badge)](https
-000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5175  ://github.com/Qu
-00000300: 6269 7450 692f 7065 6974 686f 2d64 6174  bitPi/peitho-dat
-00000310: 612f 6163 7469 6f6e 732f 776f 726b 666c  a/actions/workfl
-00000320: 6f77 732f 6369 2d63 642e 796d 6c29 0a0a  ows/ci-cd.yml)..
-00000330: 5b21 5b44 6973 636f 7264 5d28 6874 7470  [![Discord](http
-00000340: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000350: 696f 2f64 6973 636f 7264 2f31 3030 3537  io/discord/10057
-00000360: 3534 3532 3539 3432 3033 3033 3636 3f6c  54525942030366?l
-00000370: 6f67 6f3d 6469 7363 6f72 6426 6c6f 676f  ogo=discord&logo
-00000380: 436f 6c6f 723d 7768 6974 6526 7374 796c  Color=white&styl
-00000390: 653d 666f 722d 7468 652d 6261 6467 6529  e=for-the-badge)
-000003a0: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-000003b0: 642e 636f 6d2f 7769 6467 6574 3f69 643d  d.com/widget?id=
-000003c0: 3130 3035 3735 3435 3235 3934 3230 3330  1005754525942030
-000003d0: 3336 3626 7468 656d 653d 6461 726b 290a  366&theme=dark).
-000003e0: 5b21 5b4c 6963 656e 7365 2042 6164 6765  [![License Badge
-000003f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000400: 6965 6c64 732e 696f 2f62 6164 6765 2f41  ields.io/badge/A
-00000410: 7061 6368 6525 3230 322e 302d 4632 3539  pache%202.0-F259
-00000420: 3130 2e73 7667 3f73 7479 6c65 3d66 6f72  10.svg?style=for
-00000430: 2d74 6865 2d62 6164 6765 266c 6f67 6f3d  -the-badge&logo=
-00000440: 4170 6163 6865 266c 6f67 6f43 6f6c 6f72  Apache&logoColor
-00000450: 3d77 6869 7465 295d 2868 7474 7073 3a2f  =white)](https:/
-00000460: 2f77 7777 2e61 7061 6368 652e 6f72 672f  /www.apache.org/
-00000470: 6c69 6365 6e73 6573 2f4c 4943 454e 5345  licenses/LICENSE
-00000480: 2d32 2e30 290a 215b 4769 7448 7562 206c  -2.0).![GitHub l
-00000490: 6173 7420 636f 6d6d 6974 2028 6d61 7374  ast commit (mast
-000004a0: 6572 295d 2868 7474 7073 3a2f 2f69 6d67  er)](https://img
-000004b0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000004c0: 7562 2f6c 6173 742d 636f 6d6d 6974 2f51  ub/last-commit/Q
-000004d0: 7562 6974 5069 2f70 6569 7468 6f2d 6461  ubitPi/peitho-da
-000004e0: 7461 2f6d 6173 7465 723f 6c6f 676f 3d67  ta/master?logo=g
-000004f0: 6974 6875 6226 7374 796c 653d 666f 722d  ithub&style=for-
-00000500: 7468 652d 6261 6467 6529 0a0a 5b21 5b42  the-badge)..[![B
-00000510: 7567 735d 2868 7474 7073 3a2f 2f73 6f6e  ugs](https://son
-00000520: 6172 636c 6f75 642e 696f 2f61 7069 2f70  arcloud.io/api/p
-00000530: 726f 6a65 6374 5f62 6164 6765 732f 6d65  roject_badges/me
-00000540: 6173 7572 653f 7072 6f6a 6563 743d 5175  asure?project=Qu
-00000550: 6269 7450 695f 7065 6974 686f 2d64 6174  bitPi_peitho-dat
-00000560: 6126 6d65 7472 6963 3d62 7567 7329 5d28  a&metric=bugs)](
-00000570: 6874 7470 733a 2f2f 736f 6e61 7263 6c6f  https://sonarclo
-00000580: 7564 2e69 6f2f 7375 6d6d 6172 792f 6e65  ud.io/summary/ne
-00000590: 775f 636f 6465 3f69 643d 5175 6269 7450  w_code?id=QubitP
-000005a0: 695f 7065 6974 686f 2d64 6174 6129 0a5b  i_peitho-data).[
-000005b0: 215b 5675 6c6e 6572 6162 696c 6974 6965  ![Vulnerabilitie
-000005c0: 735d 2868 7474 7073 3a2f 2f73 6f6e 6172  s](https://sonar
-000005d0: 636c 6f75 642e 696f 2f61 7069 2f70 726f  cloud.io/api/pro
-000005e0: 6a65 6374 5f62 6164 6765 732f 6d65 6173  ject_badges/meas
-000005f0: 7572 653f 7072 6f6a 6563 743d 5175 6269  ure?project=Qubi
-00000600: 7450 695f 7065 6974 686f 2d64 6174 6126  tPi_peitho-data&
-00000610: 6d65 7472 6963 3d76 756c 6e65 7261 6269  metric=vulnerabi
-00000620: 6c69 7469 6573 295d 2868 7474 7073 3a2f  lities)](https:/
-00000630: 2f73 6f6e 6172 636c 6f75 642e 696f 2f73  /sonarcloud.io/s
-00000640: 756d 6d61 7279 2f6e 6577 5f63 6f64 653f  ummary/new_code?
-00000650: 6964 3d51 7562 6974 5069 5f70 6569 7468  id=QubitPi_peith
-00000660: 6f2d 6461 7461 290a 5b21 5b44 7570 6c69  o-data).[![Dupli
-00000670: 6361 7465 6420 4c69 6e65 7320 2825 295d  cated Lines (%)]
-00000680: 2868 7474 7073 3a2f 2f73 6f6e 6172 636c  (https://sonarcl
-00000690: 6f75 642e 696f 2f61 7069 2f70 726f 6a65  oud.io/api/proje
-000006a0: 6374 5f62 6164 6765 732f 6d65 6173 7572  ct_badges/measur
-000006b0: 653f 7072 6f6a 6563 743d 5175 6269 7450  e?project=QubitP
-000006c0: 695f 7065 6974 686f 2d64 6174 6126 6d65  i_peitho-data&me
-000006d0: 7472 6963 3d64 7570 6c69 6361 7465 645f  tric=duplicated_
-000006e0: 6c69 6e65 735f 6465 6e73 6974 7929 5d28  lines_density)](
-000006f0: 6874 7470 733a 2f2f 736f 6e61 7263 6c6f  https://sonarclo
-00000700: 7564 2e69 6f2f 7375 6d6d 6172 792f 6e65  ud.io/summary/ne
-00000710: 775f 636f 6465 3f69 643d 5175 6269 7450  w_code?id=QubitP
-00000720: 695f 7065 6974 686f 2d64 6174 6129 0a5b  i_peitho-data).[
-00000730: 215b 5265 6c69 6162 696c 6974 7920 5261  ![Reliability Ra
-00000740: 7469 6e67 5d28 6874 7470 733a 2f2f 736f  ting](https://so
-00000750: 6e61 7263 6c6f 7564 2e69 6f2f 6170 692f  narcloud.io/api/
-00000760: 7072 6f6a 6563 745f 6261 6467 6573 2f6d  project_badges/m
-00000770: 6561 7375 7265 3f70 726f 6a65 6374 3d51  easure?project=Q
-00000780: 7562 6974 5069 5f70 6569 7468 6f2d 6461  ubitPi_peitho-da
-00000790: 7461 266d 6574 7269 633d 7265 6c69 6162  ta&metric=reliab
-000007a0: 696c 6974 795f 7261 7469 6e67 295d 2868  ility_rating)](h
-000007b0: 7474 7073 3a2f 2f73 6f6e 6172 636c 6f75  ttps://sonarclou
-000007c0: 642e 696f 2f73 756d 6d61 7279 2f6e 6577  d.io/summary/new
-000007d0: 5f63 6f64 653f 6964 3d51 7562 6974 5069  _code?id=QubitPi
-000007e0: 5f70 6569 7468 6f2d 6461 7461 290a 5b21  _peitho-data).[!
-000007f0: 5b51 7561 6c69 7479 2047 6174 6520 5374  [Quality Gate St
-00000800: 6174 7573 5d28 6874 7470 733a 2f2f 736f  atus](https://so
-00000810: 6e61 7263 6c6f 7564 2e69 6f2f 6170 692f  narcloud.io/api/
-00000820: 7072 6f6a 6563 745f 6261 6467 6573 2f6d  project_badges/m
-00000830: 6561 7375 7265 3f70 726f 6a65 6374 3d51  easure?project=Q
-00000840: 7562 6974 5069 5f70 6569 7468 6f2d 6461  ubitPi_peitho-da
-00000850: 7461 266d 6574 7269 633d 616c 6572 745f  ta&metric=alert_
-00000860: 7374 6174 7573 295d 2868 7474 7073 3a2f  status)](https:/
-00000870: 2f73 6f6e 6172 636c 6f75 642e 696f 2f73  /sonarcloud.io/s
-00000880: 756d 6d61 7279 2f6e 6577 5f63 6f64 653f  ummary/new_code?
-00000890: 6964 3d51 7562 6974 5069 5f70 6569 7468  id=QubitPi_peith
-000008a0: 6f2d 6461 7461 290a 5b21 5b54 6563 686e  o-data).[![Techn
-000008b0: 6963 616c 2044 6562 745d 2868 7474 7073  ical Debt](https
-000008c0: 3a2f 2f73 6f6e 6172 636c 6f75 642e 696f  ://sonarcloud.io
-000008d0: 2f61 7069 2f70 726f 6a65 6374 5f62 6164  /api/project_bad
-000008e0: 6765 732f 6d65 6173 7572 653f 7072 6f6a  ges/measure?proj
-000008f0: 6563 743d 5175 6269 7450 695f 7065 6974  ect=QubitPi_peit
-00000900: 686f 2d64 6174 6126 6d65 7472 6963 3d73  ho-data&metric=s
-00000910: 7161 6c65 5f69 6e64 6578 295d 2868 7474  qale_index)](htt
+00000010: 6572 223e 0a0a 5b21 5b50 7950 495d 2868  er">..[![PyPI](h
+00000020: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000030: 6473 2e69 6f2f 7079 7069 2f76 2f70 6569  ds.io/pypi/v/pei
+00000040: 7468 6f2d 6461 7461 3f6c 6f67 6f3d 7079  tho-data?logo=py
+00000050: 7069 266c 6f67 6f43 6f6c 6f72 3d77 6869  pi&logoColor=whi
+00000060: 7465 2673 7479 6c65 3d66 6f72 2d74 6865  te&style=for-the
+00000070: 2d62 6164 6765 295d 2868 7474 7073 3a2f  -badge)](https:/
+00000080: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000090: 742f 7065 6974 686f 2d64 6174 612f 290a  t/peitho-data/).
+000000a0: 5b21 5b52 6561 6420 7468 6520 446f 6373  [![Read the Docs
+000000b0: 2028 7665 7273 696f 6e29 5d28 6874 7470   (version)](http
+000000c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000000d0: 696f 2f72 6561 6474 6865 646f 6373 2f70  io/readthedocs/p
+000000e0: 6569 7468 6f2d 6461 7461 2f6c 6174 6573  eitho-data/lates
+000000f0: 743f 6c6f 676f 3d52 6561 6425 3230 7468  t?logo=Read%20th
+00000100: 6525 3230 446f 6373 266c 6f67 6f43 6f6c  e%20Docs&logoCol
+00000110: 6f72 3d77 6869 7465 2673 7479 6c65 3d66  or=white&style=f
+00000120: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+00000130: 7474 7073 3a2f 2f70 6569 7468 6f2d 6461  ttps://peitho-da
+00000140: 7461 2e72 6561 6474 6865 646f 6373 2e69  ta.readthedocs.i
+00000150: 6f2f 656e 2f6c 6174 6573 742f 290a 5b21  o/en/latest/).[!
+00000160: 5b47 6974 4875 6220 576f 726b 666c 6f77  [GitHub Workflow
+00000170: 2053 7461 7475 735d 2868 7474 7073 3a2f   Status](https:/
+00000180: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000190: 6769 7468 7562 2f61 6374 696f 6e73 2f77  github/actions/w
+000001a0: 6f72 6b66 6c6f 772f 7374 6174 7573 2f51  orkflow/status/Q
+000001b0: 7562 6974 5069 2f70 6569 7468 6f2d 6461  ubitPi/peitho-da
+000001c0: 7461 2f63 692d 6364 2e79 6d6c 3f6c 6f67  ta/ci-cd.yml?log
+000001d0: 6f3d 6769 7468 7562 2673 7479 6c65 3d66  o=github&style=f
+000001e0: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+000001f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000200: 6d2f 5175 6269 7450 692f 7065 6974 686f  m/QubitPi/peitho
+00000210: 2d64 6174 612f 6163 7469 6f6e 732f 776f  -data/actions/wo
+00000220: 726b 666c 6f77 732f 6369 2d63 642e 796d  rkflows/ci-cd.ym
+00000230: 6c29 0a0a 5b21 5b44 6973 636f 7264 5d28  l)..[![Discord](
+00000240: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000250: 6c64 732e 696f 2f64 6973 636f 7264 2f31  lds.io/discord/1
+00000260: 3030 3537 3534 3532 3539 3432 3033 3033  0057545259420303
+00000270: 3636 3f6c 6f67 6f3d 6469 7363 6f72 6426  66?logo=discord&
+00000280: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
+00000290: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+000002a0: 6467 6529 5d28 6874 7470 733a 2f2f 6469  dge)](https://di
+000002b0: 7363 6f72 642e 636f 6d2f 7769 6467 6574  scord.com/widget
+000002c0: 3f69 643d 3130 3035 3735 3435 3235 3934  ?id=100575452594
+000002d0: 3230 3330 3336 3626 7468 656d 653d 6461  2030366&theme=da
+000002e0: 726b 290a 5b21 5b4c 6963 656e 7365 2042  rk).[![License B
+000002f0: 6164 6765 5d28 6874 7470 733a 2f2f 696d  adge](https://im
+00000300: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000310: 6765 2f41 7061 6368 6525 3230 322e 302d  ge/Apache%202.0-
+00000320: 4632 3539 3130 2e73 7667 3f73 7479 6c65  F25910.svg?style
+00000330: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
+00000340: 6f67 6f3d 4170 6163 6865 266c 6f67 6f43  ogo=Apache&logoC
+00000350: 6f6c 6f72 3d77 6869 7465 295d 2868 7474  olor=white)](htt
+00000360: 7073 3a2f 2f77 7777 2e61 7061 6368 652e  ps://www.apache.
+00000370: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
+00000380: 454e 5345 2d32 2e30 290a 215b 4769 7448  ENSE-2.0).![GitH
+00000390: 7562 206c 6173 7420 636f 6d6d 6974 2028  ub last commit (
+000003a0: 6d61 7374 6572 295d 2868 7474 7073 3a2f  master)](https:/
+000003b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000003c0: 6769 7468 7562 2f6c 6173 742d 636f 6d6d  github/last-comm
+000003d0: 6974 2f51 7562 6974 5069 2f70 6569 7468  it/QubitPi/peith
+000003e0: 6f2d 6461 7461 2f6d 6173 7465 723f 6c6f  o-data/master?lo
+000003f0: 676f 3d67 6974 6875 6226 7374 796c 653d  go=github&style=
+00000400: 666f 722d 7468 652d 6261 6467 6529 0a0a  for-the-badge)..
+00000410: 5b21 5b42 7567 735d 2868 7474 7073 3a2f  [![Bugs](https:/
+00000420: 2f73 6f6e 6172 636c 6f75 642e 696f 2f61  /sonarcloud.io/a
+00000430: 7069 2f70 726f 6a65 6374 5f62 6164 6765  pi/project_badge
+00000440: 732f 6d65 6173 7572 653f 7072 6f6a 6563  s/measure?projec
+00000450: 743d 5175 6269 7450 695f 7065 6974 686f  t=QubitPi_peitho
+00000460: 2d64 6174 6126 6d65 7472 6963 3d62 7567  -data&metric=bug
+00000470: 7329 5d28 6874 7470 733a 2f2f 736f 6e61  s)](https://sona
+00000480: 7263 6c6f 7564 2e69 6f2f 7375 6d6d 6172  rcloud.io/summar
+00000490: 792f 6e65 775f 636f 6465 3f69 643d 5175  y/new_code?id=Qu
+000004a0: 6269 7450 695f 7065 6974 686f 2d64 6174  bitPi_peitho-dat
+000004b0: 6129 0a5b 215b 5675 6c6e 6572 6162 696c  a).[![Vulnerabil
+000004c0: 6974 6965 735d 2868 7474 7073 3a2f 2f73  ities](https://s
+000004d0: 6f6e 6172 636c 6f75 642e 696f 2f61 7069  onarcloud.io/api
+000004e0: 2f70 726f 6a65 6374 5f62 6164 6765 732f  /project_badges/
+000004f0: 6d65 6173 7572 653f 7072 6f6a 6563 743d  measure?project=
+00000500: 5175 6269 7450 695f 7065 6974 686f 2d64  QubitPi_peitho-d
+00000510: 6174 6126 6d65 7472 6963 3d76 756c 6e65  ata&metric=vulne
+00000520: 7261 6269 6c69 7469 6573 295d 2868 7474  rabilities)](htt
+00000530: 7073 3a2f 2f73 6f6e 6172 636c 6f75 642e  ps://sonarcloud.
+00000540: 696f 2f73 756d 6d61 7279 2f6e 6577 5f63  io/summary/new_c
+00000550: 6f64 653f 6964 3d51 7562 6974 5069 5f70  ode?id=QubitPi_p
+00000560: 6569 7468 6f2d 6461 7461 290a 5b21 5b44  eitho-data).[![D
+00000570: 7570 6c69 6361 7465 6420 4c69 6e65 7320  uplicated Lines 
+00000580: 2825 295d 2868 7474 7073 3a2f 2f73 6f6e  (%)](https://son
+00000590: 6172 636c 6f75 642e 696f 2f61 7069 2f70  arcloud.io/api/p
+000005a0: 726f 6a65 6374 5f62 6164 6765 732f 6d65  roject_badges/me
+000005b0: 6173 7572 653f 7072 6f6a 6563 743d 5175  asure?project=Qu
+000005c0: 6269 7450 695f 7065 6974 686f 2d64 6174  bitPi_peitho-dat
+000005d0: 6126 6d65 7472 6963 3d64 7570 6c69 6361  a&metric=duplica
+000005e0: 7465 645f 6c69 6e65 735f 6465 6e73 6974  ted_lines_densit
+000005f0: 7929 5d28 6874 7470 733a 2f2f 736f 6e61  y)](https://sona
+00000600: 7263 6c6f 7564 2e69 6f2f 7375 6d6d 6172  rcloud.io/summar
+00000610: 792f 6e65 775f 636f 6465 3f69 643d 5175  y/new_code?id=Qu
+00000620: 6269 7450 695f 7065 6974 686f 2d64 6174  bitPi_peitho-dat
+00000630: 6129 0a5b 215b 5265 6c69 6162 696c 6974  a).[![Reliabilit
+00000640: 7920 5261 7469 6e67 5d28 6874 7470 733a  y Rating](https:
+00000650: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
+00000660: 6170 692f 7072 6f6a 6563 745f 6261 6467  api/project_badg
+00000670: 6573 2f6d 6561 7375 7265 3f70 726f 6a65  es/measure?proje
+00000680: 6374 3d51 7562 6974 5069 5f70 6569 7468  ct=QubitPi_peith
+00000690: 6f2d 6461 7461 266d 6574 7269 633d 7265  o-data&metric=re
+000006a0: 6c69 6162 696c 6974 795f 7261 7469 6e67  liability_rating
+000006b0: 295d 2868 7474 7073 3a2f 2f73 6f6e 6172  )](https://sonar
+000006c0: 636c 6f75 642e 696f 2f73 756d 6d61 7279  cloud.io/summary
+000006d0: 2f6e 6577 5f63 6f64 653f 6964 3d51 7562  /new_code?id=Qub
+000006e0: 6974 5069 5f70 6569 7468 6f2d 6461 7461  itPi_peitho-data
+000006f0: 290a 5b21 5b51 7561 6c69 7479 2047 6174  ).[![Quality Gat
+00000700: 6520 5374 6174 7573 5d28 6874 7470 733a  e Status](https:
+00000710: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
+00000720: 6170 692f 7072 6f6a 6563 745f 6261 6467  api/project_badg
+00000730: 6573 2f6d 6561 7375 7265 3f70 726f 6a65  es/measure?proje
+00000740: 6374 3d51 7562 6974 5069 5f70 6569 7468  ct=QubitPi_peith
+00000750: 6f2d 6461 7461 266d 6574 7269 633d 616c  o-data&metric=al
+00000760: 6572 745f 7374 6174 7573 295d 2868 7474  ert_status)](htt
+00000770: 7073 3a2f 2f73 6f6e 6172 636c 6f75 642e  ps://sonarcloud.
+00000780: 696f 2f73 756d 6d61 7279 2f6e 6577 5f63  io/summary/new_c
+00000790: 6f64 653f 6964 3d51 7562 6974 5069 5f70  ode?id=QubitPi_p
+000007a0: 6569 7468 6f2d 6461 7461 290a 5b21 5b54  eitho-data).[![T
+000007b0: 6563 686e 6963 616c 2044 6562 745d 2868  echnical Debt](h
+000007c0: 7474 7073 3a2f 2f73 6f6e 6172 636c 6f75  ttps://sonarclou
+000007d0: 642e 696f 2f61 7069 2f70 726f 6a65 6374  d.io/api/project
+000007e0: 5f62 6164 6765 732f 6d65 6173 7572 653f  _badges/measure?
+000007f0: 7072 6f6a 6563 743d 5175 6269 7450 695f  project=QubitPi_
+00000800: 7065 6974 686f 2d64 6174 6126 6d65 7472  peitho-data&metr
+00000810: 6963 3d73 7161 6c65 5f69 6e64 6578 295d  ic=sqale_index)]
+00000820: 2868 7474 7073 3a2f 2f73 6f6e 6172 636c  (https://sonarcl
+00000830: 6f75 642e 696f 2f73 756d 6d61 7279 2f6e  oud.io/summary/n
+00000840: 6577 5f63 6f64 653f 6964 3d51 7562 6974  ew_code?id=Qubit
+00000850: 5069 5f70 6569 7468 6f2d 6461 7461 290a  Pi_peitho-data).
+00000860: 5b21 5b43 6f76 6572 6167 655d 2868 7474  [![Coverage](htt
+00000870: 7073 3a2f 2f73 6f6e 6172 636c 6f75 642e  ps://sonarcloud.
+00000880: 696f 2f61 7069 2f70 726f 6a65 6374 5f62  io/api/project_b
+00000890: 6164 6765 732f 6d65 6173 7572 653f 7072  adges/measure?pr
+000008a0: 6f6a 6563 743d 5175 6269 7450 695f 7065  oject=QubitPi_pe
+000008b0: 6974 686f 2d64 6174 6126 6d65 7472 6963  itho-data&metric
+000008c0: 3d63 6f76 6572 6167 6529 5d28 6874 7470  =coverage)](http
+000008d0: 733a 2f2f 736f 6e61 7263 6c6f 7564 2e69  s://sonarcloud.i
+000008e0: 6f2f 7375 6d6d 6172 792f 6e65 775f 636f  o/summary/new_co
+000008f0: 6465 3f69 643d 5175 6269 7450 695f 7065  de?id=QubitPi_pe
+00000900: 6974 686f 2d64 6174 6129 0a5b 215b 4c69  itho-data).[![Li
+00000910: 6e65 7320 6f66 2043 6f64 655d 2868 7474  nes of Code](htt
 00000920: 7073 3a2f 2f73 6f6e 6172 636c 6f75 642e  ps://sonarcloud.
-00000930: 696f 2f73 756d 6d61 7279 2f6e 6577 5f63  io/summary/new_c
-00000940: 6f64 653f 6964 3d51 7562 6974 5069 5f70  ode?id=QubitPi_p
-00000950: 6569 7468 6f2d 6461 7461 290a 5b21 5b43  eitho-data).[![C
-00000960: 6f76 6572 6167 655d 2868 7474 7073 3a2f  overage](https:/
-00000970: 2f73 6f6e 6172 636c 6f75 642e 696f 2f61  /sonarcloud.io/a
-00000980: 7069 2f70 726f 6a65 6374 5f62 6164 6765  pi/project_badge
-00000990: 732f 6d65 6173 7572 653f 7072 6f6a 6563  s/measure?projec
-000009a0: 743d 5175 6269 7450 695f 7065 6974 686f  t=QubitPi_peitho
-000009b0: 2d64 6174 6126 6d65 7472 6963 3d63 6f76  -data&metric=cov
-000009c0: 6572 6167 6529 5d28 6874 7470 733a 2f2f  erage)](https://
-000009d0: 736f 6e61 7263 6c6f 7564 2e69 6f2f 7375  sonarcloud.io/su
-000009e0: 6d6d 6172 792f 6e65 775f 636f 6465 3f69  mmary/new_code?i
-000009f0: 643d 5175 6269 7450 695f 7065 6974 686f  d=QubitPi_peitho
-00000a00: 2d64 6174 6129 0a5b 215b 4c69 6e65 7320  -data).[![Lines 
-00000a10: 6f66 2043 6f64 655d 2868 7474 7073 3a2f  of Code](https:/
-00000a20: 2f73 6f6e 6172 636c 6f75 642e 696f 2f61  /sonarcloud.io/a
-00000a30: 7069 2f70 726f 6a65 6374 5f62 6164 6765  pi/project_badge
-00000a40: 732f 6d65 6173 7572 653f 7072 6f6a 6563  s/measure?projec
-00000a50: 743d 5175 6269 7450 695f 7065 6974 686f  t=QubitPi_peitho
-00000a60: 2d64 6174 6126 6d65 7472 6963 3d6e 636c  -data&metric=ncl
-00000a70: 6f63 295d 2868 7474 7073 3a2f 2f73 6f6e  oc)](https://son
-00000a80: 6172 636c 6f75 642e 696f 2f73 756d 6d61  arcloud.io/summa
-00000a90: 7279 2f6e 6577 5f63 6f64 653f 6964 3d51  ry/new_code?id=Q
-00000aa0: 7562 6974 5069 5f70 6569 7468 6f2d 6461  ubitPi_peitho-da
-00000ab0: 7461 290a 5b21 5b43 6f64 6520 536d 656c  ta).[![Code Smel
-00000ac0: 6c73 5d28 6874 7470 733a 2f2f 736f 6e61  ls](https://sona
-00000ad0: 7263 6c6f 7564 2e69 6f2f 6170 692f 7072  rcloud.io/api/pr
-00000ae0: 6f6a 6563 745f 6261 6467 6573 2f6d 6561  oject_badges/mea
-00000af0: 7375 7265 3f70 726f 6a65 6374 3d51 7562  sure?project=Qub
-00000b00: 6974 5069 5f70 6569 7468 6f2d 6461 7461  itPi_peitho-data
-00000b10: 266d 6574 7269 633d 636f 6465 5f73 6d65  &metric=code_sme
-00000b20: 6c6c 7329 5d28 6874 7470 733a 2f2f 736f  lls)](https://so
-00000b30: 6e61 7263 6c6f 7564 2e69 6f2f 7375 6d6d  narcloud.io/summ
-00000b40: 6172 792f 6e65 775f 636f 6465 3f69 643d  ary/new_code?id=
-00000b50: 5175 6269 7450 695f 7065 6974 686f 2d64  QubitPi_peitho-d
-00000b60: 6174 6129 0a5b 215b 4d61 696e 7461 696e  ata).[![Maintain
-00000b70: 6162 696c 6974 7920 5261 7469 6e67 5d28  ability Rating](
-00000b80: 6874 7470 733a 2f2f 736f 6e61 7263 6c6f  https://sonarclo
-00000b90: 7564 2e69 6f2f 6170 692f 7072 6f6a 6563  ud.io/api/projec
-00000ba0: 745f 6261 6467 6573 2f6d 6561 7375 7265  t_badges/measure
-00000bb0: 3f70 726f 6a65 6374 3d51 7562 6974 5069  ?project=QubitPi
-00000bc0: 5f70 6569 7468 6f2d 6461 7461 266d 6574  _peitho-data&met
-00000bd0: 7269 633d 7371 616c 655f 7261 7469 6e67  ric=sqale_rating
-00000be0: 295d 2868 7474 7073 3a2f 2f73 6f6e 6172  )](https://sonar
-00000bf0: 636c 6f75 642e 696f 2f73 756d 6d61 7279  cloud.io/summary
-00000c00: 2f6e 6577 5f63 6f64 653f 6964 3d51 7562  /new_code?id=Qub
-00000c10: 6974 5069 5f70 6569 7468 6f2d 6461 7461  itPi_peitho-data
-00000c20: 290a 5b21 5b53 6563 7572 6974 7920 5261  ).[![Security Ra
-00000c30: 7469 6e67 5d28 6874 7470 733a 2f2f 736f  ting](https://so
-00000c40: 6e61 7263 6c6f 7564 2e69 6f2f 6170 692f  narcloud.io/api/
-00000c50: 7072 6f6a 6563 745f 6261 6467 6573 2f6d  project_badges/m
-00000c60: 6561 7375 7265 3f70 726f 6a65 6374 3d51  easure?project=Q
-00000c70: 7562 6974 5069 5f70 6569 7468 6f2d 6461  ubitPi_peitho-da
-00000c80: 7461 266d 6574 7269 633d 7365 6375 7269  ta&metric=securi
-00000c90: 7479 5f72 6174 696e 6729 5d28 6874 7470  ty_rating)](http
-00000ca0: 733a 2f2f 736f 6e61 7263 6c6f 7564 2e69  s://sonarcloud.i
-00000cb0: 6f2f 7375 6d6d 6172 792f 6e65 775f 636f  o/summary/new_co
-00000cc0: 6465 3f69 643d 5175 6269 7450 695f 7065  de?id=QubitPi_pe
-00000cd0: 6974 686f 2d64 6174 6129 0a3c 2f64 6976  itho-data).</div
-00000ce0: 3e0a 0a3c 6469 7620 616c 6967 6e3d 2272  >..<div align="r
-00000cf0: 6967 6874 223e 0a0a 5b21 5b53 6f6e 6172  ight">..[![Sonar
-00000d00: 436c 6f75 645d 2868 7474 7073 3a2f 2f73  Cloud](https://s
-00000d10: 6f6e 6172 636c 6f75 642e 696f 2f69 6d61  onarcloud.io/ima
-00000d20: 6765 732f 7072 6f6a 6563 745f 6261 6467  ges/project_badg
-00000d30: 6573 2f73 6f6e 6172 636c 6f75 642d 6f72  es/sonarcloud-or
-00000d40: 616e 6765 2e73 7667 295d 2868 7474 7073  ange.svg)](https
-00000d50: 3a2f 2f73 6f6e 6172 636c 6f75 642e 696f  ://sonarcloud.io
-00000d60: 2f73 756d 6d61 7279 2f6e 6577 5f63 6f64  /summary/new_cod
-00000d70: 653f 6964 3d51 7562 6974 5069 5f70 6569  e?id=QubitPi_pei
-00000d80: 7468 6f2d 6461 7461 290a 0a3c 2f64 6976  tho-data)..</div
-00000d90: 3e0a 0a2a 2a5f 5065 6974 686f 2044 6174  >..**_Peitho Dat
-00000da0: 6120 6973 2075 6e64 6572 2064 6576 656c  a is under devel
-00000db0: 6f70 6d65 6e74 206d 6f64 652c 2062 7265  opment mode, bre
-00000dc0: 616b 696e 6720 6368 616e 6765 7320 6d69  aking changes mi
-00000dd0: 6768 7420 636f 6d65 2061 7420 7468 6973  ght come at this
-00000de0: 206d 6f6d 656e 742e 5f2a 2a0a 0a57 6861   moment._**..Wha
-00000df0: 7420 6973 2050 6569 7468 6f20 4461 7461  t is Peitho Data
-00000e00: 203c 7375 703e 215b 5079 7468 6f6e 2056   <sup>![Python V
-00000e10: 6572 7369 6f6e 2042 6164 6765 2069 7320  ersion Badge is 
-00000e20: 4d69 7373 696e 675d 2868 7474 7073 3a2f  Missing](https:/
-00000e30: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000e40: 6261 6467 652f 5079 7468 6f6e 2d33 2e31  badge/Python-3.1
-00000e50: 302d 6272 6967 6874 6772 6565 6e3f 7374  0-brightgreen?st
-00000e60: 796c 653d 666c 6174 2d73 7175 6172 6526  yle=flat-square&
-00000e70: 6c6f 676f 3d70 7974 686f 6e26 6c6f 676f  logo=python&logo
-00000e80: 436f 6c6f 723d 7768 6974 6529 3c2f 7375  Color=white)</su
-00000e90: 703e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  p>.-------------
-00000ea0: 2d2d 2d2d 2d2d 0a0a 3c61 2068 7265 663d  ------..<a href=
-00000eb0: 2268 7474 7073 3a2f 2f77 7777 2e62 696c  "https://www.bil
-00000ec0: 6962 696c 692e 636f 6d2f 7669 6465 6f2f  ibili.com/video/
-00000ed0: 4256 316b 6234 7931 6d37 6537 3f70 3d33  BV1kb4y1m7e7?p=3
-00000ee0: 223e 0a20 2020 203c 696d 6720 616c 6967  ">.    <img alig
-00000ef0: 6e3d 2272 6967 6874 2220 7769 6474 683d  n="right" width=
-00000f00: 2235 3025 2220 616c 743d 22e6 b0b8 e681  "50%" alt=".....
-00000f10: 9222 2073 7263 3d22 2e2f 7468 656d 652f  ." src="./theme/
-00000f20: e6b0 b8e6 8192 2e67 6966 223e 0a3c 2f61  .......gif">.</a
-00000f30: 3e0a 0a5b 5065 6974 686f 2044 6174 615d  >..[Peitho Data]
-00000f40: 2868 7474 7073 3a2f 2f70 6569 7468 6f2d  (https://peitho-
-00000f50: 6461 7461 2e72 6561 6474 6865 646f 6373  data.readthedocs
-00000f60: 2e69 6f2f 656e 2f6c 6174 6573 742f 2920  .io/en/latest/) 
-00000f70: 6973 2061 6e20 6f70 696e 696f 6e61 7465  is an opinionate
-00000f80: 6420 2a2a 6461 7461 2061 6e61 6c79 7469  d **data analyti
-00000f90: 6373 2a2a 2070 6163 6b61 6765 2074 6861  cs** package tha
-00000fa0: 7420 7465 616d 2063 616e 0a6c 6576 6572  t team can.lever
-00000fb0: 6167 6520 746f 2071 7569 636b 6c79 2069  age to quickly i
-00000fc0: 6e63 6f72 706f 7261 7465 2063 6170 6162  ncorporate capab
-00000fd0: 696c 6974 6965 7320 6f66 0a0a 2a20 4461  ilities of..* Da
-00000fe0: 7461 2041 6e61 6c79 7469 6373 2f56 6973  ta Analytics/Vis
-00000ff0: 7561 6c69 7a61 7469 6f6e 0a2a 204d 6163  ualization.* Mac
-00001000: 6869 6e65 204c 6561 726e 696e 670a 2a20  hine Learning.* 
-00001010: 4149 0a0a 0a44 6f63 756d 656e 7461 7469  AI...Documentati
-00001020: 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  on.-------------
-00001030: 0a0a 3c69 6d67 2073 7263 3d22 2e2f 7468  ..<img src="./th
-00001040: 656d 652f e99b b7e7 94b5 e5b0 86e5 869b  eme/............
-00001050: 2e70 6e67 2220 616c 743d 22e9 9bb7 e794  .png" alt=".....
-00001060: b5e5 b086 e586 9b2e 706e 6722 2077 6964  ........png" wid
-00001070: 7468 3d22 3525 223e 3c2f 696d 673e 0a5b  th="5%"></img>.[
-00001080: 5374 6172 7420 6578 706c 6f72 696e 6720  Start exploring 
-00001090: 5065 6974 686f 2044 6174 615d 2868 7474  Peitho Data](htt
-000010a0: 7073 3a2f 2f70 6569 7468 6f2d 6461 7461  ps://peitho-data
-000010b0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000010c0: 656e 2f6c 6174 6573 742f 290a 0a0a 4c69  en/latest/)...Li
-000010d0: 6365 6e73 650a 2d2d 2d2d 2d2d 2d0a 0a54  cense.-------..T
-000010e0: 6865 2075 7365 2061 6e64 2064 6973 7472  he use and distr
-000010f0: 6962 7574 696f 6e20 7465 726d 7320 666f  ibution terms fo
-00001100: 7220 5b50 6569 7468 6f20 4461 7461 5d28  r [Peitho Data](
-00001110: 6874 7470 733a 2f2f 7065 6974 686f 2d64  https://peitho-d
-00001120: 6174 612e 7265 6164 7468 6564 6f63 732e  ata.readthedocs.
-00001130: 696f 2f65 6e2f 6c61 7465 7374 2f29 2061  io/en/latest/) a
-00001140: 7265 2063 6f76 6572 6564 2062 7920 7468  re covered by th
-00001150: 650a 5b41 7061 6368 6520 4c69 6365 6e73  e.[Apache Licens
-00001160: 652c 2056 6572 7369 6f6e 2032 2e30 5d28  e, Version 2.0](
-00001170: 6874 7470 3a2f 2f77 7777 2e61 7061 6368  http://www.apach
-00001180: 652e 6f72 672f 6c69 6365 6e73 6573 2f4c  e.org/licenses/L
-00001190: 4943 454e 5345 2d32 2e30 2e68 746d 6c29  ICENSE-2.0.html)
-000011a0: 2e0a 0a3c 6469 7620 616c 6967 6e3d 2263  ...<div align="c
-000011b0: 656e 7465 7222 3e0a 2020 2020 3c61 2068  enter">.    <a h
-000011c0: 7265 663d 2268 7474 7073 3a2f 2f6f 7065  ref="https://ope
-000011d0: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
-000011e0: 6e73 6573 223e 0a20 2020 2020 2020 203c  nses">.        <
-000011f0: 696d 6720 616c 6967 6e3d 2263 656e 7465  img align="cente
-00001200: 7222 2077 6964 7468 3d22 3530 2522 2061  r" width="50%" a
-00001210: 6c74 3d22 4c69 6365 6e73 6520 496c 6c75  lt="License Illu
-00001220: 7374 7261 7469 6f6e 2220 7372 633d 2268  stration" src="h
-00001230: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001240: 6d2f 5175 6269 7450 692f 5175 6269 7450  m/QubitPi/QubitP
-00001250: 692f 626c 6f62 2f6d 6173 7465 722f 696d  i/blob/master/im
-00001260: 672f 6170 6163 6865 2d32 2e70 6e67 3f72  g/apache-2.png?r
-00001270: 6177 3d74 7275 6522 3e0a 2020 2020 3c2f  aw=true">.    </
-00001280: 613e 0a3c 2f64 6976 3e0a                 a>.</div>.
+00000930: 696f 2f61 7069 2f70 726f 6a65 6374 5f62  io/api/project_b
+00000940: 6164 6765 732f 6d65 6173 7572 653f 7072  adges/measure?pr
+00000950: 6f6a 6563 743d 5175 6269 7450 695f 7065  oject=QubitPi_pe
+00000960: 6974 686f 2d64 6174 6126 6d65 7472 6963  itho-data&metric
+00000970: 3d6e 636c 6f63 295d 2868 7474 7073 3a2f  =ncloc)](https:/
+00000980: 2f73 6f6e 6172 636c 6f75 642e 696f 2f73  /sonarcloud.io/s
+00000990: 756d 6d61 7279 2f6e 6577 5f63 6f64 653f  ummary/new_code?
+000009a0: 6964 3d51 7562 6974 5069 5f70 6569 7468  id=QubitPi_peith
+000009b0: 6f2d 6461 7461 290a 5b21 5b43 6f64 6520  o-data).[![Code 
+000009c0: 536d 656c 6c73 5d28 6874 7470 733a 2f2f  Smells](https://
+000009d0: 736f 6e61 7263 6c6f 7564 2e69 6f2f 6170  sonarcloud.io/ap
+000009e0: 692f 7072 6f6a 6563 745f 6261 6467 6573  i/project_badges
+000009f0: 2f6d 6561 7375 7265 3f70 726f 6a65 6374  /measure?project
+00000a00: 3d51 7562 6974 5069 5f70 6569 7468 6f2d  =QubitPi_peitho-
+00000a10: 6461 7461 266d 6574 7269 633d 636f 6465  data&metric=code
+00000a20: 5f73 6d65 6c6c 7329 5d28 6874 7470 733a  _smells)](https:
+00000a30: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
+00000a40: 7375 6d6d 6172 792f 6e65 775f 636f 6465  summary/new_code
+00000a50: 3f69 643d 5175 6269 7450 695f 7065 6974  ?id=QubitPi_peit
+00000a60: 686f 2d64 6174 6129 0a5b 215b 4d61 696e  ho-data).[![Main
+00000a70: 7461 696e 6162 696c 6974 7920 5261 7469  tainability Rati
+00000a80: 6e67 5d28 6874 7470 733a 2f2f 736f 6e61  ng](https://sona
+00000a90: 7263 6c6f 7564 2e69 6f2f 6170 692f 7072  rcloud.io/api/pr
+00000aa0: 6f6a 6563 745f 6261 6467 6573 2f6d 6561  oject_badges/mea
+00000ab0: 7375 7265 3f70 726f 6a65 6374 3d51 7562  sure?project=Qub
+00000ac0: 6974 5069 5f70 6569 7468 6f2d 6461 7461  itPi_peitho-data
+00000ad0: 266d 6574 7269 633d 7371 616c 655f 7261  &metric=sqale_ra
+00000ae0: 7469 6e67 295d 2868 7474 7073 3a2f 2f73  ting)](https://s
+00000af0: 6f6e 6172 636c 6f75 642e 696f 2f73 756d  onarcloud.io/sum
+00000b00: 6d61 7279 2f6e 6577 5f63 6f64 653f 6964  mary/new_code?id
+00000b10: 3d51 7562 6974 5069 5f70 6569 7468 6f2d  =QubitPi_peitho-
+00000b20: 6461 7461 290a 5b21 5b53 6563 7572 6974  data).[![Securit
+00000b30: 7920 5261 7469 6e67 5d28 6874 7470 733a  y Rating](https:
+00000b40: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
+00000b50: 6170 692f 7072 6f6a 6563 745f 6261 6467  api/project_badg
+00000b60: 6573 2f6d 6561 7375 7265 3f70 726f 6a65  es/measure?proje
+00000b70: 6374 3d51 7562 6974 5069 5f70 6569 7468  ct=QubitPi_peith
+00000b80: 6f2d 6461 7461 266d 6574 7269 633d 7365  o-data&metric=se
+00000b90: 6375 7269 7479 5f72 6174 696e 6729 5d28  curity_rating)](
+00000ba0: 6874 7470 733a 2f2f 736f 6e61 7263 6c6f  https://sonarclo
+00000bb0: 7564 2e69 6f2f 7375 6d6d 6172 792f 6e65  ud.io/summary/ne
+00000bc0: 775f 636f 6465 3f69 643d 5175 6269 7450  w_code?id=QubitP
+00000bd0: 695f 7065 6974 686f 2d64 6174 6129 0a0a  i_peitho-data)..
+00000be0: 3c2f 6469 763e 0a0a 3c64 6976 2061 6c69  </div>..<div ali
+00000bf0: 676e 3d22 7269 6768 7422 3e0a 0a5b 215b  gn="right">..[![
+00000c00: 536f 6e61 7243 6c6f 7564 5d28 6874 7470  SonarCloud](http
+00000c10: 733a 2f2f 736f 6e61 7263 6c6f 7564 2e69  s://sonarcloud.i
+00000c20: 6f2f 696d 6167 6573 2f70 726f 6a65 6374  o/images/project
+00000c30: 5f62 6164 6765 732f 736f 6e61 7263 6c6f  _badges/sonarclo
+00000c40: 7564 2d6f 7261 6e67 652e 7376 6729 5d28  ud-orange.svg)](
+00000c50: 6874 7470 733a 2f2f 736f 6e61 7263 6c6f  https://sonarclo
+00000c60: 7564 2e69 6f2f 7375 6d6d 6172 792f 6e65  ud.io/summary/ne
+00000c70: 775f 636f 6465 3f69 643d 5175 6269 7450  w_code?id=QubitP
+00000c80: 695f 7065 6974 686f 2d64 6174 6129 0a0a  i_peitho-data)..
+00000c90: 3c2f 6469 763e 0a0a 2a2a 5f50 6569 7468  </div>..**_Peith
+00000ca0: 6f20 4461 7461 2069 7320 756e 6465 7220  o Data is under 
+00000cb0: 6465 7665 6c6f 706d 656e 7420 6d6f 6465  development mode
+00000cc0: 2c20 6272 6561 6b69 6e67 2063 6861 6e67  , breaking chang
+00000cd0: 6573 206d 6967 6874 2063 6f6d 6520 6174  es might come at
+00000ce0: 2074 6869 7320 6d6f 6d65 6e74 2e5f 2a2a   this moment._**
+00000cf0: 0a0a 5768 6174 2069 7320 5065 6974 686f  ..What is Peitho
+00000d00: 2044 6174 6120 3c73 7570 3e21 5b50 7974   Data <sup>![Pyt
+00000d10: 686f 6e20 5665 7273 696f 6e20 4261 6467  hon Version Badg
+00000d20: 6520 6973 204d 6973 7369 6e67 5d28 6874  e is Missing](ht
+00000d30: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000d40: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
+00000d50: 6e2d 332e 3130 2d62 7269 6768 7467 7265  n-3.10-brightgre
+00000d60: 656e 3f73 7479 6c65 3d66 6c61 742d 7371  en?style=flat-sq
+00000d70: 7561 7265 266c 6f67 6f3d 7079 7468 6f6e  uare&logo=python
+00000d80: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00000d90: 293c 2f73 7570 3e0a 2d2d 2d2d 2d2d 2d2d  )</sup>.--------
+00000da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a5b 5065  -----------..[Pe
+00000db0: 6974 686f 2044 6174 615d 2868 7474 7073  itho Data](https
+00000dc0: 3a2f 2f70 6569 7468 6f2d 6461 7461 2e72  ://peitho-data.r
+00000dd0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000de0: 2f6c 6174 6573 742f 2920 6973 2061 6e20  /latest/) is an 
+00000df0: 6f70 696e 696f 6e61 7465 6420 2a2a 6461  opinionated **da
+00000e00: 7461 2061 6e61 6c79 7469 6373 2a2a 2070  ta analytics** p
+00000e10: 6163 6b61 6765 2074 6861 7420 7465 616d  ackage that team
+00000e20: 2063 616e 0a6c 6576 6572 6167 6520 746f   can.leverage to
+00000e30: 2071 7569 636b 6c79 2069 6e63 6f72 706f   quickly incorpo
+00000e40: 7261 7465 2063 6170 6162 696c 6974 6965  rate capabilitie
+00000e50: 7320 6f66 0a0a 2a20 4461 7461 2041 6e61  s of..* Data Ana
+00000e60: 6c79 7469 6373 2f56 6973 7561 6c69 7a61  lytics/Visualiza
+00000e70: 7469 6f6e 0a2a 204d 6163 6869 6e65 204c  tion.* Machine L
+00000e80: 6561 726e 696e 670a 2a20 4149 0a0a 0a44  earning.* AI...D
+00000e90: 6f63 756d 656e 7461 7469 6f6e 0a2d 2d2d  ocumentation.---
+00000ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 3c69 6d67  ----------..<img
+00000eb0: 2073 7263 3d22 2e2f 7468 656d 652f e99b   src="./theme/..
+00000ec0: b7e7 94b5 e5b0 86e5 869b 2e70 6e67 2220  ...........png" 
+00000ed0: 616c 743d 22e9 9bb7 e794 b5e5 b086 e586  alt="...........
+00000ee0: 9b2e 706e 6722 2077 6964 7468 3d22 3525  ..png" width="5%
+00000ef0: 223e 3c2f 696d 673e 0a5b 5374 6172 7420  "></img>.[Start 
+00000f00: 6578 706c 6f72 696e 6720 5065 6974 686f  exploring Peitho
+00000f10: 2044 6174 615d 2868 7474 7073 3a2f 2f70   Data](https://p
+00000f20: 6569 7468 6f2d 6461 7461 2e72 6561 6474  eitho-data.readt
+00000f30: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000f40: 6573 742f 290a 0a0a 4c69 6365 6e73 650a  est/)...License.
+00000f50: 2d2d 2d2d 2d2d 2d0a 0a54 6865 2075 7365  -------..The use
+00000f60: 2061 6e64 2064 6973 7472 6962 7574 696f   and distributio
+00000f70: 6e20 7465 726d 7320 666f 7220 5b50 6569  n terms for [Pei
+00000f80: 7468 6f20 4461 7461 5d28 6874 7470 733a  tho Data](https:
+00000f90: 2f2f 7065 6974 686f 2d64 6174 612e 7265  //peitho-data.re
+00000fa0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000fb0: 6c61 7465 7374 2f29 2061 7265 2063 6f76  latest/) are cov
+00000fc0: 6572 6564 2062 7920 7468 650a 5b41 7061  ered by the.[Apa
+00000fd0: 6368 6520 4c69 6365 6e73 652c 2056 6572  che License, Ver
+00000fe0: 7369 6f6e 2032 2e30 5d28 6874 7470 3a2f  sion 2.0](http:/
+00000ff0: 2f77 7777 2e61 7061 6368 652e 6f72 672f  /www.apache.org/
+00001000: 6c69 6365 6e73 6573 2f4c 4943 454e 5345  licenses/LICENSE
+00001010: 2d32 2e30 2e68 746d 6c29 2e0a 0a3c 6469  -2.0.html)...<di
+00001020: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00001030: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00001040: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
+00001050: 652e 6f72 672f 6c69 6365 6e73 6573 223e  e.org/licenses">
+00001060: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+00001070: 6967 6e3d 2263 656e 7465 7222 2077 6964  ign="center" wid
+00001080: 7468 3d22 3530 2522 2061 6c74 3d22 4c69  th="50%" alt="Li
+00001090: 6365 6e73 6520 496c 6c75 7374 7261 7469  cense Illustrati
+000010a0: 6f6e 2220 7372 633d 2268 7474 7073 3a2f  on" src="https:/
+000010b0: 2f67 6974 6875 622e 636f 6d2f 5175 6269  /github.com/Qubi
+000010c0: 7450 692f 5175 6269 7450 692f 626c 6f62  tPi/QubitPi/blob
+000010d0: 2f6d 6173 7465 722f 696d 672f 6170 6163  /master/img/apac
+000010e0: 6865 2d32 2e70 6e67 3f72 6177 3d74 7275  he-2.png?raw=tru
+000010f0: 6522 3e0a 2020 2020 3c2f 613e 0a3c 2f64  e">.    </a>.</d
+00001100: 6976 3e0a                                iv>.
```

### Comparing `peitho_data-2.3.7/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.3.8/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/datafication/epub.py` & `peitho_data-2.3.8/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.3.8/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/machine_learning/cnn/image_convolution.py` & `peitho_data-2.3.8/peitho_data/machine_learning/cnn/image_convolution.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.3.8/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/datafication/test_epub.py` & `peitho_data-2.3.8/peitho_data/tests/datafication/test_epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.3.8/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/machine_learning/cnn/test_image_convolution.py` & `peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/test_image_convolution.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.3.8/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/test_trello_api.py` & `peitho_data-2.3.8/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.3.8/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/trello_api.py` & `peitho_data-2.3.8/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data/word_cloud.py` & `peitho_data-2.3.8/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.3.8/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.7/setup.py` & `peitho_data-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.3.7",
+    version="2.3.8",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

