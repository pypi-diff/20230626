# Comparing `tmp/vcorelib-2.0.2.tar.gz` & `tmp/vcorelib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-2.0.2.tar", last modified: Mon Jun 26 01:12:11 2023, max compression
+gzip compressed data, was "vcorelib-2.1.0.tar", last modified: Mon Jun 26 08:16:01 2023, max compression
```

## Comparing `vcorelib-2.0.2.tar` & `vcorelib-2.1.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.162297 vcorelib-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 01:10:48.000000 vcorelib-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 01:12:11.162297 vcorelib-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-26 01:10:48.000000 vcorelib-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 01:10:48.000000 vcorelib-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:12:11.162297 vcorelib-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-26 01:10:48.000000 vcorelib-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.150297 vcorelib-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 01:10:48.000000 vcorelib-2.0.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 01:10:48.000000 vcorelib-2.0.2/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 01:10:48.000000 vcorelib-2.0.2/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.150297 vcorelib-2.0.2/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.150297 vcorelib-2.0.2/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.150297 vcorelib-2.0.2/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/math/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.154297 vcorelib-2.0.2/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.158297 vcorelib-2.0.2/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.158297 vcorelib-2.0.2/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.158297 vcorelib-2.0.2/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.162297 vcorelib-2.0.2/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.162297 vcorelib-2.0.2/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.162297 vcorelib-2.0.2/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 01:10:48.000000 vcorelib-2.0.2/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:12:11.150297 vcorelib-2.0.2/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 01:12:11.000000 vcorelib-2.0.2/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 01:12:11.000000 vcorelib-2.0.2/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:12:11.000000 vcorelib-2.0.2/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 01:12:11.000000 vcorelib-2.0.2/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 01:12:11.000000 vcorelib-2.0.2/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 08:14:39.000000 vcorelib-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 08:16:01.765561 vcorelib-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-26 08:14:39.000000 vcorelib-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 08:14:39.000000 vcorelib-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:16:01.765561 vcorelib-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-26 08:14:39.000000 vcorelib-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.757561 vcorelib-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 08:14:39.000000 vcorelib-2.1.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 08:14:39.000000 vcorelib-2.1.0/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 08:14:39.000000 vcorelib-2.1.0/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.757561 vcorelib-2.1.0/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.757561 vcorelib-2.1.0/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.757561 vcorelib-2.1.0/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.761561 vcorelib-2.1.0/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.765561 vcorelib-2.1.0/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 08:14:39.000000 vcorelib-2.1.0/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:16:01.757561 vcorelib-2.1.0/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 08:16:01.000000 vcorelib-2.1.0/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 08:16:01.000000 vcorelib-2.1.0/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:16:01.000000 vcorelib-2.1.0/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 08:16:01.000000 vcorelib-2.1.0/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 08:16:01.000000 vcorelib-2.1.0/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-2.0.2/LICENSE` & `vcorelib-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/PKG-INFO` & `vcorelib-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.0.2
+Version: 2.1.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b221710c0d25d3fedb34c758a54958e5
+    hash=1cdc07131261518d6adc3cc3b858a4e5
     =====================================
 -->
 
-# vcorelib ([2.0.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.1.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.0.2/README.md` & `vcorelib-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b221710c0d25d3fedb34c758a54958e5
+    hash=1cdc07131261518d6adc3cc3b858a4e5
     =====================================
 -->
 
-# vcorelib ([2.0.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.1.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.0.2/pyproject.toml` & `vcorelib-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "2.0.2"
+version = "2.1.0"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-2.0.2/setup.py` & `vcorelib-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/tests/test_logging.py` & `vcorelib-2.1.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/tests/test_names.py` & `vcorelib-2.1.0/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/tests/test_namespace.py` & `vcorelib-2.1.0/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/args/__init__.py` & `vcorelib-2.1.0/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/args/newline.py` & `vcorelib-2.1.0/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/asyncio/__init__.py` & `vcorelib-2.1.0/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/asyncio/cli.py` & `vcorelib-2.1.0/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/asyncio/subprocess.py` & `vcorelib-2.1.0/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/dict/__init__.py` & `vcorelib-2.1.0/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/dict/cache.py` & `vcorelib-2.1.0/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/dict/codec.py` & `vcorelib-2.1.0/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/dict/config.py` & `vcorelib-2.1.0/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/dict/env.py` & `vcorelib-2.1.0/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/graph/__init__.py` & `vcorelib-2.1.0/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/graph/abc.py` & `vcorelib-2.1.0/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/graph/edge.py` & `vcorelib-2.1.0/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/graph/node.py` & `vcorelib-2.1.0/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/graph/port.py` & `vcorelib-2.1.0/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/__init__.py` & `vcorelib-2.1.0/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/abc.py` & `vcorelib-2.1.0/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/arbiter/base.py` & `vcorelib-2.1.0/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/arbiter/context.py` & `vcorelib-2.1.0/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/arbiter/directory.py` & `vcorelib-2.1.0/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/archive/__init__.py` & `vcorelib-2.1.0/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/cache.py` & `vcorelib-2.1.0/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/decode.py` & `vcorelib-2.1.0/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/encode.py` & `vcorelib-2.1.0/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/mapping.py` & `vcorelib-2.1.0/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/io/types.py` & `vcorelib-2.1.0/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/logging.py` & `vcorelib-2.1.0/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/math/__init__.py` & `vcorelib-2.1.0/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/math/analysis/average.py` & `vcorelib-2.1.0/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-2.1.0/vcorelib/math/analysis/rate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """A class for managing rate information for some data channel."""
 
     def __init__(self, **kwargs) -> None:
         """Initialize this rate tracker."""
 
         self.average = _MovingAverage(**kwargs)
         self.prev_time_ns: int = 0
+        self.accumulated: float = 0.0
 
     @property
     def value(self) -> float:
         """An accessor for the underlying value."""
         return self.average.value
 
     @property
@@ -45,32 +46,31 @@
     def __call__(self, time_ns: int = None, value: float = 1.0) -> float:
         """
         Submit new data to the rate tracker. If this function is called with
         default arguments, the returned value will reflect the rate that this
         method is being called in hertz.
         """
 
-        result = 0.0
-
         # Use a default time if one wasn't provided.
         if time_ns is None:
             time_ns = _default_time_ns()
 
-        # Only start tracking when a second data point is encountered.
-        if self.prev_time_ns != 0:
-            assert time_ns > self.prev_time_ns
+        self.accumulated += value
 
+        # Only start tracking when a second data point is encountered.
+        if self.prev_time_ns != 0 and time_ns > self.prev_time_ns:
             # Consider 'value' as the amount of change since the last data
             # entry, so divide value by the change in time to get a rate.
-            result = self.with_dt(
-                ns_to_s(time_ns - self.prev_time_ns), value=value
+            self.with_dt(
+                ns_to_s(time_ns - self.prev_time_ns), value=self.accumulated
             )
+            self.accumulated = 0
 
         self.prev_time_ns = time_ns
-        return result
+        return self.average.value
 
     def with_dt(self, delta_s: float, value: float = 1.0) -> float:
         """Update this rate by directly providing the delta-time value."""
         return self.average(value / delta_s)
 
     @contextmanager
     def measure(
```

### Comparing `vcorelib-2.0.2/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-2.1.0/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/math/time.py` & `vcorelib-2.1.0/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/math/unit.py` & `vcorelib-2.1.0/vcorelib/math/unit.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/names.py` & `vcorelib-2.1.0/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/namespace.py` & `vcorelib-2.1.0/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/paths/__init__.py` & `vcorelib-2.1.0/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/paths/context.py` & `vcorelib-2.1.0/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/paths/info.py` & `vcorelib-2.1.0/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/paths/info_cache.py` & `vcorelib-2.1.0/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/platform/__init__.py` & `vcorelib-2.1.0/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/schemas/__init__.py` & `vcorelib-2.1.0/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/schemas/base.py` & `vcorelib-2.1.0/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/schemas/json.py` & `vcorelib-2.1.0/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/schemas/mixins.py` & `vcorelib-2.1.0/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/script/__init__.py` & `vcorelib-2.1.0/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/target/__init__.py` & `vcorelib-2.1.0/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/target/evaluation.py` & `vcorelib-2.1.0/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/target/expression.py` & `vcorelib-2.1.0/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/target/resolver.py` & `vcorelib-2.1.0/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/task/__init__.py` & `vcorelib-2.1.0/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/task/dict/melder.py` & `vcorelib-2.1.0/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/task/manager.py` & `vcorelib-2.1.0/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/task/subprocess/run.py` & `vcorelib-2.1.0/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib/task/time/sleep.py` & `vcorelib-2.1.0/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.2/vcorelib.egg-info/PKG-INFO` & `vcorelib-2.1.0/vcorelib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.0.2
+Version: 2.1.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b221710c0d25d3fedb34c758a54958e5
+    hash=1cdc07131261518d6adc3cc3b858a4e5
     =====================================
 -->
 
-# vcorelib ([2.0.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.1.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.0.2/vcorelib.egg-info/SOURCES.txt` & `vcorelib-2.1.0/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

