# Comparing `tmp/Sekiryu-0.0.1.tar.gz` & `tmp/sekiryu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sekiryu-0.0.1.tar", last modified: Sun Feb 26 18:29:42 2023, max compression
+gzip compressed data, was "sekiryu-0.0.2.tar", last modified: Mon Jun 26 18:29:24 2023, max compression
```

## Comparing `Sekiryu-0.0.1.tar` & `sekiryu-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,73 @@
-drwxr-xr-x   0 vm        (1000) vm        (1000)        0 2023-02-26 18:29:42.248953 Sekiryu-0.0.1/
--rw-r--r--   0 vm        (1000) vm        (1000)    11325 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/LICENSE
--rw-r--r--   0 vm        (1000) vm        (1000)     2827 2023-02-26 18:29:42.240953 Sekiryu-0.0.1/PKG-INFO
--rw-r--r--   0 vm        (1000) vm        (1000)     2405 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/README.md
-drwxr-xr-x   0 vm        (1000) vm        (1000)        0 2023-02-26 18:29:42.240953 Sekiryu-0.0.1/Sekiryu.egg-info/
--rw-r--r--   0 vm        (1000) vm        (1000)     2827 2023-02-26 18:29:42.000000 Sekiryu-0.0.1/Sekiryu.egg-info/PKG-INFO
--rw-r--r--   0 vm        (1000) vm        (1000)      189 2023-02-26 18:29:42.000000 Sekiryu-0.0.1/Sekiryu.egg-info/SOURCES.txt
--rw-r--r--   0 vm        (1000) vm        (1000)        1 2023-02-26 18:29:42.000000 Sekiryu-0.0.1/Sekiryu.egg-info/dependency_links.txt
--rw-r--r--   0 vm        (1000) vm        (1000)        1 2023-02-26 18:29:42.000000 Sekiryu-0.0.1/Sekiryu.egg-info/top_level.txt
--rw-r--r--   0 vm        (1000) vm        (1000)      254 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/binjai.py
--rw-r--r--   0 vm        (1000) vm        (1000)     3515 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/ghidrai.py
--rw-r--r--   0 vm        (1000) vm        (1000)       44 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/idai.py
--rw-r--r--   0 vm        (1000) vm        (1000)     3016 2023-02-26 17:57:06.000000 Sekiryu-0.0.1/server.py
--rw-r--r--   0 vm        (1000) vm        (1000)       38 2023-02-26 18:29:42.248953 Sekiryu-0.0.1/setup.cfg
--rw-r--r--   0 vm        (1000) vm        (1000)      641 2023-02-26 18:29:38.000000 Sekiryu-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.944863 sekiryu-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11325 2023-06-26 16:54:09.000000 sekiryu-0.0.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-06-26 18:29:24.944863 sekiryu-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7579 2023-06-26 16:54:09.000000 sekiryu-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.932863 sekiryu-0.0.2/sekiryu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3038 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-26 18:29:24.000000 sekiryu-0.0.2/sekiryu.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 18:29:24.944863 sekiryu-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-06-26 17:43:42.000000 sekiryu-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.932863 sekiryu-0.0.2/sources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.932863 sekiryu-0.0.2/sources/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4615 2023-06-26 17:53:16.000000 sekiryu-0.0.2/sources/modules/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2628 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/ghidra_pilot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3094 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/pcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5018 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/report.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.944863 sekiryu-0.0.2/sources/modules/rules_sgrep/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-26 17:33:35.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/argv-envp-access.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/bad-words.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1110 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/command-injection.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1570 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/double-free.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3605 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/format-string-bugs.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2462 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/incorrect-order-setuid-setgid-etc.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1686 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/incorrect-unsigned-comparison.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1445 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/incorrect-use-of-sizeof.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/incorrect-use-of-strncat.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1674 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/incorrect-use-of-strncpy-stpncpy-strlcpy.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-access-stat-lstat.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      982 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-alloca.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      633 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-atoi-atol-atof.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-gets.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      714 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-mktemp-tmpnam-tempnam.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1384 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-rand-srand.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-scanf-etc.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1566 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-sprintf-vsprintf.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/insecure-api-strcpy-stpcpy-strcat.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4732 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/integer-truncation.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3196 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/integer-wraparound.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3246 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/interesting-api-calls.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1984 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/memory-address-exposure.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/mismatched-memory-management-cpp.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2749 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/mismatched-memory-management-cpp.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/mismatched-memory-management.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1677 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/missing-break-in-switch.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      664 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/missing-default-in-switch.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/off-by-one.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/pointer-subtraction.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2318 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/ret-stack-address.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      626 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/signed-unsigned-conversion.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5387 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/signed-unsigned-conversion.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3424 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/typos.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3335 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unchecked-ret-malloc-calloc-realloc.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unchecked-ret-setuid-seteuid.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unsafe-ret-snprintf-vsnprintf.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1340 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unsafe-ret-strlcpy-strlcat.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unsafe-strlen.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2912 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/unterminated-string-strncpy-stpncpy.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2992 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/use-after-free.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4659 2023-06-26 17:07:48.000000 sekiryu-0.0.2/sources/modules/rules_sgrep/write-into-stack-buffer.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 18:29:24.944863 sekiryu-0.0.2/sources/modules/scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/scripts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/scripts/bindiff_export.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2367 2023-06-26 18:18:22.000000 sekiryu-0.0.2/sources/modules/scripts/ghidra_decompiler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2149 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-06-26 18:06:08.000000 sekiryu-0.0.2/sources/modules/sgrep.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8341 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/modules/vuln_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-06-26 16:54:09.000000 sekiryu-0.0.2/sources/sekiryu.py
```

### Comparing `Sekiryu-0.0.1/LICENSE` & `sekiryu-0.0.2/LICENSE`

 * *Files identical despite different names*

