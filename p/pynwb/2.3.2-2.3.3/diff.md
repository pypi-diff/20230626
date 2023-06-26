# Comparing `tmp/pynwb-2.3.2.tar.gz` & `tmp/pynwb-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynwb-2.3.2.tar", last modified: Wed Apr 12 01:17:22 2023, max compression
+gzip compressed data, was "pynwb-2.3.3.tar", last modified: Mon Jun 26 21:00:02 2023, max compression
```

## Comparing `pynwb-2.3.2.tar` & `pynwb-2.3.3.tar`

### file list

```diff
@@ -1,183 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 01:13:20.000000 pynwb-2.3.2/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 01:13:20.000000 pynwb-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-12 01:17:22.613450 pynwb-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-12 01:13:20.000000 pynwb-2.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 01:13:20.000000 pynwb-2.3.2/environment-ros3.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-12 01:13:20.000000 pynwb-2.3.2/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-min.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-12 01:17:22.613450 pynwb-2.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2352 2023-04-12 01:13:20.000000 pynwb-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.569450 pynwb-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/src/pynwb/
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/_due.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 01:17:22.613450 pynwb-2.3.2/src/pynwb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    57672 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/io/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/legacy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.569450 pynwb-2.3.2/src/pynwb/nwb-schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.585450 pynwb-2.3.2/src/pynwb/nwb-schema/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.behavior.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.icephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ogen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ophys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.585450 pynwb-2.3.2/src/pynwb/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/icephys_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/make_test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.589450 pynwb-2.3.2/src/pynwb/testing/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/testh5io.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.577450 pynwb-2.3.2/src/pynwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:13:42.000000 pynwb-2.3.2/src/pynwb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-04-12 01:13:20.000000 pynwb-2.3.2/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.589450 pynwb-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/back_compat/
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.2.0_subject_no_age__reference.nwb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/test_import_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/coverage/
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/coverage/runCoverage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_modular_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_nwbfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_scratch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/ros3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/ros3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/ros3/test_ros3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/utils/test_io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_core_NWBContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_epoch_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_icephys_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/validation/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-12 01:13:20.000000 pynwb-2.3.2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-04-12 01:13:20.000000 pynwb-2.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 20:55:48.000000 pynwb-2.3.3/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 20:55:48.000000 pynwb-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 21:00:02.447686 pynwb-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-26 20:55:48.000000 pynwb-2.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 20:55:49.000000 pynwb-2.3.3/environment-ros3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-26 20:55:49.000000 pynwb-2.3.3/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 21:00:02.451686 pynwb-2.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-06-26 20:55:49.000000 pynwb-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.387685 pynwb-2.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.451686 pynwb-2.3.3/src/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/_due.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 21:00:02.451686 pynwb-2.3.3/src/pynwb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57672 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.407686 pynwb-2.3.3/src/pynwb/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.407686 pynwb-2.3.3/src/pynwb/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.411686 pynwb-2.3.3/src/pynwb/legacy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.387685 pynwb-2.3.3/src/pynwb/nwb-schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.415686 pynwb-2.3.3/src/pynwb/nwb-schema/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.behavior.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.icephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ogen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ophys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.419686 pynwb-2.3.3/src/pynwb/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/icephys_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/make_test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.423686 pynwb-2.3.3/src/pynwb/testing/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/testh5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.403685 pynwb-2.3.3/src/pynwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:56:09.000000 pynwb-2.3.3/src/pynwb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-06-26 20:55:49.000000 pynwb-2.3.3/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.423686 pynwb-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.431686 pynwb-2.3.3/tests/back_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.2.0_subject_no_age__reference.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/test_import_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.435686 pynwb-2.3.3/tests/coverage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/coverage/runCoverage
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.435686 pynwb-2.3.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_modular_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26419 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_nwbfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/ros3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/ros3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/ros3/test_ros3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/utils/test_io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/read_dandi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/read_dandi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/read_dandi/test_read_dandi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_core_NWBContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_epoch_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_icephys_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/validation/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-26 20:55:49.000000 pynwb-2.3.3/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-06-26 20:55:49.000000 pynwb-2.3.3/versioneer.py
```

### Comparing `pynwb-2.3.2/Legal.txt` & `pynwb-2.3.3/Legal.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/PKG-INFO` & `pynwb-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.2
+Version: 2.3.3
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
@@ -76,18 +77,14 @@
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml
 
-.. image:: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements.svg?branch=dev
-     :target: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements/?branch=dev
-     :alt: Requirements Status
-
 .. image:: https://readthedocs.org/projects/pynwb/badge/?version=latest
      :target: https://pynwb.readthedocs.io/en/latest/?badge=latest
      :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/l/pynwb.svg
      :target: https://github.com/neurodatawithoutborders/pynwb/blob/dev/license.txt
      :alt: PyPI - License
```

### Comparing `pynwb-2.3.2/README.rst` & `pynwb-2.3.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,14 @@
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml
 
-.. image:: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements.svg?branch=dev
-     :target: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements/?branch=dev
-     :alt: Requirements Status
-
 .. image:: https://readthedocs.org/projects/pynwb/badge/?version=latest
      :target: https://pynwb.readthedocs.io/en/latest/?badge=latest
      :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/l/pynwb.svg
      :target: https://github.com/neurodatawithoutborders/pynwb/blob/dev/license.txt
      :alt: PyPI - License
```

### Comparing `pynwb-2.3.2/license.txt` & `pynwb-2.3.3/license.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/requirements-dev.txt` & `pynwb-2.3.3/requirements-dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # pinned dependencies to reproduce an entire development environment to use PyNWB, run PyNWB tests, check code style,
 # compute coverage, and create test environments. note that depending on the version of python installed, different
 # versions of requirements may be installed due to package incompatibilities.
 #
 black==23.3.0
-codecov==2.1.12
 codespell==2.2.4
 coverage==7.2.2
 flake8==6.0.0; python_version >= "3.8"
 flake8==5.0.4; python_version < "3.8"
 flake8-debugger==4.1.2
 flake8-print==5.0.0
 isort==5.12.0; python_version >= "3.8"
```

### Comparing `pynwb-2.3.2/requirements-doc.txt` & `pynwb-2.3.3/requirements-doc.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 # allensdk>=2.13.2  # allensdk reinstalls pynwb and hdmf. TODO set up a separate workflow to test allensdk
 # MarkupSafe==2.0.1  # resolve incompatibility between jinja2 and markupsafe: https://github.com/AllenInstitute/AllenSDK/issues/2308
 Pillow
 sphinx-copybutton
 dataframe_image   # used to render large dataframe as image in the sphinx gallery to improve html display
 lxml  # used by dataframe_image when using the matplotlib backend
 hdf5plugin
+importlib-metadata<4.3; python_version < "3.8"  # TODO: remove when minimum python version is 3.8
+
```

### Comparing `pynwb-2.3.2/setup.cfg` & `pynwb-2.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/setup.py` & `pynwb-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     'python_requires': '>=3.7',
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
```

### Comparing `pynwb-2.3.2/src/pynwb/__init__.py` & `pynwb-2.3.3/src/pynwb/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/_due.py` & `pynwb-2.3.3/src/pynwb/_due.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/base.py` & `pynwb-2.3.3/src/pynwb/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/behavior.py` & `pynwb-2.3.3/src/pynwb/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/core.py` & `pynwb-2.3.3/src/pynwb/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/device.py` & `pynwb-2.3.3/src/pynwb/device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/ecephys.py` & `pynwb-2.3.3/src/pynwb/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/epoch.py` & `pynwb-2.3.3/src/pynwb/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/file.py` & `pynwb-2.3.3/src/pynwb/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/icephys.py` & `pynwb-2.3.3/src/pynwb/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/image.py` & `pynwb-2.3.3/src/pynwb/image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/base.py` & `pynwb-2.3.3/src/pynwb/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/core.py` & `pynwb-2.3.3/src/pynwb/io/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/epoch.py` & `pynwb-2.3.3/src/pynwb/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/file.py` & `pynwb-2.3.3/src/pynwb/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/icephys.py` & `pynwb-2.3.3/src/pynwb/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/misc.py` & `pynwb-2.3.3/src/pynwb/io/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/ophys.py` & `pynwb-2.3.3/src/pynwb/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/io/utils.py` & `pynwb-2.3.3/src/pynwb/io/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/__init__.py` & `pynwb-2.3.3/src/pynwb/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/base.py` & `pynwb-2.3.3/src/pynwb/legacy/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/behavior.py` & `pynwb-2.3.3/src/pynwb/legacy/io/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/epoch.py` & `pynwb-2.3.3/src/pynwb/legacy/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/file.py` & `pynwb-2.3.3/src/pynwb/legacy/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/icephys.py` & `pynwb-2.3.3/src/pynwb/legacy/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/ogen.py` & `pynwb-2.3.3/src/pynwb/legacy/io/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/io/ophys.py` & `pynwb-2.3.3/src/pynwb/legacy/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/legacy/map.py` & `pynwb-2.3.3/src/pynwb/legacy/map.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/misc.py` & `pynwb-2.3.3/src/pynwb/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.base.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.base.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.behavior.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.behavior.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ecephys.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ecephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.epoch.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.epoch.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.file.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.file.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.icephys.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.icephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.image.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.image.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.misc.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.misc.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.namespace.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.namespace.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ogen.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ogen.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ophys.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ophys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml` & `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/ogen.py` & `pynwb-2.3.3/src/pynwb/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/ophys.py` & `pynwb-2.3.3/src/pynwb/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/retinotopy.py` & `pynwb-2.3.3/src/pynwb/retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/spec.py` & `pynwb-2.3.3/src/pynwb/spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/icephys_testutils.py` & `pynwb-2.3.3/src/pynwb/testing/icephys_testutils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/make_test_files.py` & `pynwb-2.3.3/src/pynwb/testing/make_test_files.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/__init__.py` & `pynwb-2.3.3/src/pynwb/testing/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/base.py` & `pynwb-2.3.3/src/pynwb/testing/mock/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/behavior.py` & `pynwb-2.3.3/src/pynwb/testing/mock/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/ecephys.py` & `pynwb-2.3.3/src/pynwb/testing/mock/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/file.py` & `pynwb-2.3.3/src/pynwb/testing/mock/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/icephys.py` & `pynwb-2.3.3/src/pynwb/testing/mock/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/ogen.py` & `pynwb-2.3.3/src/pynwb/testing/mock/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/ophys.py` & `pynwb-2.3.3/src/pynwb/testing/mock/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/mock/utils.py` & `pynwb-2.3.3/src/pynwb/testing/mock/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb/testing/testh5io.py` & `pynwb-2.3.3/src/pynwb/testing/testh5io.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         if ws:
             for w in ws:
                 if issubclass(w.category, (MissingRequiredBuildWarning,
                                            BrokenLinkWarning)):
                     raise Exception('%s: %s' % (w.category.__name__, w.message))
                 else:
-                    warnings.warn(w.message, w.category)
+                    warnings.showwarning(w.message, w.category, w.filename, w.lineno, w.file, w.line)
 
         try:
             return self.getContainer(self.read_nwbfile)
         except Exception as e:
             self.reader.close()
             self.reader = None
             raise e
@@ -137,15 +137,15 @@
 
         if ws:
             for w in ws:
                 if issubclass(w.category, (MissingRequiredBuildWarning,
                                            BrokenLinkWarning)):
                     raise Exception('%s: %s' % (w.category.__name__, w.message))
                 else:
-                    warnings.warn(w.message, w.category)
+                    warnings.showwarning(w.message, w.category, w.filename, w.lineno, w.file, w.line)
 
         try:
             return self.getContainer(self.read_exported_nwbfile)
         except Exception as e:
             self.export_reader.close()
             self.export_reader = None
             raise e
```

### Comparing `pynwb-2.3.2/src/pynwb/validate.py` & `pynwb-2.3.3/src/pynwb/validate.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/src/pynwb.egg-info/PKG-INFO` & `pynwb-2.3.3/src/pynwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.2
+Version: 2.3.3
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
@@ -76,18 +77,14 @@
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/run_all_tests.yml
 
 .. image:: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml/badge.svg
     :target: https://github.com/NeurodataWithoutBorders/pynwb/actions/workflows/deploy_release.yml
 
-.. image:: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements.svg?branch=dev
-     :target: https://requires.io/github/NeurodataWithoutBorders/pynwb/requirements/?branch=dev
-     :alt: Requirements Status
-
 .. image:: https://readthedocs.org/projects/pynwb/badge/?version=latest
      :target: https://pynwb.readthedocs.io/en/latest/?badge=latest
      :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/l/pynwb.svg
      :target: https://github.com/neurodatawithoutborders/pynwb/blob/dev/license.txt
      :alt: PyPI - License
```

### Comparing `pynwb-2.3.2/src/pynwb.egg-info/SOURCES.txt` & `pynwb-2.3.3/src/pynwb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
 tests/integration/hdf5/test_ophys.py
 tests/integration/hdf5/test_retinotopy.py
 tests/integration/hdf5/test_scratch.py
 tests/integration/ros3/__init__.py
 tests/integration/ros3/test_ros3.py
 tests/integration/utils/__init__.py
 tests/integration/utils/test_io_utils.py
+tests/read_dandi/__init__.py
+tests/read_dandi/test_read_dandi.py
 tests/unit/__init__.py
 tests/unit/test_base.py
 tests/unit/test_behavior.py
 tests/unit/test_core.py
 tests/unit/test_core_NWBContainer.py
 tests/unit/test_device.py
 tests/unit/test_ecephys.py
```

### Comparing `pynwb-2.3.2/test.py` & `pynwb-2.3.3/test.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.2_nwbfile.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.2_str_experimenter.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.2_str_pub.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.3_nwbfile.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.3_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.3_str_experimenter.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.3_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.0.3_str_pub.nwb` & `pynwb-2.3.3/tests/back_compat/1.0.3_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.0_nwbfile.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.0_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.0_str_experimenter.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.0_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.0_str_pub.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.0_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.2_nwbfile.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.2_str_experimenter.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.1.2_str_pub.nwb` & `pynwb-2.3.3/tests/back_compat/1.1.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_data.nwb` & `pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_unit.nwb` & `pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_data.nwb` & `pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_unit.nwb` & `pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_no_data.nwb` & `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_non_external_format.nwb` & `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_non_external_format.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb` & `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/2.1.0_nwbfile_with_extension.nwb` & `pynwb-2.3.3/tests/back_compat/2.1.0_nwbfile_with_extension.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/2.2.0_subject_no_age__reference.nwb` & `pynwb-2.3.3/tests/back_compat/2.2.0_subject_no_age__reference.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/test_import_structure.py` & `pynwb-2.3.3/tests/back_compat/test_import_structure.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/back_compat/test_read.py` & `pynwb-2.3.3/tests/back_compat/test_read.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_base.py` & `pynwb-2.3.3/tests/integration/hdf5/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_device.py` & `pynwb-2.3.3/tests/integration/hdf5/test_device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_ecephys.py` & `pynwb-2.3.3/tests/integration/hdf5/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_icephys.py` & `pynwb-2.3.3/tests/integration/hdf5/test_icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_image.py` & `pynwb-2.3.3/tests/integration/hdf5/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_io.py` & `pynwb-2.3.3/tests/integration/hdf5/test_io.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_misc.py` & `pynwb-2.3.3/tests/integration/hdf5/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_modular_storage.py` & `pynwb-2.3.3/tests/integration/hdf5/test_modular_storage.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_nwbfile.py` & `pynwb-2.3.3/tests/integration/hdf5/test_nwbfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
                 'stop_time': [0.25, 0.30, 0.40, 0.45],
                 'timeseries': [[(2, 1, tsa)],
                                [(3, 1, tsa)],
                                [(3, 1, tsa)],
                                [(4, 1, tsa)]],
                 'tags': [[''], [''], ['fizz', 'buzz'], ['qaz']]
             },
-            index=pd.Index(np.arange(4), name='id')
+            index=pd.Index(np.arange(4, dtype=np.int64), name='id')
         )
         # pop the timeseries column out because ts_obt has rows of lists of tuples and ts_exp has rows of lists of lists
         ts_obt = df_obt.pop('timeseries')
         ts_exp = df_exp.pop('timeseries')
         pd.testing.assert_frame_equal(df_exp, df_obt, check_like=True, check_dtype=False)
 
         # check the timeseries columns match
@@ -363,15 +363,15 @@
         df_exp = pd.DataFrame({
                 'foo': [1, 2, 3, 4],
                 'bar': ['fish', 'fowl', 'dog', 'cat'],
                 'start_time': [0.2, 0.25, 0.30, 0.35],
                 'stop_time': [0.25, 0.30, 0.40, 0.45],
                 'tags': [[''], [''], ['fizz', 'buzz'], ['qaz']]
             },
-            index=pd.Index(np.arange(4), name='id')
+            index=pd.Index(np.arange(4, dtype=np.int64), name='id')
         )
 
         df_obt = self.read_container.to_dataframe(exclude=set(['timeseries', 'timeseries_index']))
         pd.testing.assert_frame_equal(df_exp, df_obt, check_like=True, check_dtype=False)
 
 
 class TestTrials(NWBH5IOMixin, TestCase):
```

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_ogen.py` & `pynwb-2.3.3/tests/integration/hdf5/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_ophys.py` & `pynwb-2.3.3/tests/integration/hdf5/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_retinotopy.py` & `pynwb-2.3.3/tests/integration/hdf5/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/hdf5/test_scratch.py` & `pynwb-2.3.3/tests/integration/hdf5/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/ros3/test_ros3.py` & `pynwb-2.3.3/tests/integration/ros3/test_ros3.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/integration/utils/test_io_utils.py` & `pynwb-2.3.3/tests/integration/utils/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_base.py` & `pynwb-2.3.3/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_behavior.py` & `pynwb-2.3.3/tests/unit/test_behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_core.py` & `pynwb-2.3.3/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_core_NWBContainer.py` & `pynwb-2.3.3/tests/unit/test_core_NWBContainer.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_ecephys.py` & `pynwb-2.3.3/tests/unit/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_epoch.py` & `pynwb-2.3.3/tests/unit/test_epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_epoch_legacy.py` & `pynwb-2.3.3/tests/unit/test_epoch_legacy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pynwb.epoch import TimeIntervals
 from pynwb.testing import NWBH5IOMixin, TestCase
 from pynwb import NWBFile, NWBHDF5IO
 from pynwb.base import TimeSeries, TimeSeriesReference, TimeSeriesReferenceVectorData
 import numpy as np
-import warnings
 import h5py
 
 
 class TestTimeIntervalsIO(NWBH5IOMixin, TestCase):
     """
     Test that reading NWB files with version 2.4 and earlier function correctly with the TimeIntervals type.
     In NWB 2.5 TimeIntervals.timeseries was updated to use the TimeSeriesReferenceVectorData type and to
@@ -62,45 +61,39 @@
 
     def test_legacy_format(self):
         description = 'a file to test writing and reading a %s' % self.container_type
         identifier = 'TEST_%s' % self.container_type
         nwbfile = NWBFile(description, identifier, self.start_time, file_create_date=self.create_date)
         self.addContainer(nwbfile)
 
-        with warnings.catch_warnings(record=True) as ws:
-            # write the file
-            with NWBHDF5IO(self.filename, mode='w') as write_io:
-                write_io.write(nwbfile, cache_spec=False)
-            # Modify the HDF5 file to look like NWB 2.4 and earlier. This simply means
-            # modifying the neurodata_type on the TimeIntervals.timeseries column
-            with h5py.File(self.filename, mode='a') as infile:
-                infile['/intervals/epochs/timeseries'].attrs['neurodata_type'] = 'VectorData'
-                infile.attrs['nwb_version'] = '2.3.0'
-            # Make sure we didn't have warnings
-            self.assertEqual(len(ws), 0)
+        # write the file
+        with NWBHDF5IO(self.filename, mode='w') as write_io:
+            write_io.write(nwbfile, cache_spec=False)
+        # Modify the HDF5 file to look like NWB 2.4 and earlier. This simply means
+        # modifying the neurodata_type on the TimeIntervals.timeseries column
+        with h5py.File(self.filename, mode='a') as infile:
+            infile['/intervals/epochs/timeseries'].attrs['neurodata_type'] = 'VectorData'
+            infile.attrs['nwb_version'] = '2.3.0'
 
         # Read the file back
-        with warnings.catch_warnings(record=True) as ws:
-            self.reader = NWBHDF5IO(self.filename, mode='r')
-            self.read_nwbfile = self.reader.read()
-
-            # Test that the VectorData column for timeseries has been converted to TimeSeriesReferenceVectorData
-            self.assertIsInstance(self.read_nwbfile.epochs.timeseries, TimeSeriesReferenceVectorData)
-
-            # Test that slicing into epochs.timeseries works as expected
-            re = self.read_nwbfile.epochs.timeseries[0]
-            self.assertIsInstance(re, TimeSeriesReference)
-            self.assertTupleEqual((re[0], re[1], re[2].object_id), (0, 5, nwbfile.get_acquisition('a').object_id))
-
-            # Test that slicing into epochs works as expected
-            re = self.read_nwbfile.epochs[0:1]
-            self.assertListEqual(re.columns.tolist(), ['start_time', 'stop_time', 'temperature', 'tags', 'timeseries'])
-            for i in re.loc[0, 'timeseries']:
-                self.assertIsInstance(i, TimeSeriesReference)
-            self.assertTupleEqual(
-                (re.loc[0, 'timeseries'][0][0], re.loc[0, 'timeseries'][0][1], re.loc[0, 'timeseries'][0][2].object_id),
-                (0, 5, nwbfile.get_acquisition('a').object_id))
-            self.assertTupleEqual(
-                (re.loc[0, 'timeseries'][1][0], re.loc[0, 'timeseries'][1][1], re.loc[0, 'timeseries'][1][2].object_id),
-                (0, 3, nwbfile.get_acquisition('b').object_id))
-            # Make sure we didn't have warnings
-            self.assertEqual(len(ws), 0)
+        self.reader = NWBHDF5IO(self.filename, mode='r')
+        self.read_nwbfile = self.reader.read()
+
+        # Test that the VectorData column for timeseries has been converted to TimeSeriesReferenceVectorData
+        self.assertIsInstance(self.read_nwbfile.epochs.timeseries, TimeSeriesReferenceVectorData)
+
+        # Test that slicing into epochs.timeseries works as expected
+        re = self.read_nwbfile.epochs.timeseries[0]
+        self.assertIsInstance(re, TimeSeriesReference)
+        self.assertTupleEqual((re[0], re[1], re[2].object_id), (0, 5, nwbfile.get_acquisition('a').object_id))
+
+        # Test that slicing into epochs works as expected
+        re = self.read_nwbfile.epochs[0:1]
+        self.assertListEqual(re.columns.tolist(), ['start_time', 'stop_time', 'temperature', 'tags', 'timeseries'])
+        for i in re.loc[0, 'timeseries']:
+            self.assertIsInstance(i, TimeSeriesReference)
+        self.assertTupleEqual(
+            (re.loc[0, 'timeseries'][0][0], re.loc[0, 'timeseries'][0][1], re.loc[0, 'timeseries'][0][2].object_id),
+            (0, 5, nwbfile.get_acquisition('a').object_id))
+        self.assertTupleEqual(
+            (re.loc[0, 'timeseries'][1][0], re.loc[0, 'timeseries'][1][1], re.loc[0, 'timeseries'][1][2].object_id),
+            (0, 3, nwbfile.get_acquisition('b').object_id))
```

### Comparing `pynwb-2.3.2/tests/unit/test_extension.py` & `pynwb-2.3.3/tests/unit/test_extension.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_file.py` & `pynwb-2.3.3/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_icephys.py` & `pynwb-2.3.3/tests/unit/test_icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_icephys_metadata_tables.py` & `pynwb-2.3.3/tests/unit/test_icephys_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_image.py` & `pynwb-2.3.3/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_misc.py` & `pynwb-2.3.3/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_mock.py` & `pynwb-2.3.3/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_ogen.py` & `pynwb-2.3.3/tests/unit/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_ophys.py` & `pynwb-2.3.3/tests/unit/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_retinotopy.py` & `pynwb-2.3.3/tests/unit/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_scratch.py` & `pynwb-2.3.3/tests/unit/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/unit/test_spec.py` & `pynwb-2.3.3/tests/unit/test_spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tests/validation/test_validate.py` & `pynwb-2.3.3/tests/validation/test_validate.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.2/tox.ini` & `pynwb-2.3.3/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py37, py38, py39, py310
+envlist = py37, py38, py39, py310, py311
 requires = pip >= 22.0
 
 [testenv]
 download = True
 usedevelop = True
 setenv =
   PYTHONDONTWRITEBYTECODE = 1
@@ -22,42 +22,42 @@
 commands =
     python -m pip check  # Check for conflicting packages
     python -m pip list
     python test.py -v
 
 # Env to create coverage report locally
 [testenv:localcoverage]
-basepython = python3.10
+basepython = python3.11
 commands =
     python -m coverage run test.py --pynwb
     coverage html -d tests/coverage/htmlcov
 
-# Test with python 3.10; pinned dev and optional reqs
-[testenv:py310-optional]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs
+[testenv:py311-optional]
+basepython = python3.11
 install_command =
     python -m pip install {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.10; pinned dev and optional reqs; upgraded run reqs
-[testenv:py310-upgraded]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs; upgraded run reqs
+[testenv:py311-upgraded]
+basepython = python3.11
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.10; pinned dev and optional reqs; upgraded, pre-release run reqs
-[testenv:py310-prerelease]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs; upgraded, pre-release run reqs
+[testenv:py311-prerelease]
+basepython = python3.11
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv]commands}
 
@@ -87,32 +87,36 @@
 basepython = python3.9
 commands = {[testenv:build]commands}
 
 [testenv:build-py310]
 basepython = python3.10
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-optional]
-basepython = python3.10
+[testenv:build-py311]
+basepython = python3.11
+commands = {[testenv:build]commands}
+
+[testenv:build-py311-optional]
+basepython = python3.11
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-upgraded]
-basepython = python3.10
+[testenv:build-py311-upgraded]
+basepython = python3.11
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-prerelease]
-basepython = python3.10
+[testenv:build-py311-prerelease]
+basepython = python3.11
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
@@ -158,29 +162,34 @@
 commands = {[testenv:gallery]commands}
 
 [testenv:gallery-py310]
 basepython = python3.10
 deps = {[testenv:gallery]deps}
 commands = {[testenv:gallery]commands}
 
-# Test with python 3.10; pinned dev, doc, and optional reqs; upgraded run reqs
-[testenv:gallery-py310-upgraded]
-basepython = python3.10
+[testenv:gallery-py311]
+basepython = python3.11
+deps = {[testenv:gallery]deps}
+commands = {[testenv:gallery]commands}
+
+# Test with python 3.11; pinned dev, doc, and optional reqs; upgraded run reqs
+[testenv:gallery-py311-upgraded]
+basepython = python3.11
 deps =
     -rrequirements-dev.txt
 commands =
     python -m pip install -U -e .
     python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
     python -m pip check
     python -m pip list
     python test.py --example
 
-# Test with python 3.10; pinned dev, doc, and optional reqs; pre-release run reqs
-[testenv:gallery-py310-prerelease]
-basepython = python3.10
+# Test with python 3.11; pinned dev, doc, and optional reqs; pre-release run reqs
+[testenv:gallery-py311-prerelease]
+basepython = python3.11
 deps =
     -rrequirements-dev.txt
 commands =
     python -m pip install -U --pre -e .
     python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
     python -m pip check
     python -m pip list
```

### Comparing `pynwb-2.3.2/versioneer.py` & `pynwb-2.3.3/versioneer.py`

 * *Files identical despite different names*

