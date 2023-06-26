# Comparing `tmp/pymadng-0.3.9.tar.gz` & `tmp/pymadng-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymadng-0.3.9.tar", last modified: Sun Mar 12 16:22:32 2023, max compression
+gzip compressed data, was "pymadng-0.4.0.tar", last modified: Mon Jun 26 17:21:58 2023, max compression
```

## Comparing `pymadng-0.3.9.tar` & `pymadng-0.4.0.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.715580 pymadng-0.3.9/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2172 2023-02-06 15:19:39.000000 pymadng-0.3.9/.gitignore
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      219 2023-03-12 16:22:13.000000 pymadng-0.3.9/CHANGELOG
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    35149 2022-09-30 08:02:42.000000 pymadng-0.3.9/LICENSE
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      186 2022-12-08 17:54:02.000000 pymadng-0.3.9/MANIFEST.in
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3212 2023-03-12 16:22:32.715580 pymadng-0.3.9/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2353 2023-02-08 17:12:43.000000 pymadng-0.3.9/README.md
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.683580 pymadng-0.3.9/docs/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      638 2022-11-28 11:54:22.000000 pymadng-0.3.9/docs/Makefile
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      804 2022-11-28 11:54:22.000000 pymadng-0.3.9/docs/make.bat
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      116 2023-02-09 14:03:03.000000 pymadng-0.3.9/docs/requirements.txt
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.687580 pymadng-0.3.9/docs/source/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1364 2023-02-13 10:47:45.000000 pymadng-0.3.9/docs/source/conf.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5508 2023-02-13 12:53:52.000000 pymadng-0.3.9/docs/source/ex-fodo.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3061 2023-02-13 12:54:47.000000 pymadng-0.3.9/docs/source/ex-lhc-couplingLocal.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4974 2023-02-21 15:14:27.000000 pymadng-0.3.9/docs/source/ex-lowlevel.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4652 2023-02-13 12:52:26.000000 pymadng-0.3.9/docs/source/ex-managing-refs.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3224 2022-12-02 11:03:49.000000 pymadng-0.3.9/docs/source/ex-recv-lhc.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1092 2023-02-13 13:34:46.000000 pymadng-0.3.9/docs/source/examples.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     8135 2023-02-13 12:58:26.000000 pymadng-0.3.9/docs/source/gettingstarted.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      577 2023-02-13 12:43:39.000000 pymadng-0.3.9/docs/source/index.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       70 2022-12-02 15:23:48.000000 pymadng-0.3.9/docs/source/modules.rst
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      130 2023-02-08 17:19:21.000000 pymadng-0.3.9/docs/source/pymadng.rst
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.687580 pymadng-0.3.9/examples/
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.687580 pymadng-0.3.9/examples/ex-LowLevel/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2740 2023-02-13 15:45:53.000000 pymadng-0.3.9/examples/ex-LowLevel/ex-send-multypes.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2313 2023-02-13 15:54:55.000000 pymadng-0.3.9/examples/ex-LowLevel/ex-send-recv.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.687580 pymadng-0.3.9/examples/ex-benchmark-and-fork/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3786 2023-02-13 11:03:07.000000 pymadng-0.3.9/examples/ex-benchmark-and-fork/ex-benchmark-and-fork.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      320 2022-12-02 09:36:01.000000 pymadng-0.3.9/examples/ex-benchmark-and-fork/fodo.seq
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.687580 pymadng-0.3.9/examples/ex-fodo/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2499 2023-02-13 11:03:49.000000 pymadng-0.3.9/examples/ex-fodo/ex-fodos.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      320 2022-11-24 17:08:32.000000 pymadng-0.3.9/examples/ex-fodo/fodo.seq
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.691580 pymadng-0.3.9/examples/ex-lhc-couplingLocal/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2636 2023-02-09 10:53:12.000000 pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc-couplingLocal.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)  2743306 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc_as-built.seq
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     6730 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc_unset_vars.mad
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    92958 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-lhc-couplingLocal/opticsfile.21
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.691580 pymadng-0.3.9/examples/ex-managing-refs/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1111 2023-02-13 11:04:31.000000 pymadng-0.3.9/examples/ex-managing-refs/ex-managing-refs.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      320 2022-12-19 08:56:39.000000 pymadng-0.3.9/examples/ex-managing-refs/fodo.seq
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.691580 pymadng-0.3.9/examples/ex-ps-twiss/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1514 2023-02-13 11:08:13.000000 pymadng-0.3.9/examples/ex-ps-twiss/ps-twiss.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3205 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-ps-twiss/ps_fb_lhc.str
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    34062 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-ps-twiss/ps_mu.seq
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    59055 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-ps-twiss/ps_ss.seq
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      958 2022-07-20 07:07:23.000000 pymadng-0.3.9/examples/ex-ps-twiss/ps_unset_vars.mad
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.699580 pymadng-0.3.9/examples/ex-recv-lhc/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1452 2022-12-01 10:35:26.000000 pymadng-0.3.9/examples/ex-recv-lhc/defexpr_speed.mad
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3165 2022-12-14 13:15:53.000000 pymadng-0.3.9/examples/ex-recv-lhc/ex-defexpr.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)  2739614 2022-12-01 10:40:05.000000 pymadng-0.3.9/examples/ex-recv-lhc/lhc_as-built.seq
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     8662 2022-12-01 10:40:51.000000 pymadng-0.3.9/examples/ex-recv-lhc/lhc_unset_vars.mad
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    37039 2022-12-01 10:39:26.000000 pymadng-0.3.9/examples/ex-recv-lhc/opt_400_10000_400_3000.madx
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      667 2023-01-09 13:53:17.000000 pymadng-0.3.9/examples/runall.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1167 2023-03-12 16:22:17.000000 pymadng-0.3.9/pyproject.toml
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-03-12 16:22:32.715580 pymadng-0.3.9/setup.cfg
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.679580 pymadng-0.3.9/src/
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.715580 pymadng-0.3.9/src/pymadng/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      297 2023-03-12 16:22:24.000000 pymadng-0.3.9/src/pymadng/__init__.py
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)  8125664 2023-03-08 17:00:36.000000 pymadng-0.3.9/src/pymadng/mad_Darwin
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)  6162584 2023-03-08 17:00:23.000000 pymadng-0.3.9/src/pymadng/mad_Linux
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7348 2023-02-09 13:40:40.000000 pymadng-0.3.9/src/pymadng/mad_classes.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1831 2022-12-13 13:07:01.000000 pymadng-0.3.9/src/pymadng/mad_completer.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      357 2023-02-06 15:19:09.000000 pymadng-0.3.9/src/pymadng/mad_last.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    15165 2023-02-09 13:51:12.000000 pymadng-0.3.9/src/pymadng/mad_object.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    14987 2023-02-13 14:43:15.000000 pymadng-0.3.9/src/pymadng/mad_process.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2237 2023-02-06 15:19:09.000000 pymadng-0.3.9/src/pymadng/mad_strings.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.715580 pymadng-0.3.9/src/pymadng.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3212 2023-03-12 16:22:32.000000 pymadng-0.3.9/src/pymadng.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1743 2023-03-12 16:22:32.000000 pymadng-0.3.9/src/pymadng.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-03-12 16:22:32.000000 pymadng-0.3.9/src/pymadng.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       14 2023-03-12 16:22:32.000000 pymadng-0.3.9/src/pymadng.egg-info/requires.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        8 2023-03-12 16:22:32.000000 pymadng-0.3.9/src/pymadng.egg-info/top_level.txt
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-03-12 16:22:32.715580 pymadng-0.3.9/tests/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    14214 2023-02-13 14:43:31.000000 pymadng-0.3.9/tests/comm_tests.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    18791 2023-02-09 13:57:05.000000 pymadng-0.3.9/tests/obj_tests.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.318147 pymadng-0.4.0/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1844 2022-12-22 19:04:03.000000 pymadng-0.4.0/.gitignore
+-rw-rw-r--   0 josh      (1000) josh      (1000)      548 2023-06-26 17:21:05.000000 pymadng-0.4.0/CHANGELOG
+-rw-rw-r--   0 josh      (1000) josh      (1000)    35149 2022-12-22 19:04:03.000000 pymadng-0.4.0/LICENSE
+-rw-rw-r--   0 josh      (1000) josh      (1000)      186 2022-12-22 19:04:03.000000 pymadng-0.4.0/MANIFEST.in
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3212 2023-06-26 17:21:58.318147 pymadng-0.4.0/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2353 2023-02-18 14:37:57.000000 pymadng-0.4.0/README.md
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.310147 pymadng-0.4.0/docs/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      638 2022-12-22 19:04:03.000000 pymadng-0.4.0/docs/Makefile
+-rw-rw-r--   0 josh      (1000) josh      (1000)      804 2022-12-22 19:04:03.000000 pymadng-0.4.0/docs/make.bat
+-rw-rw-r--   0 josh      (1000) josh      (1000)      116 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/requirements.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.310147 pymadng-0.4.0/docs/source/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1364 2023-02-18 14:38:28.000000 pymadng-0.4.0/docs/source/conf.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     5508 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/ex-fodo.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3061 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/ex-lhc-couplingLocal.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     4974 2023-06-26 16:24:09.000000 pymadng-0.4.0/docs/source/ex-lowlevel.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     4652 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/ex-managing-refs.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3224 2022-12-22 19:04:03.000000 pymadng-0.4.0/docs/source/ex-recv-lhc.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1092 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/examples.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     8135 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/gettingstarted.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      577 2023-02-18 14:37:57.000000 pymadng-0.4.0/docs/source/index.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       70 2022-12-22 19:04:03.000000 pymadng-0.4.0/docs/source/modules.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      130 2022-12-22 19:04:03.000000 pymadng-0.4.0/docs/source/pymadng.rst
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-LowLevel/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2740 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-LowLevel/ex-send-multypes.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2313 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-LowLevel/ex-send-recv.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-benchmark-and-fork/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3786 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-benchmark-and-fork/ex-benchmark-and-fork.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      320 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-benchmark-and-fork/fodo.seq
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-fodo/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2499 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-fodo/ex-fodos.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      320 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-fodo/fodo.seq
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-lhc-couplingLocal/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2636 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc-couplingLocal.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)  2743306 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc_as-built.seq
+-rw-rw-r--   0 josh      (1000) josh      (1000)     6730 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc_unset_vars.mad
+-rw-rw-r--   0 josh      (1000) josh      (1000)    92958 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-lhc-couplingLocal/opticsfile.21
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-managing-refs/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1111 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-managing-refs/ex-managing-refs.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      320 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-managing-refs/fodo.seq
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.314147 pymadng-0.4.0/examples/ex-ps-twiss/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1514 2023-02-18 14:37:57.000000 pymadng-0.4.0/examples/ex-ps-twiss/ps-twiss.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3205 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-ps-twiss/ps_fb_lhc.str
+-rw-rw-r--   0 josh      (1000) josh      (1000)    34062 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-ps-twiss/ps_mu.seq
+-rw-rw-r--   0 josh      (1000) josh      (1000)    59055 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-ps-twiss/ps_ss.seq
+-rw-rw-r--   0 josh      (1000) josh      (1000)      958 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-ps-twiss/ps_unset_vars.mad
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.318147 pymadng-0.4.0/examples/ex-recv-lhc/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1452 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-recv-lhc/defexpr_speed.mad
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3165 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-recv-lhc/ex-defexpr.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)  2739614 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-recv-lhc/lhc_as-built.seq
+-rw-rw-r--   0 josh      (1000) josh      (1000)     8662 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-recv-lhc/lhc_unset_vars.mad
+-rw-rw-r--   0 josh      (1000) josh      (1000)    37039 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/ex-recv-lhc/opt_400_10000_400_3000.madx
+-rw-rw-r--   0 josh      (1000) josh      (1000)      667 2022-12-22 19:04:03.000000 pymadng-0.4.0/examples/runall.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1167 2023-06-26 17:18:40.000000 pymadng-0.4.0/pyproject.toml
+-rw-rw-r--   0 josh      (1000) josh      (1000)       38 2023-06-26 17:21:58.318147 pymadng-0.4.0/setup.cfg
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.310147 pymadng-0.4.0/src/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.318147 pymadng-0.4.0/src/pymadng/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      298 2023-06-26 17:18:35.000000 pymadng-0.4.0/src/pymadng/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     6505 2023-06-26 17:16:14.000000 pymadng-0.4.0/src/pymadng/madp_classes.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      333 2023-06-26 16:14:00.000000 pymadng-0.4.0/src/pymadng/madp_last.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    15124 2023-06-26 16:50:19.000000 pymadng-0.4.0/src/pymadng/madp_object.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    14117 2023-06-26 16:57:08.000000 pymadng-0.4.0/src/pymadng/madp_pymad.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1731 2023-06-26 16:26:09.000000 pymadng-0.4.0/src/pymadng/madp_strings.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.318147 pymadng-0.4.0/src/pymadng.egg-info/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3212 2023-06-26 17:21:58.000000 pymadng-0.4.0/src/pymadng.egg-info/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1672 2023-06-26 17:21:58.000000 pymadng-0.4.0/src/pymadng.egg-info/SOURCES.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-06-26 17:21:58.000000 pymadng-0.4.0/src/pymadng.egg-info/dependency_links.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       14 2023-06-26 17:21:58.000000 pymadng-0.4.0/src/pymadng.egg-info/requires.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        8 2023-06-26 17:21:58.000000 pymadng-0.4.0/src/pymadng.egg-info/top_level.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-06-26 17:21:58.318147 pymadng-0.4.0/tests/
+-rw-rw-r--   0 josh      (1000) josh      (1000)    12511 2023-06-26 16:13:31.000000 pymadng-0.4.0/tests/comm_tests.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    10121 2023-06-26 17:11:43.000000 pymadng-0.4.0/tests/obj_tests.py
```

### Comparing `pymadng-0.3.9/.gitignore` & `pymadng-0.4.0/.gitignore`

 * *Files 24% similar despite different names*

```diff
@@ -126,17 +126,8 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 #tfs tables and txt files
 *.tfs
-*/output.txt
-examples/ex-benchmark-and-fork/fodo.mad
-examples/ex-fodo/fodo.mad
-examples/ex-lhc-couplingLocal/lhc_as-built.mad
-examples/ex-lhc-couplingLocal/opticsfile.21.mad
-examples/ex-managing-refs/fodo.mad
-examples/ex-recv-lhc/lhc_as-built.mad
-examples/ex-recv-lhc/opt_400_10000_400_3000.mad
-src/pymadng/mad_Darwin
-src/pymadng/mad_Linux
+*/output.txt
```

### Comparing `pymadng-0.3.9/LICENSE` & `pymadng-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/PKG-INFO` & `pymadng-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymadng
-Version: 0.3.9
+Version: 0.4.0
 Summary: A python interface to MAD-NG running as subprocess
 Author-email: Joshua Gray <joshua.mark.gray@cern.ch>
 Project-URL: Homepage, https://github.com/MethodicalAcceleratorDesign/MADpy
 Project-URL: Bug Tracker, https://github.com/MethodicalAcceleratorDesign/MADpy/issues
 Project-URL: MAD Source, https://github.com/MethodicalAcceleratorDesign/MAD
 Project-URL: Documentation, https://pymadng.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymadng-0.3.9/README.md` & `pymadng-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/Makefile` & `pymadng-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/make.bat` & `pymadng-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/conf.py` & `pymadng-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/ex-fodo.rst` & `pymadng-0.4.0/docs/source/ex-fodo.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/ex-lhc-couplingLocal.rst` & `pymadng-0.4.0/docs/source/ex-lhc-couplingLocal.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/ex-lowlevel.rst` & `pymadng-0.4.0/docs/source/ex-lowlevel.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/ex-managing-refs.rst` & `pymadng-0.4.0/docs/source/ex-managing-refs.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/ex-recv-lhc.rst` & `pymadng-0.4.0/docs/source/ex-recv-lhc.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/examples.rst` & `pymadng-0.4.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/gettingstarted.rst` & `pymadng-0.4.0/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/docs/source/index.rst` & `pymadng-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-LowLevel/ex-send-multypes.py` & `pymadng-0.4.0/examples/ex-LowLevel/ex-send-multypes.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-LowLevel/ex-send-recv.py` & `pymadng-0.4.0/examples/ex-LowLevel/ex-send-recv.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-benchmark-and-fork/ex-benchmark-and-fork.py` & `pymadng-0.4.0/examples/ex-benchmark-and-fork/ex-benchmark-and-fork.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-fodo/ex-fodos.py` & `pymadng-0.4.0/examples/ex-fodo/ex-fodos.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc-couplingLocal.py` & `pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc-couplingLocal.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc_as-built.seq` & `pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc_as-built.seq`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-lhc-couplingLocal/lhc_unset_vars.mad` & `pymadng-0.4.0/examples/ex-lhc-couplingLocal/lhc_unset_vars.mad`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-lhc-couplingLocal/opticsfile.21` & `pymadng-0.4.0/examples/ex-lhc-couplingLocal/opticsfile.21`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-managing-refs/ex-managing-refs.py` & `pymadng-0.4.0/examples/ex-managing-refs/ex-managing-refs.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-ps-twiss/ps-twiss.py` & `pymadng-0.4.0/examples/ex-ps-twiss/ps-twiss.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-ps-twiss/ps_fb_lhc.str` & `pymadng-0.4.0/examples/ex-ps-twiss/ps_fb_lhc.str`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-ps-twiss/ps_mu.seq` & `pymadng-0.4.0/examples/ex-ps-twiss/ps_mu.seq`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-ps-twiss/ps_ss.seq` & `pymadng-0.4.0/examples/ex-ps-twiss/ps_ss.seq`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-ps-twiss/ps_unset_vars.mad` & `pymadng-0.4.0/examples/ex-ps-twiss/ps_unset_vars.mad`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-recv-lhc/defexpr_speed.mad` & `pymadng-0.4.0/examples/ex-recv-lhc/defexpr_speed.mad`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-recv-lhc/ex-defexpr.py` & `pymadng-0.4.0/examples/ex-recv-lhc/ex-defexpr.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-recv-lhc/lhc_as-built.seq` & `pymadng-0.4.0/examples/ex-recv-lhc/lhc_as-built.seq`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-recv-lhc/lhc_unset_vars.mad` & `pymadng-0.4.0/examples/ex-recv-lhc/lhc_unset_vars.mad`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/ex-recv-lhc/opt_400_10000_400_3000.madx` & `pymadng-0.4.0/examples/ex-recv-lhc/opt_400_10000_400_3000.madx`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/examples/runall.py` & `pymadng-0.4.0/examples/runall.py`

 * *Files identical despite different names*

### Comparing `pymadng-0.3.9/pyproject.toml` & `pymadng-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 # requires = ["hatchling"]
 # build-backend = "hatchling.build"
 
 [project]
 name = "pymadng"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="Joshua Gray", email="joshua.mark.gray@cern.ch" },
 ]
 description = "A python interface to MAD-NG running as subprocess"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pymadng-0.3.9/src/pymadng/mad_classes.py` & `pymadng-0.4.0/src/pymadng/madp_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,196 +1,188 @@
 from typing import Iterable, Union, Any  # To make stuff look nicer
 import numpy as np
+from .madp_pymad import mad_process, mad_ref, data_types
+from .madp_strings import get_args_string, get_kwargs_string
+from .madp_last import last_counter
 
 # TODO: Are you able to store the actual parent? 
-# TODO: Verify if functions need kwargs or not. 
-# BUG: In the case of MADX, the ?only? object that includes methods and functions, we attempt to call the functions like methods. Try MAD.MADX.abs(1).
-class mad_ref(object):    
-    def __init__(self, name: str, mad_proc):
-        assert name is not None, "Reference must have a variable to reference to. Did you forget to put a name in the receive functions?"
-        self.__name__ = name
-        self.__parent__ = (
-            "[" in name and "[".join(name.split("[")[:-1]) or None
-        )  # if name is compound, get parent by string manipulation
-        self.__mad__ = mad_proc
-
-    def __getattr__(self, item):
-        if item[0] != "_":
-            try:
-                return self[item]
-            except (IndexError, KeyError):
-                pass
-        raise AttributeError (item)  # For python
-
-    def __setattr__(self, item, value):
-        if item[0] == "_":
-            return super(mad_ref, self).__setattr__(item, value)
-        self[item] = value
-
-    def __getitem__(self, item: Union[str, int]):
-        if isinstance(item, int):
-            result = self.__mad__.safe_recv(f"{self.__name__}[{item+1}]")
-            if result is None:
-                raise IndexError(item)  # For python
-        elif isinstance(item, str):
-            result = self.__mad__.safe_recv(f"{self.__name__}['{item}']")
-            if result is None:
-                raise KeyError(item)  # For python
-        else:
-            raise TypeError("Cannot index type of ", type(item))
-
-        return result
-
-    def __setitem__(
-        self,
-        item: Union[str, int],
-        value: Union[str, int, float, np.ndarray, bool, list],
-    ):
-        if isinstance(item, int):
-            self.__mad__.send_vars(f"{self.__name__}[{item+1}]", value)
-        elif isinstance(item, str):
-            self.__mad__.send_vars(f"{self.__name__}['{item}']", value)
-        else:
-            raise TypeError("Cannot index type of ", type(item), "expected string or int")
-
-    def __add__(self, rhs):
-        return self.__gOp__(rhs, "+")
-
-    def __mul__(self, rhs):
-        return self.__gOp__(rhs, "*")
-
-    def __pow__(self, rhs):
-        return self.__gOp__(rhs, "^")
-
-    def __sub__(self, rhs):
-        return self.__gOp__(rhs, "-")
-
-    def __truediv__(self, rhs):
-        return self.__gOp__(rhs, "/")
-
-    def __mod__(self, rhs):
-        return self.__gOp__(rhs, "%")
-
-    def __eq__(self, rhs):
-        if (isinstance(rhs, type(self)) and self.__name__ == rhs.__name__):
-            return True
-        else:
-            return self.__gOp__(rhs, "==").eval()
-
-    def __gOp__(self, rhs, operator: str):
-        rtrn = mad_reflast(self.__mad__)
-        self.__mad__.safe_send(f"{rtrn.__name__} = {self.__name__} {operator} {self.__mad__.py_name}:recv()").send(rhs)
-        return rtrn
-
-    def __len__(self):
-        return self.__mad__.safe_recv(f"#{self.__name__}")
-
-    def __str__(self):
-        val = self.__mad__.recv_vars(self.__name__)
-        if isinstance(val, mad_ref):
-            return repr(val)
-        else:
-            return str(val)
-
-    def eval(self):
-        return self.__mad__.recv_vars(self.__name__)
-
-    def __repr__(self):
-        return f"MAD-NG Object(Name: {self.__name__}, Parent: {self.__parent__})"
-
-    def __dir__(self) -> Iterable[str]:
-        name = self.__name__
-        if name[:8] == "__last__":
-            name = name + ".__metatable or " + name
-        script = f"""
-            local modList={{}}; local i = 1;
-            for modname, mod in pairs({name}) do modList[i] = modname; i = i + 1; end
-            {self.__mad__.py_name}:send(modList)"""
-        self.__mad__.safe_send(script)
-        varnames = [x for x in self.__mad__.recv() if isinstance(x, str) and x[0] != "_"]
-        return varnames
-
-class mad_obj(mad_ref):
-    def __dir__(self) -> Iterable[str]:
-        if not self.__mad__.ipython_use_jedi:
-            self.__mad__.safe_send(f"{self.__mad__.py_name}:send({self.__name__}:get_varkeys(MAD.object))")
-
-        # self.__mad__.safe_send(f"{self.__mad__.py_name}:send({self.__name__}:get_varkeys(MAD.object, false))")
-        # varnames = [x for x in self.__mad__.recv()]
-        varnames = self.__mad__.safe_recv(f"{self.__name__}:get_varkeys(MAD.object, false)")
-
-        if not self.__mad__.ipython_use_jedi:
-            varnames.extend([x + "()" for x in self.__mad__.recv() if not x in varnames])
-        return varnames
-
-    def __call__(self, *args, **kwargs):
-        last_obj = mad_objlast(self.__mad__)
-        kwargs_string, kwargs_to_send = self.__mad__.mad_strs.get_kwargs_string(**kwargs)
-        args_string  ,   args_to_send = self.__mad__.mad_strs.get_args_string(*args)
-        self.__mad__.send(
-            f"{last_obj.__name__} = __mklast__( {self.__name__} {{ {kwargs_string[1:-1]} {args_string} }} )"
-        )
-        for var in kwargs_to_send + args_to_send:
-            self.__mad__.send(var)
-        return last_obj
-
-    def __iter__(self):
-        self.__iterIndex__ = -1
-        return self
-
-    def __next__(self):
-        try:
-            self.__iterIndex__ += 1
-            return self[self.__iterIndex__]
-        except IndexError:
-            raise StopIteration
-
-
-class mad_func(mad_ref):
-    # ----------------------------------Calling/Creating functions--------------------------------------#
-    def __call_func(self, funcName: str, *args):
-        """Call the function funcName and store the result in ``__last__``."""
-        rtrn_ref = mad_reflast(self.__mad__)
-        args_string, vars_to_send = self.__mad__.mad_strs.get_args_string(*args)
-        self.__mad__.send(
-            f"{rtrn_ref.__name__} = __mklast__({funcName}({args_string}))\n"
-        )
-        for var in vars_to_send:
-            self.__mad__.send(var)
-        return rtrn_ref
-    # ---------------------------------------------------------------------------------------------------#
-    
-    def __call__(self, *args: Any) -> Any:
-        ismethod = self.__parent__ and self.__mad__.safe_recv(f"""
-        MAD.typeid.is_object({self.__parent__}) or MAD.typeid.isy_matrix({self.__parent__})
-        """)
-        if ismethod:
-            return self.__call_func(self.__name__, self.__parent__, *args)
-        else:
-            return self.__call_func(self.__name__, *args)
-    def __dir__(self):
-        return super(mad_ref, self).__dir__()
+# TODO: Verify if functions need kwargs or not. (I would  not)
 
-# Separate class for __last__ objects for simplicity and fewer if statements
-class mad_last(): # The init and del for a __last__ object
-    def __init__(self, mad_proc):
-        self.__lastnum__ = mad_proc.last_counter.get()
-        self.__name__ = f"__last__[{self.__lastnum__}]"
-        self.__mad__ = mad_proc
-        self.__parent__ = "__last__"
+MADX_methods = ["load", "open_env", "close_env"]
+class madhl_ref(mad_ref):    
+  def __init__(self, name: str, mad_proc: mad_process, last_counter: last_counter):
+    super(madhl_ref, self).__init__(name, mad_proc)
+    self.__parent__ = (
+      "[" in name and "[".join(name.split("[")[:-1]) or None
+    )  # if name is compound, get parent by string manipulation
+    self.__mad__ = mad_proc
+    self.__lst_cntr__ = last_counter
+
+  def __setattr__(self, item, value):
+    if item[0] == "_":
+      return super(madhl_ref, self).__setattr__(item, value)
+    self[item] = value
+
+  def __setitem__(
+    self,
+    item: Union[str, int],
+    value: Union[str, int, float, np.ndarray, bool, list],
+  ):
+    if isinstance(item, int):
+      self.__mad__.send_vars(f"{self.__name__}[{item+1}]", value)
+    elif isinstance(item, str):
+      self.__mad__.send_vars(f"{self.__name__}['{item}']", value)
+    else:
+      raise TypeError("Cannot index type of ", type(item), "expected string or int")
+
+  def __add__(self, rhs):
+    return self.__gOp__(rhs, "+")
+
+  def __mul__(self, rhs):
+    return self.__gOp__(rhs, "*")
+
+  def __pow__(self, rhs):
+    return self.__gOp__(rhs, "^")
+
+  def __sub__(self, rhs):
+    return self.__gOp__(rhs, "-")
+
+  def __truediv__(self, rhs):
+    return self.__gOp__(rhs, "/")
+
+  def __mod__(self, rhs):
+    return self.__gOp__(rhs, "%")
+
+  def __eq__(self, rhs):
+    if (isinstance(rhs, type(self)) and self.__name__ == rhs.__name__):
+      return True
+    else:
+      return self.__gOp__(rhs, "==").eval()
+
+  def __gOp__(self, rhs, operator: str):
+    rtrn = madhl_reflast(self.__mad__, self.__lst_cntr__)
+    self.__mad__.psend(f"{rtrn.__name__} = {self.__name__} {operator} {self.__mad__.py_name}:recv()").send(rhs)
+    return rtrn
+
+  def __len__(self):
+    return self.__mad__.precv(f"#{self.__name__}")
+
+  def __str__(self):
+    val = self.__mad__.recv_vars(self.__name__)
+    if isinstance(val, madhl_ref):
+      return repr(val)
+    else:
+      return str(val)
+
+  def eval(self):
+    return self.__mad__.recv_vars(self.__name__)
+
+  def __repr__(self):
+    return f"MAD-NG Object(Name: {self.__name__}, Parent: {self.__parent__})"
+
+  def __dir__(self) -> Iterable[str]:
+    name = self.__name__
+    if name[:8] == "__last__":
+      name = name + ".__metatable or " + name
+    script = f"""
+      local modList={{}}; local i = 1;
+      for modname, mod in pairs({name}) do modList[i] = modname; i = i + 1; end
+      {self.__mad__.py_name}:send(modList)"""
+    self.__mad__.psend(script)
+    varnames = [x for x in self.__mad__.recv() if isinstance(x, str) and x[0] != "_"]
+    return varnames
+
+class madhl_obj(madhl_ref):
+  def __dir__(self) -> Iterable[str]:
+    if not self.__mad__.ipython_use_jedi:
+      self.__mad__.psend(f"{self.__mad__.py_name}:send({self.__name__}:get_varkeys(MAD.object))")
+    varnames = self.__mad__.precv(f"{self.__name__}:get_varkeys(MAD.object, false)")
+
+    if not self.__mad__.ipython_use_jedi:
+      varnames.extend([x + "()" for x in self.__mad__.recv() if not x in varnames])
+    return varnames
+
+  def __call__(self, *args, **kwargs):
+    last_obj = madhl_objlast(self.__mad__, self.__lst_cntr__)
+    kwargs_string, kwargs_to_send = get_kwargs_string(self.__mad__.py_name, **kwargs)
+    args_string  ,   args_to_send = get_args_string(self.__mad__.py_name, *args)
     
-    def __del__(self):
-        self.__mad__.last_counter.set(self.__lastnum__)
+    self.__mad__.send(
+      f"{last_obj.__name__} = __mklast__( {self.__name__} {{ {kwargs_string[1:-1]} {args_string} }} )"
+    )
+    for var in kwargs_to_send + args_to_send:
+      self.__mad__.send(var)
+    return last_obj
+
+  def __iter__(self):
+    self.__iterIndex__ = -1
+    return self
+
+  def __next__(self):
+    try:
+      self.__iterIndex__ += 1
+      return self[self.__iterIndex__]
+    except IndexError:
+      raise StopIteration
+
+
+class madhl_fun(madhl_ref):
+  # ----------------------------------Calling/Creating functions--------------------------------------#
+  def __call_func(self, funcName: str, *args):
+    """Call the function funcName and store the result in ``__last__``."""
+    rtrn_ref = madhl_reflast(self.__mad__, self.__lst_cntr__)
+    args_string, vars_to_send = get_args_string(self.__mad__.py_name, *args)
+    self.__mad__.send(
+      f"{rtrn_ref.__name__} = __mklast__({funcName}({args_string}))\n"
+    )
+    for var in vars_to_send:
+      self.__mad__.send(var)
+    return rtrn_ref
+  # ---------------------------------------------------------------------------------------------------#
+  
+  def __call__(self, *args: Any) -> Any:
+    # Checks for MADX methods
+    call_from_madx = self.__parent__ and self.__parent__.split("['")[-1].strip("']") == "MADX"
+    if call_from_madx: funcname = self.__name__.split("['")[-1].strip("']")
+
+    ismethod = self.__parent__ and (self.__mad__.precv(f"""
+    MAD.typeid.is_object({self.__parent__}) or MAD.typeid.isy_matrix({self.__parent__})
+    """))
+    if ismethod and not (call_from_madx and not funcname in MADX_methods):
+      return self.__call_func(self.__name__, self.__parent__, *args)
+    else:
+      return self.__call_func(self.__name__, *args)
+  def __dir__(self):
+    return super(madhl_ref, self).__dir__()
 
-class mad_reflast(mad_last, mad_ref):
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        obj = self.eval()
-        if isinstance(obj, (mad_obj, mad_func)):
-            return obj(*args, **kwargs)
-        else:
-            raise TypeError("Cannot call " + str(obj))
-    
-    def __dir__(self):
-        return super(mad_reflast, self).__dir__()
+# Separate class for __last__ objects for simplicity and fewer if statements
+class madhl_last(): # The init and del for a __last__ object
+  def __init__(self, mad_proc: mad_process, last_counter: last_counter):
+    self.__lastnum__ = last_counter.get()
+    self.__name__ = f"__last__[{self.__lastnum__}]"
+    self.__mad__ = mad_proc
+    self.__parent__ = "__last__"
+    self.__lst_cntr__ = last_counter
+  
+  def __del__(self):
+    self.__lst_cntr__.set(self.__lastnum__)
+
+class madhl_reflast(madhl_last, madhl_ref):
+  def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    obj = self.eval()
+    if isinstance(obj, (madhl_obj, madhl_fun)):
+      return obj(*args, **kwargs)
+    else:
+      raise TypeError("Cannot call " + str(obj))
+  
+  def __dir__(self):
+    return super(madhl_reflast, self).__dir__()
+
+class madhl_objlast(madhl_last, madhl_obj):
+  pass
+
+data_types[madhl_ref] = "ref_"
+data_types[madhl_obj] = "obj_"
+data_types[madhl_fun] = "fun_"
 
-class mad_objlast(mad_last, mad_obj):
-    pass
+data_types[madhl_reflast] = "ref_"
+data_types[madhl_objlast] = "obj_"
```

### Comparing `pymadng-0.3.9/src/pymadng/mad_object.py` & `pymadng-0.4.0/src/pymadng/madp_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,357 +1,390 @@
 import numpy as np  # For arrays  (Works well with multiprocessing and mmap)
 from typing import Any, Iterable, Union, List  # To make stuff look nicer
 
+import os, platform
+bin_path = os.path.dirname(os.path.abspath(__file__)).replace("src/pymadng", "bin") 
+
 # Custom Classes:
-from .mad_classes import mad_ref, mad_reflast
-from .mad_process import mad_process
+from .madp_classes import madhl_ref, madhl_obj, madhl_fun, madhl_reflast
+from .madp_pymad import mad_process, str_to_fun
+from .madp_strings import get_kwargs_string
+from .madp_last    import last_counter
 
 # TODO: Make it so that MAD does the loop for variables not python (speed)
 # TODO: Should I change anything that atm requires a list at end of function to *args?
 
 class MAD(object):
-    """An object that allows communication with MAD-NG
+  """An object that allows communication with MAD-NG
+
+  Attributes:
+    py_name: A string indicating the name of the reference to python from MAD-NG, for communication from MAD-NG to Python.
+    __MAD_version__: A string indicating the version of MAD-NG being used. (Also accessible from ``pymadng.MAD().MAD.env.version``)
+  """
+
+  def __init__(self, mad_path: str = None, py_name: str = "py", debug: bool = False, num_temp_vars: int = 8, ipython_use_jedi: bool = False):
+    """Create a MAD Object to interface with MAD-NG.
+
+    The modules MADX, elements, sequence, mtable, twiss, beta0, beam, survey, object, track, match are imported into
+    the MAD-NG environment by default.
+
+    Args:
+      py_name (str): The name used to interact with the python process from MAD
+        (default = "py")
+      mad_path (str): The path to the mad executable, for a value of None, the one that comes with pymadng package will be used
+        (default = None)
+      debug (bool): Sets debug mode on or off
+        (default = False)
+      num_temp_vars (int): The number of unique temporary variables you intend to use, see :doc:`Managing References <ex-managing-refs>`
+        (default = 8)
+      ipython_use_jedi (bool): Allow ipython to use jedi in tab completion, will be slower and may result in MAD-NG throwing errors
+        (default = False)
 
-    Attributes:
-        py_name: A string indicating the name of the reference to python from MAD-NG, for communication from MAD-NG to Python.
-        __MAD_version__: A string indicating the version of MAD-NG being used. (Also accessible from ``pymadng.MAD().MAD.env.version``)
-    """
-
-    def __init__(self, py_name: str = "py", mad_path: str = None, debug: bool = False, num_temp_vars: int = 8, ipython_use_jedi: bool = False):
-        """Create a MAD Object to interface with MAD-NG.
-
-        The modules MADX, elements, sequence, mtable, twiss, beta0, beam, survey, object, track, match are imported into
-        the MAD-NG environment by default.
-
-        Args:
-            py_name (str): The name used to interact with the python process from MAD
-                (default = "py")
-            mad_path (str): The path to the mad executable, for a value of None, the one that comes with pymadng package will be used
-                (default = None)
-            debug (bool): Sets debug mode on or off
-                (default = False)
-            num_temp_vars (int): The number of unique temporary variables you intend to use, see :doc:`Managing References <ex-managing-refs>`
-                (default = 8)
-            ipython_use_jedi (bool): Allow ipython to use jedi in tab completion, will be slower and may result in MAD-NG throwing errors
-                (default = False)
-
-        Returns:
-            A MAD object, allowing for communication with MAD-NG
-        """
-        self.__process = mad_process(py_name, mad_path, debug, num_temp_vars, ipython_use_jedi)
-        
-        ## Store the relavent objects into a function to get reference objects
-        self.__mad_reflast = lambda: mad_reflast(self.__process)
-        if not ipython_use_jedi: #Stop jedi running getattr on my classes...
-            try:
-                ipython = get_ipython()
-                if ipython.__class__.__name__ == 'TerminalInteractiveShell':
-                    ipython.Completer.use_jedi = False 
-            except NameError:
-                pass
-        self.py_name = py_name
-        # --------------------------------Retrieve the modules of MAD-------------------------------#
-        # Limit the 80 modules
-        modulesToImport = [
-            "element", "sequence", "mtable", "twiss", "beta0",
-            "beam", "survey", "object", "track", "match",
-        ]
-        self.load("MAD", *modulesToImport)
-        self.__MAD_version__ = self.MAD.env.version
-
-    # ------------------------------------------------------------------------------------------#
-
-    # --------------------------- Receiving data from subprocess -------------------------------#
-    def recv(
-        self, varname: str = None
-    ) -> Union[str, int, float, np.ndarray, bool, list]:
-        """Return received data from MAD-NG.
-
-        Args:
-            varname(str): The name of the variable you are receiving (Only useful when receiving references)
-                (default is None)
-
-        Returns:
-            Data from MAD-NG with type str/int/float/ndarray/bool/list, depending what was asked from MAD-NG.
-
-        Raises:
-            TypeError: If you forget to give a name when receiving a reference,  
-        """
-        return self.__process.recv(varname)
-
-    def receive(
-        self, varname: str = None
-    ) -> Union[str, int, float, np.ndarray, bool, list]:
-        """See :meth:`recv`"""
-        return self.__process.recv(varname)
-
-    def recv_and_exec(self, env: dict = {}) -> dict:
-        """Receive a string from MAD-NG and execute it.
-
-        Note: The class numpy and the instance of this object are available during the execution as ``np`` and ``mad`` respectively
-
-        Args:
-            env (dict): The environment you would like the string to be executed in.
-                (default = {})
-
-        Returns:
-            The updated environment after executing the string.
-        """
-        env["mad"] = self
-        return self.__process.recv_and_exec(env)
-
-    # --------------------------------Sending data to subprocess------------------------------------#
-    def send(self, data: Union[str, int, float, np.ndarray, bool, list]):
-        """Send data to MAD-NG.
-
-        Args:
-            data (str/int/float/ndarray/bool/list): The data to send to MAD-NG.
-
-        Returns:
-            self (the instance of the mad object)
-
-        Raises:
-            TypeError: An unsupported type was attempted to be sent to MAD-NG.
-            AssertionError: If data is a np.ndarray, the matrix must be of two dimensions.
-        """
-        self.__process.send(data)
-        return self
-
-    def send_rng(self, start: float, stop: float, size: int):
-        """Send a range to MAD-NG, equivalent to np.linspace, but in MAD-NG.
-
-        Args:
-            start (float): The start of range
-            stop (float): The end of range (inclusive)
-            size (float): The length of range
-        """
-        self.__process.send_rng(start, stop, size)
-
-    def send_lrng(self, start: float, stop: float, size: int):
-        """Send a numpy array as a logrange to MAD-NG, equivalent to np.geomspace, but in MAD-NG.
-
-        Args:
-            start (float): The start of range
-            stop (float): The end of range (inclusive)
-            size (float): The length of range
-        """
-        self.__process.send_lrng(start, stop, size)
-
-    def send_tpsa(self, monos: np.ndarray, coefficients: np.ndarray):
-        """Send the monomials and coefficients of a TPSA to MAD
-
-        The combination of monomials and coefficients creates a table representing the TPSA object in MAD-NG.
-
-        Args:
-            monos (ndarray): A list of monomials in the TPSA.
-            coefficients (ndarray): A list of coefficients in the TPSA.
-
-        Raises:
-            AssertionError: The list of monomials must be a 2-D array (each monomial is 1-D).
-            AssertionError: The number of monomials and coefficients must be identical.
-            AssertionError: The monomials must be of type 8-bit unsigned integer 
-        """
-        self.__process.send_tpsa(monos, coefficients)
-
-    def send_ctpsa(self, monos: np.ndarray, coefficients: np.ndarray):
-        """Send the monomials and coefficients of a complex TPSA to MAD-NG
-
-        The combination of monomials and coefficients creates a table representing the complex TPSA object in MAD-NG.
-        
-        Args:
-            See: :meth:`send_tpsa`.
-        
-        Raises:
-            See: :meth:`send_tpsa`.
-        """
-        self.__process.send_ctpsa(monos, coefficients)
+    Returns:
+      A MAD object, allowing for communication with MAD-NG
+    """
+    # ----------------------- Create the process --------------------------#
+    lst_cntr = last_counter(num_temp_vars)
+    # Override the type of reference created by python.
+    def recv_ref(self: mad_process) -> madhl_ref:
+      return madhl_ref(self.varname, self, lst_cntr)
     
-    # ---------------------------------------------------------------------------------------------------------#
+    def recv_obj(self: mad_process) -> madhl_obj:
+      return madhl_obj(self.varname, self, lst_cntr)
     
-    # -------------------------------- Dealing with communication of variables --------------------------------#
-    def send_vars(
-        self,
-        names: Union[str, List[str]],
-        vars: List[Union[str, int, float, np.ndarray, bool, list]],
-    ):
-        """Send variables to the MAD-NG process.
-
-        Send the variables in vars with the names in names to MAD-NG.
-
-        Args:
-            names (str/List[str]): The name(s) that would like to assign your python variable(s) in MAD-NG.
-            vars (List[str/int/float/ndarray/bool/list]): The variables to send with the name(s) 'names' in MAD-NG.
-
-        Raises:
-            AssertionError: A list of names must be matched with a list of variables
-            AssertionError: The number of names must match the number of variables
-            Other Errors: See :meth:`send`.
-        """
-        self.__process.send_vars(names, vars)
-
-    def recv_vars(self, names: Union[str, List[str]]) -> Any:
-        """Receive variables from the MAD-NG process
-
-        Given a list of variable names, receive the variables from the MAD-NG process.
-
-        Args:
-            names (str/List[str]): The name(s) of variables that you would like to receive from MAD-NG.
-
-        Returns:
-            See :meth:`recv`.
-        """
-        return self.__process.recv_vars(names)
-
-    # -------------------------------------------------------------------------------------------------------------#
-
-    def load(self, module: str, *vars: str):
-        """Import modules into the MAD-NG environment
-
-        Retrieve the classes in MAD-NG from the module ``module``, while only importing the classes in the variable length list ``vars``.
-        If no string is provided, it is assumed that you would like to import every class from the module. 
-        
-        For example, ``mad.load("MAD.gmath")`` imports all variables from the module ``MAD.gmath``. 
-        But ``mad.load("MAD", "matrix", "cmatrix")```` only imports the modules ``matrix`` and ``cmatrix`` from the module ``MAD.gmath``.
-
-        Args:
-            module (str): The name of the module to import from.
-            *vars (str): Variable length argument list of the variable(s) to import from module.
-        """
-        script = ""
-        if vars == ():
-            vars = [x.strip("()") for x in dir(mad_ref(module, self.__process))]
-        for className in vars:
-            script += f"""{className} = {module}.{className}\n"""
-        self.__process.send(script)
-
-    def loadfile(self, path: str, *vars: str):
-        """Load a .mad file into the MAD-NG environment.
-
-        If ``vars`` is not provided, this is equivalent to ``assert(loadfile(path))`` in MAD-NG.
-        If ``vars`` is provided, for each ``var`` in ``vars``, this is equivalent to ``var = require(path).var`` in MAD-NG.
-        Due to Lua querks, do not include the .mad extension in the path if you provide ``vars``, as this implies you would like to load a module.
-
-        Args:
-            path (str): The path to the file to import.
-            *vars (str): Variable length argument list of the variable(s) to import from the file.
-        """
-        if vars == ():
-            self.__process.send(f"assert(loadfile('{path}', nil, {self.py_name}._env))()")
-        else:
-            if isinstance(vars, str):
-                vars = [vars]
-            script = ""
-            for var in vars:
-                script += f"{var} = require('{path}').{var}\n"
-            self.__process.send(script)
-
-    # ----------------------- Make the class work with dict and dot access ------------------------#
-    def __getattr__(self, item):
-        if item[0] == "_" and not item[:8] == "__last__":
-            raise AttributeError(item)
-        return self.__process.recv_vars(item)
-
-    def __setitem__(self, var_name: str, var: Any) -> None:
-        if isinstance(var_name, tuple):
-            var_name = list(var_name)
-            if isinstance(var, mad_ref):
-                for i in range(len(var_name)):
-                    self.send(f"{var_name[i]} = {var.__name__}[{i+1}]") # Skip send_vars
-                return
-            else:
-                var = list(var)
-            if len(var) != len(var_name):
-                raise ValueError(
-                    "Incorrect number of values to unpack, received",
-                    len(var),
-                    "variables and",
-                    len(var_name),
-                    "keys",
-                )
-        self.__process.send_vars(var_name, var)
-
-    def __getitem__(self, var_name: str) -> Any:
-        return self.__process.recv_vars(var_name)
-    # ----------------------------------------------------------------------------------------------#
-
-    def eval(self, input: str):
-        """Evaluate an expression in MAD and return the result.
-
-        Args:
-            input (str): An expression that would like to be evaluated in MAD-NG.
-
-        Returns:
-            The evaluated result.
-        """
-        rtrn = self.__mad_reflast()
-        self.send(f"{rtrn.__name__} =" + input)
-        return rtrn.eval()
-
-    def MADX_env_send(self, input: str):
-        """Open the MAD-X environment in MAD-NG and directly send code.
-
-        Args:
-            input (str): The code that would like to be evaluated in the MAD-X environment in MAD-NG.
-        """
-        return self.__process.send("MADX:open_env()\n" + input + "\nMADX:close_env()")
-
-    def py_strs_to_mad_strs(self, input: Union[str, List[str]]):
-        """Add ' to either side of a string or each string in a list of strings
-        
-        Args: 
-            input(str/list[str]): The string(s) that you would like to add ' either side to each string.
-
-        Returns:
-            A string or list of strings with ' placed at the beginning and the end of each string.
-        """
-        if isinstance(input, list):
-            return ["'" + x + "'" for x in input]
-        else:
-            return "'" + input + "'"
-
-    # ----------------------------------------------------------------------------------------------#
-
-    # ---------------------------------------------------------------------------------------------------#
-
-    def deferred(self, **kwargs):
-        """Create a deferred expression object
-
-        For the deferred expression object, the kwargs are used as the deffered expressions, with ``=`` replaced
-        with ``:=``. To assign the returned object a name, then use ``mad['name'] = mad.deffered(kwargs)``.
-
-        Args:
-            **kwargs: A variable list of keyword arguments, keyword as the name of the deffered expression within the object and the value as a string that is sent directly to the MAD-NG environment.
-
-        Returns:
-            A reference to the deffered expression object.
-        """
-        rtrn = self.__mad_reflast()
-        kwargs_string, vars_to_send = self.__process.mad_strs.get_kwargs_string(**kwargs)
-        self.__process.send(
-            f"{rtrn.__name__} = __mklast__( MAD.typeid.deferred {{ {kwargs_string.replace('=', ':=')[1:-3]} }} )"
+    def recv_fun(self: mad_process) -> madhl_fun:
+      return madhl_fun(self.varname, self, lst_cntr)
+    
+    str_to_fun["ref_"]["recv"] = recv_ref
+    str_to_fun["obj_"]["recv"] = recv_obj
+    str_to_fun["fun_"]["recv"] = recv_fun
+
+    mad_path = mad_path or bin_path + "/mad_" + platform.system()
+    self.__process = mad_process(mad_path, py_name, debug, ipython_use_jedi)
+    #----------------------------------------------------------------------#
+
+    ## Store the relavent objects into a function to get reference objects
+    self.__mad_reflast = lambda: madhl_reflast(self.__process, lst_cntr)
+    self.__mad_ref = lambda name: madhl_ref(name, self.__process, lst_cntr)
+    if not ipython_use_jedi: #Stop jedi running getattr on my classes...
+      try:
+        ipython = get_ipython()
+        if ipython.__class__.__name__ == 'TerminalInteractiveShell':
+          ipython.Completer.use_jedi = False 
+      except NameError:
+        pass
+    self.py_name = py_name
+    # --------------------------------Retrieve the modules of MAD-------------------------------#
+    # Limit the 80 modules
+    modulesToImport = [
+      "element", "sequence", "mtable", "twiss", "beta0",
+      "beam", "survey", "object", "track", "match",
+    ]
+    self.load("MAD", *modulesToImport)
+    self.__MAD_version__ = self.MAD.env.version
+
+    self.send("""
+    function __mklast__ (a, b, ...)
+      if type(b) == "nil" then return a
+      else                     return {a, b, ...}
+      end
+    end
+    __last__ = {}
+    """)
+
+  # ------------------------------------------------------------------------------------------#
+
+  # --------------------------- Receiving data from subprocess -------------------------------#
+  def recv(
+    self, varname: str = None
+  ) -> Union[str, int, float, np.ndarray, bool, list]:
+    """Return received data from MAD-NG.
+
+    Args:
+      varname(str): The name of the variable you are receiving (Only useful when receiving references)
+        (default is None)
+
+    Returns:
+      Data from MAD-NG with type str/int/float/ndarray/bool/list, depending what was asked from MAD-NG.
+
+    Raises:
+      TypeError: If you forget to give a name when receiving a reference,  
+    """
+    return self.__process.recv(varname)
+
+  def receive(
+    self, varname: str = None
+  ) -> Union[str, int, float, np.ndarray, bool, list]:
+    """See :meth:`recv`"""
+    return self.__process.recv(varname)
+
+  def recv_and_exec(self, env: dict = {}) -> dict:
+    """Receive a string from MAD-NG and execute it.
+
+    Note: The class numpy and the instance of this object are available during the execution as ``np`` and ``mad`` respectively
+
+    Args:
+      env (dict): The environment you would like the string to be executed in.
+        (default = {})
+
+    Returns:
+      The updated environment after executing the string.
+    """
+    env["mad"] = self
+    return self.__process.recv_and_exec(env)
+
+  # --------------------------------Sending data to subprocess------------------------------------#
+  def send(self, data: Union[str, int, float, np.ndarray, bool, list]):
+    """Send data to MAD-NG.
+
+    Args:
+      data (str/int/float/ndarray/bool/list): The data to send to MAD-NG.
+
+    Returns:
+      self (the instance of the mad object)
+
+    Raises:
+      TypeError: An unsupported type was attempted to be sent to MAD-NG.
+      AssertionError: If data is a np.ndarray, the matrix must be of two dimensions.
+    """
+    self.__process.send(data)
+    return self
+
+  def send_rng(self, start: float, stop: float, size: int):
+    """Send a range to MAD-NG, equivalent to np.linspace, but in MAD-NG.
+
+    Args:
+      start (float): The start of range
+      stop (float): The end of range (inclusive)
+      size (float): The length of range
+    """
+    self.__process.send_rng(start, stop, size)
+
+  def send_lrng(self, start: float, stop: float, size: int):
+    """Send a numpy array as a logrange to MAD-NG, equivalent to np.geomspace, but in MAD-NG.
+
+    Args:
+      start (float): The start of range
+      stop (float): The end of range (inclusive)
+      size (float): The length of range
+    """
+    self.__process.send_lrng(start, stop, size)
+
+  def send_tpsa(self, monos: np.ndarray, coefficients: np.ndarray):
+    """Send the monomials and coefficients of a TPSA to MAD
+
+    The combination of monomials and coefficients creates a table representing the TPSA object in MAD-NG.
+
+    Args:
+      monos (ndarray): A list of monomials in the TPSA.
+      coefficients (ndarray): A list of coefficients in the TPSA.
+
+    Raises:
+      AssertionError: The list of monomials must be a 2-D array (each monomial is 1-D).
+      AssertionError: The number of monomials and coefficients must be identical.
+      AssertionError: The monomials must be of type 8-bit unsigned integer 
+    """
+    self.__process.send_tpsa(monos, coefficients)
+
+  def send_ctpsa(self, monos: np.ndarray, coefficients: np.ndarray):
+    """Send the monomials and coefficients of a complex TPSA to MAD-NG
+
+    The combination of monomials and coefficients creates a table representing the complex TPSA object in MAD-NG.
+    
+    Args:
+      See: :meth:`send_tpsa`.
+    
+    Raises:
+      See: :meth:`send_tpsa`.
+    """
+    self.__process.send_ctpsa(monos, coefficients)
+  
+  # ---------------------------------------------------------------------------------------------------------#
+  
+  # -------------------------------- Dealing with communication of variables --------------------------------#
+  def send_vars(
+    self,
+    names: Union[str, List[str]],
+    vars: List[Union[str, int, float, np.ndarray, bool, list]],
+  ):
+    """Send variables to the MAD-NG process.
+
+    Send the variables in vars with the names in names to MAD-NG.
+
+    Args:
+      names (str/List[str]): The name(s) that would like to assign your python variable(s) in MAD-NG.
+      vars (List[str/int/float/ndarray/bool/list]): The variables to send with the name(s) 'names' in MAD-NG.
+
+    Raises:
+      AssertionError: A list of names must be matched with a list of variables
+      AssertionError: The number of names must match the number of variables
+      Other Errors: See :meth:`send`.
+    """
+    self.__process.send_vars(names, vars)
+
+  def recv_vars(self, names: Union[str, List[str]]) -> Any:
+    """Receive variables from the MAD-NG process
+
+    Given a list of variable names, receive the variables from the MAD-NG process.
+
+    Args:
+      names (str/List[str]): The name(s) of variables that you would like to receive from MAD-NG.
+
+    Returns:
+      See :meth:`recv`.
+    """
+    return self.__process.recv_vars(names)
+
+  # -------------------------------------------------------------------------------------------------------------#
+
+  def load(self, module: str, *vars: str):
+    """Import modules into the MAD-NG environment
+
+    Retrieve the classes in MAD-NG from the module ``module``, while only importing the classes in the variable length list ``vars``.
+    If no string is provided, it is assumed that you would like to import every class from the module. 
+    
+    For example, ``mad.load("MAD.gmath")`` imports all variables from the module ``MAD.gmath``. 
+    But ``mad.load("MAD", "matrix", "cmatrix")```` only imports the modules ``matrix`` and ``cmatrix`` from the module ``MAD.gmath``.
+
+    Args:
+      module (str): The name of the module to import from.
+      *vars (str): Variable length argument list of the variable(s) to import from module.
+    """
+    script = ""
+    if vars == ():
+      vars = [x.strip("()") for x in dir(self.__mad_ref(module))]
+    for className in vars:
+      script += f"""{className} = {module}.{className}\n"""
+    self.__process.send(script)
+
+  def loadfile(self, path: str, *vars: str):
+    """Load a .mad file into the MAD-NG environment.
+
+    If ``vars`` is not provided, this is equivalent to ``assert(loadfile(path))`` in MAD-NG.
+    If ``vars`` is provided, for each ``var`` in ``vars``, this is equivalent to ``var = require(path).var`` in MAD-NG.
+    Due to Lua querks, do not include the .mad extension in the path if you provide ``vars``, as this implies you would like to load a module.
+
+    Args:
+      path (str): The path to the file to import.
+      *vars (str): Variable length argument list of the variable(s) to import from the file.
+    """
+    if vars == ():
+      self.__process.send(f"assert(loadfile('{path}', nil, {self.py_name}._env))()")
+    else:
+      if isinstance(vars, str):
+        vars = [vars]
+      script = ""
+      for var in vars:
+        script += f"{var} = require('{path}').{var}\n"
+      self.__process.send(script)
+
+  # ----------------------- Make the class work with dict and dot access ------------------------#
+  def __getattr__(self, item):
+    if item[0] == "_" and not item[:8] == "__last__":
+      raise AttributeError(item)
+    return self.__process.recv_vars(item)
+
+  def __setitem__(self, var_name: str, var: Any) -> None:
+    if isinstance(var_name, tuple):
+      var_name = list(var_name)
+      if isinstance(var, madhl_ref):
+        for i in range(len(var_name)):
+          self.send(f"{var_name[i]} = {var.__name__}[{i+1}]") # Skip send_vars
+        return
+      else:
+        var = list(var)
+      if len(var) != len(var_name):
+        raise ValueError(
+          "Incorrect number of values to unpack, received",
+          len(var),
+          "variables and",
+          len(var_name),
+          "keys",
         )
-        for var in vars_to_send:
-            self.send(var)
-        return rtrn
-
-    def __dir__(self) -> Iterable[str]:
-        pyObjs = [x for x in super(MAD, self).__dir__() if x[0] != "_"]
-        pyObjs.extend(self.globals())
-        pyObjs.extend(dir(self.recv_vars("_G")))
-        return pyObjs
-
-    def globals(self) -> List[str]:
-        """Retreive the list of names of variables in the environment of MAD
-
-        Returns:
-            A list of strings indicating the globals variables and modules within the MAD-NG environment
-        """
-        return dir(self.__process.recv_vars(f"{self.py_name}._env"))
-
-    # -------------------------------For use with the "with" statement-----------------------------------#
-    def __enter__(self):
-        return self
+    self.__process.send_vars(var_name, var)
 
-    def __exit__(self, exc_type, exc_value, tb):
-        pass
+  def __getitem__(self, var_name: str) -> Any:
+    return self.__process.recv_vars(var_name)
+  # ----------------------------------------------------------------------------------------------#
+
+  def eval(self, input: str):
+    """Evaluate an expression in MAD and return the result.
+
+    Args:
+      input (str): An expression that would like to be evaluated in MAD-NG.
+
+    Returns:
+      The evaluated result.
+    """
+    rtrn = self.__mad_reflast()
+    self.send(f"{rtrn.__name__} =" + input)
+    return rtrn.eval()
+
+  def MADX_env_send(self, input: str):
+    """Open the MAD-X environment in MAD-NG and directly send code.
+
+    Args:
+      input (str): The code that would like to be evaluated in the MAD-X environment in MAD-NG.
+    """
+    return self.__process.send("MADX:open_env()\n" + input + "\nMADX:close_env()")
+
+  def py_strs_to_mad_strs(self, input: Union[str, List[str]]):
+    """Add ' to either side of a string or each string in a list of strings
+    
+    Args: 
+      input(str/list[str]): The string(s) that you would like to add ' either side to each string.
+
+    Returns:
+      A string or list of strings with ' placed at the beginning and the end of each string.
+    """
+    if isinstance(input, list):
+      return ["'" + x + "'" for x in input]
+    else:
+      return "'" + input + "'"
+
+  # ----------------------------------------------------------------------------------------------#
+
+  # ---------------------------------------------------------------------------------------------------#
+
+  def deferred(self, **kwargs):
+    """Create a deferred expression object
+
+    For the deferred expression object, the kwargs are used as the deffered expressions, with ``=`` replaced
+    with ``:=``. To assign the returned object a name, then use ``mad['name'] = mad.deffered(kwargs)``.
+
+    Args:
+      **kwargs: A variable list of keyword arguments, keyword as the name of the deffered expression within the object and the value as a string that is sent directly to the MAD-NG environment.
+
+    Returns:
+      A reference to the deffered expression object.
+    """
+    rtrn = self.__mad_reflast()
+    kwargs_string, vars_to_send = get_kwargs_string(self.py_name, **kwargs)
+    self.__process.send(
+      f"{rtrn.__name__} = __mklast__( MAD.typeid.deferred {{ {kwargs_string.replace('=', ':=')[1:-3]} }} )"
+    )
+    for var in vars_to_send:
+      self.send(var)
+    return rtrn
+
+  def __dir__(self) -> Iterable[str]:
+    pyObjs = [x for x in super(MAD, self).__dir__() if x[0] != "_"]
+    pyObjs.extend(self.globals())
+    pyObjs.extend(dir(self.recv_vars("_G")))
+    return pyObjs
+
+  def globals(self) -> List[str]:
+    """Retreive the list of names of variables in the environment of MAD
+
+    Returns:
+      A list of strings indicating the globals variables and modules within the MAD-NG environment
+    """
+    return dir(self.__process.recv_vars(f"{self.py_name}._env"))
+
+  # -------------------------------For use with the "with" statement-----------------------------------#
+  def __enter__(self):
+    return self
+
+  def __exit__(self, exc_type, exc_value, tb):
+    pass
 
-    # ---------------------------------------------------------------------------------------------------#
+  # ---------------------------------------------------------------------------------------------------#
```

### Comparing `pymadng-0.3.9/src/pymadng/mad_process.py` & `pymadng-0.4.0/src/pymadng/madp_pymad.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,368 +1,366 @@
-import struct, os, subprocess, sys, platform, select
-from typing import Union, Tuple, Callable, Any
+import struct, os, subprocess, sys, select
+from typing import Union, Callable, Any
 import numpy as np
-from .mad_classes import mad_obj, mad_ref, mad_func, mad_reflast, mad_objlast
-from .mad_strings import mad_strings
-from .mad_last import last_counter
 
 __all__ = ["mad_process"]
 
+def get_typestring(a: Union[str, int, float, np.ndarray, bool, list]):
+  if isinstance(a, np.ndarray):
+    return a.dtype
+  elif type(a) is int: # Check for signed 32 bit int
+    if a.bit_length() < 31: return int
+    else:                   return float
+  else:
+    return type(a)
+  
 data_types = {
-        type(None)              : "nil_",
-        str                     : "str_",
-        int                     : "int_",
-        np.int32                : "int_",
-        float                   : "num_",
-        np.float64              : "num_",
-        complex                 : "cpx_",
-        np.complex128           : "cpx_",
-        bool                    : "bool",
-        list                    : "tbl_",
-        range                   : "irng",
-        np.dtype("float64")     : "mat_",
-        np.dtype("complex128")  : "cmat",
-        np.dtype("int32")       : "imat",
-        mad_obj                 : "obj_",
-        mad_ref                 : "ref_",
-        mad_func                : "fun_",
-        mad_reflast             : "ref_",
-        mad_objlast             : "obj_",
-        np.dtype("ubyte")       : "mono",
+  type(None)              : "nil_",
+  str                     : "str_",
+  int                     : "int_",
+  np.int32                : "int_",
+  float                   : "num_",
+  np.float64              : "num_",
+  complex                 : "cpx_",
+  np.complex128           : "cpx_",
+  bool                    : "bool",
+  list                    : "tbl_",
+  range                   : "irng",
+  np.dtype("float64")     : "mat_",
+  np.dtype("complex128")  : "cmat",
+  np.dtype("int32")       : "imat",
+  np.dtype("ubyte")       : "mono",
 }
-
 class mad_process:
-    def __init__(self, py_name: str, mad_path: str, debug: bool, num_temp_vars: int = 8, ipython_use_jedi: bool = False) -> None:
-        self.py_name = py_name
-        self.mad_strs = mad_strings(py_name)
-        self.last_counter = last_counter(num_temp_vars) # The mad objects require access to this
-        self.ipython_use_jedi = ipython_use_jedi        # ditto, but not entirely necessary
-
-        mad_path = mad_path or os.path.dirname(os.path.abspath(__file__)) + "/mad_" + platform.system()
-
-        self.from_mad, mad_write = os.pipe()
-        mad_read, self.to_mad = os.pipe()
-        self.fto_mad = os.fdopen(self.to_mad, "wb", buffering=0) # Sensible to not buffer stdin?
-        
-        startupChunk = f"MAD.pymad '{py_name}' {{_dbg = {str(debug).lower()}}} :__ini({mad_write})"
-
-        self.process = subprocess.Popen(
-            [mad_path, "-q", "-e", startupChunk],
-            bufsize=0,
-            stdin=mad_read,
-            stdout=sys.stdout.fileno(),
-            preexec_fn=os.setpgrp,  # Don't forward signals
-            pass_fds=[mad_write, sys.stdout.fileno(), sys.stderr.fileno()],
-        )
-        os.close(mad_write)
-        os.close(mad_read)
-
-        self.globalVars = {"np" : np} 
-        self.ffrom_mad = os.fdopen(self.from_mad, "rb")
-
-        # stdout should be line buffered by default, but for
-        # jupyter notebook, stdout is redirected and not 
-        # line buffered by default
-        self.send(
-            f"""io.stdout:setvbuf('line')
-                {self.py_name}:send(1)"""
-        )
-        checker = select.select([self.ffrom_mad], [], [], 1) # May not work on windows
-        if not checker[0] or self.recv() != 1: # Need to check number?
-            raise OSError(f"Unsuccessful starting of {mad_path} process")
-
-        self.send("""
-        function __mklast__ (a, b, ...)
-            if MAD.typeid.is_nil(b) then return a
-            else                         return {a, b, ...}
-            end
-        end
-        __last__ = {}
-        """)
-
-    def send_rng(self, start: float, stop: float, size: int):
-        """Send a numpy array as a rng to MAD"""
-        self.fto_mad.write(b"rng_")
-        send_grng(self, start, stop, size)
-
-    def send_lrng(self, start: float, stop: float, size: int):
-        """Send a numpy array as a logrange to MAD"""
-        self.fto_mad.write(b"lrng")
-        send_grng(self, start, stop, size)
-
-    def send_tpsa(self, monos: np.ndarray, coefficients: np.ndarray):
-        """Send the monomials and coeeficients of a TPSA to MAD, creating a table representing the TPSA object"""
-        self.fto_mad.write(b"tpsa")
-        send_gtpsa(self, monos, coefficients, send_num)
-
-    def send_ctpsa(self, monos: np.ndarray, coefficients: np.ndarray):
-        """Send the monomials and coeeficients of a complex TPSA to MAD, creating a table representing the complex TPSA object"""
-        self.fto_mad.write(b"ctpa")
-        send_gtpsa(self, monos, coefficients, send_cpx)
-
-    def send(self, data: Union[str, int, float, np.ndarray, bool, list]) -> None:
-        """Send data to MAD"""
-        try:
-            typ = data_types[get_typestring(data)]
-            self.fto_mad.write(typ.encode("utf-8"))
-            str_to_fun[typ]["send"](self, data)
-            return self
-        except KeyError:  # raise not in exception to reduce error output
-            pass
-        raise TypeError(
-            f"Unsupported data type, expected a type in: \n{list(data_types.keys())}, got {type(data)}"
-        )
-
-    def safe_send(self, string: str):
-        """Send a string to MAD, but first enable error handling, so that if an error occurs, an error is returned"""
-        return self.send(f"{self.py_name}:__err(true); {string}; {self.py_name}:__err(false);")
+  def __init__(self, mad_path: str, py_name: str = "py", debug: bool = False, ipython_use_jedi: bool = False) -> None:
+    self.py_name = py_name
+    self.ipython_use_jedi = ipython_use_jedi        # ditto, but not entirely necessary
+
+    self.from_mad, mad_write = os.pipe()
+    mad_read, self.to_mad = os.pipe()
+    self.fto_mad = os.fdopen(self.to_mad, "wb", buffering=0) # Sensible to not buffer stdin?
     
-    def safe_recv(self, name: str):
-        return self.send(f"{self.py_name}:__err(true):send({name}):__err(false)").recv(name)
+    startupChunk = f"MAD.pymad '{py_name}' {{_dbg = {str(debug).lower()}}} :__ini({mad_write})"
 
-    def errhdlr(self, on_off: bool):
-        """Enable or disable error handling"""
-        self.send(f"{self.py_name}:__err({str(on_off).lower()})")
-
-    def recv(
-        self, varname: str = None
-    ) -> Union[str, int, float, np.ndarray, bool, list]:
-        """Receive data from MAD, if a function is returned, it will be executed with the argument mad_communication"""
-        typ = self.ffrom_mad.read(4).decode("utf-8")
-        self.varname = varname  # For mad reference
-        return str_to_fun[typ]["recv"](self)
-
-    def recv_and_exec(self, env: dict = {}) -> dict:
-        """Read data from MAD and execute it"""
-        exec(compile(self.recv(), "ffrom_mad", "exec"), self.globalVars, env)
-        return env
-
-    # -------------------------------- Dealing with communication of variables --------------------------------#
-    def send_vars(self, names, vars):
-        if isinstance(names, str): 
-            names = [names]
-            vars = [vars]
-        else:
-            assert isinstance(vars, list), "A list of names must be matched with a list of variables"
-            assert len(vars) == len(names), "The number of names must match the number of variables"
-        for i, var in enumerate(vars):
-            if isinstance(vars[i], mad_ref):
-                self.send(f"{names[i]} = {var.__name__}")
-            else:
-                self.send(f"{names[i]} = {self.py_name}:recv()").send(var)
-
-    def recv_vars(self, names) -> Any:
-        if isinstance(names, str): 
-            names = [names]
-            cnvrt = lambda rtrn: rtrn[0]
-        else: 
-            cnvrt = lambda rtrn: tuple(rtrn)
-
-        rtrn_vars = []
-        for name in names:
-            if name[:2] != "__" or name[:8] == "__last__":  # Check for private variables
-                rtrn_vars.append(self.safe_recv(name))        
-        return cnvrt(rtrn_vars)
-
-    # -------------------------------------------------------------------------------------------------------------#
-
-    def __del__(self):
-        self.send(f"{self.py_name}:__fin()")
-        self.ffrom_mad.close()
-        self.process.terminate() #In case user left mad waiting
-        self.fto_mad.close()
-        self.process.wait()
+    self.process = subprocess.Popen(
+      [mad_path, "-q", "-e", startupChunk],
+      bufsize=0,
+      stdin=mad_read,
+      stdout=sys.stdout.fileno(),
+      preexec_fn=os.setpgrp,  # Don't forward signals
+      pass_fds=[mad_write, sys.stdout.fileno(), sys.stderr.fileno()],
+    )
+    os.close(mad_write)
+    os.close(mad_read)
 
+    self.globalVars = {"np" : np} 
+    self.ffrom_mad = os.fdopen(self.from_mad, "rb")
 
-def get_typestring(a: Union[str, int, float, np.ndarray, bool, list]):
-    if isinstance(a, np.ndarray):
-        return a.dtype
-    elif type(a) is int:
-        if a.bit_length() < 31: # Check for signed 32 bit int
-            return int
-        else: 
-            return float
+    # stdout should be line buffered by default, but for jupyter notebook, 
+    # stdout is redirected and not line buffered by default
+    self.send(
+      f"""io.stdout:setvbuf('line')
+        {self.py_name}:send(1)"""
+    )
+    checker = select.select([self.ffrom_mad], [], [], 1) # May not work on windows
+    if not checker[0] or self.recv() != 1: # Need to check number?
+      raise OSError(f"Unsuccessful starting of {mad_path} process")
+
+  def send_rng(self, start: float, stop: float, size: int):
+    """Send a numpy array as a rng to MAD"""
+    self.fto_mad.write(b"rng_")
+    send_grng(self, start, stop, size)
+
+  def send_lrng(self, start: float, stop: float, size: int):
+    """Send a numpy array as a logrange to MAD"""
+    self.fto_mad.write(b"lrng")
+    send_grng(self, start, stop, size)
+
+  def send_tpsa(self, monos: np.ndarray, coefficients: np.ndarray):
+    """Send the monomials and coeeficients of a TPSA to MAD, creating a table representing the TPSA object"""
+    self.fto_mad.write(b"tpsa")
+    send_gtpsa(self, monos, coefficients, send_num)
+
+  def send_ctpsa(self, monos: np.ndarray, coefficients: np.ndarray):
+    """Send the monomials and coeeficients of a complex TPSA to MAD, creating a table representing the complex TPSA object"""
+    self.fto_mad.write(b"ctpa")
+    send_gtpsa(self, monos, coefficients, send_cpx)
+
+  def send(self, data: Union[str, int, float, np.ndarray, bool, list]):
+    """Send data to MAD, returns self for chaining"""
+    try:
+      typ = data_types[get_typestring(data)]
+      self.fto_mad.write(typ.encode("utf-8"))
+      str_to_fun[typ]["send"](self, data)
+      return self
+    except KeyError:  # raise not in exception to reduce error output
+      pass
+    raise TypeError(
+      f"Unsupported data type, expected a type in: \n{list(data_types.keys())}, got {type(data)}"
+    )
+
+  def psend(self, string: str):
+    """Perform a protected send to MAD, by first enabling error handling, so that if an error occurs, an error is returned"""
+    return self.send(f"{self.py_name}:__err(true); {string}; {self.py_name}:__err(false);")
+  
+  def precv(self, name: str):
+    """Perform a protected send receive to MAD, by first enabling error handling, so that if an error occurs, an error is received"""
+    return self.send(f"{self.py_name}:__err(true):send({name}):__err(false)").recv(name)
+
+  def errhdlr(self, on_off: bool):
+    """Enable or disable error handling"""
+    self.send(f"{self.py_name}:__err({str(on_off).lower()})")
+
+  def recv(
+    self, varname: str = None
+  ) -> Union[str, int, float, np.ndarray, bool, list]:
+    """Receive data from MAD, if a function is returned, it will be executed with the argument mad_communication"""
+    typ = self.ffrom_mad.read(4).decode("utf-8")
+    self.varname = varname  # For mad reference
+    return str_to_fun[typ]["recv"](self)
+
+  def recv_and_exec(self, env: dict = {}) -> dict:
+    """Read data from MAD and execute it"""
+    exec(compile(self.recv(), "ffrom_mad", "exec"), self.globalVars, env)
+    return env
+
+  # ----------------- Dealing with communication of variables ---------------#
+  def send_vars(self, names, vars):
+    if isinstance(names, str): 
+      names = [names]
+      vars = [vars]
+    else:
+      assert isinstance(vars, list), "A list of names must be matched with a list of variables"
+      assert len(vars) == len(names), "The number of names must match the number of variables"
+    for i, var in enumerate(vars):
+      if isinstance(vars[i], mad_ref):
+        self.send(f"{names[i]} = {var.__name__}")
+      else:
+        self.send(f"{names[i]} = {self.py_name}:recv()").send(var)
+
+  def recv_vars(self, names) -> Any:
+    if isinstance(names, str): 
+      names = [names]
+      cnvrt = lambda rtrn: rtrn[0]
+    else: 
+      cnvrt = lambda rtrn: tuple(rtrn)
+
+    rtrn_vars = []
+    for name in names:
+      if name[:2] != "__" or name[:8] == "__last__":  # Check for private variables
+        rtrn_vars.append(self.precv(name))        
+    return cnvrt(rtrn_vars)
+
+  # -------------------------------------------------------------------------#
+
+  def __del__(self):
+    self.send(f"{self.py_name}:__fin()")
+    self.ffrom_mad.close()
+    self.process.terminate() #In case user left mad waiting
+    self.fto_mad.close()
+    self.process.wait()
+    
+class mad_ref(object):    
+  def __init__(self, name: str, mad_proc: mad_process) -> None:
+    assert name is not None, "Reference must have a variable to reference to. Did you forget to put a name in the receive functions?"
+    self.__name__ = name
+    self.__mad__ = mad_proc
+
+  def __getattr__ (self, item):
+    if item[0] != "_":
+      try:
+        return self[item]
+      except (IndexError, KeyError):
+        pass
+    raise AttributeError (item)  # For python
+
+  def __getitem__(self, item: Union[str, int]):
+    if isinstance(item, int):
+      result = self.__mad__.precv(f"{self.__name__}[{item+1}]")
+      if result is None:
+        raise IndexError(item)  # For python
+    elif isinstance(item, str):
+      result = self.__mad__.precv(f"{self.__name__}['{item}']")
+      if result is None:
+        raise KeyError(item)  # For python
     else:
-        return type(a)
+      raise TypeError("Cannot index type of ", type(item))
 
+    return result
 
-# --------------------------------------- Sending data ---------------------------------------#
+  def eval(self):
+    return self.__mad__.recv_vars(self.__name__)
+
+data_types[mad_ref] = "ref_" # Add mad_ref to the datatypes
+
+# -------------------------------- Sending data -------------------------------#
 send_nil = lambda self, input: None
 
-def send_ref(self: mad_process, obj: mad_ref) -> None:
-    send_str(self, f"return {obj.__name__}")
+def send_int(self: mad_process, input: int) -> None:
+  self.fto_mad.write(struct.pack("i", input))
 
 def send_str(self: mad_process, input: str) -> None:
-    send_int(self, len(input))
-    self.fto_mad.write(input.encode("utf-8"))
+  send_int(self, len(input))
+  self.fto_mad.write(input.encode("utf-8"))
 
-def send_int(self: mad_process, input: int) -> None:
-    self.fto_mad.write(struct.pack("i", input))
+def send_ref(self: mad_process, obj: mad_ref) -> None:
+  send_str(self, f"return {obj.__name__}")
 
 def send_num(self: mad_process, input: float) -> None:
-    self.fto_mad.write(struct.pack("d", input))
+  self.fto_mad.write(struct.pack("d", input))
 
 def send_cpx(self: mad_process, input: complex) -> None:
-    self.fto_mad.write(struct.pack("dd", input.real, input.imag))
+  self.fto_mad.write(struct.pack("dd", input.real, input.imag))
 
 def send_bool(self: mad_process, input: bool) -> None:
-    self.fto_mad.write(struct.pack("?", input))
-
-def send_shape(self: mad_process, shape: Tuple[int, int]) -> None:
-    send_int(self, shape[0])
-    send_int(self, shape[1])
+  self.fto_mad.write(struct.pack("?", input))
 
 def send_gmat(self: mad_process, mat: np.ndarray) -> None:
-    assert len(mat.shape) == 2, "Matrix must be of two dimensions"
-    send_shape(self, mat.shape)
-    self.fto_mad.write(mat.tobytes())
+  assert len(mat.shape) == 2, "Matrix must be of two dimensions"
+  send_int(self, mat.shape[0])
+  send_int(self, mat.shape[1])
+  self.fto_mad.write(mat.tobytes())
 
 def send_list(self: mad_process, lst: list) -> None:
-    n = len(lst)
-    send_int(self, n)
-    for item in lst:
-        self.send(item)  # deep copy
-    return self
+  n = len(lst)
+  send_int(self, n)
+  for item in lst:
+    self.send(item)  # deep copy
+  return self
 
 def send_grng(self: mad_process, start: float, stop: float, size: int) -> None:
-    self.fto_mad.write(struct.pack("ddi", start, stop, size))
+  self.fto_mad.write(struct.pack("ddi", start, stop, size))
 
 def send_irng(self: mad_process, rng: range) -> None:
-    self.fto_mad.write(struct.pack("iii", rng.start, rng.stop, rng.step))
+  self.fto_mad.write(struct.pack("iii", rng.start, rng.stop, rng.step))
 
 def send_mono(self: mad_process, mono: np.ndarray) -> None:
-    send_int(self, mono.size)
-    self.fto_mad.write(mono.tobytes())
+  send_int(self, mono.size)
+  self.fto_mad.write(mono.tobytes())
 
 def send_gtpsa(
-    self: mad_process,
-    monos: np.ndarray,
-    coefficients: np.ndarray,
-    fsendNum: Callable[[mad_process, Union[float, complex]], None],
+  self: mad_process,
+  monos: np.ndarray,
+  coefficients: np.ndarray,
+  fsendNum: Callable[[mad_process, Union[float, complex]], None],
 ) -> None:
-    assert len(monos.shape) == 2, "The list of monomials must have two dimensions"
-    assert len(monos) == len(coefficients), "The number of monomials must be equal to the number of coefficients"
-    assert monos.dtype == np.uint8, "The monomials must be of type 8-bit unsigned integer "
-    send_int(self, len(monos))  # Num monomials
-    send_int(self, len(monos[0]))  # Monomial length
-    for mono in monos:
-        self.fto_mad.write(mono.tobytes())
-    for coefficient in coefficients:
-        fsendNum(self, coefficient)
+  assert len(monos.shape) == 2, "The list of monomials must have two dimensions"
+  assert len(monos) == len(coefficients), "The number of monomials must be equal to the number of coefficients"
+  assert monos.dtype == np.uint8, "The monomials must be of type 8-bit unsigned integer "
+  send_int(self, len(monos))  # Num monomials
+  send_int(self, len(monos[0]))  # Monomial length
+  for mono in monos:
+    self.fto_mad.write(mono.tobytes())
+  for coefficient in coefficients:
+    fsendNum(self, coefficient)
+# -----------------------------------------------------------------------------#
 
-# --------------------------------------------------------------------------------------------#
+# --------------------------- Receiving data ----------------------------------#
 
-# --------------------------------------- Receiving data -------------------------------------#
 recv_nil = lambda self: None
 
 def recv_ref(self: mad_process) -> mad_ref:
-    return mad_ref(self.varname, self)
-
-def recv_obj(self: mad_process) -> mad_obj:
-    return mad_obj(self.varname, self)
-
-def recv_fun(self: mad_process) -> mad_func:
-    return mad_func(self.varname, self)
+  return mad_ref(self.varname, self)
 
 def recv_str(self: mad_process) -> str:
-    return self.ffrom_mad.read(recv_int(self)).decode("utf-8")
+  return self.ffrom_mad.read(recv_int(self)).decode("utf-8")
 
 def recv_int(self: mad_process) -> int:  # Must be int32
-    return int.from_bytes(self.ffrom_mad.read(4), sys.byteorder, signed=True)
+  return int.from_bytes(self.ffrom_mad.read(4), sys.byteorder, signed=True)
 
 def recv_num(self: mad_process) -> float:
-    return np.frombuffer(self.ffrom_mad.read(8), dtype=np.float64)[0]
+  return np.frombuffer(self.ffrom_mad.read(8), dtype=np.float64)[0]
 
 def recv_cpx(self: mad_process) -> complex:
-    return np.frombuffer(self.ffrom_mad.read(16), dtype=np.complex128)[0]
+  return np.frombuffer(self.ffrom_mad.read(16), dtype=np.complex128)[0]
 
 def recv_bool(self: mad_process) -> str:
-    return np.frombuffer(self.ffrom_mad.read(1), dtype=np.bool_)[0]
+  return np.frombuffer(self.ffrom_mad.read(1), dtype=np.bool_)[0]
 
 def recv_gmat(self: mad_process, dtype: np.dtype) -> str:
-    shape = np.frombuffer(self.ffrom_mad.read(8), dtype=np.int32)
-    arraySize = shape[0] * shape[1] * dtype.itemsize
-    return np.frombuffer(self.ffrom_mad.read(arraySize), dtype=dtype).reshape(shape)
+  shape = np.frombuffer(self.ffrom_mad.read(8), dtype=np.int32)
+  arraySize = shape[0] * shape[1] * dtype.itemsize
+  return np.frombuffer(self.ffrom_mad.read(arraySize), dtype=dtype).reshape(shape)
 
 def recv_mat(self: mad_process) -> str:
-    return recv_gmat(self, np.dtype("float64"))
+  return recv_gmat(self, np.dtype("float64"))
 
 def recv_cmat(self: mad_process) -> str:
-    return recv_gmat(self, np.dtype("complex128"))
+  return recv_gmat(self, np.dtype("complex128"))
 
 def recv_imat(self: mad_process) -> str:
-    return recv_gmat(self, np.dtype("int32"))
+  return recv_gmat(self, np.dtype("int32"))
 
 def recv_list(self: mad_process) -> list:
-    varname = self.varname  # cache
-    haskeys = recv_bool(self)
-    lstLen = recv_int(self)
-    vals = [self.recv(varname and varname + f"[{i+1}]") for i in range(lstLen)]
-    self.varname = varname  # reset
-    if haskeys and lstLen == 0:
-        return recv_ref(self)
-    elif haskeys:
-        return vals, recv_ref(self)
-    else:
-        return vals
+  varname = self.varname  # cache
+  haskeys = recv_bool(self)
+  lstLen = recv_int(self)
+  vals = [self.recv(varname and varname + f"[{i+1}]") for i in range(lstLen)]
+  self.varname = varname  # reset
+  if haskeys and lstLen == 0:
+    return recv_ref(self)
+  elif haskeys:
+    return vals, recv_ref(self)
+  else:
+    return vals
 
 def recv_irng(self: mad_process) -> range:
-    start, stop, step = np.frombuffer(self.ffrom_mad.read(12), dtype=np.int32)
-    return range(start, stop + 1, step)  # MAD is inclusive at both ends
+  start, stop, step = np.frombuffer(self.ffrom_mad.read(12), dtype=np.int32)
+  return range(start, stop + 1, step)  # MAD is inclusive at both ends
 
 def recv_rng(self: mad_process) -> np.ndarray:
-    return np.linspace(*struct.unpack("ddi", self.ffrom_mad.read(20)))
+  return np.linspace(*struct.unpack("ddi", self.ffrom_mad.read(20)))
 
 def recv_lrng(self: mad_process) -> np.ndarray:
-    return np.geomspace(*struct.unpack("ddi", self.ffrom_mad.read(20)))
+  return np.geomspace(*struct.unpack("ddi", self.ffrom_mad.read(20)))
 
 def recv_mono(self: mad_process) -> np.ndarray:
-    mono_len = recv_int(self)
-    return np.frombuffer(self.ffrom_mad.read(mono_len), dtype=np.ubyte)
+  mono_len = recv_int(self)
+  return np.frombuffer(self.ffrom_mad.read(mono_len), dtype=np.ubyte)
 
 def recv_gtpsa(self: mad_process, dtype: np.dtype) -> np.ndarray:
-    num_mono, mono_len = np.frombuffer(self.ffrom_mad.read(8), dtype=np.int32)
-    mono_list = np.reshape(
-        np.frombuffer(self.ffrom_mad.read(mono_len * num_mono), dtype=np.ubyte),
-        (num_mono, mono_len),
-    )
-    coefficients = np.frombuffer(
-        self.ffrom_mad.read(num_mono * dtype.itemsize), dtype=dtype
-    )
-    return mono_list, coefficients
+  num_mono, mono_len = np.frombuffer(self.ffrom_mad.read(8), dtype=np.int32)
+  mono_list = np.reshape(
+    np.frombuffer(self.ffrom_mad.read(mono_len * num_mono), dtype=np.ubyte),
+    (num_mono, mono_len),
+  )
+  coefficients = np.frombuffer(
+    self.ffrom_mad.read(num_mono * dtype.itemsize), dtype=dtype
+  )
+  return mono_list, coefficients
 
 def recv_ctpa(self: mad_process):
-    return recv_gtpsa(self, np.dtype("complex128"))
+  return recv_gtpsa(self, np.dtype("complex128"))
 
 def recv_tpsa(self: mad_process):
-    return recv_gtpsa(self, np.dtype("float64"))
+  return recv_gtpsa(self, np.dtype("float64"))
 
 def recv_err(self: mad_process):
-    self.errhdlr(False)
-    raise RuntimeError("MAD Errored (see the MAD error output)")
+  self.errhdlr(False)
+  raise RuntimeError("MAD Errored (see the MAD error output)")
 
-# --------------------------------------------------------------------------------------------#
+# -----------------------------------------------------------------------------#
 
-# -------------------------------------- Dict for data ---------------------------------------#
+# ----------------------------- Dict for data ---------------------------------#
 str_to_fun = {
-    "nil_": {"recv": recv_nil , "send": send_nil },
-    "bool": {"recv": recv_bool, "send": send_bool},
-    "str_": {"recv": recv_str , "send": send_str },
-    "tbl_": {"recv": recv_list, "send": send_list},
-    "ref_": {"recv": recv_ref , "send": send_ref },
-    "fun_": {"recv": recv_fun , "send": send_ref },
-    "obj_": {"recv": recv_obj , "send": send_ref },
-    "int_": {"recv": recv_int , "send": send_int },
-    "num_": {"recv": recv_num , "send": send_num },
-    "cpx_": {"recv": recv_cpx , "send": send_cpx },
-    "mat_": {"recv": recv_mat , "send": send_gmat},
-    "cmat": {"recv": recv_cmat, "send": send_gmat},
-    "imat": {"recv": recv_imat, "send": send_gmat},
-    "rng_": {"recv": recv_rng ,                  },
-    "lrng": {"recv": recv_lrng,                  },
-    "irng": {"recv": recv_irng, "send": send_irng},
-    "mono": {"recv": recv_mono, "send": send_mono},
-    "tpsa": {"recv": recv_tpsa,                  },
-    "ctpa": {"recv": recv_ctpa,                  },
-    "err_": {"recv": recv_err ,                  },
+  "nil_": {"recv": recv_nil , "send": send_nil },
+  "bool": {"recv": recv_bool, "send": send_bool},
+  "str_": {"recv": recv_str , "send": send_str },
+  "tbl_": {"recv": recv_list, "send": send_list},
+  "ref_": {"recv": recv_ref , "send": send_ref },
+  "fun_": {"recv": recv_ref , "send": send_ref },
+  "obj_": {"recv": recv_ref , "send": send_ref },
+  "int_": {"recv": recv_int , "send": send_int },
+  "num_": {"recv": recv_num , "send": send_num },
+  "cpx_": {"recv": recv_cpx , "send": send_cpx },
+  "mat_": {"recv": recv_mat , "send": send_gmat},
+  "cmat": {"recv": recv_cmat, "send": send_gmat},
+  "imat": {"recv": recv_imat, "send": send_gmat},
+  "rng_": {"recv": recv_rng ,                  },
+  "lrng": {"recv": recv_lrng,                  },
+  "irng": {"recv": recv_irng, "send": send_irng},
+  "mono": {"recv": recv_mono, "send": send_mono},
+  "tpsa": {"recv": recv_tpsa,                  },
+  "ctpa": {"recv": recv_ctpa,                  },
+  "err_": {"recv": recv_err ,                  },
 }
-# --------------------------------------------------------------------------------------------#
+# ---------------------------------------------------------------------------- #
```

### Comparing `pymadng-0.3.9/src/pymadng.egg-info/PKG-INFO` & `pymadng-0.4.0/src/pymadng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymadng
-Version: 0.3.9
+Version: 0.4.0
 Summary: A python interface to MAD-NG running as subprocess
 Author-email: Joshua Gray <joshua.mark.gray@cern.ch>
 Project-URL: Homepage, https://github.com/MethodicalAcceleratorDesign/MADpy
 Project-URL: Bug Tracker, https://github.com/MethodicalAcceleratorDesign/MADpy/issues
 Project-URL: MAD Source, https://github.com/MethodicalAcceleratorDesign/MAD
 Project-URL: Documentation, https://pymadng.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymadng-0.3.9/src/pymadng.egg-info/SOURCES.txt` & `pymadng-0.4.0/src/pymadng.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -38,22 +38,19 @@
 examples/ex-ps-twiss/ps_unset_vars.mad
 examples/ex-recv-lhc/defexpr_speed.mad
 examples/ex-recv-lhc/ex-defexpr.py
 examples/ex-recv-lhc/lhc_as-built.seq
 examples/ex-recv-lhc/lhc_unset_vars.mad
 examples/ex-recv-lhc/opt_400_10000_400_3000.madx
 src/pymadng/__init__.py
-src/pymadng/mad_Darwin
-src/pymadng/mad_Linux
-src/pymadng/mad_classes.py
-src/pymadng/mad_completer.py
-src/pymadng/mad_last.py
-src/pymadng/mad_object.py
-src/pymadng/mad_process.py
-src/pymadng/mad_strings.py
+src/pymadng/madp_classes.py
+src/pymadng/madp_last.py
+src/pymadng/madp_object.py
+src/pymadng/madp_pymad.py
+src/pymadng/madp_strings.py
 src/pymadng.egg-info/PKG-INFO
 src/pymadng.egg-info/SOURCES.txt
 src/pymadng.egg-info/dependency_links.txt
 src/pymadng.egg-info/requires.txt
 src/pymadng.egg-info/top_level.txt
 tests/comm_tests.py
 tests/obj_tests.py
```

### Comparing `pymadng-0.3.9/tests/comm_tests.py` & `pymadng-0.4.0/tests/comm_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,378 +1,379 @@
 import unittest, os
 from pymadng import MAD
 import numpy as np
 
 class TestExecution(unittest.TestCase):
 
-    def test_recv_and_exec(self):
-        with MAD() as mad:
-            mad.send("""py:send([==[mad.send('''py:send([=[mad.send("py:send([[a = 100/2]])")]=])''')]==])""")
-            mad.recv_and_exec()
-            mad.recv_and_exec()
-            a = mad.recv_and_exec()["a"]
-            self.assertEqual(a, 50)
-
-    def test_err(self):
-        with MAD() as mad:
-            mad.send("py:__err(true)")
-            mad.send("1+1") #Load error
-            self.assertRaises(RuntimeError, mad.recv)
-            mad.send("py:__err(true)")
-            mad.send("print(nil/2)") #Runtime error
-            self.assertRaises(RuntimeError, mad.recv)
+  def test_recv_and_exec(self):
+    with MAD() as mad:
+      mad.send("""py:send([==[mad.send('''py:send([=[mad.send("py:send([[a = 100/2]])")]=])''')]==])""")
+      mad.recv_and_exec()
+      mad.recv_and_exec()
+      a = mad.recv_and_exec()["a"]
+      self.assertEqual(a, 50)
+
+  def test_err(self):
+    with MAD() as mad:
+      mad.send("py:__err(true)")
+      mad.send("1+1") #Load error
+      self.assertRaises(RuntimeError, mad.recv)
+      mad.send("py:__err(true)")
+      mad.send("print(nil/2)") #Runtime error
+      self.assertRaises(RuntimeError, mad.recv)
 
 class TestStrings(unittest.TestCase):
 
-    def test_recv(self):
-        with MAD() as mad:
-            mad.send("py:send('hi')")
-            mad.send("""py:send([[Multiline string should work
+  def test_recv(self):
+    with MAD() as mad:
+      mad.send("py:send('hi')")
+      mad.send("""py:send([[Multiline string should work
 
 Like So.]])""")
-            self.assertEqual(mad.recv(), 'hi')
-            self.assertEqual(mad.recv(), 'Multiline string should work\n\nLike So.')
+      self.assertEqual(mad.recv(), 'hi')
+      self.assertEqual(mad.recv(), 'Multiline string should work\n\nLike So.')
 
-    def test_send(self):
-        with MAD() as mad:
-            initString = "asdfghjkl;"
-            mad.send("str = py:recv(); py:send(str .. str)")
-            mad.send(initString)
-            self.assertEqual(mad.recv(), initString * 2)
-            mad.send("str2 = py:recv(); py:send(str2 .. str2)")
-            initString = """Py Multiline string should work
+  def test_send(self):
+    with MAD() as mad:
+      initString = "asdfghjkl;"
+      mad.send("str = py:recv(); py:send(str .. str)")
+      mad.send(initString)
+      self.assertEqual(mad.recv(), initString * 2)
+      mad.send("str2 = py:recv(); py:send(str2 .. str2)")
+      initString = """Py Multiline string should work
 
 Like So.]])"""
-            mad.send(initString)
-            self.assertEqual(mad.recv(), initString * 2)
+      mad.send(initString)
+      self.assertEqual(mad.recv(), initString * 2)
 
 class TestNil(unittest.TestCase):
 
-    def test_send_recv(self):
-        with MAD() as mad:
-            mad.send("""
-            local myNil = py:recv()
-            py:send(myNil)
-            py:send(nil)
-            py:send()
-            """)
-            mad.send(None)
-            self.assertIsNone(mad.recv())
-            self.assertIsNone(mad.recv())
-            self.assertIsNone(mad.recv())
+  def test_send_recv(self):
+    with MAD() as mad:
+      mad.send("""
+      local myNil = py:recv()
+      py:send(myNil)
+      py:send(nil)
+      py:send()
+      """)
+      mad.send(None)
+      self.assertIsNone(mad.recv())
+      self.assertIsNone(mad.recv())
+      self.assertIsNone(mad.recv())
 
 class TestList(unittest.TestCase):
-    
-    def test_send_recv(self):
-        with MAD() as mad:
-            myList = [[1, 2, 3, 4, 5, 6, 7, 8, 9]] * 2
-            mad.send("""
-            local list = py:recv()
-            list[1][1] = 10
-            list[2][1] = 10
-            py:send(list)
-            """)
-            mad.send(myList)
-            myList[0][0] = 10
-            myList[1][0] = 10
-            self.assertEqual(mad.recv(), myList)
-
-    def test_send_recv_wref(self):
-        with MAD() as mad:
-            mad.send("""
-            list = {MAD.object "a" {a = 2}, MAD.object "b" {b = 2}}
-            list2 = {1, 2, 3, 4, 5, a = 10, b = 3, c = 4}
-            py:send(list)
-            py:send(list2)
-            """)
-            list1 = mad.recv("list")
-            list2 = mad.recv("list2")
-            self.assertEqual(len(list1), 2)
-            self.assertEqual(list2[0], [1, 2, 3, 4, 5])
-            self.assertEqual(list2[1].a, 10)
-            self.assertEqual(list2[1].b, 3)
-            self.assertEqual(list2[1].c, 4)
-            self.assertEqual(list1[0].a, 2)
-            self.assertEqual(list1[1].b, 2)
+  
+  def test_send_recv(self):
+    with MAD() as mad:
+      myList = [[1, 2, 3, 4, 5, 6, 7, 8, 9]] * 2
+      mad.send("""
+      local list = py:recv()
+      list[1][1] = 10
+      list[2][1] = 10
+      py:send(list)
+      """)
+      mad.send(myList)
+      myList[0][0] = 10
+      myList[1][0] = 10
+      self.assertEqual(mad.recv(), myList)
+
+  def test_send_recv_wref(self):
+    with MAD() as mad:
+      mad.send("""
+      list = {MAD.object "a" {a = 2}, MAD.object "b" {b = 2}}
+      list2 = {1, 2, 3, 4, 5, a = 10, b = 3, c = 4}
+      py:send(list)
+      py:send(list2)
+      """)
+      list1 = mad.recv("list")
+      list2 = mad.recv("list2")
+      self.assertEqual(len(list1), 2)
+      self.assertEqual(list2[0], [1, 2, 3, 4, 5])
+      self.assertEqual(list2[1].a, 10)
+      self.assertEqual(list2[1].b, 3)
+      self.assertEqual(list2[1].c, 4)
+      self.assertEqual(list1[0].a, 2)
+      self.assertEqual(list1[1].b, 2)
 
-    
+  
 class TestNums(unittest.TestCase):
 
-    eps = 2**-52; tiny = 2**-1022; huge = 2**1023
-    flt_lst = [0, tiny, 2**-64, 2**-63, 2**-53, eps, 2**-52, 2*eps, 2**-32, 2**-31, 1e-9,
-                0.1-eps, 0.1, 0.1+eps, 0.5, 0.7-eps, 0.7, 0.7+eps, 1-eps, 1, 1+eps,
-                1.1, 1.7, 2, 10, 1e2, 1e3, 1e6, 1e9, 2**31, 2**32, 2**52, 2**53,
-                2**63, 2**64, huge]
-
-    def test_send_recv_int(self):
-        with MAD() as mad:
-            int_lst = [0, 1, 2, 10, 1e2, 1e3, 1e6, 1e9, 2**31-1]
-            for i in range(len(int_lst)):
-                mad.send("""
-                local is_integer in MAD.typeid
-                local num = py:recv()
-                py:send( num)
-                py:send(-num)
-                py:send(is_integer(num))
-                """)
-                mad.send(int_lst[i])
-                recv_num = mad.recv()
-                self.assertEqual(recv_num, int_lst[i])
-                self.assertTrue(isinstance(recv_num, int))
-                recv_num = mad.recv()
-                self.assertEqual(recv_num, -int_lst[i])
-                self.assertTrue(isinstance(recv_num, int))
-                self.assertTrue(mad.recv())
-
-    def test_send_recv_num(self):
-        with MAD() as mad:
-            for i in range(len(self.flt_lst)):
-                mad.send("""
-                local num = py:recv()
-                local negative = py:recv()
-                py:send(num)
-                py:send(negative)
-                py:send(num * 1.61)
-                """)
-                mad.send(self.flt_lst[i])
-                mad.send(-self.flt_lst[i])
-                self.assertEqual(mad.recv(),  self.flt_lst[i]) #Check individual floats
-                self.assertEqual(mad.recv(), -self.flt_lst[i]) #Check negation
-                self.assertEqual(mad.recv(),  self.flt_lst[i] * 1.61) #Check manipulation
-
-    def test_send_recv_cpx(self):
-        with MAD() as mad:
-            for i in range(len(self.flt_lst)):
-                for j in range(len(self.flt_lst)):
-                    mad.send("""
-                    local my_cpx = py:recv()
-                    py:send(my_cpx)
-                    py:send(-my_cpx)
-                    py:send(my_cpx * 1.31i)
-                    """)
-                    my_cpx = self.flt_lst[i] + 1j * self.flt_lst[j]
-                    mad.send(my_cpx)
-                    self.assertEqual(mad.recv(),  my_cpx)
-                    self.assertEqual(mad.recv(), -my_cpx)
-                    self.assertEqual(mad.recv(),  my_cpx * 1.31j)
+  eps = 2**-52; tiny = 2**-1022; huge = 2**1023
+  flt_lst = [0, tiny, 2**-64, 2**-63, 2**-53, eps, 2**-52, 2*eps, 2**-32, 2**-31, 1e-9,
+        0.1-eps, 0.1, 0.1+eps, 0.5, 0.7-eps, 0.7, 0.7+eps, 1-eps, 1, 1+eps,
+        1.1, 1.7, 2, 10, 1e2, 1e3, 1e6, 1e9, 2**31, 2**32, 2**52, 2**53,
+        2**63, 2**64, huge]
+
+  def test_send_recv_int(self):
+    with MAD() as mad:
+      int_lst = [0, 1, 2, 10, 1e2, 1e3, 1e6, 1e9, 2**31-1]
+      for i in range(len(int_lst)):
+        mad.send("""
+        local is_integer in MAD.typeid
+        local num = py:recv()
+        py:send( num)
+        py:send(-num)
+        py:send(is_integer(num))
+        """)
+        mad.send(int_lst[i])
+        recv_num = mad.recv()
+        self.assertEqual(recv_num, int_lst[i])
+        self.assertTrue(isinstance(recv_num, int))
+        recv_num = mad.recv()
+        self.assertEqual(recv_num, -int_lst[i])
+        self.assertTrue(isinstance(recv_num, int))
+        self.assertTrue(mad.recv())
+
+  def test_send_recv_num(self):
+    with MAD() as mad:
+      for i in range(len(self.flt_lst)):
+        mad.send("""
+        local num = py:recv()
+        local negative = py:recv()
+        py:send(num)
+        py:send(negative)
+        py:send(num * 1.61)
+        """)
+        mad.send(self.flt_lst[i])
+        mad.send(-self.flt_lst[i])
+        self.assertEqual(mad.recv(),  self.flt_lst[i]) #Check individual floats
+        self.assertEqual(mad.recv(), -self.flt_lst[i]) #Check negation
+        self.assertEqual(mad.recv(),  self.flt_lst[i] * 1.61) #Check manipulation
+
+  def test_send_recv_cpx(self):
+    with MAD() as mad:
+      for i in range(len(self.flt_lst)):
+        for j in range(len(self.flt_lst)):
+          mad.send("""
+          local my_cpx = py:recv()
+          py:send(my_cpx)
+          py:send(-my_cpx)
+          py:send(my_cpx * 1.31i)
+          """)
+          my_cpx = self.flt_lst[i] + 1j * self.flt_lst[j]
+          mad.send(my_cpx)
+          self.assertEqual(mad.recv(),  my_cpx)
+          self.assertEqual(mad.recv(), -my_cpx)
+          self.assertEqual(mad.recv(),  my_cpx * 1.31j)
 
 class TestRngs(unittest.TestCase):
 
-    def test_recv(self):
-        with MAD() as mad:
-            mad.send("""
-            irng = 3..11..2
-            rng = MAD.nrange(3.5, 21.4, 12)
-            lrng = MAD.nlogrange(1, 20, 20)
-            py:send(irng)
-            py:send(rng)
-            py:send(lrng)
-            py:send(irng:totable())
-            py:send(rng:totable())
-            py:send(lrng:totable())
-            """)
-            self.assertEqual(mad.recv(), range(3  , 12  , 2)) #MAD is inclusive, python is exclusive (on stop)
-            self.assertTrue (np.allclose(mad.recv(), np.linspace(3.5, 21.4, 12)))
-            self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
-            self.assertEqual(mad.recv(), list(range(3, 12, 2))) #MAD is inclusive, python is exclusive (on stop)
-            self.assertTrue (np.allclose(mad.recv(), np.linspace(3.5, 21.4, 12)))
-            self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
-
-    def test_send(self):
-        with MAD() as mad:
-            mad.send("""
-            irng = py:recv() + 1 
-            rng  = py:recv() + 2
-            lrng = py:recv()
-            py:send(irng:totable())
-            py:send(rng:totable())
-            py:send(lrng:totable())
-            """)
-            mad.send(range(3, 10, 1))
-            mad.send_rng(3.5, 21.4, 14)
-            mad.send_lrng(1, 20, 20)
-            self.assertEqual(mad.recv(), list(range(4, 12, 1)))
-            self.assertTrue (np.allclose(mad.recv(), np.linspace(5.5, 23.4, 14)))
-            self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
+  def test_recv(self):
+    with MAD() as mad:
+      mad.send("""
+      irng = 3..11..2
+      rng = MAD.nrange(3.5, 21.4, 12)
+      lrng = MAD.nlogrange(1, 20, 20)
+      py:send(irng)
+      py:send(rng)
+      py:send(lrng)
+      py:send(irng:totable())
+      py:send(rng:totable())
+      py:send(lrng:totable())
+      """)
+      self.assertEqual(mad.recv(), range(3  , 12  , 2)) #MAD is inclusive, python is exclusive (on stop)
+      self.assertTrue (np.allclose(mad.recv(), np.linspace(3.5, 21.4, 12)))
+      self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
+      self.assertEqual(mad.recv(), list(range(3, 12, 2))) #MAD is inclusive, python is exclusive (on stop)
+      self.assertTrue (np.allclose(mad.recv(), np.linspace(3.5, 21.4, 12)))
+      self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
+
+  def test_send(self):
+    with MAD() as mad:
+      mad.send("""
+      irng = py:recv() + 1 
+      rng  = py:recv() + 2
+      lrng = py:recv()
+      py:send(irng:totable())
+      py:send(rng:totable())
+      py:send(lrng:totable())
+      """)
+      mad.send(range(3, 10, 1))
+      mad.send_rng(3.5, 21.4, 14)
+      mad.send_lrng(1, 20, 20)
+      self.assertEqual(mad.recv(), list(range(4, 12, 1)))
+      self.assertTrue (np.allclose(mad.recv(), np.linspace(5.5, 23.4, 14)))
+      self.assertTrue (np.allclose(mad.recv(), np.geomspace(1, 20, 20)))
 
 class TestBool(unittest.TestCase):
-    
-    def test_send_recv(self):
-        with MAD() as mad:
-            mad.send("""
-            bool1 = py:recv()
-            bool2 = py:recv()
-            py:send(not bool1)
-            py:send(not bool2)
-            """)
-            mad.send(True )
-            mad.send(False)
-            self.assertEqual(mad.recv(), False)
-            self.assertEqual(mad.recv(), True)
+  
+  def test_send_recv(self):
+    with MAD() as mad:
+      mad.send("""
+      bool1 = py:recv()
+      bool2 = py:recv()
+      py:send(not bool1)
+      py:send(not bool2)
+      """)
+      mad.send(True )
+      mad.send(False)
+      self.assertEqual(mad.recv(), False)
+      self.assertEqual(mad.recv(), True)
 
 class TestMono(unittest.TestCase):
 
-    def test_recv(self):
-        with MAD() as mad:
-            mad.send("""
-            local m = MAD.monomial({1, 2, 3, 4, 6, 20, 100})
-            py:send(m)
-            local m = MAD.monomial("WZ346oy")
-            py:send(m)
-            """)
-            
-            self.assertTrue(np.all(mad.recv() == [1, 2, 3, 4, 6, 20, 100]))
-            self.assertTrue(np.all(mad.recv() == [32, 35, 3, 4, 6, 50, 60]))
-    
-    def test_send_recv(self):
-        with MAD() as mad:
-            mad.send("""
-            local m1 = py:recv()
-            local m2 = py:recv()
-            py:send(m1 + m2)
-            """)
-            pym1 = np.random.randint(0, 255, 20, dtype=np.ubyte)
-            pym2 = np.random.randint(0, 255, 20, dtype=np.ubyte)
-            mad.send(pym1)
-            mad.send(pym2)
-            mad_res = mad.recv()
-            self.assertTrue(np.all(mad_res == pym1+pym2))
-            #Check the return is a monomial
-            self.assertEqual(mad_res.dtype, np.dtype("ubyte"))
+  def test_recv(self):
+    with MAD() as mad:
+      mad.send("""
+      local m = MAD.monomial({1, 2, 3, 4, 6, 20, 100})
+      py:send(m)
+      local m = MAD.monomial("WZ346oy")
+      py:send(m)
+      """)
+      
+      self.assertTrue(np.all(mad.recv() == [1, 2, 3, 4, 6, 20, 100]))
+      self.assertTrue(np.all(mad.recv() == [32, 35, 3, 4, 6, 50, 60]))
+  
+  def test_send_recv(self):
+    with MAD() as mad:
+      mad.send("""
+      local m1 = py:recv()
+      local m2 = py:recv()
+      py:send(m1 + m2)
+      """)
+      pym1 = np.random.randint(0, 255, 20, dtype=np.ubyte)
+      pym2 = np.random.randint(0, 255, 20, dtype=np.ubyte)
+      mad.send(pym1)
+      mad.send(pym2)
+      mad_res = mad.recv()
+      self.assertTrue(np.all(mad_res == pym1+pym2))
+      #Check the return is a monomial
+      self.assertEqual(mad_res.dtype, np.dtype("ubyte"))
 
 class TestTPSA(unittest.TestCase):
 
-    def test_recv_real(self):
-        with MAD() as mad:
-            mad.send("""
-            local d = MAD.gtpsad(3, 6)
-            res = MAD.tpsa(6):set(1,2):set(2, 1)
-            res2 = res:copy():set(3, 1)
-            res3 = res2:copy():set(4, 1)
-            py:send(res:axypbzpc(res2, res3, 1, 2, 3))
-            """)
-            monomials, coefficients = mad.recv()
-            self.assertTrue(np.all(monomials[0] == [0, 0, 0]))
-            self.assertTrue(np.all(monomials[1] == [1, 0, 0]))
-            self.assertTrue(np.all(monomials[2] == [0, 1, 0]))
-            self.assertTrue(np.all(monomials[3] == [0, 0, 1]))
-            self.assertTrue(np.all(monomials[4] == [2, 0, 0]))
-            self.assertTrue(np.all(monomials[5] == [1, 1, 0]))
-            self.assertTrue(np.all(coefficients == [11, 6, 4, 2, 1, 1]))
-
-    def test_recv_cpx(self):
-        with MAD() as mad:
-            mad.send("""
-            local d = MAD.gtpsad(3, 6)
-            res = MAD.ctpsa(6):set(1,2+1i):set(2, 1+2i)
-            res2 = res:copy():set(3, 1+2i)
-            res3 = res2:copy():set(4, 1+2i)
-            py:send(res:axypbzpc(res2, res3, 1, 2, 3))
-            """)
-            monomials, coefficients = mad.recv()
-            self.assertTrue(np.all(monomials[0] == [0, 0, 0]))
-            self.assertTrue(np.all(monomials[1] == [1, 0, 0]))
-            self.assertTrue(np.all(monomials[2] == [0, 1, 0]))
-            self.assertTrue(np.all(monomials[3] == [0, 0, 1]))
-            self.assertTrue(np.all(monomials[4] == [2, 0, 0]))
-            self.assertTrue(np.all(monomials[5] == [1, 1, 0]))
-            self.assertTrue(np.all(coefficients == [10+6j, 2+14j, 2+9j, 2+4j, -3+4j, -3+4j]))
-    
-    def test_send_tpsa(self):
-        with MAD() as mad:
-            mad.send("""
-            local tab = py:recv()
-            py:send(tab)
-            """)
-            monos = np.asarray([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1], [2, 0, 0], [1, 1, 0]], dtype=np.uint8)
-            coefficients = [11, 6, 4, 2, 1, 1]
-            mad.send_tpsa(monos, coefficients)
-            self.assertTrue(mad.recv("tab"), ["000", "100", "010", "001", "200", "110"].extend(coefficients)) #intentional?
-    
-    def test_send_ctpsa(self):
-        with MAD() as mad:
-            mad.send("""
-            local tab = py:recv()
-            py:send(tab)
-            """)
-            monos = np.asarray([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1], [2, 0, 0], [1, 1, 0]], dtype=np.uint8)
-            coefficients = [10+6j, 2+14j, 2+9j, 2+4j, -3+4j, -3+4j]
-            mad.send_ctpsa(monos, coefficients)
-            self.assertTrue(mad.recv("tab"), ["000", "100", "010", "001", "200", "110"].extend(coefficients)) #intentional?
-
-    def test_send_recv_damap(self):
-        with MAD() as mad:
-            mad.send("""
-            local sin in MAD.gmath
-            MAD.gtpsad(6, 5)
-            local M = MAD.damap {xy = 5}
-            M.x  = 1 ; M.y  = 2 ; M.t  = 3
-            M.px = 2 ; M.py = 1 ; M.pt = 1
-            res = sin(M.x) * sin(M.y)
-            py:send(res)
-            recved = MAD.tpsa():fromtable(py:recv())
-            py:send(recved)
-            """)
-            init = mad.recv()
-            mad.send_tpsa(*init)
-            final = mad.recv()
-            self.assertTrue((init[0] == final[0]).all())
-            self.assertTrue((init[1] == final[1]).all())
+  def test_recv_real(self):
+    with MAD() as mad:
+      mad.send("""
+      local d = MAD.gtpsad(3, 6)
+      res = MAD.tpsa(6):set(1,2):set(2, 1)
+      res2 = res:copy():set(3, 1)
+      res3 = res2:copy():set(4, 1)
+      py:send(res:axypbzpc(res2, res3, 1, 2, 3))
+      """)
+      monomials, coefficients = mad.recv()
+      self.assertTrue(np.all(monomials[0] == [0, 0, 0]))
+      self.assertTrue(np.all(monomials[1] == [1, 0, 0]))
+      self.assertTrue(np.all(monomials[2] == [0, 1, 0]))
+      self.assertTrue(np.all(monomials[3] == [0, 0, 1]))
+      self.assertTrue(np.all(monomials[4] == [2, 0, 0]))
+      self.assertTrue(np.all(monomials[5] == [1, 1, 0]))
+      self.assertTrue(np.all(coefficients == [11, 6, 4, 2, 1, 1]))
+
+  def test_recv_cpx(self):
+    with MAD() as mad:
+      mad.send("""
+      local d = MAD.gtpsad(3, 6)
+      res = MAD.ctpsa(6):set(1,2+1i):set(2, 1+2i)
+      res2 = res:copy():set(3, 1+2i)
+      res3 = res2:copy():set(4, 1+2i)
+      py:send(res:axypbzpc(res2, res3, 1, 2, 3))
+      """)
+      monomials, coefficients = mad.recv()
+      self.assertTrue(np.all(monomials[0] == [0, 0, 0]))
+      self.assertTrue(np.all(monomials[1] == [1, 0, 0]))
+      self.assertTrue(np.all(monomials[2] == [0, 1, 0]))
+      self.assertTrue(np.all(monomials[3] == [0, 0, 1]))
+      self.assertTrue(np.all(monomials[4] == [2, 0, 0]))
+      self.assertTrue(np.all(monomials[5] == [1, 1, 0]))
+      self.assertTrue(np.all(coefficients == [10+6j, 2+14j, 2+9j, 2+4j, -3+4j, -3+4j]))
+  
+  def test_send_tpsa(self):
+    with MAD() as mad:
+      mad.send("""
+      local tab = py:recv()
+      py:send(tab)
+      """)
+      monos = np.asarray([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1], [2, 0, 0], [1, 1, 0]], dtype=np.uint8)
+      coefficients = [11, 6, 4, 2, 1, 1]
+      mad.send_tpsa(monos, coefficients)
+      self.assertTrue(mad.recv("tab"), ["000", "100", "010", "001", "200", "110"].extend(coefficients)) #intentional?
+  
+  def test_send_ctpsa(self):
+    with MAD() as mad:
+      mad.send("""
+      local tab = py:recv()
+      py:send(tab)
+      """)
+      monos = np.asarray([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1], [2, 0, 0], [1, 1, 0]], dtype=np.uint8)
+      coefficients = [10+6j, 2+14j, 2+9j, 2+4j, -3+4j, -3+4j]
+      mad.send_ctpsa(monos, coefficients)
+      self.assertTrue(mad.recv("tab"), ["000", "100", "010", "001", "200", "110"].extend(coefficients)) #intentional?
+
+  def test_send_recv_damap(self):
+    with MAD() as mad:
+      mad.send("""
+      local sin in MAD.gmath
+      MAD.gtpsad(6, 5)
+      local M = MAD.damap {xy = 5}
+      M.x  = 1 ; M.y  = 2 ; M.t  = 3
+      M.px = 2 ; M.py = 1 ; M.pt = 1
+      res = sin(M.x) * sin(M.y)
+      py:send(res)
+      recved = MAD.tpsa():fromtable(py:recv())
+      py:send(recved)
+      """)
+      init = mad.recv()
+      mad.send_tpsa(*init)
+      final = mad.recv()
+      self.assertTrue((init[0] == final[0]).all())
+      self.assertTrue((init[1] == final[1]).all())
 
 class TestLoad(unittest.TestCase):
+  a = np.arange(1, 21).reshape(4, 5)
+  b = np.arange(1, 7 ).reshape(2, 3)
+  c = (np.arange(1, 16) + 1j).reshape(5, 3)
+
+  def test_load(self):
+    with MAD() as mad:
+      mad.load("MAD", "matrix")
+      self.assertTrue(mad.send("py:send(matrix == MAD.matrix)").recv())
+
+      mad.load("MAD.gmath")
+      self.assertTrue(mad.send("py:send(sin == MAD.gmath.sin)").recv())
+      self.assertTrue(mad.send("py:send(cos == MAD.gmath.cos)").recv())
+      self.assertTrue(mad.send("py:send(tan == MAD.gmath.tan)").recv())
+      
+      mad.load("MAD.element", "quadrupole", "sextupole", "drift")
+      self.assertTrue(mad.send("py:send(quadrupole == MAD.element.quadrupole)").recv())
+      self.assertTrue(mad.send("py:send(sextupole  == MAD.element.sextupole )").recv())
+      self.assertTrue(mad.send("py:send(drift      == MAD.element.drift     )").recv())
+
+  def test_run_file(self):
+    with open("test.mad", "w") as f:
+      f.write("""
+      local matrix, cmatrix in MAD
+      a = matrix(4, 5):seq()
+      b = cmatrix(2, 3):seq()
+      """)
+    with MAD() as mad:
+      mad.loadfile("test.mad")
+      self.assertIsNone(mad.matrix)
+      self.assertTrue(np.all(mad.a == self.a))
+      self.assertTrue(np.all(mad.b == self.b))
+    os.remove("test.mad")
+
+  def test_load_file(self):
+    with open("test.mad", "w") as f:
+      f.write("""
+      local matrix, cmatrix in MAD
+      local a = matrix(4, 5):seq()
+      local c = cmatrix(5, 3):seq() + 1i
+      return {res1 = a * c, res2 = a * c:conj()}
+      """)
+    with MAD() as mad:
+      mad.loadfile("test", "res1", "res2")
+      self.assertTrue(np.all(mad.res1 == np.matmul(self.a, self.c)))
+      self.assertTrue(np.all(mad.res2 == np.matmul(self.a, self.c.conj())))
+    os.remove("test.mad")
 
-    def test_load(self):
-        with MAD() as mad:
-            mad.load("MAD", "matrix")
-            self.assertEqual(mad.matrix, mad.MAD.matrix)
-
-            mad.load("MAD.gmath")
-            self.assertEqual(mad.sin, mad.MAD.gmath.sin)
-            self.assertEqual(mad.cos, mad.MAD.gmath.cos)
-            self.assertEqual(mad.tan, mad.MAD.gmath.tan)
-
-            mad.load("MAD.element", "quadrupole", "sextupole", "drift")
-            self.assertEqual(mad.quadrupole, mad.MAD.element.quadrupole)
-            self.assertEqual(mad.sextupole, mad.MAD.element.sextupole)
-            self.assertEqual(mad.drift, mad.MAD.element.drift)
-
-    def test_run_file(self):
-        with open("test.mad", "w") as f:
-            f.write("""
-            local matrix, cmatrix in MAD
-            a = matrix(4, 5):seq()
-            b = cmatrix(2, 3):seq()
-            """)
-        with MAD() as mad:
-            mad.loadfile("test.mad")
-            self.assertIsNone(mad.matrix)
-            self.assertTrue(np.all(mad.a == mad.MAD.matrix(4, 5).seq() .eval()))
-            self.assertTrue(np.all(mad.b == mad.MAD.cmatrix(2, 3).seq().eval()))
-        os.remove("test.mad")
-
-    def test_load_file(self):
-        with open("test.mad", "w") as f:
-            f.write("""
-            local matrix, cmatrix in MAD
-            local a = matrix(4, 5):seq()
-            local b = cmatrix(5, 3):seq()
-            return {res1 = a * b, res2 = a * b:conj()}
-            """)
-        with MAD() as mad:
-            mad.loadfile("test", "res1", "res2")
-            a = mad.MAD.matrix(4, 5).seq().eval()
-            b = mad.MAD.cmatrix(5, 3).seq().eval()
-            self.assertTrue(np.all(mad.res1 == np.matmul(a, b)))
-            self.assertTrue(np.all(mad.res2 == np.matmul(a, b.conj())))
-        os.remove("test.mad")
-
-        
+    
 class TestOutput(unittest.TestCase):
 
-    def test_print(self):
-        with MAD() as mad:
-            mad.send("print('hello world')")
-            mad.send("py:send('hello world')")
-            self.assertEqual(mad.recv(), "hello world") # Check printing does not affect pipe
+  def test_print(self):
+    with MAD() as mad:
+      mad.send("print('hello world')")
+      mad.send("py:send('hello world')")
+      self.assertEqual(mad.recv(), "hello world") # Check printing does not affect pipe
 
 if __name__ == '__main__':
-    unittest.main()
+  unittest.main()
```

