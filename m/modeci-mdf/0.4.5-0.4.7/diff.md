# Comparing `tmp/modeci-mdf-0.4.5.tar.gz` & `tmp/modeci-mdf-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeci-mdf-0.4.5.tar", last modified: Mon Apr 17 16:56:20 2023, max compression
+gzip compressed data, was "modeci-mdf-0.4.7.tar", last modified: Mon Jun 26 08:58:27 2023, max compression
```

## Comparing `modeci-mdf-0.4.5.tar` & `modeci-mdf-0.4.7.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 16:56:08.000000 modeci-mdf-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-17 16:56:08.000000 modeci-mdf-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50241 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/full_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/ddm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/mdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_mdf_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_onnx_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.910033 modeci-mdf-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-26 08:58:27.910033 modeci-mdf-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-26 08:58:27.910033 modeci-mdf-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.890033 modeci-mdf-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.894033 modeci-mdf-0.4.7/src/modeci_mdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50265 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/full_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.898033 modeci-mdf-0.4.7/src/modeci_mdf/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.898033 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.902033 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/functions/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.902033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.902033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/actr/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/actr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/actr/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.902033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/graphviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/graphviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/graphviz/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.902033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.906033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.906033 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/mdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/src/modeci_mdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.898033 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-26 08:58:27.000000 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-26 08:58:27.000000 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:58:27.000000 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-26 08:58:27.000000 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 08:58:27.000000 modeci-mdf-0.4.7/src/modeci_mdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:58:27.910033 modeci-mdf-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_mdf_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_onnx_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-26 08:58:18.000000 modeci-mdf-0.4.7/tests/test_scheduler.py
```

### Comparing `modeci-mdf-0.4.5/LICENSE` & `modeci-mdf-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/PKG-INFO` & `modeci-mdf-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.5
+Version: 0.4.7
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
@@ -28,16 +28,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: psyneulink
 Provides-Extra: neuroml
 Provides-Extra: tensorflow
 Provides-Extra: test
 Provides-Extra: optional
-Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img alt="mdf logo" width="402" src="https://raw.githubusercontent.com/ModECI/MDF/main/docs/sphinx/images/logo_light_bg.png"/>
 </p>
 
 [![Actions Status][actions-badge]][actions-link]
```

### Comparing `modeci-mdf-0.4.5/README.md` & `modeci-mdf-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/pyproject.toml` & `modeci-mdf-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/setup.cfg` & `modeci-mdf-0.4.7/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -36,25 +36,67 @@
 	typing_compat;python_version<'3.8'
 	dataclasses;python_version<'3.7'
 	graph_scheduler>=1.1.1
 	numpy
 	matplotlib
 	graphviz
 	h5py
-	onnxruntime<=1.13.1,>=1.12.0
-	skl2onnx>=1.13
+	onnxruntime==1.13.1
+	onnx==1.12.0
+	skl2onnx==1.14.0
 	attrs>=21.1.0
 	cattrs
 	modelspec<0.3,>=0.2.6
 	glom
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	=src
 
+[options.extras_require]
+psyneulink = 
+	grpcio-tools==1.42.0
+	psyneulink
+neuroml = 
+	pyNeuroML>=0.5.20
+	neuromllite>=0.5.2
+tensorflow = 
+	tensorflow
+	keras_visualizer
+	pydot
+test = 
+	pytest
+	pytest-benchmark
+	pytest-mock
+	typing_extensions;python_version<'3.8'
+optional = 
+	Sphinx~=3.0
+	recommonmark>=0.5.0
+	nbsphinx
+	sphinx_copybutton
+	sphinx-rtd-theme
+	myst_parser
+	sphinx_markdown_tables
+	sphinx-autoapi
+	pytorch-sphinx-theme==0.0.19
+	sphinxcontrib-versioning
+	Jinja2<3.1
+	torchviz
+	netron
+	torch>=1.11.0
+	torchvision<=0.12.0
+	h5py
+all = 
+	modeci-mdf[optional]
+	modeci-mdf[neuroml]
+	modeci-mdf[psyneulink]
+	modeci-mdf[tensorflow]
+dev = 
+	modeci-mdf[test]
+
 [options.packages.find]
 where = src
 exclude = 
 	tests
 	examples
 
 [options.package_data]
@@ -80,15 +122,14 @@
 ignore = E203, E231, E501, E722, W503, B950
 per-file-ignores = 
 	tests/*: T
 	examples/*: T
 	notebooks/*: T
 	docs/*: T
 	scripts/*: T
-	setup.py: T
 	setup_helpers.py: C901
 
 [mypy]
 warn_unused_configs = True
 python_version = 3.6
 files = src
 disallow_any_generics = True
```

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/__init__.py` & `modeci-mdf-0.4.7/src/modeci_mdf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 widely-used programming environments in a range of disciplines, and for easily extending these to other environments.
 """
 
 # Version of the specification for MDF
 MODECI_MDF_VERSION = "0.4"
 
 # Version of the Python module.
-__version__ = "0.4.5"
+__version__ = "0.4.7"
```

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/execution_engine.py` & `modeci-mdf-0.4.7/src/modeci_mdf/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1285,20 +1285,20 @@
                     )
 
             return args
 
         # if specified as dict
         try:
             args = condition["kwargs"]
-        except (TypeError, KeyError):
+        except (IndexError, TypeError, KeyError):
             args = {}
 
         try:
             condition = Condition(condition["type"], **args)
-        except (TypeError, KeyError):
+        except (IndexError, TypeError, KeyError):
             pass
 
         cond_type = condition.type
         cond_args = copy.copy(condition.kwargs)
 
         try:
             typ = getattr(graph_scheduler.condition, cond_type)
```

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/full_translator.py` & `modeci-mdf-0.4.7/src/modeci_mdf/full_translator.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/__init__.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/__init__.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/__init__.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/buffer.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/buffer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/dm.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/dm.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/logger.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/logger.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/model.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/pattern.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/pattern.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/scheduler.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/actr/ccm/scheduler.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/ddm.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/ddm.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/onnx.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/onnx.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/functions/standard.py` & `modeci-mdf-0.4.7/src/modeci_mdf/functions/standard.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/importer.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/actr/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/exporter.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/graphviz/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/exporter.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/exporter.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/importer.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/onnx/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/builtins.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/exporter.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/importer.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py` & `modeci-mdf-0.4.7/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/mdf.py` & `modeci-mdf-0.4.7/src/modeci_mdf/mdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,21 +189,21 @@
         Short summary of Parameter...
         """
         info = "Parameter: {} = {} (stateful: {})".format(
             self.id,
             self.value,
             self.is_stateful(),
         )
-        if self.default_initial_value:
+        if self.default_initial_value is not None:
             info += f", def init: {self.default_initial_value}"
 
-        if self.time_derivative:
+        if self.time_derivative is not None:
             info += f", time deriv: {self.time_derivative}"
 
-        if self.conditions:
+        if self.conditions is not None:
             for c in self.conditions:
                 info += f", {c}"
 
         return info
 
     def is_stateful(self) -> bool:
         """
```

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf/utils.py` & `modeci-mdf-0.4.7/src/modeci_mdf/utils.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf.egg-info/PKG-INFO` & `modeci-mdf-0.4.7/src/modeci_mdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.5
+Version: 0.4.7
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
@@ -28,16 +28,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: psyneulink
 Provides-Extra: neuroml
 Provides-Extra: tensorflow
 Provides-Extra: test
 Provides-Extra: optional
-Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img alt="mdf logo" width="402" src="https://raw.githubusercontent.com/ModECI/MDF/main/docs/sphinx/images/logo_light_bg.png"/>
 </p>
 
 [![Actions Status][actions-badge]][actions-link]
```

### Comparing `modeci-mdf-0.4.5/src/modeci_mdf.egg-info/SOURCES.txt` & `modeci-mdf-0.4.7/src/modeci_mdf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 src/modeci_mdf/__init__.py
 src/modeci_mdf/execution_engine.py
 src/modeci_mdf/full_translator.py
 src/modeci_mdf/mdf.py
 src/modeci_mdf/utils.py
 src/modeci_mdf.egg-info/PKG-INFO
 src/modeci_mdf.egg-info/SOURCES.txt
```

### Comparing `modeci-mdf-0.4.5/tests/test_examples.py` & `modeci-mdf-0.4.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_execution.py` & `modeci-mdf-0.4.7/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_helpers.py` & `modeci-mdf-0.4.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_mdf_functions.py` & `modeci-mdf-0.4.7/tests/test_mdf_functions.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_model.py` & `modeci-mdf-0.4.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_onnx_functions.py` & `modeci-mdf-0.4.7/tests/test_onnx_functions.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_parameters.py` & `modeci-mdf-0.4.7/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.5/tests/test_scheduler.py` & `modeci-mdf-0.4.7/tests/test_scheduler.py`

 * *Files identical despite different names*

