# Comparing `tmp/matgl-0.6.2.tar.gz` & `tmp/matgl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.6.2.tar", last modified: Wed Jun 21 19:18:20 2023, max compression
+gzip compressed data, was "matgl-0.7.0.tar", last modified: Sun Jun 25 23:04:09 2023, max compression
```

## Comparing `matgl-0.6.2.tar` & `matgl-0.7.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.542799 matgl-0.6.2/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.6.2/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    13333 2023-06-21 19:18:20.542518 matgl-0.6.2/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)    12164 2023-06-21 19:17:01.000000 matgl-0.6.2/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.535259 matgl-0.6.2/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.537043 matgl-0.6.2/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4160 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     4150 2023-06-21 19:11:05.000000 matgl-0.6.2/matgl/cli.py
--rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.537363 matgl-0.6.2/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.537818 matgl-0.6.2/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15933 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5278 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.538713 matgl-0.6.2/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5133 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11614 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.540330 matgl-0.6.2/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2037 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     2983 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3944 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.540977 matgl-0.6.2/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11557 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9142 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.541953 matgl-0.6.2/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10520 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    13296 2023-06-21 14:46:11.000000 matgl-0.6.2/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.536236 matgl-0.6.2/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    13333 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1024 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       39 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/entry_points.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-21 19:18:20.000000 matgl-0.6.2/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.6.2/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-21 19:18:20.542886 matgl-0.6.2/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2119 2023-06-21 19:17:13.000000 matgl-0.6.2/setup.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 19:18:20.542091 matgl-0.6.2/tests/
--rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 14:49:26.000000 matgl-0.6.2/tests/test_config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145969 matgl-0.7.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-04-22 15:15:07.000000 matgl-0.7.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    13724 2023-06-25 23:04:09.145716 matgl-0.7.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)    12555 2023-06-25 22:56:34.000000 matgl-0.7.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.140653 matgl-0.7.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141721 matgl-0.7.0/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4221 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4777 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/cli.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-15 14:38:52.000000 matgl-0.7.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141961 matgl-0.7.0/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2542 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.142309 matgl-0.7.0/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15658 2023-06-25 22:58:13.000000 matgl-0.7.0/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4875 2023-06-25 22:58:47.000000 matgl-0.7.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.142736 matgl-0.7.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5188 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2232 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11720 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.143806 matgl-0.7.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      716 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2037 2023-06-21 20:31:41.000000 matgl-0.7.0/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2996 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12641 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2231 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3578 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3935 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4053 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.144202 matgl-0.7.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11949 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9153 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2255 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145199 matgl-0.7.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1372 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10549 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-04-22 15:15:07.000000 matgl-0.7.0/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    13462 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141498 matgl-0.7.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    13724 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1024 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       39 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/entry_points.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2530 2023-06-25 22:56:34.000000 matgl-0.7.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-25 23:04:09.146019 matgl-0.7.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2014 2023-06-25 23:01:46.000000 matgl-0.7.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145310 matgl-0.7.0/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 15:33:33.000000 matgl-0.7.0/tests/test_config.py
```

### Comparing `matgl-0.6.2/LICENSE` & `matgl-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/PKG-INFO` & `matgl-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.6.2
+Version: 0.7.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -24,51 +24,60 @@
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+# Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
-# Materials Graph Library
+## Official Documentation [:books:]
 
-### Official Documentation: [:books:][doc]
+<https://matgl.ai>
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
-natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
-shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
+exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
-and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
-The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
-over the TF implementations:
+MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
+applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
+learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
+[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
+usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
 
 - A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
+- Multi-GPU support via PyTorch Lightning.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
-Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
+Nassar, Carmelo Gonzales).
 
 ## Status
 
-Major milestones are summarized below. Please refer to [change log][changelog] for details.
+Major milestones are summarized below. Please refer to the [changelog] for details.
 
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
-## Architectures
+## Current Architectures
+
+Here, we summarize the currently implemented architectures in MatGL. It should be stressed that this is by no means
+an exhaustive list, and we expect new architectures to be added by the core MatGL team as well as other contributors
+in future.
+
+<div style="float: left; padding: 10px; width: 300px">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
+<p>Figure: Schematic of M3GNet/MEGNet</p>
+</div>
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ### MEGNet
 
 [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
@@ -107,40 +116,40 @@
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available.
 
-### From the command line (from v0.6.2)
+### Command line (from v0.6.2)
 
 A CLI tool now provides the capability to perform quick relaxations or predictions using pre-trained models, as well
 as other simple administrative tasks (e.g., clearing the cache). Some simple examples:
 
 1. To perform a relaxation,
 
     ```bash
-    mgl relax -i Li2O.cif -o Li2O_relax.cif
+    mgl relax --infile Li2O.cif --outfile Li2O_relax.cif
     ```
 
 2. To use one of the pre-trained property models,
 
     ```bash
-    mgl predict -m M3GNet-MP-2018.6.1-Eform -i Li2O.cif
+    mgl predict --model M3GNet-MP-2018.6.1-Eform --infile Li2O.cif
     ```
 
 3. To clear the cache,
 
     ```bash
     mgl clear
     ```
 
 For a full range of options, use `mgl -h`.
 
-### In code
+### Code
 
 Users who just want to use the models out of the box should use the newly implemented `matgl.load_model` convenience
 method. The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -158,21 +167,21 @@
 ```python
 import matgl
 print(matgl.get_available_pretrained_models())
 ```
 
 ## Tutorials
 
-A set of [tutorials][tutorials] have been written on the use of MatGL. These were generated from [Jupyter notebooks]
-[jupyternb], which can be directly run on [Google Colab][colab].
+We wrote [tutorials] on how to use MatGL. These were generated from [Jupyter notebooks]
+[jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
-- [API documentation][apidocs] for all classes and methods.
-- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+- [API docs][apidocs] for all classes and methods.
+- [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
@@ -189,27 +198,27 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original TensorFlow (TF) implementation!**
 
    _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
    _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
-   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   ensure the best implementation. This can usually be solved by updating your `matgl` to the latest version
    and clearing your cache using the following command `mgl clear`. On the next run, the latest model will be
    downloaded. With effect from v0.5.2, we have implemented a model versioning scheme that will detect code vs model
    version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
    _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
@@ -245,17 +254,17 @@
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
 [changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
-[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
-[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mfimegnet]: https://nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
-[colab]: https://colab.research.google.com/ "Google Colab"
+[google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
```

### Comparing `matgl-0.6.2/README.md` & `matgl-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+# Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
-# Materials Graph Library
+## Official Documentation [:books:]
 
-### Official Documentation: [:books:][doc]
+<https://matgl.ai>
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
-natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
-shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
+exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
-and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
-The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
-over the TF implementations:
+MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
+applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
+learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
+[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
+usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
 
 - A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
+- Multi-GPU support via PyTorch Lightning.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
-Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
+Nassar, Carmelo Gonzales).
 
 ## Status
 
-Major milestones are summarized below. Please refer to [change log][changelog] for details.
+Major milestones are summarized below. Please refer to the [changelog] for details.
 
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
-## Architectures
+## Current Architectures
+
+Here, we summarize the currently implemented architectures in MatGL. It should be stressed that this is by no means
+an exhaustive list, and we expect new architectures to be added by the core MatGL team as well as other contributors
+in future.
+
+<div style="float: left; padding: 10px; width: 300px">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
+<p>Figure: Schematic of M3GNet/MEGNet</p>
+</div>
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ### MEGNet
 
 [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
@@ -83,40 +92,40 @@
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available.
 
-### From the command line (from v0.6.2)
+### Command line (from v0.6.2)
 
 A CLI tool now provides the capability to perform quick relaxations or predictions using pre-trained models, as well
 as other simple administrative tasks (e.g., clearing the cache). Some simple examples:
 
 1. To perform a relaxation,
 
     ```bash
-    mgl relax -i Li2O.cif -o Li2O_relax.cif
+    mgl relax --infile Li2O.cif --outfile Li2O_relax.cif
     ```
 
 2. To use one of the pre-trained property models,
 
     ```bash
-    mgl predict -m M3GNet-MP-2018.6.1-Eform -i Li2O.cif
+    mgl predict --model M3GNet-MP-2018.6.1-Eform --infile Li2O.cif
     ```
 
 3. To clear the cache,
 
     ```bash
     mgl clear
     ```
 
 For a full range of options, use `mgl -h`.
 
-### In code
+### Code
 
 Users who just want to use the models out of the box should use the newly implemented `matgl.load_model` convenience
 method. The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -134,21 +143,21 @@
 ```python
 import matgl
 print(matgl.get_available_pretrained_models())
 ```
 
 ## Tutorials
 
-A set of [tutorials][tutorials] have been written on the use of MatGL. These were generated from [Jupyter notebooks]
-[jupyternb], which can be directly run on [Google Colab][colab].
+We wrote [tutorials] on how to use MatGL. These were generated from [Jupyter notebooks]
+[jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
-- [API documentation][apidocs] for all classes and methods.
-- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+- [API docs][apidocs] for all classes and methods.
+- [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
@@ -165,27 +174,27 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original TensorFlow (TF) implementation!**
 
    _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
    _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
-   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   ensure the best implementation. This can usually be solved by updating your `matgl` to the latest version
    and clearing your cache using the following command `mgl clear`. On the next run, the latest model will be
    downloaded. With effect from v0.5.2, we have implemented a model versioning scheme that will detect code vs model
    version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
    _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
@@ -221,17 +230,17 @@
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
 [changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
-[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
-[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mfimegnet]: https://nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
-[colab]: https://colab.research.google.com/ "Google Colab"
+[google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
```

### Comparing `matgl-0.6.2/matgl/apps/pes.py` & `matgl-0.7.0/matgl/apps/pes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Implementation of Interatomic Potentials."""
 from __future__ import annotations
 
-import dgl
-import numpy as np
+from typing import TYPE_CHECKING
+
 import torch
 from torch import nn
 from torch.autograd import grad
 
 from matgl.layers import AtomRef
 from matgl.utils.io import IOMixIn
 
+if TYPE_CHECKING:
+    import dgl
+    import numpy as np
+
 
 class Potential(nn.Module, IOMixIn):
     """A class representing an interatomic potential."""
 
     __version__ = 1
 
     def __init__(
```

### Comparing `matgl-0.6.2/matgl/cli.py` & `matgl-0.7.0/matgl/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import argparse
 import logging
 import os
 import sys
 import warnings
 
 from pymatgen.core.structure import Structure
+from pymatgen.ext.matproj import MPRester
 
 import matgl
 from matgl.ext.ase import Relaxer
 
 warnings.simplefilter("ignore")
 logger = logging.getLogger("MGL")
 
@@ -56,18 +57,25 @@
     """
     Use MatGL models to perform predictions on structures.
 
     Args:
         args: Args from CLI.
     """
     model = matgl.load_model(args.model)
-    for f in args.infile:
-        structure = Structure.from_file(f)
-        val = model.predict_structure(structure)
-        print(f"{args.model} prediction for {f}: {val}.")
+    if args.infile:
+        for f in args.infile:
+            structure = Structure.from_file(f)
+            val = model.predict_structure(structure)
+            print(f"{args.model} prediction for {f}: {val}.")
+    if args.mpids:
+        mpr = MPRester()
+        for mid in args.mpids:
+            structure = mpr.get_structure_by_material_id(mid)
+            val = model.predict_structure(structure)
+            print(f"{args.model} prediction for {mid} ({structure.composition.reduced_formula}): {val}.")
 
 
 def clear_cache(args):
     """
     Clear cache command.
 
     Args:
@@ -122,28 +130,37 @@
         help="Output filename.",
     )
 
     p_relax.set_defaults(func=relax_structure)
 
     p_predict = subparsers.add_parser("predict", help="Perform a prediction with pre-trained models.")
 
-    p_predict.add_argument(
+    groups = p_predict.add_mutually_exclusive_group(required=True)
+    groups.add_argument(
+        "-p",
+        "--mpids",
+        dest="mpids",
+        nargs="+",
+        help="Materials Project IDs. Requires mp-api to be installed and set up.",
+    )
+
+    groups.add_argument(
         "-i",
         "--infile",
         dest="infile",
         nargs="+",
-        required=True,
         help="Input files containing structure. Any format supported by pymatgen's Structure.from_file method.",
     )
 
     p_predict.add_argument(
         "-m",
         "--model",
         dest="model",
         choices=matgl.get_available_pretrained_models(),
+        required=True,
         help="Model to use",
     )
 
     p_predict.set_defaults(func=predict_structure)
 
     p_clear = subparsers.add_parser("clear", help="Clear cache.")
```

### Comparing `matgl-0.6.2/matgl/config.py` & `matgl-0.7.0/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/data/transformer.py` & `matgl-0.7.0/matgl/data/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,18 @@
         raise NotImplementedError
 
 
 class Normalizer(Transformer):
     """Performs a scaling of the data by centering to the mean and dividing by the standard deviation."""
 
     def __init__(self, mean: float, std: float):
-        """Args:
-        mean: Mean of the data
-        std: Standard deviation of the data.
+        """
+        Args:
+            mean: Mean of the data
+            std: Standard deviation of the data.
         """
         self.mean = mean
         self.std = std
 
     def transform(self, data):
         """z-score the data by subtracting the mean and dividing by the standard deviation.
 
@@ -64,15 +65,16 @@
 
         Returns:
             Unscaled data
         """
         return data * self.std + self.mean
 
     def __repr__(self):
-        return f"Normalizer: Mean={self.mean}, Std: {self.std}"
+        mean, std = self.mean, self.std
+        return f"Normalizer({mean=}, {std=})"
 
     @classmethod
     def from_data(cls, data):
         """Create Normalizer from data.
 
         Args:
             data: Input data.
```

### Comparing `matgl-0.6.2/matgl/ext/ase.py` & `matgl-0.7.0/matgl/ext/ase.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 
 from __future__ import annotations
 
 import contextlib
 import io
 import pickle
 import sys
+from typing import TYPE_CHECKING
 
-import dgl
 import numpy as np
 import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes
 from ase.constraints import ExpCellFilter
-from ase.io import Trajectory
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen, NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from ase.optimize.bfgs import BFGS
 from ase.optimize.bfgslinesearch import BFGSLineSearch
 from ase.optimize.fire import FIRE
 from ase.optimize.lbfgs import LBFGS, LBFGSLineSearch
 from ase.optimize.mdmin import MDMin
-from ase.optimize.optimize import Optimizer
 from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
-from dgl.backend import tensor
 from pymatgen.core.structure import Molecule, Structure
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.optimization.neighbors import find_points_in_spheres
 
-from matgl.apps.pes import Potential
 from matgl.graph.converters import GraphConverter
 
+if TYPE_CHECKING:
+    import dgl
+    from ase.io import Trajectory
+    from ase.optimize.optimize import Optimizer
+
+    from matgl.apps.pes import Potential
+
 OPTIMIZERS = {
     "FIRE": FIRE,
     "BFGS": BFGS,
     "LBFGS": LBFGS,
     "LBFGSLineSearch": LBFGSLineSearch,
     "MDMin": MDMin,
     "SciPyFminCG": SciPyFminCG,
@@ -71,15 +74,14 @@
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
         Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
-        atomic_number = np.array(atoms.get_atomic_numbers())
         lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
         volume = atoms.get_volume()
         cart_coords = np.ascontiguousarray(np.array(atoms.get_positions()), dtype=float)
         src_id, dst_id, images, bond_dist = find_points_in_spheres(
             cart_coords,
             cart_coords,
             r=self.cutoff,
@@ -90,24 +92,25 @@
         exclude_self = (src_id != dst_id) | (bond_dist > numerical_tol)
         src_id, dst_id, images, bond_dist = (
             src_id[exclude_self],
             dst_id[exclude_self],
             images[exclude_self],
             bond_dist[exclude_self],
         )
-        u, v = tensor(src_id), tensor(dst_id)
-        g = dgl.graph((u, v))
-        g.edata["pbc_offset"] = torch.tensor(images)
-        g.edata["lattice"] = tensor(np.stack([lattice_matrix for _ in range(g.num_edges())]))
-        g.ndata["attr"] = tensor(Z)
-        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(i.symbol)] for i in atoms]))
-        g.ndata["pos"] = tensor(cart_coords)
-        g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
-        state_attr = [0.0, 0.0]
-        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
+        g, state_attr = super().get_graph_from_processed_structure(
+            AseAtomsAdaptor().get_structure(atoms),
+            src_id,
+            dst_id,
+            images,
+            [lattice_matrix],
+            Z,
+            element_types,
+            cart_coords,
+        )
+        g.ndata["volume"] = torch.tensor([volume] * g.num_nodes())
         return g, state_attr
 
 
 class M3GNetCalculator(Calculator):
     """M3GNet calculator for ASE."""
 
     implemented_properties = ("energy", "free_energy", "forces", "stress", "hessian")
```

### Comparing `matgl-0.6.2/matgl/ext/pymatgen.py` & `matgl-0.7.0/matgl/ext/pymatgen.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Interface with pymatgen objects."""
 from __future__ import annotations
 
-import dgl
+from typing import TYPE_CHECKING
+
 import numpy as np
 import scipy.sparse as sp
 import torch
-from dgl.backend import tensor
 from pymatgen.core import Element, Molecule, Structure
 from pymatgen.optimization.neighbors import find_points_in_spheres
 
 from matgl.graph.converters import GraphConverter
 
+if TYPE_CHECKING:
+    import dgl
+
 
 def get_element_list(train_structures: list[Structure | Molecule]) -> tuple[str]:
     """Get the dictionary containing elements in the training set for atomic features.
 
     Args:
         train_structures: pymatgen Molecule/Structure object
 
@@ -58,25 +61,25 @@
         weight = mol.composition.weight / len(mol)
         dist = np.linalg.norm(R[:, None, :] - R[None, :, :], axis=-1)
         dists = mol.distance_matrix.flatten()
         nbonds = (np.count_nonzero(dists <= self.cutoff) - natoms) / 2
         nbonds /= natoms
         adj = sp.csr_matrix(dist <= self.cutoff) - sp.eye(natoms, dtype=np.bool_)
         adj = adj.tocoo()
-        u, v = tensor(adj.row), tensor(adj.col)
-        g = dgl.graph((u, v))
-        g = dgl.to_bidirected(g)
-        g.ndata["pos"] = tensor(R)
-        g.ndata["attr"] = tensor(Z)
-        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in mol]))
-        g.edata["pbc_offset"] = torch.zeros(g.num_edges(), 3)
-        g.edata["lattice"] = torch.zeros(g.num_edges(), 3, 3)
+        g, _ = super().get_graph_from_processed_structure(
+            structure=mol,
+            src_id=adj.row,
+            dst_id=adj.col,
+            images=torch.zeros(len(adj.row), 3),
+            lattice_matrix=torch.zeros(1, 3, 3),
+            Z=Z,
+            element_types=element_types,
+            cart_coords=R,
+        )
         state_attr = [weight, nbonds]
-        g.edata["pbc_offshift"] = torch.zeros(g.num_edges(), 3)
-
         return g, state_attr
 
 
 class Structure2Graph(GraphConverter):
     """Construct a DGL graph from Pymatgen Structure."""
 
     def __init__(
@@ -101,15 +104,14 @@
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
         Z = np.array([np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in structure])
-        atomic_number = np.array([site.specie.Z for site in structure])
         lattice_matrix = np.ascontiguousarray(np.array(structure.lattice.matrix), dtype=float)
         volume = structure.volume
         cart_coords = np.ascontiguousarray(np.array(structure.cart_coords), dtype=float)
         src_id, dst_id, images, bond_dist = find_points_in_spheres(
             cart_coords,
             cart_coords,
             r=self.cutoff,
@@ -120,17 +122,19 @@
         exclude_self = (src_id != dst_id) | (bond_dist > numerical_tol)
         src_id, dst_id, images, bond_dist = (
             src_id[exclude_self],
             dst_id[exclude_self],
             images[exclude_self],
             bond_dist[exclude_self],
         )
-        u, v = tensor(src_id), tensor(dst_id)
-        g = dgl.graph((u, v))
-        g.edata["pbc_offset"] = torch.tensor(images)
-        g.edata["lattice"] = tensor(np.stack([lattice_matrix for _ in range(g.num_edges())]))
-        g.ndata["attr"] = tensor(Z)
-        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
-        g.ndata["pos"] = tensor(cart_coords)
-        g.ndata["volume"] = tensor([volume for _ in range(atomic_number.shape[0])])
-        state_attr = [0.0, 0.0]
+        g, state_attr = super().get_graph_from_processed_structure(
+            structure,
+            src_id,
+            dst_id,
+            images,
+            [lattice_matrix],
+            Z,
+            element_types,
+            cart_coords,
+        )
+        g.ndata["volume"] = torch.tensor([volume] * g.num_nodes())
         return g, state_attr
```

### Comparing `matgl-0.6.2/matgl/graph/compute.py` & `matgl-0.7.0/matgl/graph/compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,20 @@
     for n in n_atoms:
         j = i + n
         n_triple_s.append(torch.sum(n_triple_i[i:j]))
         i = j
 
     src_id, dst_id = (triple_bond_indices[:, 0], triple_bond_indices[:, 1])
     l_g = dgl.graph((src_id, dst_id))
-    l_g.ndata["bond_dist"] = g.edata["bond_dist"]
-    l_g.ndata["bond_vec"] = g.edata["bond_vec"]
-    l_g.ndata["pbc_offset"] = g.edata["pbc_offset"]
-    l_g.ndata["n_triple_ij"] = n_triple_ij
+    three_body_id = np.unique(triple_bond_indices)
+    max_three_body_id = max(np.concatenate([three_body_id + 1, [0]]))
+    l_g.ndata["bond_dist"] = g.edata["bond_dist"][:max_three_body_id]
+    l_g.ndata["bond_vec"] = g.edata["bond_vec"][:max_three_body_id]
+    l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][:max_three_body_id]
+    l_g.ndata["n_triple_ij"] = n_triple_ij[:max_three_body_id]
     n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)  # type: ignore
     return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
 
 def compute_pair_vector_and_distance(g: dgl.DGLGraph):
     """Calculate bond vectors and distances using dgl graphs.
 
@@ -120,20 +122,18 @@
 
     Returns:
         l_g: DGL graph containing three body information from graph
     """
     g_unbatched = dgl.unbatch(g_batched)
     l_g_unbatched = []
     for g in g_unbatched:
-        if g.edges()[0].size(dim=0) > 0:
-            valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
-            src_id_with_three_body = g.edges()[0][valid_three_body]
-            dst_id_with_three_body = g.edges()[1][valid_three_body]
-            graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
-            graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
-            graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
-            graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
-        if graph_with_three_body.edata["bond_dist"].size(dim=0) > 0:
-            l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
-            l_g_unbatched.append(l_g)
+        valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
+        src_id_with_three_body = g.edges()[0][valid_three_body]
+        dst_id_with_three_body = g.edges()[1][valid_three_body]
+        graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
+        graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
+        graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
+        graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
+        l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
+        l_g_unbatched.append(l_g)
     l_g_batched = dgl.batch(l_g_unbatched)
     return l_g_batched
```

### Comparing `matgl-0.6.2/matgl/graph/data.py` & `matgl-0.7.0/matgl/graph/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,25 +113,26 @@
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
         name: str = "MEGNETDataset",
         graph_labels: list | None = None,
     ):
-        """Args:
-        structures: Pymatgen strutcure
-        labels: property values
-        label_name: label name
-        converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
-        initial: initial distance for Gaussian expansions
-        final: final distance for Gaussian expansions
-        num_centers: number of Gaussian functions
-        width: width of Gaussian functions
-        name: Name of dataset
-        graph_labels: graph attributes either integers and floating point numbers.
+        """
+        Args:
+            structures: Pymatgen structure
+            labels: property values
+            label_name: label name
+            converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
+            initial: initial distance for Gaussian expansions
+            final: final distance for Gaussian expansions
+            num_centers: number of Gaussian functions
+            width: width of Gaussian functions
+            name: Name of dataset
+            graph_labels: graph attributes either integers and floating point numbers.
         """
         self.converter = converter
         self.structures = structures
         self.labels = torch.FloatTensor(labels)
         self.label_name = label_name
         self.initial = initial
         self.final = final
@@ -213,23 +214,24 @@
         forces: list,
         stresses: None | list,
         converter: GraphConverter,
         threebody_cutoff: float,
         name="M3GNETDataset",
         graph_labels: list | None = None,
     ):
-        """Args:
-        structures: Pymatgen strutcure
-        energies: Target energies
-        forces: Target forces
-        stresses: Target stresses
-        converter: dgl graph converter
-        threebody_cutoff: cutoff for three body
-        name: name of dataset
-        graph_labels: state attributes.
+        """
+        Args:
+            structures: Pymatgen structure
+            energies: Target energies
+            forces: Target forces
+            stresses: Target stresses
+            converter: dgl graph converter
+            threebody_cutoff: cutoff for three body
+            name: name of dataset
+            graph_labels: state attributes.
         """
         self.converter = converter
         self.structures = structures
         self.energies = energies
         self.forces = forces
         self.threebody_cutoff = threebody_cutoff
         self.stresses = np.zeros(len(self.energies)) if stresses is None else stresses
@@ -314,14 +316,14 @@
     def __getitem__(self, idx: int):
         """Get graph and label with idx."""
         return (
             self.graphs[idx],
             self.line_graphs[idx],
             self.state_attr[idx],
             self.energies[idx],
-            torch.tensor(self.forces[idx]),
-            torch.tensor(self.stresses[idx]),  # type: ignore
+            torch.tensor(self.forces[idx]).float(),
+            torch.tensor(self.stresses[idx]).float(),  # type: ignore
         )
 
     def __len__(self):
         """Get size of dataset."""
         return len(self.graphs)
```

### Comparing `matgl-0.6.2/matgl/layers/__init__.py` & `matgl-0.7.0/matgl/layers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This package implements the layers for M*GNet."""
 from __future__ import annotations
 
 from matgl.layers._activations import SoftExponential, SoftPlus2
 from matgl.layers._atom_ref import AtomRef
-from matgl.layers._basis import SphericalBesselWithHarmonics
+from matgl.layers._basis import FourierExpansion, RadialBesselFunction, SphericalBesselWithHarmonics
 from matgl.layers._bond import BondExpansion
 from matgl.layers._core import MLP, EdgeSet2Set, GatedMLP
 from matgl.layers._embedding import EmbeddingBlock
 from matgl.layers._graph_convolution import M3GNetBlock, M3GNetGraphConv, MEGNetBlock, MEGNetGraphConv
 from matgl.layers._readout import ReduceReadOut, Set2SetReadOut, WeightedReadOut, WeightedReadOutPair
 from matgl.layers._three_body import ThreeBodyInteractions
```

### Comparing `matgl-0.6.2/matgl/layers/_activations.py` & `matgl-0.7.0/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/layers/_atom_ref.py` & `matgl-0.7.0/matgl/layers/_atom_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 class AtomRef(nn.Module):
     """Get total property offset for a system."""
 
     def __init__(
         self,
         property_offset: np.array,  # type: ignore
     ) -> None:
-        """Args:
-        property_offset (np.array): a array of elemental property offset.
+        """
+        Args:
+            property_offset (np.array): a array of elemental property offset.
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
     def get_feature_matrix(self, graphs: list) -> np.typing.NDArray:
         """Get the number of atoms for different elements in the structure.
```

### Comparing `matgl-0.6.2/matgl/layers/_basis.py` & `matgl-0.7.0/matgl/layers/_basis.py`

 * *Files 21% similar despite different names*

```diff
@@ -78,78 +78,157 @@
     @lru_cache(maxsize=128)
     def _calculate_symbolic_funcs(self) -> list:
         """Spherical basis functions based on Rayleigh formula. This function
         generates
         symbolic formula.
 
         Returns: list of symbolic functions
-
         """
         x = sympy.symbols("x")
         funcs = [sympy.expand_func(sympy.functions.special.bessel.jn(i, x)) for i in range(self.max_l + 1)]
         return [sympy.lambdify(x, func, torch) for func in funcs]
 
     @lru_cache(maxsize=128)
     def _calculate_smooth_symbolic_funcs(self) -> list:
         return _get_lambda_func(max_n=self.max_n, cutoff=self.cutoff)
 
-    def __call__(self, r):
+    def __call__(self, r: torch.Tensor) -> torch.Tensor:
         """Args:
             r: torch.Tensor, distance tensor, 1D.
 
-
-        Returns: [n, max_n * max_l] spherical Bessel function results
-
+        Returns:
+            torch.Tensor: [n, max_n * max_l] spherical Bessel function results
         """
         if self.smooth:
             return self._call_smooth_sbf(r)
         return self._call_sbf(r)
 
     def _call_smooth_sbf(self, r):
         results = [i(r) for i in self.funcs]
         return torch.t(torch.stack(results))
 
     def _call_sbf(self, r):
+        r_c = r.clone()
+        r_c[r_c > self.cutoff] = self.cutoff
         roots = SPHERICAL_BESSEL_ROOTS[: self.max_l, : self.max_n]
 
         results = []
         factor = torch.tensor(sqrt(2.0 / self.cutoff**3))
         for i in range(self.max_l):
             root = roots[i]
             func = self.funcs[i]
             func_add1 = self.funcs[i + 1]
             results.append(
-                func(r[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
+                func(r_c[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
             )
         return torch.cat(results, axis=1)
 
     @staticmethod
     def rbf_j0(r, cutoff: float = 5.0, max_n: int = 3):
         """Spherical Bessel function of order 0, ensuring the function value
         vanishes at cutoff.
 
         Args:
             r: torch.Tensor pytorch tensors
             cutoff: float, the cutoff radius
             max_n: int max number of basis
-        Returns: basis function expansion using first spherical Bessel function
+
+        Returns:
+            basis function expansion using first spherical Bessel function
         """
         n = (torch.arange(1, max_n + 1)).type(dtype=torch.float32)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
 
 
+class RadialBesselFunction(nn.Module):
+    """Zeroth order bessel function of the first kind.
+
+    Implements the proposed 1D radial basis function in terms of zeroth order bessel function of the first kind with
+    increasing number of roots and a given cutoff.
+
+    Details are given in: https://arxiv.org/abs/2003.03123
+
+    This is equivalent to SphericalBesselFunction class with max_l=1, i.e. only l=0 bessel fucntions), but with
+    optional learnable frequencies.
+    """
+
+    def __init__(self, max_n: int, cutoff: float, learnable: bool = False):
+        """
+        Args:
+            max_n: int, max number of roots (including max_n)
+            cutoff: float, cutoff radius
+            learnable: bool, whether to learn the location of roots.
+        """
+        super().__init__()
+        self.max_n = max_n
+        self.inv_cutoff = 1 / cutoff
+        self.norm_const = (2 * self.inv_cutoff) ** 0.5
+
+        if learnable:
+            self.frequencies = torch.nn.Parameter(
+                data=torch.Tensor(pi * torch.arange(1, self.max_n + 1, dtype=torch.float32)),
+                requires_grad=True,
+            )
+        else:
+            self.register_buffer(
+                "frequencies",
+                pi * torch.arange(1, self.max_n + 1, dtype=torch.float32),
+            )
+
+    def forward(self, r: torch.Tensor) -> torch.Tensor:
+        r = r[:, None]  # (nEdges,1)
+        d_scaled = r * self.inv_cutoff
+        return self.norm_const * torch.sin(self.frequencies * d_scaled) / r
+
+
+class FourierExpansion(nn.Module):
+    """Fourier Expansion of a (periodic) scalar feature."""
+
+    def __init__(self, max_f: int = 5, interval: float = pi, scale_factor: float = 1.0, learnable: bool = False):
+        """Args:
+        max_f (int): the maximum frequency of the Fourier expansion.
+            Default = 5
+        interval (float): the interval of the Fourier expansion, such that functions
+            are orthonormal over [-interval, interval]. Default = pi
+        scale_factor (float): pre-factor to scale all values.
+            learnable (bool): whether to set the frequencies as learnable parameters
+            Default = False.
+        """
+        super().__init__()
+        self.max_f = max_f
+        self.interval = interval
+        self.scale_factor = scale_factor
+        # Initialize frequencies at canonical
+        if learnable:
+            self.frequencies = torch.nn.Parameter(
+                data=torch.arange(0, max_f + 1, dtype=torch.float32),
+                requires_grad=True,
+            )
+        else:
+            self.register_buffer("frequencies", torch.arange(0, max_f + 1, dtype=torch.float32))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """Expand x into cos and sin functions."""
+        result = x.new_zeros(x.shape[0], 1 + 2 * self.max_f)
+        tmp = torch.outer(x, self.frequencies)
+        result[:, ::2] = torch.cos(tmp * pi / self.interval)
+        result[:, 1::2] = torch.sin(tmp[:, 1:] * pi / self.interval)
+        return result / self.interval * self.scale_factor
+
+
 class SphericalHarmonicsFunction:
     """Spherical Harmonics function."""
 
     def __init__(self, max_l: int, use_phi: bool = True):
-        """Args:
-        max_l: int, max l (excluding l)
-        use_phi: bool, whether to use the polar angle. If not,
-        the function will compute `Y_l^0`.
+        """
+        Args:
+            max_l: int, max l (excluding l)
+            use_phi: bool, whether to use the polar angle. If not,
+            the function will compute `Y_l^0`.
         """
         self.max_l = max_l
         self.use_phi = use_phi
         funcs = []
         theta, phi = sympy.symbols("theta phi")
         for lval in range(self.max_l):
             m_list = range(-lval, lval + 1) if self.use_phi else [0]  # type: ignore
@@ -186,15 +265,14 @@
         Y_0^0 = \frac{1}{2} \sqrt{\frac{1}{\pi}}
 
     Args:
         theta: torch.Tensor, the azimuthal angle
         phi: torch.Tensor, the polar angle
 
     Returns: `Y_0^0` results
-
     """
     return 0.5 * torch.ones_like(theta) * sqrt(1.0 / pi)
 
 
 def _conjugate(x):
     return torch.conj(x)
```

### Comparing `matgl-0.6.2/matgl/layers/_bond.py` & `matgl-0.7.0/matgl/layers/_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,25 @@
         rbf_type: str = "SphericalBessel",
         smooth: bool = False,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
     ) -> None:
-        """Args:
-        max_l (int): order of angular part
-        max_n (int): order of radial part
-        cutoff (float): cutoff radius
-        rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
-        smooth (bool): whether apply the smooth version of spherical bessel functions or not
-        initial (float): initial point for gaussian expansion
-        final (float): final point for gaussian expansion
-        num_centers (int): Number of centers for gaussian expansion.
-        width (float): width of gaussian function.
+        """
+        Args:
+            max_l (int): order of angular part
+            max_n (int): order of radial part
+            cutoff (float): cutoff radius
+            rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
+            smooth (bool): whether apply the smooth version of spherical bessel functions or not
+            initial (float): initial point for gaussian expansion
+            final (float): final point for gaussian expansion
+            num_centers (int): Number of centers for gaussian expansion.
+            width (float): width of gaussian function.
         """
         super().__init__()
 
         self.max_n = max_n
         self.cutoff = cutoff
         self.max_l = max_l
         self.smooth = smooth
```

### Comparing `matgl-0.6.2/matgl/layers/_core.py` & `matgl-0.7.0/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/layers/_embedding.py` & `matgl-0.7.0/matgl/layers/_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,25 @@
         dim_edge_embedding: int | None = None,
         dim_state_feats: int | None = None,
         ntypes_node: int | None = None,
         include_state: bool = False,
         ntypes_state: int | None = None,
         dim_state_embedding: int | None = None,
     ):
-        """Args:
-        degree_rbf (int): number of rbf
-        activation (nn.Module): activation type
-        dim_node_embedding (int): dimensionality of node features
-        dim_edge_embedding (int): dimensionality of edge features
-        dim_state_feats: dimensionality of state features
-        ntypes_node: number of node labels
-        include_state: Whether to include state embedding
-        ntypes_state: number of state labels
-        dim_state_embedding: dimensionality of state embedding.
+        """
+        Args:
+            degree_rbf (int): number of rbf
+            activation (nn.Module): activation type
+            dim_node_embedding (int): dimensionality of node features
+            dim_edge_embedding (int): dimensionality of edge features
+            dim_state_feats: dimensionality of state features
+            ntypes_node: number of node labels
+            include_state: Whether to include state embedding
+            ntypes_state: number of state labels
+            dim_state_embedding: dimensionality of state embedding.
         """
         super().__init__()
         self.include_state = include_state
         self.ntypes_state = ntypes_state
         self.dim_node_embedding = dim_node_embedding
         self.dim_edge_embedding = dim_edge_embedding
         self.dim_state_feats = dim_state_feats
@@ -50,22 +51,22 @@
             dim_edges = [degree_rbf, dim_edge_embedding]
             self.layer_edge_embedding = MLP(dim_edges, activation=activation, activate_last=True)
 
     def forward(self, node_attr, edge_attr, state_attr):
         """Output embedded features.
 
         Args:
-        node_attr: node attribute
-        edge_attr: edge attribute
-        state_attr: state attribute
+            node_attr: node attribute
+            edge_attr: edge attribute
+            state_attr: state attribute
 
         Returns:
-        node_feat: embedded node features
-        edge_feat: embedded edge features
-        state_feat: embedded state features
+            node_feat: embedded node features
+            edge_feat: embedded edge features
+            state_feat: embedded state features
         """
         if self.ntypes_node is not None:
             node_feat = self.layer_node_embedding(node_attr)
         else:
             node_embed = MLP([node_attr.shape[-1], self.dim_node_embedding], activation=self.activation)
             node_feat = node_embed(node_attr.to(torch.float32))
         if self.dim_edge_embedding is not None:
```

### Comparing `matgl-0.6.2/matgl/layers/_graph_convolution.py` & `matgl-0.7.0/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/layers/_readout.py` & `matgl-0.7.0/matgl/layers/_readout.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
     def __init__(
         self,
         num_steps: int,
         num_layers: int,
         field: str,
     ):
-        """Args:
-        num_steps (int): Number of LSTM steps
-        num_layers (int): Number of layers.
-        field (str): Field of graph to perform the readout.
+        """
+        Args:
+            num_steps (int): Number of LSTM steps
+            num_layers (int): Number of layers.
+            field (str): Field of graph to perform the readout.
         """
         super().__init__()
         self.field = field
         self.num_steps = num_steps
         self.num_layers = num_layers
 
     def forward(self, g: dgl.DGLGraph):
@@ -44,52 +45,56 @@
 
 class ReduceReadOut(nn.Module):
     """Reduce atom or bond attributes into lower dimensional tensors as readout.
     This could be summing up the atoms or bonds, or taking the mean, etc.
     """
 
     def __init__(self, op: str = "mean", field: str = "node_feat"):
-        """Args:
-        op (str): op for the reduction
-        field (str): Field of graph to perform the reduction.
+        """
+        Args:
+            op (str): op for the reduction
+            field (str): Field of graph to perform the reduction.
         """
         super().__init__()
         self.op = op
         self.field = field
 
     def forward(self, g: dgl.DGLGraph):
         """Args:
-            g: DGL graph
+            g: DGL graph.
+
         Returns:
             torch.tensor.
         """
         if self.field == "node_feat":
             reduced_tensor = dgl.readout_nodes(g, feat="node_feat", op=self.op)
         elif self.field == "edge_feat":
             reduced_tensor = dgl.readout_edges(g, feat="edge_feat", op=self.op)
         return reduced_tensor
 
 
 class WeightedReadOut(nn.Module):
     """Feed node features into Gated MLP as readout."""
 
     def __init__(self, in_feats: int, dims: list[int], num_targets: int):
-        """Args:
-        in_feats: input features (nodes)
-        dims: NN architecture for Gated MLP
-        num_targets: number of target properties.
+        """
+        Args:
+            in_feats: input features (nodes)
+            dims: NN architecture for Gated MLP
+            num_targets: number of target properties.
         """
         super().__init__()
         self.in_feats = in_feats
         self.dims = [in_feats, *dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
     def forward(self, g: dgl.DGLGraph):
         """Args:
-            g: DGL graph
+            g: DGL graph.
+
         Returns:
             atomic_properties: torch.Tensor.
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
         return atomic_properties
```

### Comparing `matgl-0.6.2/matgl/layers/_three_body.py` & `matgl-0.7.0/matgl/layers/_three_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Three-Body interaction implementations."""
 
 from __future__ import annotations
 
-import dgl
+from typing import TYPE_CHECKING
+
 import numpy as np
 import torch
 from torch import nn
 
-from matgl.utils.maths import (
-    _block_repeat,
-    get_segment_indices_from_n,
-    scatter_sum,
-)
+from matgl.utils.maths import _block_repeat, get_segment_indices_from_n, scatter_sum
+
+if TYPE_CHECKING:
+    import dgl
 
 
 class ThreeBodyInteractions(nn.Module):
     """Include 3D interactions to the bond update."""
 
     def __init__(self, update_network_atom: nn.Module, update_network_bond: nn.Module, **kwargs):
         """Init ThreeBodyInteractions.
@@ -62,14 +62,16 @@
         basis = basis * weights[:, None]
         new_bonds = scatter_sum(
             basis.to(torch.float32),
             segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
             num_segments=graph.num_edges(),
             dim=0,
         )
+        if not new_bonds.data.shape[0]:
+            return edge_feat
         edge_feat_updated = edge_feat + self.update_network_bond(new_bonds)
         return edge_feat_updated
 
 
 def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool):
     """Combine the spherical Bessel function and the spherical Harmonics function.
```

### Comparing `matgl-0.6.2/matgl/models/_m3gnet.py` & `matgl-0.7.0/matgl/models/_m3gnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,26 +7,27 @@
     Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
     Computational Science, 2023, 2, 718-728. DOI: 10.1038/s43588-022-00349-3.
 
 """
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING
 
 import dgl
+import numpy as np
 import torch
 from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
     compute_pair_vector_and_distance,
     compute_theta_and_phi,
     create_line_graph,
 )
-from matgl.graph.converters import GraphConverter
 from matgl.layers import (
     MLP,
     BondExpansion,
     EmbeddingBlock,
     GatedMLP,
     M3GNetBlock,
     ReduceReadOut,
@@ -36,14 +37,17 @@
     SphericalBesselWithHarmonics,
     ThreeBodyInteractions,
     WeightedReadOut,
 )
 from matgl.utils.cutoff import polynomial_cutoff
 from matgl.utils.io import IOMixIn
 
+if TYPE_CHECKING:
+    from matgl.graph.converters import GraphConverter
+
 logger = logging.getLogger(__file__)
 
 
 class M3GNet(nn.Module, IOMixIn):
     """The main M3GNet model."""
 
     __version__ = 1
@@ -142,21 +146,27 @@
             dim_state_feats=dim_state_feats,
             include_state=include_state,
             dim_state_embedding=dim_state_embedding,
             activation=activation,
         )
 
         self.basis_expansion = SphericalBesselWithHarmonics(
-            max_n=max_n, max_l=max_l, cutoff=cutoff, use_phi=use_phi, use_smooth=use_smooth
+            max_n=max_n,
+            max_l=max_l,
+            cutoff=cutoff,
+            use_phi=use_phi,
+            use_smooth=use_smooth,
         )
         self.three_body_interactions = nn.ModuleList(
             {
                 ThreeBodyInteractions(
                     update_network_atom=MLP(
-                        dims=[dim_node_embedding, degree], activation=nn.Sigmoid(), activate_last=True
+                        dims=[dim_node_embedding, degree],
+                        activation=nn.Sigmoid(),
+                        activate_last=True,
                     ),
                     update_network_bond=GatedMLP(in_feats=degree, dims=[dim_edge_embedding], use_bias=False),
                 )
                 for _ in range(nblocks)
             }
         )
 
@@ -201,15 +211,20 @@
         self.units = units
         self.cutoff = cutoff
         self.threebody_cutoff = threebody_cutoff
         self.include_states = include_state
         self.task_type = task_type
         self.is_intensive = is_intensive
 
-    def forward(self, g: dgl.DGLGraph, state_attr: torch.Tensor | None = None, l_g: dgl.DGLGraph | None = None):
+    def forward(
+        self,
+        g: dgl.DGLGraph,
+        state_attr: torch.Tensor | None = None,
+        l_g: dgl.DGLGraph | None = None,
+    ):
         """Performs message passing and updates node representations.
 
         Args:
             g : DGLGraph for a batch of graphs.
             state_attr: State attrs for a batch of graphs.
             l_g : DGLGraph for a batch of line graphs.
 
@@ -221,26 +236,32 @@
         g.edata["bond_vec"] = bond_vec
         g.edata["bond_dist"] = bond_dist
 
         expanded_dists = self.bond_expansion(g.edata["bond_dist"])
         if l_g is None:
             l_g = create_line_graph(g, self.threebody_cutoff)
         else:
-            valid_three_body = g.edata["bond_dist"] <= self.threebody_cutoff
-            l_g.ndata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
-            l_g.ndata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
-            l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
+            three_body_id = np.unique(np.concatenate(l_g.edges()))
+            max_three_body_id = max(np.concatenate([three_body_id + 1, [0]]))
+            l_g.ndata["bond_vec"] = g.edata["bond_vec"][:max_three_body_id]
+            l_g.ndata["bond_dist"] = g.edata["bond_dist"][:max_three_body_id]
+            l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][:max_three_body_id]
         l_g.apply_edges(compute_theta_and_phi)
         g.edata["rbf"] = expanded_dists
         three_body_basis = self.basis_expansion(l_g)
         three_body_cutoff = polynomial_cutoff(g.edata["bond_dist"], self.threebody_cutoff)
         num_node_feats, num_edge_feats, num_state_feats = self.embedding(node_types, g.edata["rbf"], state_attr)
         for i in range(self.n_blocks):
             num_edge_feats = self.three_body_interactions[i](
-                g, l_g, three_body_basis, three_body_cutoff, num_node_feats, num_edge_feats
+                g,
+                l_g,
+                three_body_basis,
+                three_body_cutoff,
+                num_node_feats,
+                num_edge_feats,
             )
             num_edge_feats, num_node_feats, num_state_feats = self.graph_layers[i](
                 g, num_edge_feats, num_node_feats, num_state_feats
             )
         g.ndata["node_feat"] = num_node_feats
         g.edata["edge_feat"] = num_edge_feats
         if self.is_intensive:
@@ -251,15 +272,18 @@
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
         return torch.squeeze(output)
 
     def predict_structure(
-        self, structure, state_feats: torch.Tensor | None = None, graph_converter: GraphConverter | None = None
+        self,
+        structure,
+        state_feats: torch.Tensor | None = None,
+        graph_converter: GraphConverter | None = None,
     ):
         """Convenience method to directly predict property from structure.
 
         Args:
             structure: An input crystal/molecule.
             state_feats (torch.tensor): Graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
@@ -267,11 +291,11 @@
         Returns:
             output (torch.tensor): output property
         """
         if graph_converter is None:
             from matgl.ext.pymatgen import Structure2Graph
 
             graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)  # type: ignore
-        g, stare_feats_default = graph_converter.get_graph(structure)
+        g, state_feats_default = graph_converter.get_graph(structure)
         if state_feats is None:
-            state_feats = torch.tensor(stare_feats_default)
+            state_feats = torch.tensor(state_feats_default)
         return self(g=g, state_attr=state_feats).detach()
```

### Comparing `matgl-0.6.2/matgl/models/_megnet.py` & `matgl-0.7.0/matgl/models/_megnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 
     Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
     Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564-3572. DOI: 10.1021/acs.chemmater.9b01294.
 """
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING
 
-import dgl
 import torch
 from dgl.nn import Set2Set
 from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import compute_pair_vector_and_distance
-from matgl.graph.converters import GraphConverter
 from matgl.layers import MLP, BondExpansion, EdgeSet2Set, EmbeddingBlock, MEGNetBlock, SoftExponential, SoftPlus2
 from matgl.utils.io import IOMixIn
 
+if TYPE_CHECKING:
+    import dgl
+
+    from matgl.graph.converters import GraphConverter
+
 logger = logging.getLogger(__file__)
 
 
 class MEGNet(nn.Module, IOMixIn):
     """DGL implementation of MEGNet."""
 
     __version__ = 1
@@ -88,24 +92,25 @@
             rbf_type="Gaussian", initial=0.0, final=cutoff + 1.0, num_centers=dim_edge_embedding, width=gauss_width
         )
 
         node_dims = [dim_node_embedding, *hidden_layer_sizes_input]
         edge_dims = [dim_edge_embedding, *hidden_layer_sizes_input]
         state_dims = [dim_state_embedding, *hidden_layer_sizes_input]
 
+        activation: nn.Module
         if activation_type == "swish":
-            activation = nn.SiLU()  # type: ignore
+            activation = nn.SiLU()
         elif activation_type == "sigmoid":
-            activation = nn.Sigmoid()  # type: ignore
+            activation = nn.Sigmoid()
         elif activation_type == "tanh":
-            activation = nn.Tanh()  # type: ignore
+            activation = nn.Tanh()
         elif activation_type == "softplus2":
-            activation = SoftPlus2()  # type: ignore
+            activation = SoftPlus2()
         elif activation_type == "softexp":
-            activation = SoftExponential()  # type: ignore
+            activation = SoftExponential()
         else:
             raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
         self.embedding = EmbeddingBlock(
             degree_rbf=dim_edge_embedding,
             dim_node_embedding=dim_node_embedding,
             ntypes_node=len(self.element_types),
```

### Comparing `matgl-0.6.2/matgl/models/_wrappers.py` & `matgl-0.7.0/matgl/models/_wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-"""Implementations of pseudomodels that wraps other models."""
+"""Implementations of pseudo-models that wrap other models."""
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from torch import nn
 
-from matgl.data.transformer import Transformer
 from matgl.utils.io import IOMixIn
 
+if TYPE_CHECKING:
+    from matgl.data.transformer import Transformer
+
 
 class TransformedTargetModel(nn.Module, IOMixIn):
     """A model where the target is first transformed prior to training and the reverse transformation is performed for
     predictions. This is modelled after scikit-learn's TransformedTargetRegressor. It should be noted that this model
     is almost never used for training since the general idea is to use the transformed target for loss computation.
     Instead, it is created after a model has been fitted for serialization for end user to call the model to perform
     predictions without having to worry about what target transformations have been performed.
     """
 
     # Model version number.
     __version__ = 1
 
     def __init__(self, model: nn.Module, target_transformer: Transformer):
-        """Args:
-        model: Input model
-        target_transformer: Transformer for target.
+        """
+        Args:
+            model (nn.Module): Model to wrap.
+            target_transformer (Transformer): Transformer to use for target transformation.
         """
         super().__init__()
         self.save_args(locals())
         self.model = model
         self.transformer = target_transformer
 
     def forward(self, *args, **kwargs):
@@ -36,15 +41,15 @@
         Returns:
             Inverse transformed output.
         """
         output = self.model.forward(*args, **kwargs)
         return self.transformer.inverse_transform(output)
 
     def __repr__(self):
-        return f"TransformedTargetModel:\n\tModel: {self.model.__repr()}\n\tTransformer: {self.transformer.__repr__()}"
+        return f"{type(self).__name__}:\n\tModel: {self.model!r}\n\tTransformer: {self.transformer!r}"
 
     def predict_structure(self, *args, **kwargs):
         """Pass through to parent model.predict_structure with inverse transform.
 
         Args:
             *args: Pass-through to self.model.predict_structure.
             **kwargs: Pass-through to self.model.predict_structure.
```

### Comparing `matgl-0.6.2/matgl/utils/io.py` & `matgl-0.7.0/matgl/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,20 +133,21 @@
         return model
 
 
 class RemoteFile:
     """Handling of download of remote files to a local cache."""
 
     def __init__(self, uri: str, cache_location: str | Path = MATGL_CACHE, force_download: bool = False):
-        """Args:
-        uri: Uniform resource identifier.
-        cache_location: Directory to cache downloaded RemoteFile. By default, downloaded models are saved at
-        $HOME/.matgl.
-        force_download: To speed up access, a model with the same name in the cache location will be used if
-        present. If you want to force a re-download, set this to True.
+        """
+        Args:
+            uri: Uniform resource identifier.
+            cache_location: Directory to cache downloaded RemoteFile. By default, downloaded models are saved at
+            $HOME/.matgl.
+            force_download: To speed up access, a model with the same name in the cache location will be used if
+            present. If you want to force a re-download, set this to True.
         """
         self.uri = uri
         toks = uri.split("/")
         self.model_name = toks[-2]
         self.fname = toks[-1]
         cache_location = Path(cache_location)
         os.makedirs(cache_location / self.model_name, exist_ok=True)
```

### Comparing `matgl-0.6.2/matgl/utils/maths.py` & `matgl-0.7.0/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/utils/sb_roots.npy` & `matgl-0.7.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/matgl/utils/training.py` & `matgl-0.7.0/matgl/utils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Utils for training MatGL models."""
 
 from __future__ import annotations
 
 import math
+from typing import TYPE_CHECKING
 
-import dgl
-import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
 from torch import nn
-from torch.optim import Optimizer
 
 from matgl.apps.pes import Potential
 from matgl.models import M3GNet
 
+if TYPE_CHECKING:
+    import dgl
+    import numpy as np
+    from torch.optim import Optimizer
+
 
 class MatglLightningModuleMixin:
     """Mix-in class implementing common functions for training."""
 
     def training_step(self, batch: tuple, batch_idx: int):
         """Training step.
 
@@ -57,30 +60,33 @@
         self.log_dict(  # type: ignore
             {f"val_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
+        return results["Total_Loss"]
 
     def test_step(self, batch: tuple, batch_idx: int):
         """Test step.
 
         Args:
             batch: Data batch.
             batch_idx: Batch index.
         """
+        torch.set_grad_enabled(True)
         results, batch_size = self.step(batch)  # type: ignore
         self.log_dict(  # type: ignore
             {f"test_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
+        return results
 
     def configure_optimizers(self):
         """Configure optimizers."""
         if self.optimizer is None:
             optimizer = torch.optim.Adam(
                 self.parameters(),
                 lr=self.lr,
@@ -122,15 +128,15 @@
             batch_idx: Batch index.
             dataloader_idx: Data loader index.
 
         Returns:
             Prediction
         """
         torch.set_grad_enabled(True)
-        return self(batch)
+        return self.step(batch)
 
 
 class ModelLightningModule(MatglLightningModuleMixin, pl.LightningModule):
     """A PyTorch.LightningModule for training MEGNet and M3GNet models."""
 
     def __init__(
         self,
```

### Comparing `matgl-0.6.2/matgl.egg-info/PKG-INFO` & `matgl-0.7.0/matgl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.6.2
+Version: 0.7.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -24,51 +24,60 @@
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+# Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
-# Materials Graph Library
+## Official Documentation [:books:]
 
-### Official Documentation: [:books:][doc]
+<https://matgl.ai>
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
-natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
-shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
+exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
-and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
-The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
-over the TF implementations:
+MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
+applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
+learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
+[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
+usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
 
 - A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
+- Multi-GPU support via PyTorch Lightning.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
-Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
+Nassar, Carmelo Gonzales).
 
 ## Status
 
-Major milestones are summarized below. Please refer to [change log][changelog] for details.
+Major milestones are summarized below. Please refer to the [changelog] for details.
 
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
-## Architectures
+## Current Architectures
+
+Here, we summarize the currently implemented architectures in MatGL. It should be stressed that this is by no means
+an exhaustive list, and we expect new architectures to be added by the core MatGL team as well as other contributors
+in future.
+
+<div style="float: left; padding: 10px; width: 300px">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
+<p>Figure: Schematic of M3GNet/MEGNet</p>
+</div>
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ### MEGNet
 
 [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
@@ -107,40 +116,40 @@
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available.
 
-### From the command line (from v0.6.2)
+### Command line (from v0.6.2)
 
 A CLI tool now provides the capability to perform quick relaxations or predictions using pre-trained models, as well
 as other simple administrative tasks (e.g., clearing the cache). Some simple examples:
 
 1. To perform a relaxation,
 
     ```bash
-    mgl relax -i Li2O.cif -o Li2O_relax.cif
+    mgl relax --infile Li2O.cif --outfile Li2O_relax.cif
     ```
 
 2. To use one of the pre-trained property models,
 
     ```bash
-    mgl predict -m M3GNet-MP-2018.6.1-Eform -i Li2O.cif
+    mgl predict --model M3GNet-MP-2018.6.1-Eform --infile Li2O.cif
     ```
 
 3. To clear the cache,
 
     ```bash
     mgl clear
     ```
 
 For a full range of options, use `mgl -h`.
 
-### In code
+### Code
 
 Users who just want to use the models out of the box should use the newly implemented `matgl.load_model` convenience
 method. The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -158,21 +167,21 @@
 ```python
 import matgl
 print(matgl.get_available_pretrained_models())
 ```
 
 ## Tutorials
 
-A set of [tutorials][tutorials] have been written on the use of MatGL. These were generated from [Jupyter notebooks]
-[jupyternb], which can be directly run on [Google Colab][colab].
+We wrote [tutorials] on how to use MatGL. These were generated from [Jupyter notebooks]
+[jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
-- [API documentation][apidocs] for all classes and methods.
-- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+- [API docs][apidocs] for all classes and methods.
+- [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
@@ -189,27 +198,27 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original TensorFlow (TF) implementation!**
 
    _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
    _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
-   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   ensure the best implementation. This can usually be solved by updating your `matgl` to the latest version
    and clearing your cache using the following command `mgl clear`. On the next run, the latest model will be
    downloaded. With effect from v0.5.2, we have implemented a model versioning scheme that will detect code vs model
    version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
    _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
@@ -245,17 +254,17 @@
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
 [changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
-[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
-[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mfimegnet]: https://nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
-[colab]: https://colab.research.google.com/ "Google Colab"
+[google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
```

### Comparing `matgl-0.6.2/matgl.egg-info/SOURCES.txt` & `matgl-0.7.0/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.6.2/pyproject.toml` & `matgl-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,38 +29,41 @@
 )
 '''
 
 [tool.ruff]
 target-version = "py39"
 line-length = 120
 select = [
-  "B",   # flake8-bugbear
-  "C4",  # flake8-comprehensions
-  "D",   # pydocstyle
-  "E",   # pycodestyle error
-  "EXE", # flake8-executable
-  "F",   # pyflakes
-  "I",   # isort
-  "ICN", # flake8-import-conventions
-  "ISC", # flake8-implicit-str-concat
-  "PD",  # pandas-vet
-  "PIE", # flake8-pie
-  "PL",  # pylint
-  "PT",  # flake8-pytest-style
-  "PYI", # flakes8-pyi
-  "Q",   # flake8-quotes
-  "RET", # flake8-return
-  "RSE", # flake8-raise
-  "RUF", # Ruff-specific rules
-  "SIM", # flake8-simplify
-  "TID", # tidy imports
-  "TID", # flake8-tidy-imports
-  "UP",  # pyupgrade
-  "W",   # pycodestyle warning
-  "YTT", # flake8-2020
+  "B",    # flake8-bugbear
+  "C4",   # flake8-comprehensions
+  "D",    # pydocstyle
+  "E",    # pycodestyle error
+  "EXE",  # flake8-executable
+  "F",    # pyflakes
+  "I",    # isort
+  "ICN",  # flake8-import-conventions
+  "ISC",  # flake8-implicit-str-concat
+  "PD",   # pandas-vet
+  "PERF", # perflint
+  "PIE",  # flake8-pie
+  "PL",   # pylint
+  "PT",   # flake8-pytest-style
+  "PYI",  # flakes8-pyi
+  "Q",    # flake8-quotes
+  "RET",  # flake8-return
+  "RSE",  # flake8-raise
+  "RUF",  # Ruff-specific rules
+  "SIM",  # flake8-simplify
+  "SLOT", # flake8-slots
+  "TCH",  # flake8-type-checking
+  "TID",  # tidy imports
+  "TID",  # flake8-tidy-imports
+  "UP",   # pyupgrade
+  "W",    # pycodestyle warning
+  "YTT",  # flake8-2020
 ]
 ignore = [
   "B019",    # functools.lru_cache on methods can lead to memory leaks
   "D105",    # Missing docstring in magic method
   "D205",    # 1 blank line required between summary line and description
   "D212",    # Multi-line docstring summary should start at the first line
   "PLR",     # pylint refactor
```

### Comparing `matgl-0.6.2/setup.py` & `matgl-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.6.2",
+    version="0.7.0",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -39,18 +39,14 @@
     install_requires=(
         "ase",
         "dgl",
         "pymatgen",
         "pytorch_lightning",
         "torch",
     ),
-    extra_requires={
-        "ase": ["ase>=3.22.1"],
-        "pymatgen": ["pymatgen>=2023.5.31"],
-    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

