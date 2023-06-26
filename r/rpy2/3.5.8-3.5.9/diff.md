# Comparing `tmp/rpy2-3.5.8.tar.gz` & `tmp/rpy2-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpy2-3.5.8.tar", last modified: Mon Feb  6 02:50:03 2023, max compression
+gzip compressed data, was "rpy2-3.5.9.tar", last modified: Fri Feb 24 20:26:35 2023, max compression
```

## Comparing `rpy2-3.5.8.tar` & `rpy2-3.5.9.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.278449 rpy2-3.5.8/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      592 2023-02-06 02:46:27.000000 rpy2-3.5.8/AUTHORS
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    18092 2023-02-06 02:46:27.000000 rpy2-3.5.8/LICENSE
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      456 2023-02-06 02:46:27.000000 rpy2-3.5.8/MANIFEST.in
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    90722 2023-02-06 02:46:27.000000 rpy2-3.5.8/NEWS
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3994 2023-02-06 02:50:03.278449 rpy2-3.5.8/PKG-INFO
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3057 2023-02-06 02:46:27.000000 rpy2-3.5.8/README.md
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.266448 rpy2-3.5.8/doc/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     8419 2023-02-06 02:46:27.000000 rpy2-3.5.8/doc/Makefile
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    18092 2023-02-06 02:46:27.000000 rpy2-3.5.8/gpl-2.0.txt
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2268 2023-02-06 02:46:27.000000 rpy2-3.5.8/pyproject.toml
--rw-rw-r--   0 laurent   (1000) laurent   (1000)       69 2023-02-06 02:46:27.000000 rpy2-3.5.8/requirements.txt
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.266448 rpy2-3.5.8/rpy2/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)       91 2023-02-06 02:49:21.000000 rpy2-3.5.8/rpy2/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     9393 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/_rinterface_cffi_build.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.270449 rpy2-3.5.8/rpy2/interactive/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1468 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/interactive/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1626 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/interactive/packages.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1765 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/interactive/process_revents.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.270449 rpy2-3.5.8/rpy2/ipython/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)       77 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/ipython/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2494 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/ipython/ggplot.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     9227 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/ipython/html.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    31873 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/ipython/rmagic.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    43944 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.270449 rpy2-3.5.8/rpy2/rinterface_lib/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      127 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/RPY2.h
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    12859 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/R_API.h
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      157 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/R_API_eventloop.c
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1748 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/R_API_eventloop.h
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1521 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/_bufferprotocol.c
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    23545 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/_rinterface_capi.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2226 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/bufferprotocol.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     9652 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/callbacks.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4851 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/conversion.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    11172 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/embedded.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2934 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/embedded_mswin.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3855 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/ffi_proxy.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1625 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/memorymanagement.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      531 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/na_values.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4992 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/openrlib.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    36594 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rinterface_lib/sexp.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.270449 rpy2-3.5.8/rpy2/rlike/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rlike/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     9276 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rlike/container.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      985 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rlike/functional.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      363 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/rlike/indexing.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.270449 rpy2-3.5.8/rpy2/robjects/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    13553 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      256 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/constants.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    12667 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/conversion.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     5569 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/environments.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    16422 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/functions.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    14487 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/help.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2897 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/language.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.274449 rpy2-3.5.8/rpy2/robjects/lib/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      918 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/dbplyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    14486 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/dplyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    28326 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/ggplot2.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2340 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/grdevices.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     7631 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/grid.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1244 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/lib/tidyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    11148 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/methods.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     8161 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/numpy2ri.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    19493 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/packages.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     5109 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/packages_utils.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    13383 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/pandas2ri.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     6598 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/robject.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    50823 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/robjects/vectors.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    16785 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/situation.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.274449 rpy2-3.5.8/rpy2/tests/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/__init__.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.274449 rpy2-3.5.8/rpy2/tests/ipython/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/ipython/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      546 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/ipython/test_ggplot.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1352 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/ipython/test_html.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    15073 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/ipython/test_rmagic.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.274449 rpy2-3.5.8/rpy2/tests/rinterface/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1004 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_bufferprotocol.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    10733 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_callbacks.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      291 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_conversion.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    11481 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_embedded_r.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      422 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_endr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     5944 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_environment.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1544 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_externalptr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     5489 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_functions.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      990 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_memorymanagement.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3439 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_na.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1316 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_noinitialization.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1813 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_openrlib.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     7757 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_sexp.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      542 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_symbol.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1392 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_threading.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1757 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_bool.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1907 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_byte.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1560 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_complex.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1709 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_float.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     5543 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_int.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1390 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_lang.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2310 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_list.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2268 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_numpy.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1581 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_pairlist.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2379 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vector_str.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3762 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rinterface/test_vectors.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.274449 rpy2-3.5.8/rpy2/tests/rlike/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     8131 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rlike/test_container.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      638 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rlike/test_functional.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      218 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/rlike/test_indexing.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.278449 rpy2-3.5.8/rpy2/tests/robjects/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/__init__.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.278449 rpy2-3.5.8/rpy2/tests/robjects/lib/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/__init__.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      487 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_dbplyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4636 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_dplyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3182 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_ggplot2.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1164 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_grdevices.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1407 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_grid.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1402 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/lib/test_tidyr.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4079 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_array.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     6469 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_conversion.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     8625 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_conversion_numpy.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4796 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_dataframe.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2964 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_environment.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      730 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_formula.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4838 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_function.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2426 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_help.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1281 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_language.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3006 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_methods.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     6871 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_packages.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     2614 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_packages_utils.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    22046 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_pandas_conversions.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3062 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_robjects.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      690 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_rs4.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      634 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_serialization.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      943 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_translated_function.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)    12376 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_vector.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4207 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_vector_datetime.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3485 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_vector_extractdelegator.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     1468 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/robjects/test_vector_factor.py
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      449 2023-02-06 02:46:27.000000 rpy2-3.5.8/rpy2/tests/utils.py
-drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:50:03.266448 rpy2-3.5.8/rpy2.egg-info/
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     3994 2023-02-06 02:50:03.000000 rpy2-3.5.8/rpy2.egg-info/PKG-INFO
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     4310 2023-02-06 02:50:03.000000 rpy2-3.5.8/rpy2.egg-info/SOURCES.txt
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        1 2023-02-06 02:50:03.000000 rpy2-3.5.8/rpy2.egg-info/dependency_links.txt
--rw-rw-r--   0 laurent   (1000) laurent   (1000)        1 2023-02-06 02:49:57.000000 rpy2-3.5.8/rpy2.egg-info/not-zip-safe
--rw-rw-r--   0 laurent   (1000) laurent   (1000)      231 2023-02-06 02:50:03.000000 rpy2-3.5.8/rpy2.egg-info/requires.txt
--rw-rw-r--   0 laurent   (1000) laurent   (1000)       47 2023-02-06 02:50:03.000000 rpy2-3.5.8/rpy2.egg-info/top_level.txt
--rw-rw-r--   0 laurent   (1000) laurent   (1000)       38 2023-02-06 02:50:03.278449 rpy2-3.5.8/setup.cfg
--rw-rw-r--   0 laurent   (1000) laurent   (1000)     6970 2023-02-06 02:46:27.000000 rpy2-3.5.8/setup.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.215089 rpy2-3.5.9/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      592 2023-02-06 02:46:27.000000 rpy2-3.5.9/AUTHORS
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    18092 2023-02-06 02:46:27.000000 rpy2-3.5.9/LICENSE
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      456 2023-02-06 02:46:27.000000 rpy2-3.5.9/MANIFEST.in
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    92004 2023-02-24 20:25:12.000000 rpy2-3.5.9/NEWS
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4050 2023-02-24 20:26:35.215089 rpy2-3.5.9/PKG-INFO
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3091 2023-02-24 20:25:12.000000 rpy2-3.5.9/README.md
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.199089 rpy2-3.5.9/doc/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     8419 2023-02-06 02:46:27.000000 rpy2-3.5.9/doc/Makefile
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    18092 2023-02-06 02:46:27.000000 rpy2-3.5.9/gpl-2.0.txt
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2329 2023-02-24 20:25:12.000000 rpy2-3.5.9/pyproject.toml
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)       69 2023-02-06 02:46:27.000000 rpy2-3.5.9/requirements.txt
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.199089 rpy2-3.5.9/rpy2/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)       91 2023-02-06 02:51:10.000000 rpy2-3.5.9/rpy2/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     9393 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/_rinterface_cffi_build.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.199089 rpy2-3.5.9/rpy2/interactive/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1468 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/interactive/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1626 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/interactive/packages.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1765 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/interactive/process_revents.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.203089 rpy2-3.5.9/rpy2/ipython/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)       77 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/ipython/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2494 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/ipython/ggplot.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     9227 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/ipython/html.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    32312 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/ipython/rmagic.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    43944 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.203089 rpy2-3.5.9/rpy2/rinterface_lib/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      127 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/RPY2.h
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    12859 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/R_API.h
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      157 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/R_API_eventloop.c
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1748 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/R_API_eventloop.h
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1521 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/_bufferprotocol.c
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    23545 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/_rinterface_capi.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2226 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/bufferprotocol.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     9652 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/callbacks.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4851 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/conversion.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    11172 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/embedded.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2968 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/rinterface_lib/embedded_mswin.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3855 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/ffi_proxy.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1625 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/memorymanagement.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      531 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/na_values.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4992 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/openrlib.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    36594 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rinterface_lib/sexp.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.203089 rpy2-3.5.9/rpy2/rlike/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rlike/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     9276 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rlike/container.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      985 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rlike/functional.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      363 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/rlike/indexing.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.207089 rpy2-3.5.9/rpy2/robjects/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    13549 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/robjects/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      256 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/constants.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    13026 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/robjects/conversion.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     5569 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/environments.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    16554 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/robjects/functions.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    14487 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/help.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2897 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/language.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.207089 rpy2-3.5.9/rpy2/robjects/lib/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      918 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/dbplyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    14486 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/dplyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    28326 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/ggplot2.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2340 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/grdevices.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     7631 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/grid.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1244 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/lib/tidyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    11148 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/methods.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     8356 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/robjects/numpy2ri.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    19493 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/packages.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     5109 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/packages_utils.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    13383 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/pandas2ri.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     6598 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/robjects/robject.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    50826 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/robjects/vectors.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    16685 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/situation.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.207089 rpy2-3.5.9/rpy2/tests/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/__init__.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.207089 rpy2-3.5.9/rpy2/tests/ipython/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/ipython/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      546 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/ipython/test_ggplot.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1352 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/ipython/test_html.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    15073 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/ipython/test_rmagic.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.211089 rpy2-3.5.9/rpy2/tests/rinterface/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1004 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_bufferprotocol.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    10733 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_callbacks.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      291 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_conversion.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    11481 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_embedded_r.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      422 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_endr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     5944 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_environment.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1544 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_externalptr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     5489 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_functions.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      990 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_memorymanagement.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3439 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_na.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1316 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_noinitialization.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1813 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_openrlib.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     7757 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_sexp.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      542 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_symbol.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1392 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_threading.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1757 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_bool.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1907 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_byte.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1560 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_complex.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1709 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_float.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     5543 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_int.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1390 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_lang.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2310 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_list.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2268 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_numpy.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1581 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_pairlist.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2379 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vector_str.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3762 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rinterface/test_vectors.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.211089 rpy2-3.5.9/rpy2/tests/rlike/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     8131 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rlike/test_container.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      638 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rlike/test_functional.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      218 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/rlike/test_indexing.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.215089 rpy2-3.5.9/rpy2/tests/robjects/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/__init__.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.215089 rpy2-3.5.9/rpy2/tests/robjects/lib/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        0 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/__init__.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      487 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_dbplyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4636 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_dplyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3182 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_ggplot2.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1164 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_grdevices.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1407 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_grid.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1402 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/lib/test_tidyr.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4079 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_array.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     6469 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_conversion.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    10150 2023-02-24 20:25:12.000000 rpy2-3.5.9/rpy2/tests/robjects/test_conversion_numpy.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4796 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_dataframe.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2964 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_environment.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      730 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_formula.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4838 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_function.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2426 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_help.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1281 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_language.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3006 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_methods.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     6871 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_packages.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     2614 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_packages_utils.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    22046 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_pandas_conversions.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3062 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_robjects.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      690 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_rs4.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      634 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_serialization.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      943 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_translated_function.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)    12376 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_vector.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4207 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_vector_datetime.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     3485 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_vector_extractdelegator.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     1468 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/robjects/test_vector_factor.py
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      449 2023-02-06 02:46:27.000000 rpy2-3.5.9/rpy2/tests/utils.py
+drwxrwxr-x   0 laurent   (1000) laurent   (1000)        0 2023-02-24 20:26:35.199089 rpy2-3.5.9/rpy2.egg-info/
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4050 2023-02-24 20:26:35.000000 rpy2-3.5.9/rpy2.egg-info/PKG-INFO
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     4310 2023-02-24 20:26:35.000000 rpy2-3.5.9/rpy2.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        1 2023-02-24 20:26:35.000000 rpy2-3.5.9/rpy2.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)        1 2023-02-06 02:49:57.000000 rpy2-3.5.9/rpy2.egg-info/not-zip-safe
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)      284 2023-02-24 20:26:35.000000 rpy2-3.5.9/rpy2.egg-info/requires.txt
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)       47 2023-02-24 20:26:35.000000 rpy2-3.5.9/rpy2.egg-info/top_level.txt
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)       38 2023-02-24 20:26:35.215089 rpy2-3.5.9/setup.cfg
+-rw-rw-r--   0 laurent   (1000) laurent   (1000)     6970 2023-02-06 02:46:27.000000 rpy2-3.5.9/setup.py
```

### Comparing `rpy2-3.5.8/AUTHORS` & `rpy2-3.5.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/LICENSE` & `rpy2-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/NEWS` & `rpy2-3.5.9/NEWS`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Release 3.5.9
+=============
+
+New features
+------------
+
+- Type hints in :mod:`rpy2` are now checked with `mypy`.
+
+Bugs fixed
+----------
+
+- Building the path to the R shared library was incorrectly
+  using the output of `R CMD config LIBnn` (issue #982).
+
+- R started raising warnings when calling `formals` on `SPECIALSXP` R objects.
+  Internal functions :mod:`rpy.robjects.functions` calling `formals` no longer
+  propagate the warnings.
+  
+- The :mod:`numpy` converter was not turning `NA_character_` into
+  `None` (issue #979).
+
+- :mod:`rpy2.situation` included an eager `import rpy2` that could cause a version
+   mismatch error with some build/install toolchain (issue #984). The import is now
+   lazy/delayed.
+
+- Installation targets `pandas`, `all`, and `test` now specify `pandas>=1.2.0`
+  (which should limit frequencies of issues like #998).
+
+Changes
+-------
+
+- :class:`rpy2.robjects.conversion.Converter` objects are no longer functioning context
+  managers. An exception is now raised when trying to use it that way.
+  The feature was introduced with rpy2-3.5.7 but it does not guarantee the locality
+  of a context manager and can result in permanently changed conversion rules.
+  The method :meth:`rpy2.robjects.conversion.Converter.context` should be used instead.
+
+
 Release 3.5.8
 =============
 
 New features
 ------------
 
 - Default value for the interactivity status of the embedded R
```

### Comparing `rpy2-3.5.8/PKG-INFO` & `rpy2-3.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpy2
-Version: 3.5.8
+Version: 3.5.9
 Summary: Python interface to the R language (embedded R)
 Author-email: Laurent Gautier <lgautier@gmail.com>
 License: GPLv2+
 Project-URL: Homepage, https://rpy2.github.io
 Project-URL: Documentation, https://rpy2.github.io/doc.html
 Project-URL: Source, https://github.com/rpy2/rpy2
 Project-URL: Tracker, https://github.com/rpy2/rpy2/issue
@@ -18,14 +18,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: numpy
 Provides-Extra: pandas
+Provides-Extra: types
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 # Python -> R bridge
 
 [![pypi](https://img.shields.io/pypi/v/rpy2.svg?style=flat-square)](https://pypi.python.org/pypi/rpy2)
@@ -47,15 +48,15 @@
 specific functionalities not otherwise required to use the rest of rpy2.
 
 For example, to be able to run the unit tests:
 ```bash
 pip install rpy2[test]
 ```
 
-To install all dependencies, use:
+To install all optional dependencies (numpy, pandas, ipython), use:
 
 ```bash
 pip install rpy2[all]
 ```
 
 The package is known to compile on Linux, MacOSX
 (provided that developper tools are installed, and you are ready
```

### Comparing `rpy2-3.5.8/README.md` & `rpy2-3.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 specific functionalities not otherwise required to use the rest of rpy2.
 
 For example, to be able to run the unit tests:
 ```bash
 pip install rpy2[test]
 ```
 
-To install all dependencies, use:
+To install all optional dependencies (numpy, pandas, ipython), use:
 
 ```bash
 pip install rpy2[all]
 ```
 
 The package is known to compile on Linux, MacOSX
 (provided that developper tools are installed, and you are ready
```

### Comparing `rpy2-3.5.8/doc/Makefile` & `rpy2-3.5.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/gpl-2.0.txt` & `rpy2-3.5.9/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/pyproject.toml` & `rpy2-3.5.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,19 @@
     "tzlocal",
     "packaging;platform_system=='Windows'",
     "typing-extensions;python_version<'3.8'"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-test = ["pytest", "ipython", "numpy", "pandas"]
-numpy = ["pandas"]
-pandas = ["numpy", "pandas"]
-all = ["pytest", "ipython", "pandas", "numpy"]
+test = ["pytest", "ipython", "numpy", "pandas>=1.2.0"]
+numpy = []
+pandas = ["numpy", "pandas>=1.2.0"]
+types = ["mypy", "types-pytz", "types-tzlocal"]
+all = ["pytest", "ipython", "pandas>=1.2.0", "numpy"]
 
 [project.urls]
 Homepage = "https://rpy2.github.io"
 Documentation = "https://rpy2.github.io/doc.html"
 Source = "https://github.com/rpy2/rpy2"
 Tracker = "https://github.com/rpy2/rpy2/issue"
```

### Comparing `rpy2-3.5.8/rpy2/_rinterface_cffi_build.py` & `rpy2-3.5.9/rpy2/_rinterface_cffi_build.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/interactive/__init__.py` & `rpy2-3.5.9/rpy2/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/interactive/packages.py` & `rpy2-3.5.9/rpy2/interactive/packages.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/interactive/process_revents.py` & `rpy2-3.5.9/rpy2/interactive/process_revents.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/ipython/ggplot.py` & `rpy2-3.5.9/rpy2/ipython/ggplot.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/ipython/html.py` & `rpy2-3.5.9/rpy2/ipython/html.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/ipython/rmagic.py` & `rpy2-3.5.9/rpy2/ipython/rmagic.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,35 +352,48 @@
         return value
 
     def _import_name_into_r(
             self, arg: str, env: ri.SexpEnvironment,
             local_ns: dict
     ) -> None:
         lhs, rhs = _parse_input_argument(arg)
+        val = None
         try:
             val = _find(rhs, local_ns)
         except NameError:
-            val = _find(rhs, self.shell.user_ns)
-        env[lhs] = val
+            if self.shell is None:
+                warnings.warn(
+                    f'The shell is None. Unable to look for {rhs}.'
+                )
+            else:
+                val = _find(rhs, self.shell.user_ns)
+        if val is not None:
+            env[lhs] = val
 
     def _find_converter(
             self, name: str, local_ns: dict
     ) -> ro.conversion.Converter:
+        converter = None
         if name is None:
             converter = self.converter
         else:
             try:
                 converter = _find(name, local_ns)
             except NameError:
-                converter = _find(name, self.shell.user_ns)
+                if self.shell is None:
+                    warnings.warn(
+                        f'The shell is None. Unable to look for converter {name}.'
+                    )
+                else:
+                    converter = _find(name, self.shell.user_ns)
 
-            if not isinstance(converter, Converter):
-                raise TypeError("'%s' must be a %s object (but it is a %s)."
-                                % (converter, Converter,
-                                   type(converter)))
+        if not isinstance(converter, Converter):
+            raise TypeError("'%s' must be a %s object (but it is a %s)."
+                            % (converter, Converter,
+                               type(converter)))
         return converter
 
     # @skip_doctest
     @magic_arguments()
     @argument(
         '-c', '--converter',
         default=None,
```

### Comparing `rpy2-3.5.8/rpy2/rinterface.py` & `rpy2-3.5.9/rpy2/rinterface.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/R_API.h` & `rpy2-3.5.9/rpy2/rinterface_lib/R_API.h`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/R_API_eventloop.h` & `rpy2-3.5.9/rpy2/rinterface_lib/R_API_eventloop.h`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/_bufferprotocol.c` & `rpy2-3.5.9/rpy2/rinterface_lib/_bufferprotocol.c`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/_rinterface_capi.py` & `rpy2-3.5.9/rpy2/rinterface_lib/_rinterface_capi.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/bufferprotocol.py` & `rpy2-3.5.9/rpy2/rinterface_lib/bufferprotocol.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/callbacks.py` & `rpy2-3.5.9/rpy2/rinterface_lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/conversion.py` & `rpy2-3.5.9/rpy2/rinterface_lib/conversion.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/embedded.py` & `rpy2-3.5.9/rpy2/rinterface_lib/embedded.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/embedded_mswin.py` & `rpy2-3.5.9/rpy2/rinterface_lib/embedded_mswin.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 _DEFAULT_MAX_NSIZE: int = 50000000  # max language heap size
 _DEFAULT_PPSIZE: int = 50000  # stack size
 _DEFAULT_C_STACK_LIMIT: int = -1
 _DEFAULT_R_INTERACTIVE: bool = True
 
 
 def _initr_win32(
-        interactive: bool = True,
+        interactive: typing.Optional[bool] = None,
         _want_setcallbacks: bool = True,
-        _c_stack_limit: int = _DEFAULT_C_STACK_LIMIT
+        _c_stack_limit: typing.Optional[int] = _DEFAULT_C_STACK_LIMIT
 
 ) -> typing.Optional[int]:
     """Initialize the embedded R.
 
     :param interactive: Should R run in interactive or non-interactive mode?
     if `None` the value in `_DEFAULT_R_INTERACTIVE` will be used.
     :param _want_setcallbacks: Should custom rpy2 callbacks for R frontends
```

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/ffi_proxy.py` & `rpy2-3.5.9/rpy2/rinterface_lib/ffi_proxy.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/memorymanagement.py` & `rpy2-3.5.9/rpy2/rinterface_lib/memorymanagement.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/na_values.py` & `rpy2-3.5.9/rpy2/rinterface_lib/na_values.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/openrlib.py` & `rpy2-3.5.9/rpy2/rinterface_lib/openrlib.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rinterface_lib/sexp.py` & `rpy2-3.5.9/rpy2/rinterface_lib/sexp.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rlike/container.py` & `rpy2-3.5.9/rpy2/rlike/container.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/rlike/functional.py` & `rpy2-3.5.9/rpy2/rlike/functional.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/__init__.py` & `rpy2-3.5.9/rpy2/robjects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     clsmap = (conversion.converter_ctx.get()
               .rpy2py_nc_name[rinterface.BoolSexpVector])
     cls = clsmap.find(obj.rclass)
     return cls(obj)
 
 
 @default_converter.rpy2py.register(rinterface.StrSexpVector)
-def _convert_rpy2py_strvector(obj):    
+def _convert_rpy2py_strvector(obj):
     cls = _vector_matrix_array(obj, vectors.StrVector,
                                vectors.StrMatrix, vectors.StrArray)
     return cls(obj)
 
 
 @default_converter.rpy2py.register(rinterface.ByteSexpVector)
 def _convert_rpy2py_bytevector(obj):
```

### Comparing `rpy2-3.5.8/rpy2/robjects/conversion.py` & `rpy2-3.5.9/rpy2/robjects/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,21 +300,32 @@
         assert isinstance(converter, Converter)
         new_name = '%s + %s' % (self.name, converter.name)
         # create a copy of `self` as the result converter
         result_converter = Converter(new_name, template=self)
         overlay_converter(converter, result_converter)
         return result_converter
 
+    def context(self) -> 'ConversionContext':
+        """
+        Create a Conversion context to use in a `with` statement.
+
+        >>> with conversion_rules.context() as cv:
+        ...     # Do something while using those conversion_rules.
+        >>> # Do something else whith the earlier conversion rules restored.
+
+        :return: A :class:`ConversionContext`
+        """
+        return ConversionContext(self)
+
     def __enter__(self):
-        self._original_converter = converter_ctx.get()
-        set_conversion(self)
-        return self
+        raise Exception(
+            "Use the converter's method context instead."
+        )
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        set_conversion(self._original_converter)
         return False
 
     def __str__(self):
         res = [str(type(self))]
         for subcv in ('py2rpy', 'rpy2py'):
             res.append(subcv)
             for cls in getattr(self, subcv).registry.keys():
```

### Comparing `rpy2-3.5.8/rpy2/robjects/environments.py` & `rpy2-3.5.9/rpy2/robjects/environments.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/functions.py` & `rpy2-3.5.9/rpy2/robjects/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 # Needed to avoid circular imports.
 __formals = baseenv_ri.find('formals')
 __args = baseenv_ri.find('args')
 __is_null = baseenv_ri.find('is.null')
 
 
 def _formals_fixed(func):
-    res = __formals(func)
-    if res is rpy2.rinterface_lib.sexp.NULL:
-        res = __formals(__args(func))
+    if func.typeof is rpy2.rinterface_lib.sexp.RTYPES.SPECIALSXP:
+        res = rpy2.rinterface_lib.sexp.NULL
+    else:
+        res = __formals(func)
+        if res is rpy2.rinterface_lib.sexp.NULL:
+            res = __formals(__args(func))
     return res
 
 
 # docstring_property and DocstringProperty
 # from Bradley Froehle
 # https://gist.github.com/bfroehle/4041015
 def docstring_property(class_doc):
```

### Comparing `rpy2-3.5.8/rpy2/robjects/help.py` & `rpy2-3.5.9/rpy2/robjects/help.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/language.py` & `rpy2-3.5.9/rpy2/robjects/language.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/dbplyr.py` & `rpy2-3.5.9/rpy2/robjects/lib/dbplyr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/dplyr.py` & `rpy2-3.5.9/rpy2/robjects/lib/dplyr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/ggplot2.py` & `rpy2-3.5.9/rpy2/robjects/lib/ggplot2.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/grdevices.py` & `rpy2-3.5.9/rpy2/robjects/lib/grdevices.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/grid.py` & `rpy2-3.5.9/rpy2/robjects/lib/grid.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/lib/tidyr.py` & `rpy2-3.5.9/rpy2/robjects/lib/tidyr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/methods.py` & `rpy2-3.5.9/rpy2/robjects/methods.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/numpy2ri.py` & `rpy2-3.5.9/rpy2/robjects/numpy2ri.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,22 +164,23 @@
     # (will become integers), so we build a temporary list o2
     # with the factors as strings. This fix might good to have
     # as a default.
     o2 = list()
     # An added complication is that the conversion defined
     # in this module will make __getitem__ at the robjects
     # level return numpy arrays
-    for column in rinterface.ListSexpVector(obj):
-        if 'factor' in column.rclass:
-            levels = column.do_slot('levels')
-            column = tuple(
-                None if x is rinterface.NA_Integer
-                else levels[x-1] for x in column
-            )
-        o2.append(column)
+    with conversion.get_conversion().context() as cv:
+        for column in rinterface.ListSexpVector(obj):
+            if 'factor' in column.rclass:
+                levels = column.do_slot('levels')
+                column = tuple(
+                    None if x is rinterface.NA_Integer
+                    else levels[x-1] for x in column
+                )
+            o2.append(cv.rpy2py(column))
     names = obj.do_slot('names')
     if names == rinterface.NULL:
         res = numpy.rec.fromarrays(o2)
     else:
         res = numpy.rec.fromarrays(o2, names=tuple(names))
     return res
 
@@ -198,23 +199,33 @@
 
 
 @rpy2py.register(rinterface.FloatSexpVector)
 def rpy2py_floatvector(obj):
     return numpy.array(obj)
 
 
+@rpy2py.register(rinterface.CharSexp)
+def rpy2py_charvector(obj):
+    if obj == rinterface.NA_Character:
+        return None
+    else:
+        return obj
+
+
+@rpy2py.register(rinterface.StrSexpVector)
+def rpy2py_strvector(obj):
+    res = numpy.array(obj)
+    res[res == rinterface.NA_Character] = None
+    return res
+
+
 @rpy2py.register(Sexp)
 def rpy2py_sexp(obj):
-    if obj.typeof is rinterface.RTYPES.CHARSXP:
-        res = None
-    elif (obj.typeof in _vectortypes) and (obj.typeof != RTYPES.VECSXP):
+    if (obj.typeof in _vectortypes) and (obj.typeof != RTYPES.VECSXP):
         res = numpy.array(obj)
-        # Special case for R string arrays.
-        if obj.typeof is rinterface.RTYPES.STRSXP:
-            res[res == rinterface.NA_Character] = None
     else:
         res = ro.default_converter.rpy2py(obj)
     return res
 
 
 converter._rpy2py_nc_map.update(
     {
```

### Comparing `rpy2-3.5.8/rpy2/robjects/packages.py` & `rpy2-3.5.9/rpy2/robjects/packages.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/packages_utils.py` & `rpy2-3.5.9/rpy2/robjects/packages_utils.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/pandas2ri.py` & `rpy2-3.5.9/rpy2/robjects/pandas2ri.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/robject.py` & `rpy2-3.5.9/rpy2/robjects/robject.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/robjects/vectors.py` & `rpy2-3.5.9/rpy2/robjects/vectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1260,15 +1260,15 @@
             will not be turned to string vectors.
         :param checknames: Boolean indicating whether column names
             should be transformed to R syntactically valid names.
         """
         if isinstance(obj, rinterface.ListSexpVector):
             if obj.typeof != rinterface.RTYPES.VECSXP:
                 raise ValueError(
-                    "obj should of typeof RTYPES.VECSXP "
+                    "obj should be of typeof RTYPES.VECSXP "
                     " (and we get %s)" % rinterface.RTYPES(obj.typeof)
                 )
             if (
                     self._is_list(obj)[0] or
                     globalenv_ri.find('inherits')(
                         obj, self._dataframe_name
                     )[0]
```

### Comparing `rpy2-3.5.8/rpy2/situation.py` & `rpy2-3.5.9/rpy2/situation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,14 @@
 logger = logging.getLogger(__name__)
 
 if sys.maxsize > 2**32:
     r_version_folder = 'x64'
 else:
     r_version_folder = 'i386'
 
-try:
-    import rpy2  # noqa:F401
-    has_rpy2 = True
-except ImportError:
-    has_rpy2 = False
-
 
 class CFFI_MODE(enum.Enum):
     API = 'API'
     ABI = 'ABI'
     BOTH = 'BOTH'
     ANY = 'ANY'
 
@@ -185,17 +179,17 @@
     return lib_path
 
 
 # TODO: Does r_ld_library_path_from_subprocess() supersed this?
 def get_rlib_path(r_home: str, system: str) -> str:
     """Get the path for the R shared library."""
     if system == 'FreeBSD' or system == 'Linux':
-        lib_path = os.path.join(r_home, get_r_libnn(r_home), 'libR.so')
+        lib_path = os.path.join(r_home, 'lib', 'libR.so')
     elif system == 'Darwin':
-        lib_path = os.path.join(r_home, get_r_libnn(r_home), 'libR.dylib')
+        lib_path = os.path.join(r_home, 'lib', 'libR.dylib')
     elif system == 'Windows':
         # i386
         os.environ['PATH'] = os.pathsep.join(
             (os.environ['PATH'],
              os.path.join(r_home, 'bin', r_version_folder))
         )
         lib_path = os.path.join(r_home, 'bin', r_version_folder, 'R.dll')
@@ -363,21 +357,21 @@
 
 
 def iter_info():
 
     make_bold = _make_bold_win32 if os.name == 'nt' else _make_bold_unix
 
     yield make_bold('rpy2 version:')
-    if has_rpy2:
+    try:
         # TODO: the repeated import is needed, without which Python
         #   raises an UnboundLocalError (local variable reference before
         #   assignment).
         import rpy2  # noqa: F811
         yield rpy2.__version__
-    else:
+    except ImportError:
         yield 'rpy2 cannot be imported'
 
     yield make_bold('Python version:')
     yield sys.version
 
     yield make_bold("Looking for R's HOME:")
 
@@ -417,24 +411,25 @@
     if os.name != 'nt':
         yield make_bold("R's additions to LD_LIBRARY_PATH:")
         if r_home is None:
             yield '     *** undefined when not R home can be determined'
         else:
             yield r_ld_library_path_from_subprocess(r_home)
 
-    if has_rpy2:
+    try:
+        import rpy2.rinterface_lib.openrlib
+        rlib_status = 'OK'
+    except ImportError as ie:
         try:
-            import rpy2.rinterface_lib.openrlib
-            rlib_status = 'OK'
-        except ImportError as ie:
+            import rpy2
             rlib_status = '*** Error while loading: %s ***' % str(ie)
-        except OSError as ose:
-            rlib_status = str(ose)
-    else:
-        rlib_status = '*** rpy2 is not installed'
+        except ImportError:
+            rlib_status = '*** rpy2 is not installed'
+    except OSError as ose:
+        rlib_status = str(ose)
 
     yield make_bold("R version:")
     yield '    In the PATH: %s' % r_version_from_subprocess()
     yield '    Loading R library from rpy2: %s' % rlib_status
 
     r_libs = os.environ.get('R_LIBS')
     yield make_bold('Additional directories to load R packages from:')
```

### Comparing `rpy2-3.5.8/rpy2/tests/ipython/test_ggplot.py` & `rpy2-3.5.9/rpy2/tests/ipython/test_ggplot.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/ipython/test_html.py` & `rpy2-3.5.9/rpy2/tests/ipython/test_html.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/ipython/test_rmagic.py` & `rpy2-3.5.9/rpy2/tests/ipython/test_rmagic.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_bufferprotocol.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_bufferprotocol.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_callbacks.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_embedded_r.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_embedded_r.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_environment.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_environment.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_externalptr.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_externalptr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_functions.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_functions.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_memorymanagement.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_memorymanagement.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_na.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_na.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_noinitialization.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_noinitialization.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_openrlib.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_openrlib.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_sexp.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_sexp.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_symbol.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_symbol.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_threading.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_threading.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_bool.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_bool.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_byte.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_byte.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_complex.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_complex.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_float.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_float.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_int.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_int.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_lang.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_lang.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_list.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_list.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_numpy.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_numpy.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_pairlist.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_pairlist.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vector_str.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vector_str.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rinterface/test_vectors.py` & `rpy2-3.5.9/rpy2/tests/rinterface/test_vectors.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rlike/test_container.py` & `rpy2-3.5.9/rpy2/tests/rlike/test_container.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/rlike/test_functional.py` & `rpy2-3.5.9/rpy2/tests/rlike/test_functional.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/lib/test_dplyr.py` & `rpy2-3.5.9/rpy2/tests/robjects/lib/test_dplyr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/lib/test_ggplot2.py` & `rpy2-3.5.9/rpy2/tests/robjects/lib/test_ggplot2.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/lib/test_grdevices.py` & `rpy2-3.5.9/rpy2/tests/robjects/lib/test_grdevices.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/lib/test_grid.py` & `rpy2-3.5.9/rpy2/tests/robjects/lib/test_grid.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/lib/test_tidyr.py` & `rpy2-3.5.9/rpy2/tests/robjects/lib/test_tidyr.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_array.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_array.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_conversion.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_conversion.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_conversion_numpy.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_conversion_numpy.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,29 +17,21 @@
     import numpy
     has_numpy = True
     import rpy2.robjects.numpy2ri as rpyn
 except:
     numpy = DummyNamespace()
 
 
-@pytest.fixture()
-def numpy_conversion():
-    with conversion.localconverter(
-            robjects.default_converter + rpyn.converter
-    ) as lc:
-        yield
-
-
 @pytest.mark.skipif(not has_numpy,
                     reason='package numpy cannot be imported')
-@pytest.mark.usefixtures('numpy_conversion')
 class TestNumpyConversions(object):
 
     def check_homogeneous(self, obj, mode, storage_mode):
-        converted = conversion.converter_ctx.get().py2rpy(obj)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            converted = cv.py2rpy(obj)
         assert r["mode"](converted)[0] == mode
         assert r["storage.mode"](converted)[0] == storage_mode
         assert list(obj) == list(converted)
         assert r["is.array"](converted)[0] is True
         return converted
 
     def test_vector_boolean(self):
@@ -49,15 +41,15 @@
         assert tuple(l) == tuple(b_r)
 
     def test_vector_integer(self):
         l = [1, 2, 3]
         i = numpy.array(l, dtype="i")
         i_r = self.check_homogeneous(i, "numeric", "integer")
         assert tuple(l) == tuple(i_r)
-        
+
     def test_vector_float(self):
         l = [1.0, 2.0, 3.0]
         f = numpy.array(l, dtype="f")
         f_r = self.check_homogeneous(f, "numeric", "double")
         for orig, conv in zip(l, f_r):
             assert abs(orig-conv) < 0.000001
         
@@ -74,31 +66,33 @@
         u = numpy.array(l, dtype="U")
         u_r = self.check_homogeneous(u, "character", "character")
         assert tuple(l) == tuple(u_r)
 
     def test_vector_bytes(self):
         l = [b'a', b'b', b'c']
         s = numpy.array(l, dtype = '|S1')
-        converted = conversion.converter_ctx.get().py2rpy(s)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            converted = cv.py2rpy(s)
         assert r["mode"](converted)[0] == 'raw'
         assert r["storage.mode"](converted)[0] == 'raw'
         assert bytearray(b''.join(l)) == bytearray(converted)
 
     def test_array(self):
-
         i2d = numpy.array([[1, 2, 3], [4, 5, 6]], dtype='i')
-        i2d_r = conversion.converter_ctx.get().py2rpy(i2d)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            i2d_r = cv.py2rpy(i2d)
         assert r['storage.mode'](i2d_r)[0] == 'integer'
         assert tuple(r['dim'](i2d_r)) == (2, 3)
 
         # Make sure we got the row/column swap right:
         assert r['['](i2d_r, 1, 2)[0] == i2d[0, 1]
 
         f3d = numpy.arange(24, dtype='f').reshape((2, 3, 4))
-        f3d_r = conversion.converter_ctx.get().py2rpy(f3d)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            f3d_r = cv.py2rpy(f3d)
 
         assert r['storage.mode'](f3d_r)[0] == 'double'
         assert tuple(r['dim'](f3d_r)) == (2, 3, 4)
 
         # Make sure we got the row/column swap right:
         #assert r['['](f3d_r, 1, 2, 3)[0] == f3d[0, 1, 2]
 
@@ -107,75 +101,79 @@
     @pytest.mark.parametrize(
         'constructor',
         (numpy.int32, numpy.int64,
          numpy.uint32, numpy.uint64)
     )
     def test_scalar_int(self, constructor):
         np_value = constructor(100)
-        r_vec = conversion.converter_ctx.get().py2rpy(np_value)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            r_vec = cv.py2rpy(np_value)
         r_scalar = numpy.array(r_vec)[0]
         assert np_value == r_scalar
 
     @pytest.mark.skipif(not (has_numpy and hasattr(numpy, 'float128')),
                         reason='numpy.float128 not available on this system')
     def test_scalar_f128(self):
         f128 = numpy.float128(100.000000003)
-        f128_r = conversion.converter_ctx.get().py2rpy(f128)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            f128_r = cv.py2rpy(f128)
         f128_test = numpy.array(f128_r)[0]
         assert f128 == f128_test
 
     def test_object_array(self):
         o = numpy.array([1, "a", 3.2], dtype=numpy.object_)
-        o_r = conversion.converter_ctx.get().py2rpy(o)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            o_r = cv.py2rpy(o)
         assert r['mode'](o_r)[0] == 'list'
         assert r['[['](o_r, 1)[0] == 1
         assert r['[['](o_r, 2)[0] == 'a'
         assert r['[['](o_r, 3)[0] == 3.2
 
     def test_record_array(self):
         rec = numpy.array([(1, 2.3), (2, -0.7), (3, 12.1)],
                           dtype=[("count", "i"), ("value", numpy.double)])
-        rec_r = conversion.converter_ctx.get().py2rpy(rec)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            rec_r = cv.py2rpy(rec)
         assert r["is.data.frame"](rec_r)[0] is True
         assert tuple(r["names"](rec_r)) == ("count", "value")
         count_r = rec_r[rec_r.names.index('count')]
         value_r = rec_r[rec_r.names.index('value')]
         assert r["storage.mode"](count_r)[0] == 'integer'
         assert r["storage.mode"](value_r)[0] == 'double'
         assert count_r[1] == 2
         assert value_r[2] == 12.1
 
     def test_bad_array(self):
         u = numpy.array([1, 2, 3], dtype=numpy.uint32)
         with pytest.raises(ValueError):
-            conversion.converter_ctx.get().py2rpy(u)
+            with (robjects.default_converter + rpyn.converter).context() as cv:
+                cv.py2rpy(u)
 
     def test_assign_numpy_object(self):
         x = numpy.arange(-10., 10., 1)
         env = robjects.Environment()
-        env['x'] = x
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            env['x'] = x
         assert len(env) == 1
         # do have an R object of the right type ?
-        with conversion.localconverter(
-            robjects.default_converter
-        ) as lc:
+        with robjects.default_converter.context() as lc:
             x_r = env['x']
 
         assert robjects.rinterface.RTYPES.REALSXP == x_r.typeof
         #
         assert tuple(x_r.dim) == (20,)
 
-
     def test_dataframe_to_numpy(self):
         df = robjects.vectors.DataFrame(
             {'a': 1,
              'b': 2,
              'c': robjects.vectors.FactorVector('e'),
              'd': robjects.vectors.StrVector(['xyz'])})
-        rec = conversion.rpy2py(df)
+        with conversion.localconverter(robjects.default_converter + rpyn.converter) as cv:
+            rec = cv.rpy2py(df)
         assert numpy.recarray == type(rec)
         assert rec.a[0] == 1
         assert rec.b[0] == 2
         assert rec.c[0] == 'e'
         assert rec.d[0] == 'xyz'
 
     @pytest.mark.parametrize(
@@ -187,40 +185,44 @@
         df = cls(
             robjects.ListVector(
                 {'a': 1,
                  'b': 2,
                  'c': robjects.vectors.FactorVector('e')}
             )
         )
-        rec = conversion.rpy2py(df)
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            rec = cv.rpy2py(df)
         assert rpy2.rlike.container.OrdDict == type(rec)
         assert rec['a'][0] == 1
         assert rec['b'][0] == 2
         assert rec['c'][0] == 1  # not 'e'.
 
-
     def test_atomic_vector_to_numpy(self):
         v = robjects.vectors.IntVector((1,2,3))
-        a = rpyn.rpy2py(v)
+        with rpyn.converter.context() as cv:
+            a = cv.rpy2py(v)
         assert isinstance(a, numpy.ndarray)
         assert v[0] == 1
 
     def test_rx2(self):
         df = robjects.vectors.DataFrame({
             "A": robjects.vectors.IntVector([1,2,3]),
             "B": robjects.vectors.IntVector([1,2,3])})
-        b = df.rx2('B')
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            b = df.rx2('B')
         assert tuple((1,2,3)) == tuple(b)
 
     def test_rint_to_numpy(self):
-        a = robjects.r('c(1:4)')
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            a = robjects.r('c(1:4)')
         assert isinstance(a, numpy.ndarray)
 
     def test_rfloat_to_numpy(self):
-        a = robjects.r('c(1.0, 2.0, 3.0)')
+        with (robjects.default_converter + rpyn.converter).context() as cv:
+            a = robjects.r('c(1.0, 2.0, 3.0)')
         assert isinstance(a, numpy.ndarray)
 
 
 @pytest.mark.skipif(not has_numpy,
                     reason='package numpy cannot be imported')
 @pytest.mark.parametrize('dtype',
                          ('uint32', 'uint64'))
@@ -250,7 +252,28 @@
                           ([b'a', b'b', b'c'], rinterface.ByteSexpVector)))
 def test_numpy_O_py2rpy(values, expected_cls):
     a = numpy.array(values, dtype='O')
     v = rpyn.numpy_O_py2rpy(a)
     assert isinstance(v, expected_cls)
 
     
+@pytest.mark.skipif(not has_numpy,
+                    reason='package numpy cannot be imported')
+@pytest.mark.parametrize(
+    'rcode,expected_values',
+    (('c(TRUE, FALSE)', (True, False, )),
+     ('c(1, 2, 3)', (1, 2, 3)),
+     ('c(1.0, 2.0, 3.0)', (1.0, 2.0, 3.0)),
+     ('c("ab", "cd", NA_character_)', ('ab', 'cd', None)))
+)
+def test_rpy2py(rcode, expected_values):
+    with (robjects.default_converter + rpyn.converter).context():
+        values = robjects.r(rcode)
+    assert tuple(values) == expected_values
+
+
+@pytest.mark.skipif(not has_numpy,
+                    reason='package numpy cannot be imported')
+def test_NA_CharSexp():
+    with (robjects.default_converter + rpyn.converter).context():
+        values = robjects.r('c(NA_character_)')
+    assert values[0] is None
```

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_dataframe.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_environment.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_environment.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_formula.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_formula.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_function.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_function.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_help.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_help.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_language.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_language.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_methods.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_methods.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_packages.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_packages.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_packages_utils.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_packages_utils.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_pandas_conversions.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_pandas_conversions.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_robjects.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_robjects.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_rs4.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_rs4.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_serialization.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_serialization.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_translated_function.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_translated_function.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_vector.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_vector.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_vector_datetime.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_vector_datetime.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_vector_extractdelegator.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_vector_extractdelegator.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2/tests/robjects/test_vector_factor.py` & `rpy2-3.5.9/rpy2/tests/robjects/test_vector_factor.py`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/rpy2.egg-info/PKG-INFO` & `rpy2-3.5.9/rpy2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpy2
-Version: 3.5.8
+Version: 3.5.9
 Summary: Python interface to the R language (embedded R)
 Author-email: Laurent Gautier <lgautier@gmail.com>
 License: GPLv2+
 Project-URL: Homepage, https://rpy2.github.io
 Project-URL: Documentation, https://rpy2.github.io/doc.html
 Project-URL: Source, https://github.com/rpy2/rpy2
 Project-URL: Tracker, https://github.com/rpy2/rpy2/issue
@@ -18,14 +18,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: numpy
 Provides-Extra: pandas
+Provides-Extra: types
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 # Python -> R bridge
 
 [![pypi](https://img.shields.io/pypi/v/rpy2.svg?style=flat-square)](https://pypi.python.org/pypi/rpy2)
@@ -47,15 +48,15 @@
 specific functionalities not otherwise required to use the rest of rpy2.
 
 For example, to be able to run the unit tests:
 ```bash
 pip install rpy2[test]
 ```
 
-To install all dependencies, use:
+To install all optional dependencies (numpy, pandas, ipython), use:
 
 ```bash
 pip install rpy2[all]
 ```
 
 The package is known to compile on Linux, MacOSX
 (provided that developper tools are installed, and you are ready
```

### Comparing `rpy2-3.5.8/rpy2.egg-info/SOURCES.txt` & `rpy2-3.5.9/rpy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpy2-3.5.8/setup.py` & `rpy2-3.5.9/setup.py`

 * *Files identical despite different names*

