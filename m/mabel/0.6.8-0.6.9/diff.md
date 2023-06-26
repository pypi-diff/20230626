# Comparing `tmp/mabel-0.6.8.tar.gz` & `tmp/mabel-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mabel-0.6.8.tar", last modified: Thu Oct 27 18:48:50 2022, max compression
+gzip compressed data, was "mabel-0.6.9.tar", last modified: Thu Oct 27 19:07:13 2022, max compression
```

## Comparing `mabel-0.6.8.tar` & `mabel-0.6.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.667100 mabel-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-10-27 18:48:40.000000 mabel-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-27 18:48:40.000000 mabel-0.6.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     7245 2022-10-27 18:48:50.667100 mabel-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-10-27 18:48:40.000000 mabel-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.651099 mabel-0.6.8/mabel/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/adapters/disk/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/disk/disk_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/disk/disk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/adapters/google/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/google/bigquery_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/google/google_cloud_storage_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/google/google_cloud_storage_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/adapters/minio/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/minio/minio_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/minio/minio_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/adapters/null/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/null/null_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/adapters/null/null_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel/data/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.659099 mabel-0.6.8/mabel/data/internals/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/collected_set.py
--rw-r--r--   0 runner    (1001) docker     (121)  1049358 2022-10-27 18:48:49.000000 mabel-0.6.8/mabel/data/internals/dictset.c
--rw-r--r--   0 runner    (1001) docker     (121)    18488 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/dictset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/dnf_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/dumb_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)   580271 2022-10-27 18:48:49.000000 mabel-0.6.8/mabel/data/internals/expression.c
--rw-r--r--   0 runner    (1001) docker     (121)    10375 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)   566920 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel/data/internals/group_by.c
--rw-r--r--   0 runner    (1001) docker     (121)     8937 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/group_by.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/records.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.659099 mabel-0.6.8/mabel/data/internals/storage_classes/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/storage_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/storage_classes/base_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_compressed_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_disk.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/internals/xmler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.663099 mabel-0.6.8/mabel/data/readers/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.663099 mabel-0.6.8/mabel/data/readers/internals/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10946 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/base_inner_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/decompressors.py
--rw-r--r--   0 runner    (1001) docker     (121)   569824 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel/data/readers/internals/inline_evaluator.c
--rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/inline_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/inline_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/multiprocess_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)   561381 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel/data/readers/internals/parallel_reader.c
--rw-r--r--   0 runner    (1001) docker     (121)    10547 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/parallel_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12797 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/internals/threaded_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    14129 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/readers/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.663099 mabel-0.6.8/mabel/data/validator/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/validator/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.663099 mabel-0.6.8/mabel/data/writers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4954 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/batch_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.663099 mabel-0.6.8/mabel/data/writers/internals/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/internals/base_inner_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/internals/blob_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/internals/writer_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8244 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/stream_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/data/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.667100 mabel-0.6.8/mabel/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/errors/render_error_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.667100 mabel-0.6.8/mabel/logging/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/add_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/create_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/google_cloud_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/levels.py
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/logging/log_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.667100 mabel-0.6.8/mabel/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/parameter_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/resource_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9153 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/utils/token_labeler.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-27 18:48:40.000000 mabel-0.6.8/mabel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 18:48:50.655099 mabel-0.6.8/mabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7245 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 18:48:50.000000 mabel-0.6.8/mabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 18:48:50.667100 mabel-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-27 18:48:40.000000 mabel-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.597045 mabel-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-10-27 19:07:04.000000 mabel-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-27 19:07:04.000000 mabel-0.6.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     7245 2022-10-27 19:07:13.597045 mabel-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-10-27 19:07:04.000000 mabel-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.581044 mabel-0.6.9/mabel/
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/adapters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/adapters/disk/
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/disk/disk_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/disk/disk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/adapters/google/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/google/bigquery_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/google/google_cloud_storage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/google/google_cloud_storage_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/adapters/minio/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/minio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/minio/minio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/minio/minio_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/adapters/null/
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/null/null_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/adapters/null/null_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.589044 mabel-0.6.9/mabel/data/internals/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/collected_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1049358 2022-10-27 19:07:12.000000 mabel-0.6.9/mabel/data/internals/dictset.c
+-rw-r--r--   0 runner    (1001) docker     (121)    18488 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/dictset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/dnf_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/dumb_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)   580271 2022-10-27 19:07:12.000000 mabel-0.6.9/mabel/data/internals/expression.c
+-rw-r--r--   0 runner    (1001) docker     (121)    10375 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)   566920 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel/data/internals/group_by.c
+-rw-r--r--   0 runner    (1001) docker     (121)     8937 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/group_by.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/records.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.589044 mabel-0.6.9/mabel/data/internals/storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/storage_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/storage_classes/base_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_compressed_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_disk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/internals/xmler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.589044 mabel-0.6.9/mabel/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/data/readers/internals/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10946 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/base_inner_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/decompressors.py
+-rw-r--r--   0 runner    (1001) docker     (121)   569824 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel/data/readers/internals/inline_evaluator.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/inline_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/inline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/multiprocess_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)   561381 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel/data/readers/internals/parallel_reader.c
+-rw-r--r--   0 runner    (1001) docker     (121)    10547 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/parallel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12797 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/internals/threaded_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14129 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/readers/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/data/validator/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/validator/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/data/writers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4954 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/batch_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/data/writers/internals/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/internals/base_inner_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/internals/blob_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/internals/writer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8244 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/stream_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/data/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/errors/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/errors/render_error_stack.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.593044 mabel-0.6.9/mabel/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/add_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/create_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/google_cloud_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/levels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/logging/log_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.597045 mabel-0.6.9/mabel/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/parameter_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/resource_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9153 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/utils/token_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-27 19:07:05.000000 mabel-0.6.9/mabel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:07:13.585044 mabel-0.6.9/mabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7245 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 19:07:13.000000 mabel-0.6.9/mabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 19:07:13.597045 mabel-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-27 19:07:05.000000 mabel-0.6.9/setup.py
```

### Comparing `mabel-0.6.8/LICENSE` & `mabel-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/PKG-INFO` & `mabel-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mabel
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python Data Libraries
 Home-page: https://github.com/mabel-dev/mabel/
 Author: joocer
 Author-email: justin.joyce@joocer.com
 Maintainer: Joocer
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mabel-0.6.8/README.md` & `mabel-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/__init__.py` & `mabel-0.6.9/mabel/__init__.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/disk/disk_reader.py` & `mabel-0.6.9/mabel/adapters/disk/disk_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/disk/disk_writer.py` & `mabel-0.6.9/mabel/adapters/disk/disk_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/google/bigquery_writer.py` & `mabel-0.6.9/mabel/adapters/google/bigquery_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/google/google_cloud_storage_reader.py` & `mabel-0.6.9/mabel/adapters/google/google_cloud_storage_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/google/google_cloud_storage_writer.py` & `mabel-0.6.9/mabel/adapters/google/google_cloud_storage_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/minio/minio_reader.py` & `mabel-0.6.9/mabel/adapters/minio/minio_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/minio/minio_writer.py` & `mabel-0.6.9/mabel/adapters/minio/minio_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/null/null_reader.py` & `mabel-0.6.9/mabel/adapters/null/null_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/adapters/null/null_writer.py` & `mabel-0.6.9/mabel/adapters/null/null_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/collected_set.py` & `mabel-0.6.9/mabel/data/internals/collected_set.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/dictset.c` & `mabel-0.6.9/mabel/data/internals/dictset.c`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/dictset.py` & `mabel-0.6.9/mabel/data/internals/dictset.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/display.py` & `mabel-0.6.9/mabel/data/internals/display.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/dnf_filters.py` & `mabel-0.6.9/mabel/data/internals/dnf_filters.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/expression.c` & `mabel-0.6.9/mabel/data/internals/expression.c`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/expression.py` & `mabel-0.6.9/mabel/data/internals/expression.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/group_by.c` & `mabel-0.6.9/mabel/data/internals/group_by.c`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/group_by.py` & `mabel-0.6.9/mabel/data/internals/group_by.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/histogram.py` & `mabel-0.6.9/mabel/data/internals/histogram.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/index.py` & `mabel-0.6.9/mabel/data/internals/index.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/records.py` & `mabel-0.6.9/mabel/data/internals/records.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/storage_classes/base_storage_class.py` & `mabel-0.6.9/mabel/data/internals/storage_classes/base_storage_class.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_compressed_memory.py` & `mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_compressed_memory.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_disk.py` & `mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_disk.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/storage_classes/storage_class_memory.py` & `mabel-0.6.9/mabel/data/internals/storage_classes/storage_class_memory.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/internals/xmler.py` & `mabel-0.6.9/mabel/data/internals/xmler.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/base_inner_reader.py` & `mabel-0.6.9/mabel/data/readers/internals/base_inner_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/cursor.py` & `mabel-0.6.9/mabel/data/readers/internals/cursor.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/decompressors.py` & `mabel-0.6.9/mabel/data/readers/internals/decompressors.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/inline_evaluator.c` & `mabel-0.6.9/mabel/data/readers/internals/inline_evaluator.c`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/inline_evaluator.py` & `mabel-0.6.9/mabel/data/readers/internals/inline_evaluator.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/inline_functions.py` & `mabel-0.6.9/mabel/data/readers/internals/inline_functions.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/multiprocess_wrapper.py` & `mabel-0.6.9/mabel/data/readers/internals/multiprocess_wrapper.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/parallel_reader.c` & `mabel-0.6.9/mabel/data/readers/internals/parallel_reader.c`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/parallel_reader.py` & `mabel-0.6.9/mabel/data/readers/internals/parallel_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/sql_reader.py` & `mabel-0.6.9/mabel/data/readers/internals/sql_reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/internals/threaded_wrapper.py` & `mabel-0.6.9/mabel/data/readers/internals/threaded_wrapper.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/readers/reader.py` & `mabel-0.6.9/mabel/data/readers/reader.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/validator/schema.py` & `mabel-0.6.9/mabel/data/validator/schema.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/batch_writer.py` & `mabel-0.6.9/mabel/data/writers/batch_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/internals/base_inner_writer.py` & `mabel-0.6.9/mabel/data/writers/internals/base_inner_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/internals/blob_writer.py` & `mabel-0.6.9/mabel/data/writers/internals/blob_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/internals/writer_pool.py` & `mabel-0.6.9/mabel/data/writers/internals/writer_pool.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/stream_writer.py` & `mabel-0.6.9/mabel/data/writers/stream_writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/data/writers/writer.py` & `mabel-0.6.9/mabel/data/writers/writer.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/errors/__init__.py` & `mabel-0.6.9/mabel/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/errors/render_error_stack.py` & `mabel-0.6.9/mabel/errors/render_error_stack.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/logging/add_level.py` & `mabel-0.6.9/mabel/logging/add_level.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/logging/create_logger.py` & `mabel-0.6.9/mabel/logging/create_logger.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/logging/google_cloud_logger.py` & `mabel-0.6.9/mabel/logging/google_cloud_logger.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/logging/levels.py` & `mabel-0.6.9/mabel/logging/levels.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/logging/log_formatter.py` & `mabel-0.6.9/mabel/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/colors.py` & `mabel-0.6.9/mabel/utils/colors.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/common.py` & `mabel-0.6.9/mabel/utils/common.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/dates.py` & `mabel-0.6.9/mabel/utils/dates.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/entropy.py` & `mabel-0.6.9/mabel/utils/entropy.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/monkey_patch.py` & `mabel-0.6.9/mabel/utils/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/parameter_validator.py` & `mabel-0.6.9/mabel/utils/parameter_validator.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/paths.py` & `mabel-0.6.9/mabel/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/resource_monitoring.py` & `mabel-0.6.9/mabel/utils/resource_monitoring.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/text.py` & `mabel-0.6.9/mabel/utils/text.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel/utils/token_labeler.py` & `mabel-0.6.9/mabel/utils/token_labeler.py`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/mabel.egg-info/PKG-INFO` & `mabel-0.6.9/mabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mabel
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python Data Libraries
 Home-page: https://github.com/mabel-dev/mabel/
 Author: joocer
 Author-email: justin.joyce@joocer.com
 Maintainer: Joocer
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mabel-0.6.8/mabel.egg-info/SOURCES.txt` & `mabel-0.6.9/mabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mabel-0.6.8/setup.py` & `mabel-0.6.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 with open("mabel/version.py", "r") as v:
     vers = v.read()
 exec(vers)  # nosec
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
-with open("requirements.txt") as f:
-    required = f.read().splitlines()
-
+try:
+    with open("requirements.txt", "r") as f:
+        required = f.read().splitlines()
+except:
+    with open("mabel.egg-info/requires.txt", "r") as f:
+        required = f.read().splitlines()
 
 ext_modules = cythonize(
     [
         "mabel/data/internals/group_by.py",
         "mabel/data/internals/dictset.py",
         "mabel/data/internals/expression.py",
         "mabel/data/readers/internals/inline_evaluator.py",
```

