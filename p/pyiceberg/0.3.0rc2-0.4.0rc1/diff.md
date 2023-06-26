# Comparing `tmp/pyiceberg-0.3.0rc2.tar.gz` & `tmp/pyiceberg-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiceberg-0.3.0rc2.tar", max compression
+gzip compressed data, was "pyiceberg-0.4.0rc1.tar", max compression
```

## Comparing `pyiceberg-0.3.0rc2.tar` & `pyiceberg-0.4.0rc1.tar`

### file list

```diff
@@ -1,111 +1,121 @@
--rw-r--r--   0        0        0    12548 2022-12-02 14:33:08.931249 pyiceberg-0.3.0rc2/LICENSE
--rw-r--r--   0        0        0     1614 2023-02-01 22:37:13.095491 pyiceberg-0.3.0rc2/Makefile
--rw-r--r--   0        0        0      251 2022-12-02 14:33:08.931589 pyiceberg-0.3.0rc2/NOTICE
--rw-r--r--   0        0        0     1218 2023-02-01 22:37:13.096041 pyiceberg-0.3.0rc2/README.md
--rw-r--r--   0        0        0       20 2023-02-01 22:37:13.096146 pyiceberg-0.3.0rc2/dev/.rat-excludes
--rwxr-xr-x   0        0        0     2529 2023-02-01 22:37:13.096268 pyiceberg-0.3.0rc2/dev/check-license
--rw-r--r--   0        0        0     1020 2023-02-01 22:37:13.096367 pyiceberg-0.3.0rc2/dev/docker-compose-azurite.yml
--rw-r--r--   0        0        0     1601 2023-01-31 17:44:44.361556 pyiceberg-0.3.0rc2/dev/docker-compose.yml
--rwxr-xr-x   0        0        0     1198 2023-02-01 22:37:13.096463 pyiceberg-0.3.0rc2/dev/run-azurite.sh
--rwxr-xr-x   0        0        0     1194 2023-02-01 22:37:13.096634 pyiceberg-0.3.0rc2/dev/run-minio.sh
--rw-r--r--   0        0        0      808 2023-02-01 22:37:13.099663 pyiceberg-0.3.0rc2/pyiceberg/__init__.py
--rw-r--r--   0        0        0      785 2022-11-24 08:06:13.045505 pyiceberg-0.3.0rc2/pyiceberg/avro/__init__.py
--rw-r--r--   0        0        0     1684 2022-12-22 10:04:24.888689 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/__init__.py
--rw-r--r--   0        0        0     1621 2022-11-24 08:06:13.045660 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/bzip2.py
--rw-r--r--   0        0        0     1131 2022-11-24 08:06:13.045739 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/codec.py
--rw-r--r--   0        0        0     1416 2022-11-24 08:06:13.045844 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/deflate.py
--rw-r--r--   0        0        0     2701 2022-11-24 08:06:13.045901 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/snappy_codec.py
--rw-r--r--   0        0        0     2075 2022-11-24 08:06:13.045960 pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/zstandard_codec.py
--rw-r--r--   0        0        0     6534 2023-02-01 22:37:13.099847 pyiceberg-0.3.0rc2/pyiceberg/avro/decoder.py
--rw-r--r--   0        0        0     6375 2023-02-01 22:37:13.100032 pyiceberg-0.3.0rc2/pyiceberg/avro/file.py
--rw-r--r--   0        0        0    10964 2023-02-01 22:37:13.100212 pyiceberg-0.3.0rc2/pyiceberg/avro/reader.py
--rw-r--r--   0        0        0    10218 2023-02-01 22:37:13.100900 pyiceberg-0.3.0rc2/pyiceberg/avro/resolver.py
--rw-r--r--   0        0        0    14440 2023-02-01 22:37:13.101088 pyiceberg-0.3.0rc2/pyiceberg/catalog/__init__.py
--rw-r--r--   0        0        0    23940 2023-01-03 15:06:48.507752 pyiceberg-0.3.0rc2/pyiceberg/catalog/glue.py
--rw-r--r--   0        0        0    21820 2023-02-01 22:37:13.101268 pyiceberg-0.3.0rc2/pyiceberg/catalog/hive.py
--rw-r--r--   0        0        0    19762 2023-02-01 22:37:13.101497 pyiceberg-0.3.0rc2/pyiceberg/catalog/rest.py
--rw-r--r--   0        0        0      785 2022-11-24 08:06:42.281296 pyiceberg-0.3.0rc2/pyiceberg/cli/__init__.py
--rw-r--r--   0        0        0    12024 2023-02-01 22:37:13.101656 pyiceberg-0.3.0rc2/pyiceberg/cli/console.py
--rw-r--r--   0        0        0     7351 2023-02-01 22:37:13.102089 pyiceberg-0.3.0rc2/pyiceberg/cli/output.py
--rw-r--r--   0        0        0     9720 2023-02-02 14:30:44.640440 pyiceberg-0.3.0rc2/pyiceberg/conversions.py
--rw-r--r--   0        0        0     2720 2023-02-01 22:37:13.102565 pyiceberg-0.3.0rc2/pyiceberg/exceptions.py
--rw-r--r--   0        0        0    24124 2023-02-01 22:37:13.102788 pyiceberg-0.3.0rc2/pyiceberg/expressions/__init__.py
--rw-r--r--   0        0        0    19887 2023-02-02 14:30:44.640797 pyiceberg-0.3.0rc2/pyiceberg/expressions/literals.py
--rw-r--r--   0        0        0     6639 2023-02-01 13:47:59.922080 pyiceberg-0.3.0rc2/pyiceberg/expressions/parser.py
--rw-r--r--   0        0        0    32868 2023-02-02 22:41:59.575094 pyiceberg-0.3.0rc2/pyiceberg/expressions/visitors.py
--rw-r--r--   0        0        0     1190 2022-12-22 10:04:24.892892 pyiceberg-0.3.0rc2/pyiceberg/files.py
--rw-r--r--   0        0        0    10518 2023-02-01 22:37:13.103592 pyiceberg-0.3.0rc2/pyiceberg/io/__init__.py
--rw-r--r--   0        0        0     9998 2023-02-01 22:37:13.103798 pyiceberg-0.3.0rc2/pyiceberg/io/fsspec.py
--rw-r--r--   0        0        0     2408 2023-02-01 22:37:13.103912 pyiceberg-0.3.0rc2/pyiceberg/io/memory.py
--rw-r--r--   0        0        0    26769 2023-02-02 22:41:59.575543 pyiceberg-0.3.0rc2/pyiceberg/io/pyarrow.py
--rw-r--r--   0        0        0    10114 2023-02-01 22:37:13.104506 pyiceberg-0.3.0rc2/pyiceberg/manifest.py
--rw-r--r--   0        0        0     7786 2023-02-01 22:37:13.104956 pyiceberg-0.3.0rc2/pyiceberg/partitioning.py
--rw-r--r--   0        0        0    51485 2023-02-02 22:41:59.576281 pyiceberg-0.3.0rc2/pyiceberg/schema.py
--rw-r--r--   0        0        0     2928 2023-01-03 19:09:33.345644 pyiceberg-0.3.0rc2/pyiceberg/serializers.py
--rw-r--r--   0        0        0    13055 2023-02-02 14:30:44.641780 pyiceberg-0.3.0rc2/pyiceberg/table/__init__.py
--rw-r--r--   0        0        0    16649 2023-02-01 22:37:13.106742 pyiceberg-0.3.0rc2/pyiceberg/table/metadata.py
--rw-r--r--   0        0        0     1499 2023-02-01 22:37:13.106879 pyiceberg-0.3.0rc2/pyiceberg/table/refs.py
--rw-r--r--   0        0        0     5073 2023-02-01 22:37:13.107028 pyiceberg-0.3.0rc2/pyiceberg/table/snapshots.py
--rw-r--r--   0        0        0     5994 2023-02-01 22:37:13.107183 pyiceberg-0.3.0rc2/pyiceberg/table/sorting.py
--rw-r--r--   0        0        0    27156 2023-02-01 22:37:13.107605 pyiceberg-0.3.0rc2/pyiceberg/transforms.py
--rw-r--r--   0        0        0     5678 2023-02-01 22:37:13.107789 pyiceberg-0.3.0rc2/pyiceberg/typedef.py
--rw-r--r--   0        0        0    18061 2023-02-01 22:37:13.107976 pyiceberg-0.3.0rc2/pyiceberg/types.py
--rw-r--r--   0        0        0      785 2022-11-24 08:06:13.053196 pyiceberg-0.3.0rc2/pyiceberg/utils/__init__.py
--rw-r--r--   0        0        0     3098 2022-12-22 10:04:24.896890 pyiceberg-0.3.0rc2/pyiceberg/utils/bin_packing.py
--rw-r--r--   0        0        0     5821 2023-02-01 22:37:13.108124 pyiceberg-0.3.0rc2/pyiceberg/utils/config.py
--rw-r--r--   0        0        0     6386 2023-02-01 22:37:13.108238 pyiceberg-0.3.0rc2/pyiceberg/utils/datetime.py
--rw-r--r--   0        0        0     3084 2022-11-24 08:06:13.054083 pyiceberg-0.3.0rc2/pyiceberg/utils/decimal.py
--rw-r--r--   0        0        0     1860 2023-02-01 22:37:13.108342 pyiceberg-0.3.0rc2/pyiceberg/utils/deprecated.py
--rw-r--r--   0        0        0     1349 2022-12-22 10:04:24.897947 pyiceberg-0.3.0rc2/pyiceberg/utils/parsing.py
--rw-r--r--   0        0        0    17400 2023-02-01 22:37:13.108476 pyiceberg-0.3.0rc2/pyiceberg/utils/schema_conversion.py
--rw-r--r--   0        0        0     2139 2023-02-01 22:37:13.108712 pyiceberg-0.3.0rc2/pyiceberg/utils/singleton.py
--rw-r--r--   0        0        0     5848 2023-02-02 23:52:08.676392 pyiceberg-0.3.0rc2/pyproject.toml
--rw-r--r--   0        0        0     6551 2023-02-01 22:37:13.109172 pyiceberg-0.3.0rc2/tests/avro/test_decoder.py
--rw-r--r--   0        0        0     2008 2023-02-01 22:37:13.109300 pyiceberg-0.3.0rc2/tests/avro/test_file.py
--rw-r--r--   0        0        0    15116 2023-02-01 22:37:13.109465 pyiceberg-0.3.0rc2/tests/avro/test_reader.py
--rw-r--r--   0        0        0     8077 2023-02-01 22:37:13.109624 pyiceberg-0.3.0rc2/tests/avro/test_resolver.py
--rw-r--r--   0        0        0    13944 2023-02-01 22:37:13.109765 pyiceberg-0.3.0rc2/tests/catalog/integration_test_glue.py
--rw-r--r--   0        0        0    17683 2023-02-01 22:37:13.109923 pyiceberg-0.3.0rc2/tests/catalog/test_base.py
--rw-r--r--   0        0        0    20407 2023-02-02 23:50:44.890200 pyiceberg-0.3.0rc2/tests/catalog/test_glue.py
--rw-r--r--   0        0        0    26117 2023-02-01 22:37:13.110300 pyiceberg-0.3.0rc2/tests/catalog/test_hive.py
--rw-r--r--   0        0        0    30498 2023-02-01 22:37:13.110497 pyiceberg-0.3.0rc2/tests/catalog/test_rest.py
--rw-r--r--   0        0        0    39857 2023-02-01 22:37:13.110918 pyiceberg-0.3.0rc2/tests/cli/test_console.py
--rw-r--r--   0        0        0      799 2022-12-02 14:33:08.938744 pyiceberg-0.3.0rc2/tests/cli/test_output.py
--rw-r--r--   0        0        0    51997 2023-02-02 23:50:44.890486 pyiceberg-0.3.0rc2/tests/conftest.py
--rw-r--r--   0        0        0     5853 2023-02-01 22:37:13.111363 pyiceberg-0.3.0rc2/tests/expressions/test_evaluator.py
--rw-r--r--   0        0        0    41633 2023-02-01 22:37:13.111596 pyiceberg-0.3.0rc2/tests/expressions/test_expressions.py
--rw-r--r--   0        0        0    24909 2023-02-01 22:37:13.111754 pyiceberg-0.3.0rc2/tests/expressions/test_literals.py
--rw-r--r--   0        0        0     4938 2023-02-01 22:37:13.111866 pyiceberg-0.3.0rc2/tests/expressions/test_parser.py
--rw-r--r--   0        0        0    12446 2023-02-01 22:37:13.111983 pyiceberg-0.3.0rc2/tests/expressions/test_projection.py
--rw-r--r--   0        0        0    56347 2023-02-02 22:41:59.578325 pyiceberg-0.3.0rc2/tests/expressions/test_visitors.py
--rw-r--r--   0        0        0    19528 2023-02-02 23:12:05.222559 pyiceberg-0.3.0rc2/tests/io/test_fsspec.py
--rw-r--r--   0        0        0    11158 2023-02-01 22:37:13.112518 pyiceberg-0.3.0rc2/tests/io/test_io.py
--rw-r--r--   0        0        0    38010 2023-02-01 22:37:13.112738 pyiceberg-0.3.0rc2/tests/io/test_pyarrow.py
--rw-r--r--   0        0        0     8962 2023-02-01 22:37:13.116486 pyiceberg-0.3.0rc2/tests/table/test_init.py
--rw-r--r--   0        0        0    31242 2023-02-01 22:37:13.116658 pyiceberg-0.3.0rc2/tests/table/test_metadata.py
--rw-r--r--   0        0        0     5243 2023-02-01 22:37:13.116773 pyiceberg-0.3.0rc2/tests/table/test_partitioning.py
--rw-r--r--   0        0        0     1434 2023-02-01 22:37:13.116917 pyiceberg-0.3.0rc2/tests/table/test_refs.py
--rw-r--r--   0        0        0     4951 2023-02-01 22:37:13.117058 pyiceberg-0.3.0rc2/tests/table/test_snapshots.py
--rw-r--r--   0        0        0     4085 2023-02-01 22:37:13.117154 pyiceberg-0.3.0rc2/tests/table/test_sorting.py
--rw-r--r--   0        0        0    21467 2023-02-01 22:37:13.117301 pyiceberg-0.3.0rc2/tests/test_conversions.py
--rw-r--r--   0        0        0    27064 2023-02-01 22:37:13.117464 pyiceberg-0.3.0rc2/tests/test_schema.py
--rw-r--r--   0        0        0    33382 2023-02-02 23:50:54.853388 pyiceberg-0.3.0rc2/tests/test_transforms.py
--rw-r--r--   0        0        0     2567 2023-02-01 22:37:13.118199 pyiceberg-0.3.0rc2/tests/test_typedef.py
--rw-r--r--   0        0        0    18114 2023-02-01 22:37:13.118362 pyiceberg-0.3.0rc2/tests/test_types.py
--rw-r--r--   0        0        0     1113 2023-02-01 22:37:13.118492 pyiceberg-0.3.0rc2/tests/test_version.py
--rw-r--r--   0        0        0     2727 2023-02-01 22:37:13.118604 pyiceberg-0.3.0rc2/tests/utils/test_bin_packing.py
--rw-r--r--   0        0        0     2181 2023-02-01 22:37:13.118698 pyiceberg-0.3.0rc2/tests/utils/test_config.py
--rw-r--r--   0        0        0     1354 2023-02-01 22:37:13.118796 pyiceberg-0.3.0rc2/tests/utils/test_deprecated.py
--rw-r--r--   0        0        0     7118 2023-02-01 22:37:13.118964 pyiceberg-0.3.0rc2/tests/utils/test_manifest.py
--rw-r--r--   0        0        0    12315 2023-02-01 22:37:13.119073 pyiceberg-0.3.0rc2/tests/utils/test_schema_conversion.py
--rw-r--r--   0        0        0     1334 2023-02-01 22:37:13.119228 pyiceberg-0.3.0rc2/tests/utils/test_singleton.py
--rw-r--r--   0        0        0    74745 2022-12-02 14:33:08.946465 pyiceberg-0.3.0rc2/vendor/fb303/FacebookService.py
--rw-r--r--   0        0        0      853 2022-12-02 14:33:08.946568 pyiceberg-0.3.0rc2/vendor/fb303/__init__.py
--rw-r--r--   0        0        0      943 2022-12-02 14:33:08.946641 pyiceberg-0.3.0rc2/vendor/fb303/constants.py
--rw-r--r--   0        0        0     1549 2022-12-02 14:33:08.946707 pyiceberg-0.3.0rc2/vendor/fb303/ttypes.py
--rw-r--r--   0        0        0  2241478 2022-12-02 14:33:08.949289 pyiceberg-0.3.0rc2/vendor/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0      856 2022-12-02 14:33:08.949446 pyiceberg-0.3.0rc2/vendor/hive_metastore/__init__.py
--rw-r--r--   0        0        0     2401 2022-12-02 14:33:08.949506 pyiceberg-0.3.0rc2/vendor/hive_metastore/constants.py
--rw-r--r--   0        0        0  1354270 2022-12-22 09:59:35.298067 pyiceberg-0.3.0rc2/vendor/hive_metastore/ttypes.py
--rw-r--r--   0        0        0     2997 2023-02-02 23:52:09.374699 pyiceberg-0.3.0rc2/setup.py
--rw-r--r--   0        0        0     2909 2023-02-02 23:52:09.374970 pyiceberg-0.3.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    12548 2022-12-02 14:33:08.931249 pyiceberg-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     2063 2023-06-26 08:00:39.798947 pyiceberg-0.4.0rc1/Makefile
+-rw-r--r--   0        0        0      251 2022-12-02 14:33:08.931589 pyiceberg-0.4.0rc1/NOTICE
+-rw-r--r--   0        0        0     1218 2023-06-22 07:56:06.334404 pyiceberg-0.4.0rc1/README.md
+-rw-r--r--   0        0        0       20 2023-04-26 09:54:47.766320 pyiceberg-0.4.0rc1/dev/.rat-excludes
+-rw-r--r--   0        0        0     2975 2023-06-26 08:00:39.799351 pyiceberg-0.4.0rc1/dev/Dockerfile
+-rwxr-xr-x   0        0        0     2529 2023-04-26 09:54:47.766490 pyiceberg-0.4.0rc1/dev/check-license
+-rw-r--r--   0        0        0     1018 2023-05-11 18:59:33.655015 pyiceberg-0.4.0rc1/dev/docker-compose-azurite.yml
+-rw-r--r--   0        0        0     2569 2023-05-11 18:59:33.655087 pyiceberg-0.4.0rc1/dev/docker-compose-integration.yml
+-rw-r--r--   0        0        0     1626 2023-05-11 18:59:33.655176 pyiceberg-0.4.0rc1/dev/docker-compose.yml
+-rwxr-xr-x   0        0        0      912 2023-06-26 08:00:39.799561 pyiceberg-0.4.0rc1/dev/entrypoint.sh
+-rw-r--r--   0        0        0     5267 2023-06-26 08:00:39.799891 pyiceberg-0.4.0rc1/dev/provision.py
+-rwxr-xr-x   0        0        0     1198 2023-04-26 09:54:47.766904 pyiceberg-0.4.0rc1/dev/run-azurite.sh
+-rwxr-xr-x   0        0        0     1194 2023-04-26 09:54:47.766997 pyiceberg-0.4.0rc1/dev/run-minio.sh
+-rw-r--r--   0        0        0     1526 2023-05-22 23:14:10.622990 pyiceberg-0.4.0rc1/dev/spark-defaults.conf
+-rw-r--r--   0        0        0      808 2023-06-26 08:45:12.059730 pyiceberg-0.4.0rc1/pyiceberg/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-01 21:38:02.315613 pyiceberg-0.4.0rc1/pyiceberg/avro/__init__.py
+-rw-r--r--   0        0        0     1684 2022-12-22 10:04:24.888689 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/__init__.py
+-rw-r--r--   0        0        0     1621 2022-11-24 08:06:13.045660 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/bzip2.py
+-rw-r--r--   0        0        0     1131 2022-11-24 08:06:13.045739 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/codec.py
+-rw-r--r--   0        0        0     1416 2022-11-24 08:06:13.045844 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/deflate.py
+-rw-r--r--   0        0        0     2702 2023-06-26 08:15:00.501668 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/snappy_codec.py
+-rw-r--r--   0        0        0     2075 2022-11-24 08:06:13.045960 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/zstandard_codec.py
+-rw-r--r--   0        0        0     7038 2023-06-26 08:15:00.501810 pyiceberg-0.4.0rc1/pyiceberg/avro/decoder.py
+-rw-r--r--   0        0        0     6853 2023-06-26 08:15:00.501957 pyiceberg-0.4.0rc1/pyiceberg/avro/file.py
+-rw-r--r--   0        0        0    11784 2023-06-26 08:15:00.502120 pyiceberg-0.4.0rc1/pyiceberg/avro/reader.py
+-rw-r--r--   0        0        0    11684 2023-06-26 08:15:00.502294 pyiceberg-0.4.0rc1/pyiceberg/avro/resolver.py
+-rw-r--r--   0        0        0    20398 2023-06-26 08:15:00.502502 pyiceberg-0.4.0rc1/pyiceberg/catalog/__init__.py
+-rw-r--r--   0        0        0    30334 2023-06-26 08:15:00.502710 pyiceberg-0.4.0rc1/pyiceberg/catalog/dynamodb.py
+-rw-r--r--   0        0        0    20916 2023-06-26 08:15:00.502909 pyiceberg-0.4.0rc1/pyiceberg/catalog/glue.py
+-rw-r--r--   0        0        0    20256 2023-06-26 08:15:00.503111 pyiceberg-0.4.0rc1/pyiceberg/catalog/hive.py
+-rw-r--r--   0        0        0     2998 2023-06-26 08:15:00.503214 pyiceberg-0.4.0rc1/pyiceberg/catalog/noop.py
+-rw-r--r--   0        0        0    23422 2023-06-26 08:15:00.503400 pyiceberg-0.4.0rc1/pyiceberg/catalog/rest.py
+-rw-r--r--   0        0        0      785 2022-11-24 08:06:42.281296 pyiceberg-0.4.0rc1/pyiceberg/cli/__init__.py
+-rw-r--r--   0        0        0    12027 2023-06-26 08:15:00.503571 pyiceberg-0.4.0rc1/pyiceberg/cli/console.py
+-rw-r--r--   0        0        0     7378 2023-06-26 08:15:00.503705 pyiceberg-0.4.0rc1/pyiceberg/cli/output.py
+-rw-r--r--   0        0        0     9829 2023-06-26 08:15:00.503849 pyiceberg-0.4.0rc1/pyiceberg/conversions.py
+-rw-r--r--   0        0        0     3085 2023-06-26 08:15:00.503993 pyiceberg-0.4.0rc1/pyiceberg/exceptions.py
+-rw-r--r--   0        0        0    30678 2023-06-26 08:15:00.504186 pyiceberg-0.4.0rc1/pyiceberg/expressions/__init__.py
+-rw-r--r--   0        0        0    21961 2023-06-26 08:15:00.504392 pyiceberg-0.4.0rc1/pyiceberg/expressions/literals.py
+-rw-r--r--   0        0        0     7149 2023-06-26 08:15:00.504557 pyiceberg-0.4.0rc1/pyiceberg/expressions/parser.py
+-rw-r--r--   0        0        0    55299 2023-06-26 08:15:00.504819 pyiceberg-0.4.0rc1/pyiceberg/expressions/visitors.py
+-rw-r--r--   0        0        0     1198 2023-06-26 08:15:00.504963 pyiceberg-0.4.0rc1/pyiceberg/files.py
+-rw-r--r--   0        0        0    11090 2023-06-26 08:15:00.505113 pyiceberg-0.4.0rc1/pyiceberg/io/__init__.py
+-rw-r--r--   0        0        0    10733 2023-06-26 08:15:00.505296 pyiceberg-0.4.0rc1/pyiceberg/io/fsspec.py
+-rw-r--r--   0        0        0     2574 2023-06-26 08:15:00.505452 pyiceberg-0.4.0rc1/pyiceberg/io/memory.py
+-rw-r--r--   0        0        0    40921 2023-06-26 08:15:00.505736 pyiceberg-0.4.0rc1/pyiceberg/io/pyarrow.py
+-rw-r--r--   0        0        0    13521 2023-06-26 08:15:00.505921 pyiceberg-0.4.0rc1/pyiceberg/manifest.py
+-rw-r--r--   0        0        0     7881 2023-06-26 08:15:00.506092 pyiceberg-0.4.0rc1/pyiceberg/partitioning.py
+-rw-r--r--   0        0        0    52797 2023-06-26 08:15:00.506544 pyiceberg-0.4.0rc1/pyiceberg/schema.py
+-rw-r--r--   0        0        0     2940 2023-06-26 08:15:00.506763 pyiceberg-0.4.0rc1/pyiceberg/serializers.py
+-rw-r--r--   0        0        0    28940 2023-06-26 08:15:00.507030 pyiceberg-0.4.0rc1/pyiceberg/table/__init__.py
+-rw-r--r--   0        0        0    16674 2023-06-26 08:15:00.507242 pyiceberg-0.4.0rc1/pyiceberg/table/metadata.py
+-rw-r--r--   0        0        0     1577 2023-06-26 08:15:00.507408 pyiceberg-0.4.0rc1/pyiceberg/table/refs.py
+-rw-r--r--   0        0        0     5347 2023-06-26 08:15:00.507583 pyiceberg-0.4.0rc1/pyiceberg/table/snapshots.py
+-rw-r--r--   0        0        0     6531 2023-06-26 08:15:00.507767 pyiceberg-0.4.0rc1/pyiceberg/table/sorting.py
+-rw-r--r--   0        0        0    28318 2023-06-26 08:15:00.507997 pyiceberg-0.4.0rc1/pyiceberg/transforms.py
+-rw-r--r--   0        0        0     6151 2023-06-26 08:15:00.508184 pyiceberg-0.4.0rc1/pyiceberg/typedef.py
+-rw-r--r--   0        0        0    20264 2023-06-26 08:15:00.508392 pyiceberg-0.4.0rc1/pyiceberg/types.py
+-rw-r--r--   0        0        0      785 2022-11-24 08:06:13.053196 pyiceberg-0.4.0rc1/pyiceberg/utils/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-26 08:15:00.508561 pyiceberg-0.4.0rc1/pyiceberg/utils/bin_packing.py
+-rw-r--r--   0        0        0     6471 2023-06-26 08:15:00.508702 pyiceberg-0.4.0rc1/pyiceberg/utils/config.py
+-rw-r--r--   0        0        0     6405 2023-06-26 08:15:00.509030 pyiceberg-0.4.0rc1/pyiceberg/utils/datetime.py
+-rw-r--r--   0        0        0     3111 2023-06-26 08:15:00.509180 pyiceberg-0.4.0rc1/pyiceberg/utils/decimal.py
+-rw-r--r--   0        0        0     1862 2023-06-26 08:15:00.509307 pyiceberg-0.4.0rc1/pyiceberg/utils/deprecated.py
+-rw-r--r--   0        0        0     1350 2023-06-26 08:15:00.509440 pyiceberg-0.4.0rc1/pyiceberg/utils/parsing.py
+-rw-r--r--   0        0        0    17618 2023-06-26 08:15:00.509619 pyiceberg-0.4.0rc1/pyiceberg/utils/schema_conversion.py
+-rw-r--r--   0        0        0     2140 2023-06-26 08:15:00.509772 pyiceberg-0.4.0rc1/pyiceberg/utils/singleton.py
+-rw-r--r--   0        0        0     6836 2023-06-26 08:48:05.170801 pyiceberg-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6551 2023-04-26 09:54:47.775757 pyiceberg-0.4.0rc1/tests/avro/test_decoder.py
+-rw-r--r--   0        0        0     2008 2023-04-26 09:54:47.775847 pyiceberg-0.4.0rc1/tests/avro/test_file.py
+-rw-r--r--   0        0        0    15116 2023-04-26 09:54:47.775997 pyiceberg-0.4.0rc1/tests/avro/test_reader.py
+-rw-r--r--   0        0        0     8616 2023-06-26 08:00:39.817203 pyiceberg-0.4.0rc1/tests/avro/test_resolver.py
+-rw-r--r--   0        0        0    11592 2023-06-26 08:15:00.510095 pyiceberg-0.4.0rc1/tests/catalog/integration_test_dynamodb.py
+-rw-r--r--   0        0        0    11780 2023-06-26 08:15:00.510242 pyiceberg-0.4.0rc1/tests/catalog/integration_test_glue.py
+-rw-r--r--   0        0        0    18074 2023-06-26 08:15:00.510401 pyiceberg-0.4.0rc1/tests/catalog/test_base.py
+-rw-r--r--   0        0        0    20923 2023-05-01 21:45:18.704369 pyiceberg-0.4.0rc1/tests/catalog/test_dynamodb.py
+-rw-r--r--   0        0        0    20601 2023-06-26 08:15:00.510587 pyiceberg-0.4.0rc1/tests/catalog/test_glue.py
+-rw-r--r--   0        0        0    25678 2023-06-04 13:37:00.195421 pyiceberg-0.4.0rc1/tests/catalog/test_hive.py
+-rw-r--r--   0        0        0    31137 2023-06-26 08:15:00.510936 pyiceberg-0.4.0rc1/tests/catalog/test_rest.py
+-rw-r--r--   0        0        0    42591 2023-06-26 08:15:00.511189 pyiceberg-0.4.0rc1/tests/cli/test_console.py
+-rw-r--r--   0        0        0      799 2022-12-02 14:33:08.938744 pyiceberg-0.4.0rc1/tests/cli/test_output.py
+-rw-r--r--   0        0        0    61479 2023-06-26 08:15:00.511486 pyiceberg-0.4.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0    45204 2023-05-01 21:45:18.705300 pyiceberg-0.4.0rc1/tests/expressions/test_evaluator.py
+-rw-r--r--   0        0        0    43602 2023-06-26 08:15:00.511722 pyiceberg-0.4.0rc1/tests/expressions/test_expressions.py
+-rw-r--r--   0        0        0    25456 2023-05-01 21:45:18.705504 pyiceberg-0.4.0rc1/tests/expressions/test_literals.py
+-rw-r--r--   0        0        0     5188 2023-05-01 21:45:18.705651 pyiceberg-0.4.0rc1/tests/expressions/test_parser.py
+-rw-r--r--   0        0        0    12446 2023-04-26 09:54:47.778813 pyiceberg-0.4.0rc1/tests/expressions/test_projection.py
+-rw-r--r--   0        0        0    64029 2023-06-26 08:00:39.820219 pyiceberg-0.4.0rc1/tests/expressions/test_visitors.py
+-rw-r--r--   0        0        0    19528 2023-04-26 09:54:47.779721 pyiceberg-0.4.0rc1/tests/io/test_fsspec.py
+-rw-r--r--   0        0        0    11456 2023-05-01 21:45:18.706178 pyiceberg-0.4.0rc1/tests/io/test_io.py
+-rw-r--r--   0        0        0    44659 2023-06-26 08:15:00.511993 pyiceberg-0.4.0rc1/tests/io/test_pyarrow.py
+-rw-r--r--   0        0        0    10762 2023-06-26 08:00:39.820673 pyiceberg-0.4.0rc1/tests/io/test_pyarrow_visitor.py
+-rw-r--r--   0        0        0    12694 2023-06-26 08:15:00.512192 pyiceberg-0.4.0rc1/tests/table/test_init.py
+-rw-r--r--   0        0        0    31242 2023-04-26 09:54:47.780462 pyiceberg-0.4.0rc1/tests/table/test_metadata.py
+-rw-r--r--   0        0        0     5243 2023-04-26 09:54:47.780608 pyiceberg-0.4.0rc1/tests/table/test_partitioning.py
+-rw-r--r--   0        0        0     1434 2023-04-26 09:54:47.780721 pyiceberg-0.4.0rc1/tests/table/test_refs.py
+-rw-r--r--   0        0        0     4951 2023-04-26 09:54:47.780871 pyiceberg-0.4.0rc1/tests/table/test_snapshots.py
+-rw-r--r--   0        0        0     4085 2023-04-26 09:54:47.780991 pyiceberg-0.4.0rc1/tests/table/test_sorting.py
+-rw-r--r--   0        0        0    21467 2023-04-26 09:54:47.781149 pyiceberg-0.4.0rc1/tests/test_conversions.py
+-rw-r--r--   0        0        0    10446 2023-06-26 08:15:00.512351 pyiceberg-0.4.0rc1/tests/test_integration.py
+-rw-r--r--   0        0        0    27064 2023-04-26 09:54:47.781399 pyiceberg-0.4.0rc1/tests/test_schema.py
+-rw-r--r--   0        0        0    33953 2023-06-26 08:00:39.822555 pyiceberg-0.4.0rc1/tests/test_transforms.py
+-rw-r--r--   0        0        0     2567 2023-04-26 09:54:47.781682 pyiceberg-0.4.0rc1/tests/test_typedef.py
+-rw-r--r--   0        0        0    18554 2023-06-26 08:15:00.512534 pyiceberg-0.4.0rc1/tests/test_types.py
+-rw-r--r--   0        0        0     1113 2023-04-26 09:54:47.781968 pyiceberg-0.4.0rc1/tests/test_version.py
+-rw-r--r--   0        0        0     2725 2023-06-26 08:00:39.822930 pyiceberg-0.4.0rc1/tests/utils/test_bin_packing.py
+-rw-r--r--   0        0        0     2250 2023-06-26 08:00:39.823033 pyiceberg-0.4.0rc1/tests/utils/test_config.py
+-rw-r--r--   0        0        0     1354 2023-04-26 09:54:47.782246 pyiceberg-0.4.0rc1/tests/utils/test_deprecated.py
+-rw-r--r--   0        0        0     9312 2023-06-26 08:00:39.824675 pyiceberg-0.4.0rc1/tests/utils/test_manifest.py
+-rw-r--r--   0        0        0    12321 2023-06-26 08:00:39.824976 pyiceberg-0.4.0rc1/tests/utils/test_schema_conversion.py
+-rw-r--r--   0        0        0     1334 2023-04-26 09:54:47.782780 pyiceberg-0.4.0rc1/tests/utils/test_singleton.py
+-rw-r--r--   0        0        0    74745 2022-12-02 14:33:08.946465 pyiceberg-0.4.0rc1/vendor/fb303/FacebookService.py
+-rw-r--r--   0        0        0      853 2022-12-02 14:33:08.946568 pyiceberg-0.4.0rc1/vendor/fb303/__init__.py
+-rw-r--r--   0        0        0      943 2022-12-02 14:33:08.946641 pyiceberg-0.4.0rc1/vendor/fb303/constants.py
+-rw-r--r--   0        0        0     1549 2022-12-02 14:33:08.946707 pyiceberg-0.4.0rc1/vendor/fb303/ttypes.py
+-rw-r--r--   0        0        0  2241478 2023-06-06 21:21:16.752393 pyiceberg-0.4.0rc1/vendor/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0      856 2022-12-02 14:33:08.949446 pyiceberg-0.4.0rc1/vendor/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     2401 2022-12-02 14:33:08.949506 pyiceberg-0.4.0rc1/vendor/hive_metastore/constants.py
+-rw-r--r--   0        0        0  1354270 2022-12-22 09:59:35.298067 pyiceberg-0.4.0rc1/vendor/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 pyiceberg-0.4.0rc1/PKG-INFO
```

### Comparing `pyiceberg-0.3.0rc2/LICENSE` & `pyiceberg-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/README.md` & `pyiceberg-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/dev/check-license` & `pyiceberg-0.4.0rc1/dev/check-license`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/dev/docker-compose-azurite.yml` & `pyiceberg-0.4.0rc1/dev/docker-compose-azurite.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 services:
   azurite:
     image: mcr.microsoft.com/azure-storage/azurite
     container_name: azurite
     hostname: azurite
     ports:
       - 10000:10000
-    command: [ "azurite-blob", "--loose", "--blobHost", "0.0.0.0" ]
+    command: ["azurite-blob", "--loose", "--blobHost", "0.0.0.0"]
```

### Comparing `pyiceberg-0.3.0rc2/dev/docker-compose.yml` & `pyiceberg-0.4.0rc1/dev/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 services:
   minio:
     image: minio/minio
     container_name: pyiceberg-minio
     environment:
       - MINIO_ROOT_USER=admin
       - MINIO_ROOT_PASSWORD=password
+      - MINIO_DOMAIN=minio
     ports:
       - 9001:9001
       - 9000:9000
-    command: [ "server", "/data", "--console-address", ":9001" ]
+    command: ["server", "/data", "--console-address", ":9001"]
   mc:
     depends_on:
       - minio
     image: minio/mc
     container_name: pyiceberg-mc
     environment:
       - AWS_ACCESS_KEY_ID=admin
```

### Comparing `pyiceberg-0.3.0rc2/dev/run-azurite.sh` & `pyiceberg-0.4.0rc1/dev/run-azurite.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/dev/run-minio.sh` & `pyiceberg-0.4.0rc1/dev/run-minio.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/bzip2.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/bzip2.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/codec.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/deflate.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/deflate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/snappy_codec.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/snappy_codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 try:
     import snappy
 
     class SnappyCodec(Codec):
         @staticmethod
         def _check_crc32(bytes_: bytes, checksum: bytes) -> None:
-            """Incrementally compute CRC-32 from bytes and compare to a checksum
+            """Incrementally compute CRC-32 from bytes and compare to a checksum.
 
             Args:
               bytes_ (bytes): The bytes to check against `checksum`
               checksum (bytes): Byte representation of a checksum
 
             Raises:
               ValueError: If the computed CRC-32 does not match the checksum
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/codecs/zstandard_codec.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/zstandard_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/decoder.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/decoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,23 +34,19 @@
 
 class BinaryDecoder:
     """Read leaf values."""
 
     _input_stream: InputStream
 
     def __init__(self, input_stream: InputStream) -> None:
-        """
-        reader is a Python object on which we can call read, seek, and tell.
-        """
+        """Reader is a Python object on which we can call read, seek, and tell."""
         self._input_stream = input_stream
 
     def read(self, n: int) -> bytes:
-        """
-        Read n bytes.
-        """
+        """Read n bytes."""
         if n < 0:
             raise ValueError(f"Requested {n} bytes to read, expected positive integer.")
         data: List[bytes] = []
 
         n_remaining = n
         while n_remaining > 0:
             data_read = self._input_stream.read(n_remaining)
@@ -66,111 +62,122 @@
 
         return b"".join(data)
 
     def skip(self, n: int) -> None:
         self._input_stream.seek(n, SEEK_CUR)
 
     def read_boolean(self) -> bool:
-        """
-        a boolean is written as a single byte
+        """Reads a value from the stream as a boolean.
+
+        A boolean is written as a single byte
         whose value is either 0 (false) or 1 (true).
         """
         return ord(self.read(1)) == 1
 
     def read_int(self) -> int:
-        """int/long values are written using variable-length, zigzag coding."""
+        """Reads a value from the stream as an integer.
+
+        int/long values are written using variable-length, zigzag coding.
+        """
         b = ord(self.read(1))
         n = b & 0x7F
         shift = 7
         while (b & 0x80) != 0:
             b = ord(self.read(1))
             n |= (b & 0x7F) << shift
             shift += 7
         datum = (n >> 1) ^ -(n & 1)
         return datum
 
     def read_float(self) -> float:
-        """
+        """Reads a value from the stream as a float.
+
         A float is written as 4 bytes.
         The float is converted into a 32-bit integer using a method equivalent to
         Java's floatToIntBits and then encoded in little-endian format.
         """
         return float(STRUCT_FLOAT.unpack(self.read(4))[0])
 
     def read_double(self) -> float:
-        """
+        """Reads a value from the stream as a double.
+
         A double is written as 8 bytes.
         The double is converted into a 64-bit integer using a method equivalent to
         Java's doubleToLongBits and then encoded in little-endian format.
         """
         return float(STRUCT_DOUBLE.unpack(self.read(8))[0])
 
     def read_decimal_from_bytes(self, precision: int, scale: int) -> decimal.Decimal:
-        """
+        """Reads a value from the stream as a decimal.
+
         Decimal bytes are decoded as signed short, int or long depending on the
         size of bytes.
         """
         size = self.read_int()
         return self.read_decimal_from_fixed(precision, scale, size)
 
     def read_decimal_from_fixed(self, _: int, scale: int, size: int) -> decimal.Decimal:
-        """
+        """Reads a value from the stream as a decimal.
+
         Decimal is encoded as fixed. Fixed instances are encoded using the
         number of bytes declared in the schema.
         """
         data = self.read(size)
         unscaled_datum = int.from_bytes(data, byteorder="big", signed=True)
         return unscaled_to_decimal(unscaled_datum, scale)
 
     def read_bytes(self) -> bytes:
-        """
-        Bytes are encoded as a long followed by that many bytes of data.
-        """
+        """Bytes are encoded as a long followed by that many bytes of data."""
         num_bytes = self.read_int()
         return self.read(num_bytes) if num_bytes > 0 else b""
 
     def read_utf8(self) -> str:
-        """
+        """Reads a utf-8 encoded string from the stream.
+
         A string is encoded as a long followed by
         that many bytes of UTF-8 encoded character data.
         """
         return self.read_bytes().decode("utf-8")
 
     def read_uuid_from_fixed(self) -> UUID:
-        """Reads a UUID as a fixed[16]"""
+        """Reads a UUID as a fixed[16]."""
         return UUID(bytes=self.read(16))
 
     def read_time_millis(self) -> time:
-        """
-        int is decoded as python time object which represents
+        """Reads a milliseconds granularity time from the stream.
+
+        Int is decoded as python time object which represents
         the number of milliseconds after midnight, 00:00:00.000.
         """
         millis = self.read_int()
         return micros_to_time(millis * 1000)
 
     def read_time_micros(self) -> time:
-        """
-        long is decoded as python time object which represents
+        """Reads a microseconds granularity time from the stream.
+
+        Long is decoded as python time object which represents
         the number of microseconds after midnight, 00:00:00.000000.
         """
         return micros_to_time(self.read_int())
 
     def read_timestamp_micros(self) -> datetime:
-        """
-        long is decoded as python datetime object which represents
+        """Reads a microsecond granularity timestamp from the stream.
+
+        Long is decoded as python datetime object which represents
         the number of microseconds from the unix epoch, 1 January 1970.
         """
         return micros_to_timestamp(self.read_int())
 
     def read_timestamptz_micros(self) -> datetime:
-        """
-        long is decoded as python datetime object which represents
+        """Reads a microsecond granularity timestamptz from the stream.
+
+        Long is decoded as python datetime object which represents
         the number of microseconds from the unix epoch, 1 January 1970.
 
-        Adjusted to UTC
+        Adjusted to UTC.
         """
         return micros_to_timestamptz(self.read_int())
 
     def skip_boolean(self) -> None:
         self.skip(1)
 
     def skip_int(self) -> None:
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/file.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # pylint: disable=W0621
-"""
-Avro reader for reading Avro files
-"""
+"""Avro reader for reading Avro files."""
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
+from enum import Enum
 from types import TracebackType
 from typing import (
     Callable,
     Dict,
     Generic,
     Optional,
     Type,
@@ -73,15 +72,15 @@
     meta: Dict[str, str]
     sync: bytes
 
     def compression_codec(self) -> Optional[Type[Codec]]:
         """Get the file's compression codec algorithm from the file's metadata.
 
         In the case of a null codec, we return a None indicating that we
-        don't need to compress/decompress
+        don't need to compress/decompress.
         """
         codec_name = self.meta.get(_CODEC_KEY, "null")
         if codec_name not in KNOWN_CODECS:
             raise ValueError(f"Unsupported codec: {codec_name}")
 
         return KNOWN_CODECS[codec_name]
 
@@ -101,73 +100,78 @@
 class Block(Generic[D]):
     reader: Reader
     block_records: int
     block_decoder: BinaryDecoder
     position: int = 0
 
     def __iter__(self) -> Block[D]:
+        """Returns an iterator for the Block class."""
         return self
 
     def has_next(self) -> bool:
         return self.position < self.block_records
 
     def __next__(self) -> D:
+        """Returns the next item when iterating over the Block class."""
         if self.has_next():
             self.position += 1
             return self.reader.read(self.block_decoder)
         raise StopIteration
 
 
 class AvroFile(Generic[D]):
     input_file: InputFile
     read_schema: Optional[Schema]
     read_types: Dict[int, Callable[..., StructProtocol]]
+    read_enums: Dict[int, Callable[..., Enum]]
     input_stream: InputStream
     header: AvroFileHeader
     schema: Schema
     reader: Reader
 
     decoder: BinaryDecoder
     block: Optional[Block[D]] = None
 
     def __init__(
         self,
         input_file: InputFile,
         read_schema: Optional[Schema] = None,
         read_types: Dict[int, Callable[..., StructProtocol]] = EMPTY_DICT,
+        read_enums: Dict[int, Callable[..., Enum]] = EMPTY_DICT,
     ) -> None:
         self.input_file = input_file
         self.read_schema = read_schema
         self.read_types = read_types
+        self.read_enums = read_enums
 
     def __enter__(self) -> AvroFile[D]:
-        """
-        Opens the file and reads the header and generates
-        a reader tree to start reading the payload
+        """Generates a reader tree for the payload within an avro file.
 
         Returns:
             A generator returning the AvroStructs
         """
         self.input_stream = self.input_file.open(seekable=False)
         self.decoder = BinaryDecoder(self.input_stream)
         self.header = self._read_header()
         self.schema = self.header.get_schema()
         if not self.read_schema:
             self.read_schema = self.schema
 
-        self.reader = resolve(self.schema, self.read_schema, self.read_types)
+        self.reader = resolve(self.schema, self.read_schema, self.read_types, self.read_enums)
 
         return self
 
     def __exit__(
         self, exctype: Optional[Type[BaseException]], excinst: Optional[BaseException], exctb: Optional[TracebackType]
     ) -> None:
+        """Performs cleanup when exiting the scope of a 'with' statement."""
         self.input_stream.close()
 
     def __iter__(self) -> AvroFile[D]:
+        """Returns an iterator for the AvroFile class."""
         return self
 
     def _read_block(self) -> int:
         # If there is already a block, we'll have the sync bytes
         if self.block:
             sync_marker = self.decoder.read(SYNC_SIZE)
             if sync_marker != self.header.sync:
@@ -181,14 +185,15 @@
 
         self.block = Block(
             reader=self.reader, block_records=block_records, block_decoder=BinaryDecoder(MemoryInputStream(block_bytes))
         )
         return block_records
 
     def __next__(self) -> D:
+        """Returns the next item when iterating over the AvroFile class."""
         if self.block and self.block.has_next():
             return next(self.block)
 
         try:
             new_block = self._read_block()
         except EOFError as exc:
             raise StopIteration from exc
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/reader.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """
-Classes for building the Reader tree
+Classes for building the Reader tree.
 
 Constructing a reader tree from the schema makes it easy
 to decouple the reader implementation from the schema.
 
 The reader tree can be changed in such a way that the
-read schema is different, while respecting the read schema
+read schema is different, while respecting the read schema.
 """
 from __future__ import annotations
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from dataclasses import field as dataclassfield
 from datetime import datetime, time
@@ -43,15 +43,15 @@
 from pyiceberg.avro.decoder import BinaryDecoder
 from pyiceberg.typedef import StructProtocol
 from pyiceberg.types import StructType
 from pyiceberg.utils.singleton import Singleton
 
 
 def _skip_map_array(decoder: BinaryDecoder, skip_entry: Callable[[], None]) -> None:
-    """Skips over an array or map
+    """Skips over an array or map.
 
     Both the array and map are encoded similar, and we can re-use
     the logic of skipping in an efficient way.
 
     From the Avro spec:
 
     Maps (and arrays) are encoded as a series of blocks.
@@ -61,18 +61,18 @@
 
     If a block's count is negative, its absolute value is used, and the count is followed immediately by a
     long block size indicating the number of bytes in the block. This block size permits fast skipping
     through data, e.g., when projecting a record to a subset of its fields.
 
     Args:
         decoder:
-            The decoder that reads the types from the underlying data
+            The decoder that reads the types from the underlying data.
         skip_entry:
             Function to skip over the underlying data, element in case of an array, and the
-            key/value in the case of a map
+            key/value in the case of a map.
     """
     block_count = decoder.read_int()
     while block_count != 0:
         if block_count < 0:
             # The length in bytes in encoded, so we can skip over it right away
             block_size = decoder.read_int()
             decoder.skip(block_size)
@@ -88,35 +88,49 @@
         ...
 
     @abstractmethod
     def skip(self, decoder: BinaryDecoder) -> None:
         ...
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Reader class."""
         return f"{self.__class__.__name__}()"
 
 
 class NoneReader(Reader):
     def read(self, _: BinaryDecoder) -> None:
         return None
 
     def skip(self, decoder: BinaryDecoder) -> None:
         return None
 
 
+class DefaultReader(Reader):
+    default_value: Any
+
+    def __init__(self, default_value: Any) -> None:
+        self.default_value = default_value
+
+    def read(self, _: BinaryDecoder) -> Any:
+        return self.default_value
+
+    def skip(self, decoder: BinaryDecoder) -> None:
+        pass
+
+
 class BooleanReader(Reader):
     def read(self, decoder: BinaryDecoder) -> bool:
         return decoder.read_boolean()
 
     def skip(self, decoder: BinaryDecoder) -> None:
         decoder.skip_boolean()
 
 
 class IntegerReader(Reader):
-    """Longs and ints are encoded the same way, and there is no long in Python"""
+    """Longs and ints are encoded the same way, and there is no long in Python."""
 
     def read(self, decoder: BinaryDecoder) -> int:
         return decoder.read_int()
 
     def skip(self, decoder: BinaryDecoder) -> None:
         decoder.skip_int()
 
@@ -192,17 +206,19 @@
     def read(self, decoder: BinaryDecoder) -> bytes:
         return decoder.read(len(self))
 
     def skip(self, decoder: BinaryDecoder) -> None:
         decoder.skip(len(self))
 
     def __len__(self) -> int:
+        """Returns the length of an instance of the FixedReader class."""
         return self._len
 
     def __repr__(self) -> str:
+        """Returns the string representation of the FixedReader class."""
         return f"FixedReader({self._len})"
 
 
 class BinaryReader(Reader):
     def read(self, decoder: BinaryDecoder) -> bytes:
         return decoder.read_bytes()
 
@@ -218,14 +234,15 @@
     def read(self, decoder: BinaryDecoder) -> Decimal:
         return decoder.read_decimal_from_bytes(self.precision, self.scale)
 
     def skip(self, decoder: BinaryDecoder) -> None:
         decoder.skip_bytes()
 
     def __repr__(self) -> str:
+        """Returns the string representation of the DecimalReader class."""
         return f"DecimalReader({self.precision}, {self.scale})"
 
 
 @dataclass(frozen=True)
 class OptionReader(Reader):
     option: Reader = dataclassfield()
 
@@ -272,37 +289,40 @@
                 struct = self.create_struct()
             else:
                 raise ValueError(f"Unable to initialize struct: {self.create_struct}") from e
 
         if not isinstance(struct, StructProtocol):
             raise ValueError(f"Incompatible with StructProtocol: {self.create_struct}")
 
-        for (pos, field) in self.field_readers:
+        for pos, field in self.field_readers:
             if pos is not None:
                 struct[pos] = field.read(decoder)  # later: pass reuse in here
             else:
                 field.skip(decoder)
 
         return struct
 
     def skip(self, decoder: BinaryDecoder) -> None:
         for _, field in self.field_readers:
             field.skip(decoder)
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the StructReader class."""
         return (
             self.field_readers == other.field_readers and self.create_struct == other.create_struct
             if isinstance(other, StructReader)
             else False
         )
 
     def __repr__(self) -> str:
+        """Returns the string representation of the StructReader class."""
         return f"StructReader(({','.join(repr(field) for field in self.field_readers)}), {repr(self.create_struct)})"
 
     def __hash__(self) -> int:
+        """Returns a hashed representation of the StructReader class."""
         return hash(self.field_readers)
 
 
 @dataclass(frozen=True)
 class ListReader(Reader):
     element: Reader
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/avro/resolver.py` & `pyiceberg-0.4.0rc1/pyiceberg/avro/resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # pylint: disable=arguments-renamed,unused-argument
+from enum import Enum
 from typing import (
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
 )
 
+from pyiceberg.avro.decoder import BinaryDecoder
 from pyiceberg.avro.reader import (
     BinaryReader,
     BooleanReader,
     DateReader,
     DecimalReader,
+    DefaultReader,
     DoubleReader,
     FixedReader,
     FloatReader,
     IntegerReader,
     ListReader,
     MapReader,
     NoneReader,
@@ -73,89 +76,127 @@
     StructType,
     TimestampType,
     TimestamptzType,
     TimeType,
     UUIDType,
 )
 
+STRUCT_ROOT = -1
+
 
 def construct_reader(
     file_schema: Union[Schema, IcebergType], read_types: Dict[int, Callable[..., StructProtocol]] = EMPTY_DICT
 ) -> Reader:
-    """Constructs a reader from a file schema
+    """Constructs a reader from a file schema.
 
     Args:
-        file_schema (Schema | IcebergType): The schema of the Avro file
+        file_schema (Schema | IcebergType): The schema of the Avro file.
 
     Raises:
-        NotImplementedError: If attempting to resolve an unrecognized object type
+        NotImplementedError: If attempting to resolve an unrecognized object type.
     """
     return resolve(file_schema, file_schema, read_types)
 
 
 def resolve(
     file_schema: Union[Schema, IcebergType],
     read_schema: Union[Schema, IcebergType],
     read_types: Dict[int, Callable[..., StructProtocol]] = EMPTY_DICT,
+    read_enums: Dict[int, Callable[..., Enum]] = EMPTY_DICT,
 ) -> Reader:
-    """Resolves the file and read schema to produce a reader
+    """Resolves the file and read schema to produce a reader.
 
     Args:
         file_schema (Schema | IcebergType): The schema of the Avro file
-        read_schema (Schema | IcebergType): The requested read schema which is equal, subset or superset of the file schema
-        read_types (Dict[int, Callable[[Schema], StructProtocol]]): A dict of types to use for struct data
+        read_schema (Schema | IcebergType): The requested read schema which is equal, subset or superset of the file schema.
+        read_types (Dict[int, Callable[..., StructProtocol]]): A dict of types to use for struct data.
+        read_enums (Dict[int, Callable[..., Enum]]): A dict of fields that have to be converted to an enum.
 
     Raises:
-        NotImplementedError: If attempting to resolve an unrecognized object type
+        NotImplementedError: If attempting to resolve an unrecognized object type.
     """
-    return visit_with_partner(file_schema, read_schema, SchemaResolver(read_types), SchemaPartnerAccessor())  # type: ignore
+    return visit_with_partner(
+        file_schema, read_schema, SchemaResolver(read_types, read_enums), SchemaPartnerAccessor()
+    )  # type: ignore
+
+
+class EnumReader(Reader):
+    """An Enum reader to wrap primitive values into an Enum."""
+
+    enum: Callable[..., Enum]
+    reader: Reader
+
+    def __init__(self, enum: Callable[..., Enum], reader: Reader) -> None:
+        self.enum = enum
+        self.reader = reader
+
+    def read(self, decoder: BinaryDecoder) -> Enum:
+        return self.enum(self.reader.read(decoder))
+
+    def skip(self, decoder: BinaryDecoder) -> None:
+        pass
 
 
 class SchemaResolver(PrimitiveWithPartnerVisitor[IcebergType, Reader]):
     read_types: Dict[int, Callable[..., StructProtocol]]
+    read_enums: Dict[int, Callable[..., Enum]]
     context: List[int]
 
-    def __init__(self, read_types: Dict[int, Callable[..., StructProtocol]] = EMPTY_DICT) -> None:
+    def __init__(
+        self,
+        read_types: Dict[int, Callable[..., StructProtocol]] = EMPTY_DICT,
+        read_enums: Dict[int, Callable[..., Enum]] = EMPTY_DICT,
+    ) -> None:
         self.read_types = read_types
+        self.read_enums = read_enums
         self.context = []
 
     def schema(self, schema: Schema, expected_schema: Optional[IcebergType], result: Reader) -> Reader:
         return result
 
     def before_field(self, field: NestedField, field_partner: Optional[NestedField]) -> None:
         self.context.append(field.field_id)
 
     def after_field(self, field: NestedField, field_partner: Optional[NestedField]) -> None:
         self.context.pop()
 
     def struct(self, struct: StructType, expected_struct: Optional[IcebergType], field_readers: List[Reader]) -> Reader:
-        # -1 indicates the struct root
-        read_struct_id = self.context[-1] if len(self.context) > 0 else -1
+        read_struct_id = self.context[STRUCT_ROOT] if len(self.context) > 0 else STRUCT_ROOT
         struct_callable = self.read_types.get(read_struct_id, Record)
 
         if not expected_struct:
             return StructReader(tuple(enumerate(field_readers)), struct_callable, struct)
 
         if not isinstance(expected_struct, StructType):
             raise ResolveError(f"File/read schema are not aligned for struct, got {expected_struct}")
 
         expected_positions: Dict[int, int] = {field.field_id: pos for pos, field in enumerate(expected_struct.fields)}
 
         # first, add readers for the file fields that must be in order
         results: List[Tuple[Optional[int], Reader]] = [
-            (expected_positions.get(field.field_id), result_reader) for field, result_reader in zip(struct.fields, field_readers)
+            (
+                expected_positions.get(field.field_id),
+                # Check if we need to convert it to an Enum
+                result_reader if not (enum_type := self.read_enums.get(field.field_id)) else EnumReader(enum_type, result_reader),
+            )
+            for field, result_reader in zip(struct.fields, field_readers)
         ]
 
         file_fields = {field.field_id: field for field in struct.fields}
         for pos, read_field in enumerate(expected_struct.fields):
             if read_field.field_id not in file_fields:
-                if read_field.required:
+                if isinstance(read_field, NestedField) and read_field.initial_default is not None:
+                    # The field is not in the file, but there is a default value
+                    # and that one can be required
+                    results.append((pos, DefaultReader(read_field.initial_default)))
+                elif read_field.required:
                     raise ResolveError(f"{read_field} is non-optional, and not part of the file schema")
-                # Just set the new field to None
-                results.append((pos, NoneReader()))
+                else:
+                    # Just set the new field to None
+                    results.append((pos, NoneReader()))
 
         return StructReader(tuple(results), struct_callable, expected_struct)
 
     def field(self, field: NestedField, expected_field: Optional[IcebergType], field_reader: Reader) -> Reader:
         return field_reader if field.required else OptionReader(field_reader)
 
     def list(self, list_type: ListType, expected_list: Optional[IcebergType], element_reader: Reader) -> Reader:
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/catalog/glue.py` & `pyiceberg-0.4.0rc1/pyiceberg/catalog/dynamodb.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,540 +10,772 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
-
-
 import uuid
+from time import time
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Set,
-    Tuple,
-    Type,
     Union,
 )
 
 import boto3
 
 from pyiceberg.catalog import (
     ICEBERG,
-    MANIFEST,
-    MANIFEST_LIST,
-    METADATA,
     METADATA_LOCATION,
-    PREVIOUS_METADATA,
+    PREVIOUS_METADATA_LOCATION,
     TABLE_TYPE,
-    WAREHOUSE_LOCATION,
     Catalog,
     Identifier,
     Properties,
     PropertiesUpdateSummary,
-    delete_data_files,
-    delete_files,
 )
 from pyiceberg.exceptions import (
+    ConditionalCheckFailedException,
+    GenericDynamoDbError,
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchIcebergTableError,
     NoSuchNamespaceError,
     NoSuchPropertyException,
     NoSuchTableError,
     TableAlreadyExistsError,
 )
-from pyiceberg.io import FileIO, load_file_io
+from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.serializers import FromInputFile, ToOutputFile
-from pyiceberg.table import Table
-from pyiceberg.table.metadata import TableMetadata, new_table_metadata
+from pyiceberg.serializers import FromInputFile
+from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table
+from pyiceberg.table.metadata import new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.typedef import EMPTY_DICT
 
-EXTERNAL_TABLE_TYPE = "EXTERNAL_TABLE"
-GLUE_CLIENT = "glue"
-
-PROP_GLUE_TABLE = "Table"
-PROP_GLUE_TABLE_TYPE = "TableType"
-PROP_GLUE_TABLE_DESCRIPTION = "Description"
-PROP_GLUE_TABLE_PARAMETERS = "Parameters"
-PROP_GLUE_TABLE_DATABASE_NAME = "DatabaseName"
-PROP_GLUE_TABLE_NAME = "Name"
-PROP_GLUE_TABLE_OWNER = "Owner"
-PROP_GLUE_TABLE_STORAGE_DESCRIPTOR = "StorageDescriptor"
-
-PROP_GLUE_TABLELIST = "TableList"
-
-PROP_GLUE_DATABASE = "Database"
-PROP_GLUE_DATABASE_LIST = "DatabaseList"
-PROP_GLUE_DATABASE_NAME = "Name"
-PROP_GLUE_DATABASE_LOCATION = "LocationUri"
-PROP_GLUE_DATABASE_DESCRIPTION = "Description"
-PROP_GLUE_DATABASE_PARAMETERS = "Parameters"
-
-PROP_GLUE_NEXT_TOKEN = "NextToken"
-
-GLUE_DESCRIPTION_KEY = "comment"
-GLUE_DATABASE_LOCATION_KEY = "location"
-
-
-def _construct_parameters(metadata_location: str) -> Properties:
-    return {TABLE_TYPE: ICEBERG.upper(), METADATA_LOCATION: metadata_location}
-
-
-def _construct_table_input(table_name: str, metadata_location: str, properties: Properties) -> Dict[str, Any]:
-    table_input = {
-        PROP_GLUE_TABLE_NAME: table_name,
-        PROP_GLUE_TABLE_TYPE: EXTERNAL_TABLE_TYPE,
-        PROP_GLUE_TABLE_PARAMETERS: _construct_parameters(metadata_location),
-    }
-
-    if table_description := properties.get(GLUE_DESCRIPTION_KEY):
-        table_input[PROP_GLUE_TABLE_DESCRIPTION] = table_description
-
-    return table_input
-
-
-def _construct_database_input(database_name: str, properties: Properties) -> Dict[str, Any]:
-    database_input: Dict[str, Any] = {PROP_GLUE_DATABASE_NAME: database_name}
-    parameters = {}
-    for k, v in properties.items():
-        if k == GLUE_DESCRIPTION_KEY:
-            database_input[PROP_GLUE_DATABASE_DESCRIPTION] = v
-        elif k == GLUE_DATABASE_LOCATION_KEY:
-            database_input[PROP_GLUE_DATABASE_LOCATION] = v
-        else:
-            parameters[k] = v
-    database_input[PROP_GLUE_DATABASE_PARAMETERS] = parameters
-    return database_input
-
+DYNAMODB_CLIENT = "dynamodb"
 
-def _write_metadata(metadata: TableMetadata, io: FileIO, metadate_path: str) -> None:
-    ToOutputFile.table_metadata(metadata, io.new_output(metadate_path))
+DYNAMODB_COL_IDENTIFIER = "identifier"
+DYNAMODB_COL_NAMESPACE = "namespace"
+DYNAMODB_COL_VERSION = "v"
+DYNAMODB_COL_UPDATED_AT = "updated_at"
+DYNAMODB_COL_CREATED_AT = "created_at"
+DYNAMODB_NAMESPACE = "NAMESPACE"
+DYNAMODB_NAMESPACE_GSI = "namespace-identifier"
+DYNAMODB_PAY_PER_REQUEST = "PAY_PER_REQUEST"
 
+DYNAMODB_TABLE_NAME = "table-name"
+DYNAMODB_TABLE_NAME_DEFAULT = "iceberg"
 
-class GlueCatalog(Catalog):
-    @staticmethod
-    def identifier_to_database(
-        identifier: Union[str, Identifier], err: Union[Type[ValueError], Type[NoSuchNamespaceError]] = ValueError
-    ) -> str:
-        tuple_identifier = Catalog.identifier_to_tuple(identifier)
-        if len(tuple_identifier) != 1:
-            raise err(f"Invalid database, hierarchical namespaces are not supported: {identifier}")
+PROPERTY_KEY_PREFIX = "p."
 
-        return tuple_identifier[0]
+ACTIVE = "ACTIVE"
+ITEM = "Item"
 
-    @staticmethod
-    def identifier_to_database_and_table(
-        identifier: Union[str, Identifier],
-        err: Union[Type[ValueError], Type[NoSuchTableError], Type[NoSuchNamespaceError]] = ValueError,
-    ) -> Tuple[str, str]:
-        tuple_identifier = Catalog.identifier_to_tuple(identifier)
-        if len(tuple_identifier) != 2:
-            raise err(f"Invalid path, hierarchical namespaces are not supported: {identifier}")
-
-        return tuple_identifier[0], tuple_identifier[1]
 
+class DynamoDbCatalog(Catalog):
     def __init__(self, name: str, **properties: str):
         super().__init__(name, **properties)
-        self.glue = boto3.client(GLUE_CLIENT)
-
-    def _convert_glue_to_iceberg(self, glue_table: Dict[str, Any]) -> Table:
-        properties: Properties = glue_table.get(PROP_GLUE_TABLE_PARAMETERS, {})
-
-        if TABLE_TYPE not in properties:
-            raise NoSuchPropertyException(
-                f"Property {TABLE_TYPE} missing, could not determine type: "
-                f"{glue_table[PROP_GLUE_TABLE_DATABASE_NAME]}.{glue_table[PROP_GLUE_TABLE_NAME]}"
-            )
-        glue_table_type = properties[TABLE_TYPE]
+        self.dynamodb = boto3.client(DYNAMODB_CLIENT)
+        self.dynamodb_table_name = self.properties.get(DYNAMODB_TABLE_NAME, DYNAMODB_TABLE_NAME_DEFAULT)
+        self._ensure_catalog_table_exists_or_create()
+
+    def _ensure_catalog_table_exists_or_create(self) -> None:
+        if self._dynamodb_table_exists():
+            return None
 
-        if glue_table_type.lower() != ICEBERG:
-            raise NoSuchIcebergTableError(
-                f"Property table_type is {glue_table_type}, expected {ICEBERG}: "
-                f"{glue_table[PROP_GLUE_TABLE_DATABASE_NAME]}.{glue_table[PROP_GLUE_TABLE_NAME]}"
-            )
-
-        if METADATA_LOCATION not in properties:
-            raise NoSuchPropertyException(
-                f"Table property {METADATA_LOCATION} is missing, cannot find metadata for: "
-                f"{glue_table[PROP_GLUE_TABLE_DATABASE_NAME]}.{glue_table[PROP_GLUE_TABLE_NAME]}"
+        try:
+            self.dynamodb.create_table(
+                TableName=self.dynamodb_table_name,
+                AttributeDefinitions=CREATE_CATALOG_ATTRIBUTE_DEFINITIONS,
+                KeySchema=CREATE_CATALOG_KEY_SCHEMA,
+                GlobalSecondaryIndexes=CREATE_CATALOG_GLOBAL_SECONDARY_INDEXES,
+                BillingMode=DYNAMODB_PAY_PER_REQUEST,
             )
-        metadata_location = properties[METADATA_LOCATION]
-
-        io = load_file_io(properties=self.properties, location=metadata_location)
-        file = io.new_input(metadata_location)
-        metadata = FromInputFile.table_metadata(file)
-        return Table(
-            identifier=(glue_table[PROP_GLUE_TABLE_DATABASE_NAME], glue_table[PROP_GLUE_TABLE_NAME]),
-            metadata=metadata,
-            metadata_location=metadata_location,
-            io=self._load_file_io(metadata.properties),
-        )
-
-    def _default_warehouse_location(self, database_name: str, table_name: str) -> str:
-        database_properties = self.load_namespace_properties(database_name)
-        if database_location := database_properties.get(GLUE_DATABASE_LOCATION_KEY):
-            database_location = database_location.rstrip("/")
-            return f"{database_location}/{table_name}"
-
-        if warehouse_path := self.properties.get(WAREHOUSE_LOCATION):
-            warehouse_path = warehouse_path.rstrip("/")
-            return f"{warehouse_path}/{database_name}.db/{table_name}"
-
-        raise ValueError("No default path is set, please specify a location when creating a table")
-
-    def _resolve_table_location(self, location: Optional[str], database_name: str, table_name: str) -> str:
-        if not location:
-            return self._default_warehouse_location(database_name, table_name)
-        return location
+        except (
+            self.dynamodb.exceptions.ResourceInUseException,
+            self.dynamodb.exceptions.LimitExceededException,
+            self.dynamodb.exceptions.InternalServerError,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
 
-    def _create_glue_table(self, identifier: Union[str, Identifier], table_input: Dict[str, Any]) -> None:
-        database_name, table_name = self.identifier_to_database_and_table(identifier)
+    def _dynamodb_table_exists(self) -> bool:
         try:
-            self.glue.create_table(DatabaseName=database_name, TableInput=table_input)
-        except self.glue.exceptions.AlreadyExistsException as e:
-            raise TableAlreadyExistsError(f"Table {database_name}.{table_name} already exists") from e
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchNamespaceError(f"Database {database_name} does not exist") from e
+            response = self.dynamodb.describe_table(TableName=self.dynamodb_table_name)
+        except self.dynamodb.exceptions.ResourceNotFoundException:
+            return False
+        except self.dynamodb.exceptions.InternalServerError as e:
+            raise GenericDynamoDbError(e.message) from e
+
+        if response["Table"]["TableStatus"] != ACTIVE:
+            raise GenericDynamoDbError(f"DynamoDB table for catalog {self.dynamodb_table_name} is not {ACTIVE}")
+        else:
+            return True
 
     def create_table(
         self,
         identifier: Union[str, Identifier],
         schema: Schema,
         location: Optional[str] = None,
         partition_spec: PartitionSpec = UNPARTITIONED_PARTITION_SPEC,
         sort_order: SortOrder = UNSORTED_SORT_ORDER,
         properties: Properties = EMPTY_DICT,
     ) -> Table:
-        """Create an Iceberg table in Glue catalog
+        """
+        Create an Iceberg table.
 
         Args:
             identifier: Table identifier.
             schema: Table's schema.
             location: Location for the table. Optional Argument.
             partition_spec: PartitionSpec for the table.
             sort_order: SortOrder for the table.
             properties: Table properties that can be a string based dictionary.
 
         Returns:
-            Table: the created table instance
+            Table: the created table instance.
 
         Raises:
-            AlreadyExistsError: If a table with the name already exists
-            ValueError: If the identifier is invalid, or no path is given to store metadata
+            AlreadyExistsError: If a table with the name already exists.
+            ValueError: If the identifier is invalid, or no path is given to store metadata.
 
         """
         database_name, table_name = self.identifier_to_database_and_table(identifier)
 
         location = self._resolve_table_location(location, database_name, table_name)
-        metadata_location = f"{location}/metadata/00000-{uuid.uuid4()}.metadata.json"
+        metadata_location = self._get_metadata_location(location=location)
         metadata = new_table_metadata(
             location=location, schema=schema, partition_spec=partition_spec, sort_order=sort_order, properties=properties
         )
         io = load_file_io(properties=self.properties, location=metadata_location)
-        _write_metadata(metadata, io, metadata_location)
+        self._write_metadata(metadata, io, metadata_location)
 
-        self._create_glue_table(
-            identifier=identifier, table_input=_construct_table_input(table_name, metadata_location, properties)
-        )
-        loaded_table = self.load_table(identifier=(database_name, table_name))
-        return loaded_table
+        self._ensure_namespace_exists(database_name=database_name)
 
-    def load_table(self, identifier: Union[str, Identifier]) -> Table:
-        """Loads the table's metadata and returns the table instance.
+        try:
+            self._put_dynamo_item(
+                item=_get_create_table_item(
+                    database_name=database_name, table_name=table_name, properties=properties, metadata_location=metadata_location
+                ),
+                condition_expression=f"attribute_not_exists({DYNAMODB_COL_IDENTIFIER})",
+            )
+        except ConditionalCheckFailedException as e:
+            raise TableAlreadyExistsError(f"Table {database_name}.{table_name} already exists") from e
 
-        You can also use this method to check for table existence using 'try catalog.table() except TableNotFoundError'
-        Note: This method doesn't scan data stored in the table.
+        return self.load_table(identifier=identifier)
+
+    def _commit_table(self, table_request: CommitTableRequest) -> CommitTableResponse:
+        """Updates the table.
 
         Args:
-            identifier: Table identifier.
+            table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
-            Table: the table instance with its metadata
+            CommitTableResponse: The updated metadata.
 
         Raises:
-            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid
+            NoSuchTableError: If a table with the given identifier does not exist.
         """
-        database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
-        try:
-            load_table_response = self.glue.get_table(DatabaseName=database_name, Name=table_name)
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchTableError(f"Table does not exists: {database_name}.{table_name}") from e
+        raise NotImplementedError
 
-        return self._convert_glue_to_iceberg(load_table_response.get(PROP_GLUE_TABLE, {}))
+    def load_table(self, identifier: Union[str, Identifier]) -> Table:
+        """
+        Loads the table's metadata and returns the table instance.
 
-    def drop_table(self, identifier: Union[str, Identifier]) -> None:
-        """Drop a table.
+        You can also use this method to check for table existence using 'try catalog.table() except TableNotFoundError'.
+        Note: This method doesn't scan data stored in the table.
 
         Args:
             identifier: Table identifier.
 
+        Returns:
+            Table: the table instance with its metadata.
+
         Raises:
-            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid
+            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid.
         """
         database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
-        try:
-            self.glue.delete_table(DatabaseName=database_name, Name=table_name)
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchTableError(f"Table does not exists: {database_name}.{table_name}") from e
-
-    def purge_table(self, identifier: Union[str, Identifier]) -> None:
-        """Drop a table and purge all data and metadata files.
+        dynamo_table_item = self._get_iceberg_table_item(database_name=database_name, table_name=table_name)
+        return self._convert_dynamo_table_item_to_iceberg_table(dynamo_table_item=dynamo_table_item)
 
-        Note: This method only logs warning rather than raise exception when encountering file deletion failure
+    def drop_table(self, identifier: Union[str, Identifier]) -> None:
+        """Drop a table.
 
         Args:
-            identifier (str | Identifier): Table identifier.
+            identifier: Table identifier.
 
         Raises:
-            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid
+            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid.
         """
-        table = self.load_table(identifier)
-        self.drop_table(identifier)
-        io = load_file_io(self.properties, table.metadata_location)
-        metadata = table.metadata
-        manifest_lists_to_delete = set()
-        manifests_to_delete = []
-        for snapshot in metadata.snapshots:
-            manifests_to_delete += snapshot.manifests(io)
-            if snapshot.manifest_list is not None:
-                manifest_lists_to_delete.add(snapshot.manifest_list)
-
-        manifest_paths_to_delete = {manifest.manifest_path for manifest in manifests_to_delete}
-        prev_metadata_files = {log.metadata_file for log in metadata.metadata_log}
-
-        delete_data_files(io, manifests_to_delete)
-        delete_files(io, manifest_paths_to_delete, MANIFEST)
-        delete_files(io, manifest_lists_to_delete, MANIFEST_LIST)
-        delete_files(io, prev_metadata_files, PREVIOUS_METADATA)
-        delete_files(io, {table.metadata_location}, METADATA)
+        database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
+
+        try:
+            self._delete_dynamo_item(
+                namespace=database_name,
+                identifier=f"{database_name}.{table_name}",
+                condition_expression=f"attribute_exists({DYNAMODB_COL_IDENTIFIER})",
+            )
+        except ConditionalCheckFailedException as e:
+            raise NoSuchTableError(f"Table does not exist: {database_name}.{table_name}") from e
 
     def rename_table(self, from_identifier: Union[str, Identifier], to_identifier: Union[str, Identifier]) -> Table:
-        """Rename a fully classified table name
+        """Rename a fully classified table name.
 
-        This method can only rename Iceberg tables in AWS Glue
+        This method can only rename Iceberg tables in AWS Glue.
 
         Args:
             from_identifier: Existing table identifier.
             to_identifier: New table identifier.
 
         Returns:
-            Table: the updated table instance with its metadata
+            Table: the updated table instance with its metadata.
 
         Raises:
-            ValueError: When the from table identifier is invalid
-            NoSuchTableError: When a table with the name does not exist
-            NoSuchIcebergTableError: When the from table is not a valid iceberg table
-            NoSuchPropertyException: When the from table miss some required properties
-            NoSuchNamespaceError: When the destination namespace doesn't exist
+            ValueError: When from table identifier is invalid.
+            NoSuchTableError: When a table with the name does not exist.
+            NoSuchIcebergTableError: When from table is not a valid iceberg table.
+            NoSuchPropertyException: When from table miss some required properties.
+            NoSuchNamespaceError: When the destination namespace doesn't exist.
         """
         from_database_name, from_table_name = self.identifier_to_database_and_table(from_identifier, NoSuchTableError)
         to_database_name, to_table_name = self.identifier_to_database_and_table(to_identifier)
-        try:
-            get_table_response = self.glue.get_table(DatabaseName=from_database_name, Name=from_table_name)
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchTableError(f"Table does not exists: {from_database_name}.{from_table_name}") from e
 
-        glue_table = get_table_response[PROP_GLUE_TABLE]
+        from_table_item = self._get_iceberg_table_item(database_name=from_database_name, table_name=from_table_name)
 
         try:
-            # verify that from_identifier is a valid iceberg table
-            self._convert_glue_to_iceberg(glue_table)
+            # Verify that from_identifier is a valid iceberg table
+            self._convert_dynamo_table_item_to_iceberg_table(dynamo_table_item=from_table_item)
         except NoSuchPropertyException as e:
             raise NoSuchPropertyException(
-                f"Failed to rename table {from_database_name}.{from_table_name} since it miss required properties"
+                f"Failed to rename table {from_database_name}.{from_table_name} since it is missing required properties"
             ) from e
         except NoSuchIcebergTableError as e:
             raise NoSuchIcebergTableError(
                 f"Failed to rename table {from_database_name}.{from_table_name} since it is not a valid iceberg table"
             ) from e
 
-        new_table_input = {PROP_GLUE_TABLE_NAME: to_table_name}
-        # use the same Glue info to create the new table, pointing to the old metadata
-        if table_type := glue_table.get(PROP_GLUE_TABLE_TYPE):
-            new_table_input[PROP_GLUE_TABLE_TYPE] = table_type
-        if table_parameters := glue_table.get(PROP_GLUE_TABLE_PARAMETERS):
-            new_table_input[PROP_GLUE_TABLE_PARAMETERS] = table_parameters
-        if table_owner := glue_table.get(PROP_GLUE_TABLE_OWNER):
-            new_table_input[PROP_GLUE_TABLE_OWNER] = table_owner
-        if table_storage_descriptor := glue_table.get(PROP_GLUE_TABLE_STORAGE_DESCRIPTOR):
-            new_table_input[PROP_GLUE_TABLE_STORAGE_DESCRIPTOR] = table_storage_descriptor
-        if table_description := glue_table.get(PROP_GLUE_TABLE_DESCRIPTION):
-            new_table_input[PROP_GLUE_TABLE_DESCRIPTION] = table_description
+        self._ensure_namespace_exists(database_name=from_database_name)
+        self._ensure_namespace_exists(database_name=to_database_name)
+
+        try:
+            self._put_dynamo_item(
+                item=_get_rename_table_item(
+                    from_dynamo_table_item=from_table_item, to_database_name=to_database_name, to_table_name=to_table_name
+                ),
+                condition_expression=f"attribute_not_exists({DYNAMODB_COL_IDENTIFIER})",
+            )
+        except ConditionalCheckFailedException as e:
+            raise TableAlreadyExistsError(f"Table {to_database_name}.{to_table_name} already exists") from e
 
-        self._create_glue_table(identifier=to_identifier, table_input=new_table_input)
         try:
             self.drop_table(from_identifier)
-        except Exception as e:
-            self.drop_table(to_identifier)
-            raise ValueError(
-                f"Fail to drop old table {from_database_name}.{from_table_name}, "
-                f"after renaming to {to_database_name}.{to_table_name} roll back to use the old one"
-            ) from e
+        except (NoSuchTableError, GenericDynamoDbError) as e:
+            log_message = f"Failed to drop old table {from_database_name}.{from_table_name}. "
+
+            try:
+                self.drop_table(to_identifier)
+                log_message += f"Rolled back table creation for {to_database_name}.{to_table_name}."
+            except (NoSuchTableError, GenericDynamoDbError):
+                log_message += (
+                    f"Failed to roll back table creation for {to_database_name}.{to_table_name}. " f"Please clean up manually"
+                )
+
+            raise ValueError(log_message) from e
+
         return self.load_table(to_identifier)
 
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         """Create a namespace in the catalog.
 
         Args:
-            namespace: Namespace identifier
-            properties: A string dictionary of properties for the given namespace
+            namespace: Namespace identifier.
+            properties: A string dictionary of properties for the given namespace.
 
         Raises:
-            ValueError: If the identifier is invalid
-            AlreadyExistsError: If a namespace with the given name already exists
+            ValueError: If the identifier is invalid.
+            AlreadyExistsError: If a namespace with the given name already exists.
         """
         database_name = self.identifier_to_database(namespace)
+
         try:
-            self.glue.create_database(DatabaseInput=_construct_database_input(database_name, properties))
-        except self.glue.exceptions.AlreadyExistsException as e:
+            self._put_dynamo_item(
+                item=_get_create_database_item(database_name=database_name, properties=properties),
+                condition_expression=f"attribute_not_exists({DYNAMODB_COL_NAMESPACE})",
+            )
+        except ConditionalCheckFailedException as e:
             raise NamespaceAlreadyExistsError(f"Database {database_name} already exists") from e
 
     def drop_namespace(self, namespace: Union[str, Identifier]) -> None:
         """Drop a namespace.
 
-        A Glue namespace can only be dropped if it is empty
+        A Glue namespace can only be dropped if it is empty.
 
         Args:
-            namespace: Namespace identifier
+            namespace: Namespace identifier.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid
-            NamespaceNotEmptyError: If the namespace is not empty
+            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid.
+            NamespaceNotEmptyError: If the namespace is not empty.
         """
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
-        try:
-            table_list = self.list_tables(namespace=database_name)
-        except NoSuchNamespaceError as e:
-            raise NoSuchNamespaceError(f"Database does not exists: {database_name}") from e
+        table_identifiers = self.list_tables(namespace=database_name)
 
-        if len(table_list) > 0:
+        if len(table_identifiers) > 0:
             raise NamespaceNotEmptyError(f"Database {database_name} is not empty")
 
-        self.glue.delete_database(Name=database_name)
+        try:
+            self._delete_dynamo_item(
+                namespace=database_name,
+                identifier=DYNAMODB_NAMESPACE,
+                condition_expression=f"attribute_exists({DYNAMODB_COL_IDENTIFIER})",
+            )
+        except ConditionalCheckFailedException as e:
+            raise NoSuchNamespaceError(f"Database does not exist: {database_name}") from e
 
     def list_tables(self, namespace: Union[str, Identifier]) -> List[Identifier]:
-        """List tables under the given namespace in the catalog (including non-Iceberg tables)
+        """List tables under the given namespace in the catalog (including non-Iceberg tables).
 
         Args:
             namespace (str | Identifier): Namespace identifier to search.
 
         Returns:
             List[Identifier]: list of table identifiers.
-
-        Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid
         """
-
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
-        table_list = []
+
+        paginator = self.dynamodb.get_paginator("query")
+
         try:
-            table_list_response = self.glue.get_tables(DatabaseName=database_name)
-            next_token = table_list_response.get(PROP_GLUE_NEXT_TOKEN)
-            table_list += table_list_response.get(PROP_GLUE_TABLELIST, [])
-            while next_token:
-                table_list_response = self.glue.get_tables(DatabaseName=database_name, NextToken=next_token)
-                next_token = table_list_response.get(PROP_GLUE_NEXT_TOKEN)
-                table_list += table_list_response.get(PROP_GLUE_TABLELIST, [])
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchNamespaceError(f"Database does not exists: {database_name}") from e
-        return [(database_name, table.get(PROP_GLUE_TABLE_NAME)) for table in table_list]
+            page_iterator = paginator.paginate(
+                TableName=self.dynamodb_table_name,
+                IndexName=DYNAMODB_NAMESPACE_GSI,
+                KeyConditionExpression=f"{DYNAMODB_COL_NAMESPACE} = :namespace ",
+                ExpressionAttributeValues={
+                    ":namespace": {
+                        "S": database_name,
+                    }
+                },
+            )
+        except (
+            self.dynamodb.exceptions.ProvisionedThroughputExceededException,
+            self.dynamodb.exceptions.RequestLimitExceeded,
+            self.dynamodb.exceptions.InternalServerError,
+            self.dynamodb.exceptions.ResourceNotFoundException,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
+
+        table_identifiers = []
+        for page in page_iterator:
+            for item in page["Items"]:
+                _dict = _convert_dynamo_item_to_regular_dict(item)
+                identifier_col = _dict[DYNAMODB_COL_IDENTIFIER]
+                if identifier_col == DYNAMODB_NAMESPACE:
+                    continue
+
+                table_identifiers.append(self.identifier_to_tuple(identifier_col))
+
+        return table_identifiers
 
     def list_namespaces(self, namespace: Union[str, Identifier] = ()) -> List[Identifier]:
-        """List namespaces from the given namespace. If not given, list top-level namespaces from the catalog.
+        """List top-level namespaces from the catalog.
+
+        We do not support hierarchical namespace.
 
         Returns:
-            List[Identifier]: a List of namespace identifiers
+            List[Identifier]: a List of namespace identifiers.
         """
-        # Glue does not support hierarchical namespace, therefore return an empty list
+        # Hierarchical namespace is not supported. Return an empty list
         if namespace:
             return []
-        database_list = []
-        databases_response = self.glue.get_databases()
-        next_token = databases_response.get(PROP_GLUE_NEXT_TOKEN)
-        database_list += databases_response.get(PROP_GLUE_DATABASE_LIST, [])
-        while next_token:
-            databases_response = self.glue.get_databases(NextToken=next_token)
-            next_token = databases_response.get(PROP_GLUE_NEXT_TOKEN)
-            database_list += databases_response.get(PROP_GLUE_DATABASE_LIST, [])
-        return [self.identifier_to_tuple(database.get(PROP_GLUE_DATABASE_NAME)) for database in database_list]
+
+        paginator = self.dynamodb.get_paginator("query")
+
+        try:
+            page_iterator = paginator.paginate(
+                TableName=self.dynamodb_table_name,
+                ConsistentRead=True,
+                KeyConditionExpression=f"{DYNAMODB_COL_IDENTIFIER} = :identifier",
+                ExpressionAttributeValues={
+                    ":identifier": {
+                        "S": DYNAMODB_NAMESPACE,
+                    }
+                },
+            )
+        except (
+            self.dynamodb.exceptions.ProvisionedThroughputExceededException,
+            self.dynamodb.exceptions.RequestLimitExceeded,
+            self.dynamodb.exceptions.InternalServerError,
+            self.dynamodb.exceptions.ResourceNotFoundException,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
+
+        database_identifiers = []
+        for page in page_iterator:
+            for item in page["Items"]:
+                _dict = _convert_dynamo_item_to_regular_dict(item)
+                namespace_col = _dict[DYNAMODB_COL_NAMESPACE]
+                database_identifiers.append(self.identifier_to_tuple(namespace_col))
+
+        return database_identifiers
 
     def load_namespace_properties(self, namespace: Union[str, Identifier]) -> Properties:
-        """Get properties for a namespace.
+        """
+        Get properties for a namespace.
 
         Args:
-            namespace: Namespace identifier
+            namespace: Namespace identifier.
 
         Returns:
-            Properties: Properties for the given namespace
+            Properties: Properties for the given namespace.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or identifier is invalid
+            NoSuchNamespaceError: If a namespace with the given name does not exist, or identifier is invalid.
         """
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
-        try:
-            database_response = self.glue.get_database(Name=database_name)
-        except self.glue.exceptions.EntityNotFoundException as e:
-            raise NoSuchNamespaceError(f"Database does not exists: {database_name}") from e
-        except self.glue.exceptions.InvalidInputException as e:
-            raise NoSuchNamespaceError(f"Invalid input for namespace {database_name}") from e
-
-        database = database_response[PROP_GLUE_DATABASE]
-        if PROP_GLUE_DATABASE_PARAMETERS not in database:
-            return {}
-
-        properties = dict(database[PROP_GLUE_DATABASE_PARAMETERS])
-        if database_location := database.get(PROP_GLUE_DATABASE_LOCATION):
-            properties[GLUE_DATABASE_LOCATION_KEY] = database_location
-        if database_description := database.get(PROP_GLUE_DATABASE_DESCRIPTION):
-            properties[GLUE_DESCRIPTION_KEY] = database_description
-
-        return properties
+        namespace_item = self._get_iceberg_namespace_item(database_name=database_name)
+        namespace_dict = _convert_dynamo_item_to_regular_dict(namespace_item)
+        return _get_namespace_properties(namespace_dict=namespace_dict)
 
     def update_namespace_properties(
         self, namespace: Union[str, Identifier], removals: Optional[Set[str]] = None, updates: Properties = EMPTY_DICT
     ) -> PropertiesUpdateSummary:
-        """Removes provided property keys and updates properties for a namespace.
+        """
+        Removes or updates provided property keys for a namespace.
 
         Args:
             namespace: Namespace identifier
             removals: Set of property keys that need to be removed. Optional Argument.
             updates: Properties to be updated for the given namespace.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist， or identifier is invalid
+            NoSuchNamespaceError: If a namespace with the given name does not exist， or identifier is invalid.
             ValueError: If removals and updates have overlapping keys.
         """
-        removed: Set[str] = set()
-        updated: Set[str] = set()
-
-        if updates and removals:
-            overlap = set(removals) & set(updates.keys())
-            if overlap:
-                raise ValueError(f"Updates and deletes have an overlap: {overlap}")
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
-        current_properties = self.load_namespace_properties(namespace=database_name)
-        new_properties = dict(current_properties)
+        namespace_item = self._get_iceberg_namespace_item(database_name=database_name)
+        namespace_dict = _convert_dynamo_item_to_regular_dict(namespace_item)
+        current_properties = _get_namespace_properties(namespace_dict=namespace_dict)
+
+        properties_update_summary, updated_properties = self._get_updated_props_and_update_summary(
+            current_properties=current_properties, removals=removals, updates=updates
+        )
 
-        if removals:
-            for key in removals:
-                if key in new_properties:
-                    new_properties.pop(key)
-                    removed.add(key)
-        if updates:
-            for key, value in updates.items():
-                new_properties[key] = value
-                updated.add(key)
+        try:
+            self._put_dynamo_item(
+                item=_get_update_database_item(
+                    namespace_item=namespace_item,
+                    updated_properties=updated_properties,
+                ),
+                condition_expression=f"attribute_exists({DYNAMODB_COL_NAMESPACE})",
+            )
+        except ConditionalCheckFailedException as e:
+            raise NoSuchNamespaceError(f"Database {database_name} does not exist") from e
+
+        return properties_update_summary
+
+    def _get_iceberg_table_item(self, database_name: str, table_name: str) -> Dict[str, Any]:
+        try:
+            return self._get_dynamo_item(identifier=f"{database_name}.{table_name}", namespace=database_name)
+        except ValueError as e:
+            raise NoSuchTableError(f"Table does not exist: {database_name}.{table_name}") from e
+
+    def _get_iceberg_namespace_item(self, database_name: str) -> Dict[str, Any]:
+        try:
+            return self._get_dynamo_item(identifier=DYNAMODB_NAMESPACE, namespace=database_name)
+        except ValueError as e:
+            raise NoSuchNamespaceError(f"Namespace does not exist: {database_name}") from e
+
+    def _ensure_namespace_exists(self, database_name: str) -> Dict[str, Any]:
+        return self._get_iceberg_namespace_item(database_name)
+
+    def _get_dynamo_item(self, identifier: str, namespace: str) -> Dict[str, Any]:
+        try:
+            response = self.dynamodb.get_item(
+                TableName=self.dynamodb_table_name,
+                ConsistentRead=True,
+                Key={
+                    DYNAMODB_COL_IDENTIFIER: {
+                        "S": identifier,
+                    },
+                    DYNAMODB_COL_NAMESPACE: {
+                        "S": namespace,
+                    },
+                },
+            )
+            if ITEM in response:
+                return response[ITEM]
+            else:
+                raise ValueError(f"Item not found. identifier: {identifier} - namespace: {namespace}")
+        except self.dynamodb.exceptions.ResourceNotFoundException as e:
+            raise ValueError(f"Item not found. identifier: {identifier} - namespace: {namespace}") from e
+        except (
+            self.dynamodb.exceptions.ProvisionedThroughputExceededException,
+            self.dynamodb.exceptions.RequestLimitExceeded,
+            self.dynamodb.exceptions.InternalServerError,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
 
-        self.glue.update_database(Name=database_name, DatabaseInput=_construct_database_input(database_name, new_properties))
+    def _put_dynamo_item(self, item: Dict[str, Any], condition_expression: str) -> None:
+        try:
+            self.dynamodb.put_item(TableName=self.dynamodb_table_name, Item=item, ConditionExpression=condition_expression)
+        except self.dynamodb.exceptions.ConditionalCheckFailedException as e:
+            raise ConditionalCheckFailedException(f"Condition expression check failed: {condition_expression} - {item}") from e
+        except (
+            self.dynamodb.exceptions.ProvisionedThroughputExceededException,
+            self.dynamodb.exceptions.RequestLimitExceeded,
+            self.dynamodb.exceptions.InternalServerError,
+            self.dynamodb.exceptions.ResourceNotFoundException,
+            self.dynamodb.exceptions.ItemCollectionSizeLimitExceededException,
+            self.dynamodb.exceptions.TransactionConflictException,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
+
+    def _delete_dynamo_item(self, namespace: str, identifier: str, condition_expression: str) -> None:
+        try:
+            self.dynamodb.delete_item(
+                TableName=self.dynamodb_table_name,
+                Key={
+                    DYNAMODB_COL_IDENTIFIER: {
+                        "S": identifier,
+                    },
+                    DYNAMODB_COL_NAMESPACE: {
+                        "S": namespace,
+                    },
+                },
+                ConditionExpression=condition_expression,
+            )
+        except self.dynamodb.exceptions.ConditionalCheckFailedException as e:
+            raise ConditionalCheckFailedException(
+                f"Condition expression check failed: {condition_expression} - {identifier}"
+            ) from e
+        except (
+            self.dynamodb.exceptions.ProvisionedThroughputExceededException,
+            self.dynamodb.exceptions.RequestLimitExceeded,
+            self.dynamodb.exceptions.InternalServerError,
+            self.dynamodb.exceptions.ResourceNotFoundException,
+            self.dynamodb.exceptions.ItemCollectionSizeLimitExceededException,
+            self.dynamodb.exceptions.TransactionConflictException,
+        ) as e:
+            raise GenericDynamoDbError(e.message) from e
+
+    def _convert_dynamo_table_item_to_iceberg_table(self, dynamo_table_item: Dict[str, Any]) -> Table:
+        table_dict = _convert_dynamo_item_to_regular_dict(dynamo_table_item)
+
+        for prop in [_add_property_prefix(prop) for prop in (TABLE_TYPE, METADATA_LOCATION)] + [
+            DYNAMODB_COL_IDENTIFIER,
+            DYNAMODB_COL_NAMESPACE,
+            DYNAMODB_COL_CREATED_AT,
+        ]:
+            if prop not in table_dict.keys():
+                raise NoSuchPropertyException(f"Iceberg required property {prop} is missing: {dynamo_table_item}")
+
+        table_type = table_dict[_add_property_prefix(TABLE_TYPE)]
+        identifier = table_dict[DYNAMODB_COL_IDENTIFIER]
+        metadata_location = table_dict[_add_property_prefix(METADATA_LOCATION)]
+        database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
 
-        expected_to_change = (removals or set()).difference(removed)
+        if table_type.lower() != ICEBERG:
+            raise NoSuchIcebergTableError(
+                f"Property table_type is {table_type}, expected {ICEBERG}: " f"{database_name}.{table_name}"
+            )
 
-        return PropertiesUpdateSummary(
-            removed=list(removed or []), updated=list(updates.keys() if updates else []), missing=list(expected_to_change)
+        io = load_file_io(properties=self.properties, location=metadata_location)
+        file = io.new_input(metadata_location)
+        metadata = FromInputFile.table_metadata(file)
+        return Table(
+            identifier=(self.name, database_name, table_name),
+            metadata=metadata,
+            metadata_location=metadata_location,
+            io=self._load_file_io(metadata.properties, metadata_location),
+            catalog=self,
         )
+
+
+def _get_create_table_item(database_name: str, table_name: str, properties: Properties, metadata_location: str) -> Dict[str, Any]:
+    current_timestamp_ms = str(round(time() * 1000))
+    _dict = {
+        DYNAMODB_COL_IDENTIFIER: {
+            "S": f"{database_name}.{table_name}",
+        },
+        DYNAMODB_COL_NAMESPACE: {
+            "S": database_name,
+        },
+        DYNAMODB_COL_VERSION: {
+            "S": str(uuid.uuid4()),
+        },
+        DYNAMODB_COL_CREATED_AT: {
+            "N": current_timestamp_ms,
+        },
+        DYNAMODB_COL_UPDATED_AT: {
+            "N": current_timestamp_ms,
+        },
+    }
+
+    for key, val in properties.items():
+        _dict[_add_property_prefix(key)] = {"S": val}
+
+    _dict[_add_property_prefix(TABLE_TYPE)] = {"S": ICEBERG.upper()}
+    _dict[_add_property_prefix(METADATA_LOCATION)] = {"S": metadata_location}
+    _dict[_add_property_prefix(PREVIOUS_METADATA_LOCATION)] = {"S": ""}
+
+    return _dict
+
+
+def _get_rename_table_item(from_dynamo_table_item: Dict[str, Any], to_database_name: str, to_table_name: str) -> Dict[str, Any]:
+    _dict = from_dynamo_table_item
+    current_timestamp_ms = str(round(time() * 1000))
+    _dict[DYNAMODB_COL_IDENTIFIER]["S"] = f"{to_database_name}.{to_table_name}"
+    _dict[DYNAMODB_COL_NAMESPACE]["S"] = to_database_name
+    _dict[DYNAMODB_COL_VERSION]["S"] = str(uuid.uuid4())
+    _dict[DYNAMODB_COL_UPDATED_AT]["N"] = current_timestamp_ms
+    return _dict
+
+
+def _get_create_database_item(database_name: str, properties: Properties) -> Dict[str, Any]:
+    current_timestamp_ms = str(round(time() * 1000))
+    _dict = {
+        DYNAMODB_COL_IDENTIFIER: {
+            "S": DYNAMODB_NAMESPACE,
+        },
+        DYNAMODB_COL_NAMESPACE: {
+            "S": database_name,
+        },
+        DYNAMODB_COL_VERSION: {
+            "S": str(uuid.uuid4()),
+        },
+        DYNAMODB_COL_CREATED_AT: {
+            "N": current_timestamp_ms,
+        },
+        DYNAMODB_COL_UPDATED_AT: {
+            "N": current_timestamp_ms,
+        },
+    }
+
+    for key, val in properties.items():
+        _dict[_add_property_prefix(key)] = {"S": val}
+
+    return _dict
+
+
+def _get_update_database_item(namespace_item: Dict[str, Any], updated_properties: Properties) -> Dict[str, Any]:
+    current_timestamp_ms = str(round(time() * 1000))
+
+    _dict = {
+        DYNAMODB_COL_IDENTIFIER: namespace_item[DYNAMODB_COL_IDENTIFIER],
+        DYNAMODB_COL_NAMESPACE: namespace_item[DYNAMODB_COL_NAMESPACE],
+        DYNAMODB_COL_VERSION: {
+            "S": str(uuid.uuid4()),
+        },
+        DYNAMODB_COL_CREATED_AT: namespace_item[DYNAMODB_COL_CREATED_AT],
+        DYNAMODB_COL_UPDATED_AT: {
+            "N": current_timestamp_ms,
+        },
+    }
+
+    for key, val in updated_properties.items():
+        _dict[_add_property_prefix(key)] = {"S": val}
+
+    return _dict
+
+
+CREATE_CATALOG_ATTRIBUTE_DEFINITIONS = [
+    {
+        "AttributeName": DYNAMODB_COL_IDENTIFIER,
+        "AttributeType": "S",
+    },
+    {
+        "AttributeName": DYNAMODB_COL_NAMESPACE,
+        "AttributeType": "S",
+    },
+]
+
+CREATE_CATALOG_KEY_SCHEMA = [
+    {
+        "AttributeName": DYNAMODB_COL_IDENTIFIER,
+        "KeyType": "HASH",
+    },
+    {
+        "AttributeName": DYNAMODB_COL_NAMESPACE,
+        "KeyType": "RANGE",
+    },
+]
+
+
+CREATE_CATALOG_GLOBAL_SECONDARY_INDEXES = [
+    {
+        "IndexName": DYNAMODB_NAMESPACE_GSI,
+        "KeySchema": [
+            {
+                "AttributeName": DYNAMODB_COL_NAMESPACE,
+                "KeyType": "HASH",
+            },
+            {
+                "AttributeName": DYNAMODB_COL_IDENTIFIER,
+                "KeyType": "RANGE",
+            },
+        ],
+        "Projection": {
+            "ProjectionType": "KEYS_ONLY",
+        },
+    }
+]
+
+
+def _get_namespace_properties(namespace_dict: Dict[str, str]) -> Properties:
+    return {_remove_property_prefix(key): val for key, val in namespace_dict.items() if key.startswith(PROPERTY_KEY_PREFIX)}
+
+
+def _convert_dynamo_item_to_regular_dict(dynamo_json: Dict[str, Any]) -> Dict[str, str]:
+    """Converts a dynamo json to a regular json.
+
+    Example of a dynamo json:
+    {
+        "AlbumTitle": {
+            "S": "Songs About Life",
+        },
+        "Artist": {
+            "S": "Acme Band",
+        },
+        "SongTitle": {
+            "S": "Happy Day",
+        }
+    }
+
+    Converted to regular json:
+    {
+        "AlbumTitle": "Songs About Life",
+        "Artist": "Acme Band",
+        "SongTitle": "Happy Day"
+    }
+
+    Only "S" and "N" data types are supported since those are the only ones that Iceberg is utilizing.
+    """
+    regular_json = {}
+    for column_name, val_dict in dynamo_json.items():
+        keys = list(val_dict.keys())
+
+        if len(keys) != 1:
+            raise ValueError(f"Expecting only 1 key: {keys}")
+
+        data_type = keys[0]
+        if data_type not in ("S", "N"):
+            raise ValueError("Only S and N data types are supported.")
+
+        values = list(val_dict.values())
+        assert len(values) == 1
+        column_value = values[0]
+        regular_json[column_name] = column_value
+
+    return regular_json
+
+
+def _add_property_prefix(prop: str) -> str:
+    return PROPERTY_KEY_PREFIX + prop
+
+
+def _remove_property_prefix(prop: str) -> str:
+    return prop.lstrip(PROPERTY_KEY_PREFIX)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/catalog/hive.py` & `pyiceberg-0.4.0rc1/pyiceberg/catalog/hive.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 import getpass
 import time
-import uuid
 from types import TracebackType
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Set,
-    Tuple,
     Type,
     Union,
 )
 from urllib.parse import urlparse
 
 from hive_metastore.ThriftHiveMetastore import Client
 from hive_metastore.ttypes import AlreadyExistsException
@@ -42,18 +40,19 @@
     StorageDescriptor,
 )
 from hive_metastore.ttypes import Table as HiveTable
 from thrift.protocol import TBinaryProtocol
 from thrift.transport import TSocket, TTransport
 
 from pyiceberg.catalog import (
+    EXTERNAL_TABLE,
     ICEBERG,
+    LOCATION,
     METADATA_LOCATION,
     TABLE_TYPE,
-    WAREHOUSE_LOCATION,
     Catalog,
     Identifier,
     Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     NamespaceAlreadyExistsError,
@@ -62,17 +61,17 @@
     NoSuchNamespaceError,
     NoSuchTableError,
     TableAlreadyExistsError,
 )
 from pyiceberg.io import FileIO, load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema, SchemaVisitor, visit
-from pyiceberg.serializers import FromInputFile, ToOutputFile
-from pyiceberg.table import Table
-from pyiceberg.table.metadata import TableMetadata, new_table_metadata
+from pyiceberg.serializers import FromInputFile
+from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table
+from pyiceberg.table.metadata import new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.typedef import EMPTY_DICT
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DecimalType,
@@ -106,19 +105,18 @@
     UUIDType: "string",
     BinaryType: "binary",
     FixedType: "binary",
 }
 
 COMMENT = "comment"
 OWNER = "owner"
-LOCATION = "location"
 
 
 class _HiveClient:
-    """Helper class to nicely open and close the transport"""
+    """Helper class to nicely open and close the transport."""
 
     _transport: TTransport
     _client: Client
 
     def __init__(self, uri: str):
         url_parts = urlparse(uri)
         transport = TSocket.TSocket(url_parts.hostname, url_parts.port)
@@ -214,35 +212,14 @@
         else:
             return HIVE_PRIMITIVE_TYPES[type(primitive)]
 
 
 class HiveCatalog(Catalog):
     _client: _HiveClient
 
-    @staticmethod
-    def identifier_to_database(
-        identifier: Union[str, Identifier], err: Union[Type[ValueError], Type[NoSuchNamespaceError]] = ValueError
-    ) -> str:
-        tuple_identifier = Catalog.identifier_to_tuple(identifier)
-        if len(tuple_identifier) != 1:
-            raise err(f"Invalid database, hierarchical namespaces are not supported: {identifier}")
-
-        return tuple_identifier[0]
-
-    @staticmethod
-    def identifier_to_database_and_table(
-        identifier: Union[str, Identifier],
-        err: Union[Type[ValueError], Type[NoSuchTableError], Type[NoSuchNamespaceError]] = ValueError,
-    ) -> Tuple[str, str]:
-        tuple_identifier = Catalog.identifier_to_tuple(identifier)
-        if len(tuple_identifier) != 2:
-            raise err(f"Invalid path, hierarchical namespaces are not supported: {identifier}")
-
-        return tuple_identifier[0], tuple_identifier[1]
-
     def __init__(self, name: str, **properties: str):
         super().__init__(name, **properties)
         self._client = _HiveClient(properties["uri"])
 
     def _convert_hive_into_iceberg(self, table: HiveTable, io: FileIO) -> Table:
         properties: Dict[str, str] = table.parameters
         if TABLE_TYPE not in properties:
@@ -261,104 +238,103 @@
 
         file = io.new_input(metadata_location)
         metadata = FromInputFile.table_metadata(file)
         return Table(
             identifier=(table.dbName, table.tableName),
             metadata=metadata,
             metadata_location=metadata_location,
-            io=self._load_file_io(metadata.properties),
+            io=self._load_file_io(metadata.properties, metadata_location),
+            catalog=self,
         )
 
-    def _write_metadata(self, metadata: TableMetadata, io: FileIO, metadata_path: str) -> None:
-        ToOutputFile.table_metadata(metadata, io.new_output(metadata_path))
-
-    def _resolve_table_location(self, location: Optional[str], database_name: str, table_name: str) -> str:
-        if not location:
-            database_properties = self.load_namespace_properties(database_name)
-            if database_location := database_properties.get(LOCATION):
-                database_location = database_location.rstrip("/")
-                return f"{database_location}/{table_name}"
-
-            if warehouse_location := self.properties.get(WAREHOUSE_LOCATION):
-                warehouse_location = warehouse_location.rstrip("/")
-                return f"{warehouse_location}/{database_name}/{table_name}"
-            raise ValueError("Cannot determine location from warehouse, please provide an explicit location")
-        return location
-
     def create_table(
         self,
         identifier: Union[str, Identifier],
         schema: Schema,
         location: Optional[str] = None,
         partition_spec: PartitionSpec = UNPARTITIONED_PARTITION_SPEC,
         sort_order: SortOrder = UNSORTED_SORT_ORDER,
         properties: Properties = EMPTY_DICT,
     ) -> Table:
-        """Create a table
+        """Create a table.
 
         Args:
             identifier: Table identifier.
             schema: Table's schema.
             location: Location for the table. Optional Argument.
             partition_spec: PartitionSpec for the table.
             sort_order: SortOrder for the table.
             properties: Table properties that can be a string based dictionary.
 
         Returns:
-            Table: the created table instance
+            Table: the created table instance.
 
         Raises:
-            AlreadyExistsError: If a table with the name already exists
-            ValueError: If the identifier is invalid
+            AlreadyExistsError: If a table with the name already exists.
+            ValueError: If the identifier is invalid.
         """
         database_name, table_name = self.identifier_to_database_and_table(identifier)
         current_time_millis = int(time.time() * 1000)
 
         location = self._resolve_table_location(location, database_name, table_name)
 
-        metadata_location = f"{location}/metadata/00000-{uuid.uuid4()}.metadata.json"
+        metadata_location = self._get_metadata_location(location=location)
         metadata = new_table_metadata(
             location=location, schema=schema, partition_spec=partition_spec, sort_order=sort_order, properties=properties
         )
         io = load_file_io({**self.properties, **properties}, location=location)
         self._write_metadata(metadata, io, metadata_location)
 
         tbl = HiveTable(
             dbName=database_name,
             tableName=table_name,
             owner=properties[OWNER] if properties and OWNER in properties else getpass.getuser(),
             createTime=current_time_millis // 1000,
             lastAccessTime=current_time_millis // 1000,
             sd=_construct_hive_storage_descriptor(schema, location),
-            tableType="EXTERNAL_TABLE",
+            tableType=EXTERNAL_TABLE,
             parameters=_construct_parameters(metadata_location),
         )
         try:
             with self._client as open_client:
                 open_client.create_table(tbl)
                 hive_table = open_client.get_table(dbname=database_name, tbl_name=table_name)
         except AlreadyExistsException as e:
             raise TableAlreadyExistsError(f"Table {database_name}.{table_name} already exists") from e
 
         return self._convert_hive_into_iceberg(hive_table, io)
 
+    def _commit_table(self, table_request: CommitTableRequest) -> CommitTableResponse:
+        """Updates the table.
+
+        Args:
+            table_request (CommitTableRequest): The table requests to be carried out.
+
+        Returns:
+            CommitTableResponse: The updated metadata.
+
+        Raises:
+            NoSuchTableError: If a table with the given identifier does not exist.
+        """
+        raise NotImplementedError
+
     def load_table(self, identifier: Union[str, Identifier]) -> Table:
         """Loads the table's metadata and returns the table instance.
 
-        You can also use this method to check for table existence using 'try catalog.table() except TableNotFoundError'
+        You can also use this method to check for table existence using 'try catalog.table() except TableNotFoundError'.
         Note: This method doesn't scan data stored in the table.
 
         Args:
             identifier: Table identifier.
 
         Returns:
-            Table: the table instance with its metadata
+            Table: the table instance with its metadata.
 
         Raises:
-            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid
+            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid.
         """
         database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
         try:
             with self._client as open_client:
                 hive_table = open_client.get_table(dbname=database_name, tbl_name=table_name)
         except NoSuchObjectException as e:
             raise NoSuchTableError(f"Table does not exists: {table_name}") from e
@@ -369,42 +345,42 @@
     def drop_table(self, identifier: Union[str, Identifier]) -> None:
         """Drop a table.
 
         Args:
             identifier: Table identifier.
 
         Raises:
-            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid
+            NoSuchTableError: If a table with the name does not exist, or the identifier is invalid.
         """
         database_name, table_name = self.identifier_to_database_and_table(identifier, NoSuchTableError)
         try:
             with self._client as open_client:
                 open_client.drop_table(dbname=database_name, name=table_name, deleteData=False)
         except NoSuchObjectException as e:
-            # When the namespace doesn't exists, it throws the same error
+            # When the namespace doesn't exist, it throws the same error
             raise NoSuchTableError(f"Table does not exists: {table_name}") from e
 
     def purge_table(self, identifier: Union[str, Identifier]) -> None:
         # This requires to traverse the reachability set, and drop all the data files.
         raise NotImplementedError("Not yet implemented")
 
     def rename_table(self, from_identifier: Union[str, Identifier], to_identifier: Union[str, Identifier]) -> Table:
-        """Rename a fully classified table name
+        """Rename a fully classified table name.
 
         Args:
             from_identifier: Existing table identifier.
             to_identifier: New table identifier.
 
         Returns:
-            Table: the updated table instance with its metadata
+            Table: the updated table instance with its metadata.
 
         Raises:
-            ValueError: When the from table identifier is invalid
-            NoSuchTableError: When a table with the name does not exist
-            NoSuchNamespaceError: When the destination namespace doesn't exists
+            ValueError: When from table identifier is invalid.
+            NoSuchTableError: When a table with the name does not exist.
+            NoSuchNamespaceError: When the destination namespace doesn't exist.
         """
         from_database_name, from_table_name = self.identifier_to_database_and_table(from_identifier, NoSuchTableError)
         to_database_name, to_table_name = self.identifier_to_database_and_table(to_identifier)
         try:
             with self._client as open_client:
                 tbl = open_client.get_table(dbname=from_database_name, tbl_name=from_table_name)
                 tbl.dbName = to_database_name
@@ -416,91 +392,91 @@
             raise NoSuchNamespaceError(f"Database does not exists: {to_database_name}") from e
         return self.load_table(to_identifier)
 
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         """Create a namespace in the catalog.
 
         Args:
-            namespace: Namespace identifier
-            properties: A string dictionary of properties for the given namespace
+            namespace: Namespace identifier.
+            properties: A string dictionary of properties for the given namespace.
 
         Raises:
-            ValueError: If the identifier is invalid
-            AlreadyExistsError: If a namespace with the given name already exists
+            ValueError: If the identifier is invalid.
+            AlreadyExistsError: If a namespace with the given name already exists.
         """
         database_name = self.identifier_to_database(namespace)
         hive_database = HiveDatabase(name=database_name, parameters=properties)
 
         try:
             with self._client as open_client:
                 open_client.create_database(_annotate_namespace(hive_database, properties))
         except AlreadyExistsException as e:
             raise NamespaceAlreadyExistsError(f"Database {database_name} already exists") from e
 
     def drop_namespace(self, namespace: Union[str, Identifier]) -> None:
         """Drop a namespace.
 
         Args:
-            namespace: Namespace identifier
+            namespace: Namespace identifier.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid
-            NamespaceNotEmptyError: If the namespace is not empty
+            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid.
+            NamespaceNotEmptyError: If the namespace is not empty.
         """
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
         try:
             with self._client as open_client:
                 open_client.drop_database(database_name, deleteData=False, cascade=False)
         except InvalidOperationException as e:
             raise NamespaceNotEmptyError(f"Database {database_name} is not empty") from e
         except MetaException as e:
             raise NoSuchNamespaceError(f"Database does not exists: {database_name}") from e
 
     def list_tables(self, namespace: Union[str, Identifier]) -> List[Identifier]:
-        """List tables under the given namespace in the catalog (including non-Iceberg tables)
+        """List tables under the given namespace in the catalog (including non-Iceberg tables).
 
-        When the database doesn't exist, it will just return an empty list
+        When the database doesn't exist, it will just return an empty list.
 
         Args:
             namespace: Database to list.
 
         Returns:
             List[Identifier]: list of table identifiers.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid
+            NoSuchNamespaceError: If a namespace with the given name does not exist, or the identifier is invalid.
         """
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
         with self._client as open_client:
             return [(database_name, table_name) for table_name in open_client.get_all_tables(db_name=database_name)]
 
     def list_namespaces(self, namespace: Union[str, Identifier] = ()) -> List[Identifier]:
         """List namespaces from the given namespace. If not given, list top-level namespaces from the catalog.
 
         Returns:
-            List[Identifier]: a List of namespace identifiers
+            List[Identifier]: a List of namespace identifiers.
         """
-        # Hive does not support hierarchical namespaces, therefore return an empty list
+        # Hierarchical namespace is not supported. Return an empty list
         if namespace:
             return []
 
         with self._client as open_client:
             return list(map(self.identifier_to_tuple, open_client.get_all_databases()))
 
     def load_namespace_properties(self, namespace: Union[str, Identifier]) -> Properties:
         """Get properties for a namespace.
 
         Args:
-            namespace: Namespace identifier
+            namespace: Namespace identifier.
 
         Returns:
-            Properties: Properties for the given namespace
+            Properties: Properties for the given namespace.
 
         Raises:
-            NoSuchNamespaceError: If a namespace with the given name does not exist, or identifier is invalid
+            NoSuchNamespaceError: If a namespace with the given name does not exist, or identifier is invalid.
         """
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
         try:
             with self._client as open_client:
                 database = open_client.get_database(name=database_name)
                 properties = database.parameters
                 properties[LOCATION] = database.locationUri
@@ -512,46 +488,42 @@
 
     def update_namespace_properties(
         self, namespace: Union[str, Identifier], removals: Optional[Set[str]] = None, updates: Properties = EMPTY_DICT
     ) -> PropertiesUpdateSummary:
         """Removes provided property keys and updates properties for a namespace.
 
         Args:
-            namespace: Namespace identifier
+            namespace: Namespace identifier.
             removals: Set of property keys that need to be removed. Optional Argument.
             updates: Properties to be updated for the given namespace.
 
         Raises:
             NoSuchNamespaceError: If a namespace with the given name does not exist
             ValueError: If removals and updates have overlapping keys.
         """
-        removed: Set[str] = set()
-        updated: Set[str] = set()
-
-        if updates and removals:
-            overlap = set(removals) & set(updates.keys())
-            if overlap:
-                raise ValueError(f"Updates and deletes have an overlap: {overlap}")
-
+        self._check_for_overlap(updates=updates, removals=removals)
         database_name = self.identifier_to_database(namespace, NoSuchNamespaceError)
         with self._client as open_client:
             try:
                 database = open_client.get_database(database_name)
                 parameters = database.parameters
             except NoSuchObjectException as e:
                 raise NoSuchNamespaceError(f"Database does not exists: {database_name}") from e
+
+            removed: Set[str] = set()
+            updated: Set[str] = set()
+
             if removals:
                 for key in removals:
                     if key in parameters:
                         parameters[key] = None
                         removed.add(key)
             if updates:
                 for key, value in updates.items():
                     parameters[key] = value
                     updated.add(key)
+
             open_client.alter_database(database_name, _annotate_namespace(database, parameters))
 
         expected_to_change = (removals or set()).difference(removed)
 
-        return PropertiesUpdateSummary(
-            removed=list(removed or []), updated=list(updates.keys() if updates else []), missing=list(expected_to_change)
-        )
+        return PropertiesUpdateSummary(removed=list(removed or []), updated=list(updated or []), missing=list(expected_to_change))
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/catalog/rest.py` & `pyiceberg-0.4.0rc1/pyiceberg/catalog/rest.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import (
     Any,
     Dict,
     List,
     Literal,
     Optional,
     Set,
+    Tuple,
     Type,
     Union,
 )
 
 from pydantic import Field, ValidationError
 from requests import HTTPError, Session
 
@@ -38,41 +39,48 @@
     Identifier,
     Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     AuthorizationExpiredError,
     BadRequestError,
+    CommitFailedException,
+    CommitStateUnknownException,
     ForbiddenError,
     NamespaceAlreadyExistsError,
     NoSuchNamespaceError,
     NoSuchTableError,
     OAuthError,
     RESTError,
     ServerError,
     ServiceUnavailableError,
     TableAlreadyExistsError,
     UnauthorizedError,
 )
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.table import Table, TableMetadata
+from pyiceberg.table import (
+    CommitTableRequest,
+    CommitTableResponse,
+    Table,
+    TableMetadata,
+)
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.typedef import EMPTY_DICT, IcebergBaseModel
 
 ICEBERG_REST_SPEC_VERSION = "0.14.1"
 
 
 class Endpoints:
     get_config: str = "config"
     list_namespaces: str = "namespaces"
     create_namespace: str = "namespaces"
     load_namespace_metadata: str = "namespaces/{namespace}"
     drop_namespace: str = "namespaces/{namespace}"
-    update_properties: str = "namespaces/{namespace}/properties"
+    update_namespace_properties: str = "namespaces/{namespace}/properties"
     list_tables: str = "namespaces/{namespace}/tables"
     create_table: str = "namespaces/{namespace}/tables"
     load_table: str = "namespaces/{namespace}/tables/{table}"
     update_table: str = "namespaces/{namespace}/tables/{table}"
     drop_table: str = "namespaces/{namespace}/tables/{table}?purgeRequested={purge}"
     table_exists: str = "namespaces/{namespace}/tables/{table}"
     get_token: str = "oauth/tokens"
@@ -92,14 +100,17 @@
 TOKEN_EXCHANGE = "urn:ietf:params:oauth:grant-type:token-exchange"
 SEMICOLON = ":"
 KEY = "key"
 CERT = "cert"
 CLIENT = "client"
 CA_BUNDLE = "cabundle"
 SSL = "ssl"
+SIGV4 = "rest.sigv4-enabled"
+SIGV4_REGION = "rest.signing-region"
+SIGV4_SERVICE = "rest.signing-name"
 
 NAMESPACE_SEPARATOR = b"\x1F".decode("UTF-8")
 
 
 class TableResponse(IcebergBaseModel):
     metadata_location: str = Field(alias="metadata-location")
     metadata: TableMetadata = Field()
@@ -168,120 +179,125 @@
     ]
     error_description: Optional[str]
     error_uri: Optional[str]
 
 
 class RestCatalog(Catalog):
     uri: str
-    session: Session
-    properties: Properties
+    _session: Session
 
-    def __init__(
-        self,
-        name: str,
-        **properties: str,
-    ):
-        """Rest Catalog
+    def __init__(self, name: str, **properties: str):
+        """Rest Catalog.
 
         You either need to provide a client_id and client_secret, or an already valid token.
 
         Args:
-            name: Name to identify the catalog
-            properties: Properties that are passed along to the configuration
+            name: Name to identify the catalog.
+            properties: Properties that are passed along to the configuration.
         """
-        self.properties = properties
+        super().__init__(name, **properties)
         self.uri = properties[URI]
-        self._create_session()
-        super().__init__(name, **self._fetch_config(properties))
+        self._fetch_config()
+        self._session = self._create_session()
 
-    def _create_session(self) -> None:
-        """Creates a request session with provided catalog configuration"""
+    def _create_session(self) -> Session:
+        """Creates a request session with provided catalog configuration."""
+        session = Session()
 
-        self.session = Session()
         # Sets the client side and server side SSL cert verification, if provided as properties.
         if ssl_config := self.properties.get(SSL):
             if ssl_ca_bundle := ssl_config.get(CA_BUNDLE):  # type: ignore
-                self.session.verify = ssl_ca_bundle
+                session.verify = ssl_ca_bundle
             if ssl_client := ssl_config.get(CLIENT):  # type: ignore
                 if all(k in ssl_client for k in (CERT, KEY)):
-                    self.session.cert = (ssl_client[CERT], ssl_client[KEY])
+                    session.cert = (ssl_client[CERT], ssl_client[KEY])
                 elif ssl_client_cert := ssl_client.get(CERT):
-                    self.session.cert = ssl_client_cert
+                    session.cert = ssl_client_cert
 
         # If we have credentials, but not a token, we want to fetch a token
         if TOKEN not in self.properties and CREDENTIAL in self.properties:
-            self.properties[TOKEN] = self._fetch_access_token(self.properties[CREDENTIAL])
+            self.properties[TOKEN] = self._fetch_access_token(session, self.properties[CREDENTIAL])
 
         # Set Auth token for subsequent calls in the session
         if token := self.properties.get(TOKEN):
-            self.session.headers[AUTHORIZATION_HEADER] = f"{BEARER_PREFIX} {token}"
+            session.headers[AUTHORIZATION_HEADER] = f"{BEARER_PREFIX} {token}"
 
         # Set HTTP headers
-        self.session.headers["Content-type"] = "application/json"
-        self.session.headers["X-Client-Version"] = ICEBERG_REST_SPEC_VERSION
-        self.session.headers["User-Agent"] = f"PyIceberg/{__version__}"
+        session.headers["Content-type"] = "application/json"
+        session.headers["X-Client-Version"] = ICEBERG_REST_SPEC_VERSION
+        session.headers["User-Agent"] = f"PyIceberg/{__version__}"
+
+        # Configure SigV4 Request Signing
+        if str(self.properties.get(SIGV4, False)).lower() == "true":
+            self._init_sigv4(session)
+
+        return session
 
     def _check_valid_namespace_identifier(self, identifier: Union[str, Identifier]) -> Identifier:
-        """The identifier should have at least one element"""
+        """The identifier should have at least one element."""
         identifier_tuple = Catalog.identifier_to_tuple(identifier)
         if len(identifier_tuple) < 1:
             raise NoSuchNamespaceError(f"Empty namespace identifier: {identifier}")
         return identifier_tuple
 
     def url(self, endpoint: str, prefixed: bool = True, **kwargs: Any) -> str:
-        """Constructs the endpoint
+        """Constructs the endpoint.
 
         Args:
-            endpoint: Resource identifier that points to the REST catalog
-            prefixed: If the prefix return by the config needs to be appended
+            endpoint: Resource identifier that points to the REST catalog.
+            prefixed: If the prefix return by the config needs to be appended.
 
         Returns:
-            The base url of the rest catalog
+            The base url of the rest catalog.
         """
-
         url = self.uri
         url = url + "v1/" if url.endswith("/") else url + "/v1/"
 
         if prefixed:
             url += self.properties.get(PREFIX, "")
             url = url if url.endswith("/") else url + "/"
 
         return url + endpoint.format(**kwargs)
 
-    def _fetch_access_token(self, credential: str) -> str:
+    def _fetch_access_token(self, session: Session, credential: str) -> str:
         if SEMICOLON in credential:
             client_id, client_secret = credential.split(SEMICOLON)
         else:
             client_id, client_secret = None, credential
         data = {GRANT_TYPE: CLIENT_CREDENTIALS, CLIENT_ID: client_id, CLIENT_SECRET: client_secret, SCOPE: CATALOG_SCOPE}
         url = self.url(Endpoints.get_token, prefixed=False)
         # Uses application/x-www-form-urlencoded by default
-        response = self.session.post(url=url, data=data)
+        response = session.post(url=url, data=data)
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {400: OAuthError, 401: OAuthError})
 
         return TokenResponse(**response.json()).access_token
 
-    def _fetch_config(self, properties: Properties) -> Properties:
+    def _fetch_config(self) -> None:
         params = {}
-        if warehouse_location := properties.get(WAREHOUSE_LOCATION):
+        if warehouse_location := self.properties.get(WAREHOUSE_LOCATION):
             params[WAREHOUSE_LOCATION] = warehouse_location
 
-        response = self.session.get(self.url(Endpoints.get_config, prefixed=False), params=params)
+        with self._create_session() as session:
+            response = session.get(self.url(Endpoints.get_config, prefixed=False), params=params)
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {})
         config_response = ConfigResponse(**response.json())
+
         config = config_response.defaults
-        config.update(properties)
+        config.update(self.properties)
         config.update(config_response.overrides)
-        return config
+        self.properties = config
+
+        # Update URI based on overrides
+        self.uri = config[URI]
 
     def _split_identifier_for_path(self, identifier: Union[str, Identifier]) -> Properties:
         identifier_tuple = self.identifier_to_tuple(identifier)
         if len(identifier_tuple) <= 1:
             raise NoSuchTableError(f"Missing namespace or invalid identifier: {'.'.join(identifier_tuple)}")
         return {"namespace": NAMESPACE_SEPARATOR.join(identifier_tuple[:-1]), "table": identifier_tuple[-1]}
 
@@ -335,14 +351,71 @@
             errs = ", ".join(err["msg"] for err in e.errors())
             response = (
                 f"RESTError {exc.response.status_code}: Received unexpected JSON Payload: {exc.response.text}, errors: {errs}"
             )
 
         raise exception(response) from exc
 
+    def _init_sigv4(self, session: Session) -> None:
+        from urllib import parse
+
+        import boto3
+        from botocore.auth import SigV4Auth
+        from botocore.awsrequest import AWSRequest
+        from requests import PreparedRequest
+        from requests.adapters import HTTPAdapter
+
+        class SigV4Adapter(HTTPAdapter):
+            def __init__(self, **properties: str):
+                super().__init__()
+                self._properties = properties
+
+            def add_headers(self, request: PreparedRequest, **kwargs: Any) -> None:  # pylint: disable=W0613
+                boto_session = boto3.Session()
+                credentials = boto_session.get_credentials().get_frozen_credentials()
+                region = self._properties.get(SIGV4_REGION, boto_session.region_name)
+                service = self._properties.get(SIGV4_SERVICE, "execute-api")
+
+                url = str(request.url).split("?")[0]
+                query = str(parse.urlsplit(request.url).query)
+                params = dict(parse.parse_qsl(query))
+
+                # remove the connection header as it will be updated after signing
+                del request.headers["connection"]
+
+                aws_request = AWSRequest(
+                    method=request.method, url=url, params=params, data=request.body, headers=dict(request.headers)
+                )
+
+                SigV4Auth(credentials, service, region).add_auth(aws_request)
+                original_header = request.headers
+                signed_headers = aws_request.headers
+                relocated_headers = {}
+
+                # relocate headers if there is a conflict with signed headers
+                for header, value in original_header.items():
+                    if header in signed_headers and signed_headers[header] != value:
+                        relocated_headers[f"Original-{header}"] = value
+
+                request.headers.update(relocated_headers)
+                request.headers.update(signed_headers)
+
+        session.mount(self.uri, SigV4Adapter(**self.properties))
+
+    def _response_to_table(self, identifier_tuple: Tuple[str, ...], table_response: TableResponse) -> Table:
+        return Table(
+            identifier=(self.name,) + identifier_tuple if self.name else identifier_tuple,
+            metadata_location=table_response.metadata_location,
+            metadata=table_response.metadata,
+            io=self._load_file_io(
+                {**table_response.metadata.properties, **table_response.config}, table_response.metadata_location
+            ),
+            catalog=self,
+        )
+
     def create_table(
         self,
         identifier: Union[str, Identifier],
         schema: Schema,
         location: Optional[str] = None,
         partition_spec: PartitionSpec = UNPARTITIONED_PARTITION_SPEC,
         sort_order: SortOrder = UNSORTED_SORT_ORDER,
@@ -354,64 +427,53 @@
             location=location,
             table_schema=schema,
             partition_spec=partition_spec,
             write_order=sort_order,
             properties=properties,
         )
         serialized_json = request.json()
-        response = self.session.post(
+        response = self._session.post(
             self.url(Endpoints.create_table, namespace=namespace_and_table["namespace"]),
             data=serialized_json,
         )
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {409: TableAlreadyExistsError})
 
         table_response = TableResponse(**response.json())
-
-        return Table(
-            identifier=(self.name,) + self.identifier_to_tuple(identifier),
-            metadata_location=table_response.metadata_location,
-            metadata=table_response.metadata,
-            io=self._load_file_io({**table_response.metadata.properties, **table_response.config}),
-        )
+        return self._response_to_table(self.identifier_to_tuple(identifier), table_response)
 
     def list_tables(self, namespace: Union[str, Identifier]) -> List[Identifier]:
         namespace_tuple = self._check_valid_namespace_identifier(namespace)
         namespace_concat = NAMESPACE_SEPARATOR.join(namespace_tuple)
-        response = self.session.get(self.url(Endpoints.list_tables, namespace=namespace_concat))
+        response = self._session.get(self.url(Endpoints.list_tables, namespace=namespace_concat))
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchNamespaceError})
         return [(*table.namespace, table.name) for table in ListTablesResponse(**response.json()).identifiers]
 
     def load_table(self, identifier: Union[str, Identifier]) -> Table:
         identifier_tuple = self.identifier_to_tuple(identifier)
 
         if len(identifier_tuple) <= 1:
             raise NoSuchTableError(f"Missing namespace or invalid identifier: {identifier}")
 
-        response = self.session.get(self.url(Endpoints.load_table, prefixed=True, **self._split_identifier_for_path(identifier)))
+        response = self._session.get(self.url(Endpoints.load_table, prefixed=True, **self._split_identifier_for_path(identifier)))
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchTableError})
 
         table_response = TableResponse(**response.json())
-        return Table(
-            identifier=(self.name,) + identifier_tuple if self.name else identifier_tuple,
-            metadata_location=table_response.metadata_location,
-            metadata=table_response.metadata,
-            io=self._load_file_io({**table_response.metadata.properties, **table_response.config}),
-        )
+        return self._response_to_table(identifier_tuple, table_response)
 
     def drop_table(self, identifier: Union[str, Identifier], purge_requested: bool = False) -> None:
-        response = self.session.delete(
+        response = self._session.delete(
             self.url(Endpoints.drop_table, prefixed=True, purge=purge_requested, **self._split_identifier_for_path(identifier)),
         )
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchTableError})
 
@@ -419,43 +481,73 @@
         self.drop_table(identifier=identifier, purge_requested=True)
 
     def rename_table(self, from_identifier: Union[str, Identifier], to_identifier: Union[str, Identifier]) -> Table:
         payload = {
             "source": self._split_identifier_for_json(from_identifier),
             "destination": self._split_identifier_for_json(to_identifier),
         }
-        response = self.session.post(self.url(Endpoints.rename_table), json=payload)
+        response = self._session.post(self.url(Endpoints.rename_table), json=payload)
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchTableError, 409: TableAlreadyExistsError})
 
         return self.load_table(to_identifier)
 
+    def _commit_table(self, table_request: CommitTableRequest) -> CommitTableResponse:
+        """Updates the table.
+
+        Args:
+            table_request (CommitTableRequest): The table requests to be carried out.
+
+        Returns:
+            CommitTableResponse: The updated metadata.
+
+        Raises:
+            NoSuchTableError: If a table with the given identifier does not exist.
+        """
+        response = self._session.post(
+            self.url(Endpoints.update_table, prefixed=True, **self._split_identifier_for_path(table_request.identifier)),
+            data=table_request.json(),
+        )
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            self._handle_non_200_response(
+                exc,
+                {
+                    409: CommitFailedException,
+                    500: CommitStateUnknownException,
+                    502: CommitStateUnknownException,
+                    504: CommitStateUnknownException,
+                },
+            )
+        return CommitTableResponse(**response.json())
+
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         namespace_tuple = self._check_valid_namespace_identifier(namespace)
         payload = {"namespace": namespace_tuple, "properties": properties}
-        response = self.session.post(self.url(Endpoints.create_namespace), json=payload)
+        response = self._session.post(self.url(Endpoints.create_namespace), json=payload)
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchNamespaceError, 409: NamespaceAlreadyExistsError})
 
     def drop_namespace(self, namespace: Union[str, Identifier]) -> None:
         namespace_tuple = self._check_valid_namespace_identifier(namespace)
         namespace = NAMESPACE_SEPARATOR.join(namespace_tuple)
-        response = self.session.delete(self.url(Endpoints.drop_namespace, namespace=namespace))
+        response = self._session.delete(self.url(Endpoints.drop_namespace, namespace=namespace))
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchNamespaceError})
 
     def list_namespaces(self, namespace: Union[str, Identifier] = ()) -> List[Identifier]:
         namespace_tuple = self.identifier_to_tuple(namespace)
-        response = self.session.get(
+        response = self._session.get(
             self.url(
                 f"{Endpoints.list_namespaces}?parent={NAMESPACE_SEPARATOR.join(namespace_tuple)}"
                 if namespace_tuple
                 else Endpoints.list_namespaces
             ),
         )
         try:
@@ -465,29 +557,29 @@
 
         namespaces = ListNamespaceResponse(**response.json())
         return [namespace_tuple + child_namespace for child_namespace in namespaces.namespaces]
 
     def load_namespace_properties(self, namespace: Union[str, Identifier]) -> Properties:
         namespace_tuple = self._check_valid_namespace_identifier(namespace)
         namespace = NAMESPACE_SEPARATOR.join(namespace_tuple)
-        response = self.session.get(self.url(Endpoints.load_namespace_metadata, namespace=namespace))
+        response = self._session.get(self.url(Endpoints.load_namespace_metadata, namespace=namespace))
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchNamespaceError})
 
         return NamespaceResponse(**response.json()).properties
 
     def update_namespace_properties(
         self, namespace: Union[str, Identifier], removals: Optional[Set[str]] = None, updates: Properties = EMPTY_DICT
     ) -> PropertiesUpdateSummary:
         namespace_tuple = self._check_valid_namespace_identifier(namespace)
         namespace = NAMESPACE_SEPARATOR.join(namespace_tuple)
         payload = {"removals": list(removals or []), "updates": updates}
-        response = self.session.post(self.url(Endpoints.update_properties, namespace=namespace), json=payload)
+        response = self._session.post(self.url(Endpoints.update_namespace_properties, namespace=namespace), json=payload)
         try:
             response.raise_for_status()
         except HTTPError as exc:
             self._handle_non_200_response(exc, {404: NoSuchNamespaceError})
         parsed_response = UpdateNamespacePropertiesResponse(**response.json())
         return PropertiesUpdateSummary(
             removed=parsed_response.removed,
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/cli/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/cli/console.py` & `pyiceberg-0.4.0rc1/pyiceberg/cli/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,21 +46,21 @@
 
         return wrapper
 
     return decorator
 
 
 @click.group()
-@click.option("--catalog", default="default")
+@click.option("--catalog")
 @click.option("--verbose", type=click.BOOL)
 @click.option("--output", type=click.Choice(["text", "json"]), default="text")
 @click.option("--uri")
 @click.option("--credential")
 @click.pass_context
-def run(ctx: Context, catalog: str, verbose: bool, output: str, uri: Optional[str], credential: Optional[str]) -> None:
+def run(ctx: Context, catalog: Optional[str], verbose: bool, output: str, uri: Optional[str], credential: Optional[str]) -> None:
     properties = {}
     if uri:
         properties["uri"] = uri
     if credential:
         properties["credential"] = credential
 
     ctx.ensure_object(dict)
@@ -79,41 +79,39 @@
         ctx.obj["output"].exception(
             ValueError("Could not determine catalog type from uri. REST (http/https) and Hive (thrift) is supported")
         )
         ctx.exit(1)
 
 
 def _catalog_and_output(ctx: Context) -> Tuple[Catalog, Output]:
-    """
-    Small helper to set the types
-    """
+    """Small helper to set the types."""
     return ctx.obj["catalog"], ctx.obj["output"]
 
 
 @run.command()
 @click.pass_context
 @click.argument("parent", required=False)
 @catch_exception()
 def list(ctx: Context, parent: Optional[str]) -> None:  # pylint: disable=redefined-builtin
-    """Lists tables or namespaces"""
+    """Lists tables or namespaces."""
     catalog, output = _catalog_and_output(ctx)
 
     identifiers = catalog.list_namespaces(parent or ())
     if not identifiers and parent:
         identifiers = catalog.list_tables(parent)
     output.identifiers(identifiers)
 
 
 @run.command()
 @click.option("--entity", type=click.Choice(["any", "namespace", "table"]), default="any")
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def describe(ctx: Context, entity: Literal["name", "namespace", "table"], identifier: str) -> None:
-    """Describes a namespace or a table"""
+    """Describes a namespace or a table."""
     catalog, output = _catalog_and_output(ctx)
     identifier_tuple = Catalog.identifier_to_tuple(identifier)
 
     is_namespace = False
     if entity in {"namespace", "any"} and len(identifier_tuple) > 0:
         try:
             namespace_properties = catalog.load_namespace_properties(identifier_tuple)
@@ -139,124 +137,124 @@
 
 @run.command()
 @click.argument("identifier")
 @click.option("--history", is_flag=True)
 @click.pass_context
 @catch_exception()
 def files(ctx: Context, identifier: str, history: bool) -> None:
-    """Lists all the files of the table"""
+    """Lists all the files of the table."""
     catalog, output = _catalog_and_output(ctx)
 
     catalog_table = catalog.load_table(identifier)
     output.files(catalog_table, history)
 
 
 @run.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def schema(ctx: Context, identifier: str) -> None:
-    """Gets the schema of the table"""
+    """Gets the schema of the table."""
     catalog, output = _catalog_and_output(ctx)
     table = catalog.load_table(identifier)
     output.schema(table.schema())
 
 
 @run.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def spec(ctx: Context, identifier: str) -> None:
-    """Returns the partition spec of the table"""
+    """Returns the partition spec of the table."""
     catalog, output = _catalog_and_output(ctx)
     table = catalog.load_table(identifier)
     output.spec(table.spec())
 
 
 @run.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def uuid(ctx: Context, identifier: str) -> None:
-    """Returns the UUID of the table"""
+    """Returns the UUID of the table."""
     catalog, output = _catalog_and_output(ctx)
     metadata = catalog.load_table(identifier).metadata
     output.uuid(metadata.table_uuid)
 
 
 @run.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def location(ctx: Context, identifier: str) -> None:
-    """Returns the location of the table"""
+    """Returns the location of the table."""
     catalog, output = _catalog_and_output(ctx)
     table = catalog.load_table(identifier)
     output.text(table.location())
 
 
 @run.group()
 def drop() -> None:
-    """Operations to drop a namespace or table"""
+    """Operations to drop a namespace or table."""
 
 
 @drop.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def table(ctx: Context, identifier: str) -> None:  # noqa: F811
-    """Drops a table"""
+    """Drops a table."""
     catalog, output = _catalog_and_output(ctx)
 
     catalog.drop_table(identifier)
     output.text(f"Dropped table: {identifier}")
 
 
 @drop.command()
 @click.argument("identifier")
 @click.pass_context
 @catch_exception()
 def namespace(ctx: Context, identifier: str) -> None:
-    """Drops a namespace"""
+    """Drops a namespace."""
     catalog, output = _catalog_and_output(ctx)
 
     catalog.drop_namespace(identifier)
     output.text(f"Dropped namespace: {identifier}")
 
 
 @run.command()
 @click.argument("from_identifier")
 @click.argument("to_identifier")
 @click.pass_context
 @catch_exception()
 def rename(ctx: Context, from_identifier: str, to_identifier: str) -> None:
-    """Renames a table"""
+    """Renames a table."""
     catalog, output = _catalog_and_output(ctx)
 
     catalog.rename_table(from_identifier, to_identifier)
     output.text(f"Renamed table from {from_identifier} to {to_identifier}")
 
 
 @run.group()
 def properties() -> None:
-    """Properties on tables/namespaces"""
+    """Properties on tables/namespaces."""
 
 
 @properties.group()
 def get() -> None:
-    """Fetch properties on tables/namespaces"""
+    """Fetch properties on tables/namespaces."""
 
 
 @get.command("namespace")
 @click.argument("identifier")
 @click.argument("property_name", required=False)
 @click.pass_context
 @catch_exception()
 def get_namespace(ctx: Context, identifier: str, property_name: str) -> None:
-    """Fetch properties on a namespace"""
+    """Fetch properties on a namespace."""
     catalog, output = _catalog_and_output(ctx)
     identifier_tuple = Catalog.identifier_to_tuple(identifier)
 
     namespace_properties = catalog.load_namespace_properties(identifier_tuple)
     assert namespace_properties
 
     if property_name:
@@ -270,15 +268,15 @@
 
 @get.command("table")
 @click.argument("identifier")
 @click.argument("property_name", required=False)
 @click.pass_context
 @catch_exception()
 def get_table(ctx: Context, identifier: str, property_name: str) -> None:
-    """Fetch properties on a table"""
+    """Fetch properties on a table."""
     catalog, output = _catalog_and_output(ctx)
     identifier_tuple = Catalog.identifier_to_tuple(identifier)
 
     metadata = catalog.load_table(identifier_tuple).metadata
     assert metadata
 
     if property_name:
@@ -288,59 +286,59 @@
             raise NoSuchPropertyException(f"Could not find property {property_name} on table {identifier}")
     else:
         output.describe_properties(metadata.properties)
 
 
 @properties.group()
 def set() -> None:
-    """Sets a property on tables/namespaces"""
+    """Sets a property on tables/namespaces."""
 
 
 @set.command()  # type: ignore
 @click.argument("identifier")
 @click.argument("property_name")
 @click.argument("property_value")
 @click.pass_context
 @catch_exception()
 def namespace(ctx: Context, identifier: str, property_name: str, property_value: str) -> None:  # noqa: F811
-    """Sets a property on a namespace"""
+    """Sets a property on a namespace."""
     catalog, output = _catalog_and_output(ctx)
 
     catalog.update_namespace_properties(identifier, updates={property_name: property_value})
     output.text(f"Updated {property_name} on {identifier}")
 
 
 @set.command()  # type: ignore
 @click.argument("identifier")
 @click.argument("property_name")
 @click.argument("property_value")
 @click.pass_context
 @catch_exception()
 def table(ctx: Context, identifier: str, property_name: str, property_value: str) -> None:  # noqa: F811
-    """Sets a property on a table"""
+    """Sets a property on a table."""
     catalog, output = _catalog_and_output(ctx)
     identifier_tuple = Catalog.identifier_to_tuple(identifier)
 
     _ = catalog.load_table(identifier_tuple)
     output.text(f"Setting {property_name}={property_value} on {identifier}")
     raise NotImplementedError("Writing is WIP")
 
 
 @properties.group()
 def remove() -> None:
-    """Removes a property from tables/namespaces"""
+    """Removes a property from tables/namespaces."""
 
 
 @remove.command()  # type: ignore
 @click.argument("identifier")
 @click.argument("property_name")
 @click.pass_context
 @catch_exception()
 def namespace(ctx: Context, identifier: str, property_name: str) -> None:  # noqa: F811
-    """Removes a property from a namespace"""
+    """Removes a property from a namespace."""
     catalog, output = _catalog_and_output(ctx)
 
     result = catalog.update_namespace_properties(identifier, removals={property_name})
 
     if result.removed == [property_name]:
         output.text(f"Property {property_name} removed from {identifier}")
     else:
@@ -349,15 +347,15 @@
 
 @remove.command()  # type: ignore
 @click.argument("identifier")
 @click.argument("property_name")
 @click.pass_context
 @catch_exception()
 def table(ctx: Context, identifier: str, property_name: str) -> None:  # noqa: F811
-    """Removes a property from a table"""
+    """Removes a property from a table."""
     catalog, output = _catalog_and_output(ctx)
     table = catalog.load_table(identifier)
     if property_name in table.metadata.properties:
         # We should think of the process here
         # Do we want something similar as in Java:
         # https://github.com/apache/iceberg/blob/master/api/src/main/java/org/apache/iceberg/Table.java#L178
         del table.metadata.properties
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/cli/output.py` & `pyiceberg-0.4.0rc1/pyiceberg/cli/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from pyiceberg.partitioning import PartitionSpec
 from pyiceberg.schema import Schema
 from pyiceberg.table import Table, TableMetadata
 from pyiceberg.typedef import IcebergBaseModel, Identifier, Properties
 
 
 class Output(ABC):
-    """Output interface for exporting"""
+    """Output interface for exporting."""
 
     @abstractmethod
     def exception(self, ex: Exception) -> None:
         ...
 
     @abstractmethod
     def identifiers(self, identifiers: List[Identifier]) -> None:
@@ -66,15 +66,15 @@
 
     @abstractmethod
     def uuid(self, uuid: Optional[UUID]) -> None:
         ...
 
 
 class ConsoleOutput(Output):
-    """Writes to the console"""
+    """Writes to the console."""
 
     verbose: bool
 
     def __init__(self, **properties: Any) -> None:
         self.verbose = properties.get("verbose", False)
 
     @property
@@ -138,15 +138,15 @@
         for snapshot in snapshots:
             manifest_list_str = f": {snapshot.manifest_list}" if snapshot.manifest_list else ""
             list_tree = snapshot_tree.add(f"Snapshot {snapshot.snapshot_id}, schema {snapshot.schema_id}{manifest_list_str}")
 
             manifest_list = snapshot.manifests(io)
             for manifest in manifest_list:
                 manifest_tree = list_tree.add(f"Manifest: {manifest.manifest_path}")
-                for manifest_entry in manifest.fetch_manifest_entry(io):
+                for manifest_entry in manifest.fetch_manifest_entry(io, discard_deleted=False):
                     manifest_tree.add(f"Datafile: {manifest_entry.data_file.file_path}")
         Console().print(snapshot_tree)
 
     def describe_properties(self, properties: Properties) -> None:
         output_table = self._table
         for k, v in properties.items():
             output_table.add_row(k, v)
@@ -165,15 +165,15 @@
         Console().print(str(spec))
 
     def uuid(self, uuid: Optional[UUID]) -> None:
         Console().print(str(uuid) if uuid else "missing")
 
 
 class JsonOutput(Output):
-    """Writes json to stdout"""
+    """Writes json to stdout."""
 
     verbose: bool
 
     def __init__(self, **properties: Any) -> None:
         self.verbose = properties.get("verbose", False)
 
     def _out(self, d: Any) -> None:
@@ -183,15 +183,15 @@
         self._out({"type": ex.__class__.__name__, "message": str(ex)})
 
     def identifiers(self, identifiers: List[Identifier]) -> None:
         self._out([".".join(identifier) for identifier in identifiers])
 
     def describe_table(self, table: Table) -> None:
         class FauxTable(IcebergBaseModel):
-            """Just to encode it using Pydantic"""
+            """Just to encode it using Pydantic."""
 
             identifier: Identifier
             metadata_location: str
             metadata: TableMetadata
 
         print(FauxTable(identifier=table.identifier, metadata=table.metadata, metadata_location=table.metadata_location).json())
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/conversions.py` & `pyiceberg-0.4.0rc1/pyiceberg/conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Utility module for various conversions around PrimitiveType implementations
+"""Utility module for various conversions around PrimitiveType implementations.
 
 This module enables:
-    - Converting partition strings to built-in python objects
-    - Converting a value to a byte buffer
-    - Converting a byte buffer to a value
+    - Converting partition strings to built-in python objects.
+    - Converting a value to a byte buffer.
+    - Converting a byte buffer to a value.
 
 Note:
     Conversion logic varies based on the PrimitiveType implementation. Therefore conversion functions
     are defined here as generic functions using the @singledispatch decorator. For each PrimitiveType
     implementation, a concrete function is registered for each generic conversion function. For PrimitiveType
     implementations that share the same conversion logic, registrations can be stacked.
 """
@@ -34,14 +34,15 @@
 from typing import (
     Any,
     Callable,
     Optional,
     Union,
 )
 
+from pyiceberg.typedef import L
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DecimalType,
     DoubleType,
     FixedType,
@@ -62,37 +63,37 @@
 _LONG_STRUCT = Struct("<q")
 _FLOAT_STRUCT = Struct("<f")
 _DOUBLE_STRUCT = Struct("<d")
 _UUID_STRUCT = Struct(">QQ")
 
 
 def handle_none(func: Callable) -> Callable:  # type: ignore
-    """A decorator function to handle cases where partition values are `None` or "__HIVE_DEFAULT_PARTITION__"
+    """A decorator function to handle cases where partition values are `None` or "__HIVE_DEFAULT_PARTITION__".
 
     Args:
-        func (Callable): A function registered to the singledispatch function `partition_to_py`
+        func (Callable): A function registered to the singledispatch function `partition_to_py`.
     """
 
     def wrapper(primitive_type: PrimitiveType, value_str: Optional[str]) -> Any:
         if value_str is None:
             return None
         elif value_str == "__HIVE_DEFAULT_PARTITION__":
             return None
         return func(primitive_type, value_str)
 
     return wrapper
 
 
 @singledispatch
 def partition_to_py(primitive_type: PrimitiveType, value_str: str) -> Union[int, float, str, uuid.UUID, bytes, Decimal]:
-    """A generic function which converts a partition string to a python built-in
+    """A generic function which converts a partition string to a python built-in.
 
     Args:
-        primitive_type(PrimitiveType): An implementation of the PrimitiveType base class
-        value_str(str): A string representation of a partition value
+        primitive_type (PrimitiveType): An implementation of the PrimitiveType base class.
+        value_str (str): A string representation of a partition value.
     """
     raise TypeError(f"Cannot convert '{value_str}' to unsupported type: {primitive_type}")
 
 
 @partition_to_py.register(BooleanType)
 @handle_none
 def _(primitive_type: BooleanType, value_str: str) -> Union[int, float, str, uuid.UUID]:
@@ -103,17 +104,18 @@
 @partition_to_py.register(LongType)
 @partition_to_py.register(DateType)
 @partition_to_py.register(TimeType)
 @partition_to_py.register(TimestampType)
 @partition_to_py.register(TimestamptzType)
 @handle_none
 def _(primitive_type: PrimitiveType, value_str: str) -> int:
-    """
+    """Converts a string to an integer value.
+
     Raises:
-        ValueError: If the scale/exponent is not 0
+        ValueError: If the scale/exponent is not 0.
     """
     _, _, exponent = Decimal(value_str).as_tuple()
     if exponent != 0:  # Raise if there are digits to the right of the decimal
         raise ValueError(f"Cannot convert partition value, value cannot have fractional digits for {primitive_type} partition")
     return int(float(value_str))
 
 
@@ -147,23 +149,23 @@
 @handle_none
 def _(_: DecimalType, value_str: str) -> Decimal:
     return Decimal(value_str)
 
 
 @singledispatch
 def to_bytes(primitive_type: PrimitiveType, _: Union[bool, bytes, Decimal, float, int, str, uuid.UUID]) -> bytes:
-    """A generic function which converts a built-in python value to bytes
+    """A generic function which converts a built-in python value to bytes.
 
     This conversion follows the serialization scheme for storing single values as individual binary values defined in the Iceberg specification that
     can be found at https://iceberg.apache.org/spec/#appendix-d-single-value-serialization
 
     Args:
-        primitive_type(PrimitiveType): An implementation of the PrimitiveType base class
+        primitive_type (PrimitiveType): An implementation of the PrimitiveType base class.
         _: The value to convert to bytes (The type of this value depends on which dispatched function is
-            used--check dispatchable functions for type hints)
+            used--check dispatchable functions for type hints).
     """
     raise TypeError(f"scale does not match {primitive_type}")
 
 
 @to_bytes.register(BooleanType)
 def _(_: BooleanType, value: bool) -> bytes:
     return _BOOL_STRUCT.pack(1 if value else 0)
@@ -181,15 +183,16 @@
 @to_bytes.register(TimestamptzType)
 def _(_: PrimitiveType, value: int) -> bytes:
     return _LONG_STRUCT.pack(value)
 
 
 @to_bytes.register(FloatType)
 def _(_: FloatType, value: float) -> bytes:
-    """
+    """Converts a float value into bytes.
+
     Note: float in python is implemented using a double in C. Therefore this involves a conversion of a 32-bit (single precision)
     float to a 64-bit (double precision) float which introduces some imprecision.
     """
     return _FLOAT_STRUCT.pack(value)
 
 
 @to_bytes.register(DoubleType)
@@ -211,46 +214,46 @@
 @to_bytes.register(FixedType)
 def _(_: PrimitiveType, value: bytes) -> bytes:
     return value
 
 
 @to_bytes.register(DecimalType)
 def _(primitive_type: DecimalType, value: Decimal) -> bytes:
-    """Convert a Decimal value to bytes given a DecimalType instance with defined precision and scale
+    """Convert a Decimal value to bytes given a DecimalType instance with defined precision and scale.
 
     Args:
-        primitive_type (DecimalType): A DecimalType instance with precision and scale
-        value (Decimal): A Decimal instance
+        primitive_type (DecimalType): A DecimalType instance with precision and scale.
+        value (Decimal): A Decimal instance.
 
     Raises:
-        ValueError: If either the precision or scale of `value` does not match that defined in the DecimalType instance
+        ValueError: If either the precision or scale of `value` does not match that defined in the DecimalType instance.
 
 
     Returns:
-        bytes: The byte representation of `value`
+        bytes: The byte representation of `value`.
     """
     _, digits, exponent = value.as_tuple()
-
-    if -exponent != primitive_type.scale:
-        raise ValueError(f"Cannot serialize value, scale of value does not match type {primitive_type}: {-exponent}")
+    exponent = abs(int(exponent))
+    if exponent != primitive_type.scale:
+        raise ValueError(f"Cannot serialize value, scale of value does not match type {primitive_type}: {exponent}")
     elif len(digits) > primitive_type.precision:
         raise ValueError(
             f"Cannot serialize value, precision of value is greater than precision of type {primitive_type}: {len(digits)}"
         )
 
     return decimal_to_bytes(value)
 
 
 @singledispatch
-def from_bytes(primitive_type: PrimitiveType, b: bytes) -> Union[bool, bytes, Decimal, float, int, str, uuid.UUID]:
-    """A generic function which converts bytes to a built-in python value
+def from_bytes(primitive_type: PrimitiveType, b: bytes) -> L:
+    """A generic function which converts bytes to a built-in python value.
 
     Args:
-        primitive_type(PrimitiveType): An implementation of the PrimitiveType base class
-        b(bytes): The bytes to convert
+        primitive_type (PrimitiveType): An implementation of the PrimitiveType base class.
+        b (bytes): The bytes to convert.
     """
     raise TypeError(f"Cannot deserialize bytes, type {primitive_type} not supported: {str(b)}")
 
 
 @from_bytes.register(BooleanType)
 def _(_: BooleanType, b: bytes) -> bool:
     return _BOOL_STRUCT.unpack(b)[0] != 0
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/exceptions.py` & `pyiceberg-0.4.0rc1/pyiceberg/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,80 +13,100 @@
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 
 class TableAlreadyExistsError(Exception):
-    """Raised when creating a table with a name that already exists"""
+    """Raised when creating a table with a name that already exists."""
 
 
 class NamespaceNotEmptyError(Exception):
-    """Raised when a name-space being dropped is not empty"""
+    """Raised when a name-space being dropped is not empty."""
 
 
 class NamespaceAlreadyExistsError(Exception):
-    """Raised when a name-space being created already exists in the catalog"""
+    """Raised when a name-space being created already exists in the catalog."""
 
 
 class ValidationError(Exception):
-    """Raises when there is an issue with the schema"""
+    """Raises when there is an issue with the schema."""
 
 
 class NoSuchTableError(Exception):
-    """Raises when the table can't be found in the REST catalog"""
+    """Raises when the table can't be found in the REST catalog."""
 
 
 class NoSuchIcebergTableError(NoSuchTableError):
-    """Raises when the table found in the REST catalog is not an iceberg table"""
+    """Raises when the table found in the REST catalog is not an iceberg table."""
 
 
 class NoSuchNamespaceError(Exception):
-    """Raised when a referenced name-space is not found"""
+    """Raised when a referenced name-space is not found."""
 
 
 class RESTError(Exception):
-    """Raises when there is an unknown response from the REST Catalog"""
+    """Raises when there is an unknown response from the REST Catalog."""
 
 
 class BadRequestError(RESTError):
-    """Raises when an invalid request is being made"""
+    """Raises when an invalid request is being made."""
 
 
 class UnauthorizedError(RESTError):
-    """Raises when you don't have the proper authorization"""
+    """Raises when you don't have the proper authorization."""
 
 
 class ServiceUnavailableError(RESTError):
-    """Raises when the service doesn't respond"""
+    """Raises when the service doesn't respond."""
 
 
 class ServerError(RESTError):
-    """Raises when there is an unhandled exception on the server side"""
+    """Raises when there is an unhandled exception on the server side."""
 
 
 class ForbiddenError(RESTError):
-    """Raises when you don't have the credentials to perform the action on the REST catalog"""
+    """Raises when you don't have the credentials to perform the action on the REST catalog."""
 
 
 class AuthorizationExpiredError(RESTError):
-    """When the credentials are expired when performing an action on the REST catalog"""
+    """When the credentials are expired when performing an action on the REST catalog."""
 
 
 class OAuthError(RESTError):
-    """Raises when there is an error with the OAuth call"""
+    """Raises when there is an error with the OAuth call."""
 
 
 class NoSuchPropertyException(Exception):
-    """When a property is missing"""
+    """When a property is missing."""
 
 
 class NotInstalledError(Exception):
-    """When an optional dependency is not installed"""
+    """When an optional dependency is not installed."""
 
 
 class SignError(Exception):
-    """Raises when unable to sign a S3 request"""
+    """Raises when unable to sign a S3 request."""
 
 
 class ResolveError(Exception):
     pass
+
+
+class DynamoDbError(Exception):
+    pass
+
+
+class ConditionalCheckFailedException(DynamoDbError):
+    pass
+
+
+class GenericDynamoDbError(DynamoDbError):
+    pass
+
+
+class CommitFailedException(RESTError):
+    """Commit failed, refresh and try again."""
+
+
+class CommitStateUnknownException(RESTError):
+    """Commit failed due to unknown reason."""
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/expressions/literals.py` & `pyiceberg-0.4.0rc1/pyiceberg/expressions/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     timestamptz_to_micros,
 )
 from pyiceberg.utils.decimal import decimal_to_unscaled, unscaled_to_decimal
 from pyiceberg.utils.singleton import Singleton
 
 
 class Literal(Generic[L], ABC):
-    """Literal which has a value and can be converted between types"""
+    """Literal which has a value and can be converted between types."""
 
     _value: L
 
     def __init__(self, value: L, value_type: Type[L]):
         if value is None or not isinstance(value, value_type):
             raise TypeError(f"Invalid literal value: {value!r} (not a {value_type})")
         if isinstance(value, float) and isnan(value):
@@ -76,57 +76,66 @@
 
     @singledispatchmethod
     @abstractmethod
     def to(self, type_var: IcebergType) -> Literal[L]:
         ...  # pragma: no cover
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Literal class."""
         return f"{type(self).__name__}({self.value!r})"
 
     def __str__(self) -> str:
+        """Returns the string representation of the Literal class."""
         return str(self.value)
 
     def __hash__(self) -> int:
+        """Returns a hashed representation of the Literal class."""
         return hash(self.value)
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Literal class."""
         if not isinstance(other, Literal):
             return False
         return self.value == other.value
 
     def __ne__(self, other: Any) -> bool:
+        """Returns the inequality of two instances of the Literal class."""
         return not self.__eq__(other)
 
     def __lt__(self, other: Any) -> bool:
+        """Returns if one instance of the Literal class is less than another instance."""
         return self.value < other.value
 
     def __gt__(self, other: Any) -> bool:
+        """Returns if one instance of the Literal class is greater than another instance."""
         return self.value > other.value
 
     def __le__(self, other: Any) -> bool:
+        """Returns if one instance of the Literal class is less than or equal to another instance."""
         return self.value <= other.value
 
     def __ge__(self, other: Any) -> bool:
+        """Returns if one instance of the Literal class is greater than or equal to another instance."""
         return self.value >= other.value
 
 
 def literal(value: L) -> Literal[L]:
     """
-    A generic Literal factory to construct an Iceberg Literal based on Python primitive data type
+    A generic Literal factory to construct an Iceberg Literal based on Python primitive data type.
 
     Args:
-        value(Python primitive type): the value to be associated with literal
+        value (Python primitive type): the value to be associated with literal.
 
     Example:
-        from pyiceberg.expressions.literals import literal
+        from pyiceberg.expressions.literals import literal.
         >>> literal(123)
         LongLiteral(123)
     """
     if isinstance(value, float):
-        return DoubleLiteral(value)
+        return DoubleLiteral(value)  # type: ignore
     elif isinstance(value, bool):
         return BooleanLiteral(value)
     elif isinstance(value, int):
         return LongLiteral(value)
     elif isinstance(value, str):
         return StringLiteral(value)
     elif isinstance(value, UUID):
@@ -137,25 +146,29 @@
         return DecimalLiteral(value)
     else:
         raise TypeError(f"Invalid literal value: {repr(value)}")
 
 
 class AboveMax(Literal[L]):
     def __repr__(self) -> str:
+        """Returns the string representation of the AboveMax class."""
         return f"{self.__class__.__name__}()"
 
     def __str__(self) -> str:
+        """Returns the string representation of the AboveMax class."""
         return self.__class__.__name__
 
 
 class BelowMin(Literal[L]):
     def __repr__(self) -> str:
+        """Returns the string representation of the BelowMin class."""
         return f"{self.__class__.__name__}()"
 
     def __str__(self) -> str:
+        """Returns the string representation of the BelowMin class."""
         return self.__class__.__name__
 
 
 class FloatAboveMax(AboveMax[float], Singleton):
     def __init__(self) -> None:
         super().__init__(FloatType.max, float)
 
@@ -310,28 +323,37 @@
 
 class FloatLiteral(Literal[float]):
     def __init__(self, value: float) -> None:
         super().__init__(value, float)
         self._value32 = struct.unpack("<f", struct.pack("<f", value))[0]
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the FloatLiteral class."""
         return self._value32 == other
 
     def __lt__(self, other: Any) -> bool:
+        """Returns if one instance of the FloatLiteral class is less than another instance."""
         return self._value32 < other
 
     def __gt__(self, other: Any) -> bool:
+        """Returns if one instance of the FloatLiteral class is greater than another instance."""
         return self._value32 > other
 
     def __le__(self, other: Any) -> bool:
+        """Returns if one instance of the FloatLiteral class is less than or equal to another instance."""
         return self._value32 <= other
 
     def __ge__(self, other: Any) -> bool:
+        """Returns if one instance of the FloatLiteral class is greater than or equal to another instance."""
         return self._value32 >= other
 
+    def __hash__(self) -> int:
+        """Returns a hashed representation of the FloatLiteral class."""
+        return hash(self._value32)
+
     @singledispatchmethod
     def to(self, type_var: IcebergType) -> Literal:  # type: ignore
         raise TypeError(f"Cannot convert FloatLiteral into {type_var}")
 
     @to.register(FloatType)
     def _(self, _: FloatType) -> Literal[float]:
         return self
@@ -430,30 +452,30 @@
 
 
 class DecimalLiteral(Literal[Decimal]):
     def __init__(self, value: Decimal) -> None:
         super().__init__(value, Decimal)
 
     def increment(self) -> Literal[Decimal]:
-        original_scale = abs(self.value.as_tuple().exponent)
+        original_scale = abs(int(self.value.as_tuple().exponent))
         unscaled = decimal_to_unscaled(self.value)
         return DecimalLiteral(unscaled_to_decimal(unscaled + 1, original_scale))
 
     def decrement(self) -> Literal[Decimal]:
-        original_scale = abs(self.value.as_tuple().exponent)
+        original_scale = abs(int(self.value.as_tuple().exponent))
         unscaled = decimal_to_unscaled(self.value)
         return DecimalLiteral(unscaled_to_decimal(unscaled - 1, original_scale))
 
     @singledispatchmethod
     def to(self, type_var: IcebergType) -> Literal:  # type: ignore
         raise TypeError(f"Cannot convert DecimalLiteral into {type_var}")
 
     @to.register(DecimalType)
     def _(self, type_var: DecimalType) -> Literal[Decimal]:
-        if type_var.scale == abs(self.value.as_tuple().exponent):
+        if type_var.scale == abs(int(self.value.as_tuple().exponent)):
             return self
         raise ValueError(f"Could not convert {self.value} into a {type_var}")
 
     @to.register(IntegerType)
     def _(self, _: IntegerType) -> Literal[int]:
         value_int = int(self.value.to_integral_value())
         if value_int > IntegerType.max:
@@ -551,22 +573,30 @@
     @to.register(UUIDType)
     def _(self, _: UUIDType) -> Literal[UUID]:
         return UUIDLiteral(UUID(self.value))
 
     @to.register(DecimalType)
     def _(self, type_var: DecimalType) -> Literal[Decimal]:
         dec = Decimal(self.value)
-        if type_var.scale == abs(dec.as_tuple().exponent):
+        scale = abs(int(dec.as_tuple().exponent))
+        if type_var.scale == scale:
             return DecimalLiteral(dec)
         else:
-            raise ValueError(
-                f"Could not convert {self.value} into a {type_var}, scales differ {type_var.scale} <> {abs(dec.as_tuple().exponent)}"
-            )
+            raise ValueError(f"Could not convert {self.value} into a {type_var}, scales differ {type_var.scale} <> {scale}")
+
+    @to.register(BooleanType)
+    def _(self, type_var: BooleanType) -> Literal[bool]:
+        value_upper = self.value.upper()
+        if value_upper in ["TRUE", "FALSE"]:
+            return BooleanLiteral(value_upper == "TRUE")
+        else:
+            raise ValueError(f"Could not convert {self.value} into a {type_var}")
 
     def __repr__(self) -> str:
+        """Returns the string representation of the StringLiteral class."""
         return f"literal({repr(self.value)})"
 
 
 class UUIDLiteral(Literal[UUID]):
     def __init__(self, value: UUID) -> None:
         super().__init__(value, UUID)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/expressions/parser.py` & `pyiceberg-0.4.0rc1/pyiceberg/expressions/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,18 @@
     LessThan,
     LessThanOrEqual,
     Not,
     NotEqualTo,
     NotIn,
     NotNaN,
     NotNull,
+    NotStartsWith,
     Or,
     Reference,
+    StartsWith,
 )
 from pyiceberg.expressions.literals import (
     DecimalLiteral,
     Literal,
     LongLiteral,
     StringLiteral,
 )
@@ -67,14 +69,15 @@
 AND = CaselessKeyword("and")
 OR = CaselessKeyword("or")
 NOT = CaselessKeyword("not")
 IS = CaselessKeyword("is")
 IN = CaselessKeyword("in")
 NULL = CaselessKeyword("null")
 NAN = CaselessKeyword("nan")
+LIKE = CaselessKeyword("like")
 
 identifier = Word(alphas, alphanums + "_$").set_results_name("identifier")
 column = delimited_list(identifier, delim=".", combine=True).set_results_name("column")
 
 
 @column.set_parse_action
 def _(result: ParseResults) -> Reference:
@@ -203,15 +206,30 @@
 
 
 @not_in.set_parse_action
 def _(result: ParseResults) -> BooleanExpression:
     return NotIn(result.column, result.literal_set)
 
 
-predicate = (comparison | in_check | null_check | nan_check | boolean).set_results_name("predicate")
+starts_with = column + LIKE + string
+not_starts_with = column + NOT + LIKE + string
+starts_check = starts_with | not_starts_with
+
+
+@starts_with.set_parse_action
+def _(result: ParseResults) -> BooleanExpression:
+    return StartsWith(result.column, result.raw_quoted_string)
+
+
+@not_starts_with.set_parse_action
+def _(result: ParseResults) -> BooleanExpression:
+    return NotStartsWith(result.column, result.raw_quoted_string)
+
+
+predicate = (comparison | in_check | null_check | nan_check | starts_check | boolean).set_results_name("predicate")
 
 
 def handle_not(result: ParseResults) -> Not:
     return Not(result[0][0])
 
 
 def handle_and(result: ParseResults) -> And:
@@ -229,9 +247,9 @@
         (Suppress(AND), 2, opAssoc.LEFT, handle_and),
         (Suppress(OR), 2, opAssoc.LEFT, handle_or),
     ],
 ).set_name("expr")
 
 
 def parse(expr: str) -> BooleanExpression:
-    """Parses a boolean expression"""
+    """Parses a boolean expression."""
     return boolean_expression.parse_string(expr)[0]
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/expressions/visitors.py` & `pyiceberg-0.4.0rc1/pyiceberg/expressions/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,874 +10,890 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from functools import singledispatch
+from functools import cached_property, reduce
 from typing import (
     Any,
-    Callable,
     Generic,
-    List,
+    Iterable,
     Set,
     Tuple,
+    Type,
     TypeVar,
+    Union,
 )
 
-from pyiceberg.conversions import from_bytes
-from pyiceberg.expressions import (
-    AlwaysFalse,
-    AlwaysTrue,
-    And,
-    BooleanExpression,
-    BoundEqualTo,
-    BoundGreaterThan,
-    BoundGreaterThanOrEqual,
-    BoundIn,
-    BoundIsNaN,
-    BoundIsNull,
-    BoundLessThan,
-    BoundLessThanOrEqual,
-    BoundLiteralPredicate,
-    BoundNotEqualTo,
-    BoundNotIn,
-    BoundNotNaN,
-    BoundNotNull,
-    BoundPredicate,
-    BoundSetPredicate,
-    BoundTerm,
-    BoundUnaryPredicate,
-    L,
-    Not,
-    Or,
-    UnboundPredicate,
-)
-from pyiceberg.expressions.literals import Literal
-from pyiceberg.manifest import ManifestFile, PartitionFieldSummary
-from pyiceberg.partitioning import PartitionSpec
-from pyiceberg.schema import Schema
-from pyiceberg.typedef import StructProtocol
-from pyiceberg.types import (
-    DoubleType,
-    FloatType,
-    IcebergType,
-    PrimitiveType,
+from pyiceberg.expressions.literals import (
+    AboveMax,
+    BelowMin,
+    Literal,
+    literal,
 )
+from pyiceberg.schema import Accessor, Schema
+from pyiceberg.typedef import L, StructProtocol
+from pyiceberg.types import DoubleType, FloatType, NestedField
+from pyiceberg.utils.singleton import Singleton
 
-T = TypeVar("T")
 
+def _to_unbound_term(term: Union[str, UnboundTerm[Any]]) -> UnboundTerm[Any]:
+    return Reference(term) if isinstance(term, str) else term
 
-class BooleanExpressionVisitor(Generic[T], ABC):
-    @abstractmethod
-    def visit_true(self) -> T:
-        """Visit method for an AlwaysTrue boolean expression
 
-        Note: This visit method has no arguments since AlwaysTrue instances have no context.
-        """
+def _to_literal_set(values: Union[Iterable[L], Iterable[Literal[L]]]) -> Set[Literal[L]]:
+    return {_to_literal(v) for v in values}
 
-    @abstractmethod
-    def visit_false(self) -> T:
-        """Visit method for an AlwaysFalse boolean expression
 
-        Note: This visit method has no arguments since AlwaysFalse instances have no context.
-        """
+def _to_literal(value: Union[L, Literal[L]]) -> Literal[L]:
+    if isinstance(value, Literal):
+        return value
+    else:
+        return literal(value)
 
-    @abstractmethod
-    def visit_not(self, child_result: T) -> T:
-        """Visit method for a Not boolean expression
 
-        Args:
-            child_result (T): The result of visiting the child of the Not boolean expression
-        """
+class BooleanExpression(ABC):
+    """An expression that evaluates to a boolean."""
 
     @abstractmethod
-    def visit_and(self, left_result: T, right_result: T) -> T:
-        """Visit method for an And boolean expression
-
-        Args:
-            left_result (T): The result of visiting the left side of the expression
-            right_result (T): The result of visiting the right side of the expression
-        """
-
-    @abstractmethod
-    def visit_or(self, left_result: T, right_result: T) -> T:
-        """Visit method for an Or boolean expression
-
-        Args:
-            left_result (T): The result of visiting the left side of the expression
-            right_result (T): The result of visiting the right side of the expression
-        """
-
-    @abstractmethod
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> T:
-        """Visit method for an unbound predicate in an expression tree
-
-        Args:
-            predicate (UnboundPredicate[L): An instance of an UnboundPredicate
-        """
-
-    @abstractmethod
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> T:
-        """Visit method for a bound predicate in an expression tree
-
-        Args:
-            predicate (BoundPredicate[L]): An instance of a BoundPredicate
-        """
-
-
-@singledispatch
-def visit(obj: BooleanExpression, visitor: BooleanExpressionVisitor[T]) -> T:
-    """A generic function for applying a boolean expression visitor to any point within an expression
-
-    The function traverses the expression in post-order fashion
-
-    Args:
-        obj(BooleanExpression): An instance of a BooleanExpression
-        visitor(BooleanExpressionVisitor[T]): An instance of an implementation of the generic BooleanExpressionVisitor base class
-
-    Raises:
-        NotImplementedError: If attempting to visit an unsupported expression
-    """
-    raise NotImplementedError(f"Cannot visit unsupported expression: {obj}")
-
-
-@visit.register(AlwaysTrue)
-def _(_: AlwaysTrue, visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit an AlwaysTrue boolean expression with a concrete BooleanExpressionVisitor"""
-    return visitor.visit_true()
+    def __invert__(self) -> BooleanExpression:
+        """Transform the Expression into its negated version."""
 
 
-@visit.register(AlwaysFalse)
-def _(_: AlwaysFalse, visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit an AlwaysFalse boolean expression with a concrete BooleanExpressionVisitor"""
-    return visitor.visit_false()
+class Term(Generic[L], ABC):
+    """A simple expression that evaluates to a value."""
 
 
-@visit.register(Not)
-def _(obj: Not, visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit a Not boolean expression with a concrete BooleanExpressionVisitor"""
-    child_result: T = visit(obj.child, visitor=visitor)
-    return visitor.visit_not(child_result=child_result)
+class Bound(ABC):
+    """Represents a bound value expression."""
 
 
-@visit.register(And)
-def _(obj: And, visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit an And boolean expression with a concrete BooleanExpressionVisitor"""
-    left_result: T = visit(obj.left, visitor=visitor)
-    right_result: T = visit(obj.right, visitor=visitor)
-    return visitor.visit_and(left_result=left_result, right_result=right_result)
-
-
-@visit.register(UnboundPredicate)
-def _(obj: UnboundPredicate[L], visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit an unbound boolean expression with a concrete BooleanExpressionVisitor"""
-    return visitor.visit_unbound_predicate(predicate=obj)
-
-
-@visit.register(BoundPredicate)
-def _(obj: BoundPredicate[L], visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit a bound boolean expression with a concrete BooleanExpressionVisitor"""
-    return visitor.visit_bound_predicate(predicate=obj)
-
-
-@visit.register(Or)
-def _(obj: Or, visitor: BooleanExpressionVisitor[T]) -> T:
-    """Visit an Or boolean expression with a concrete BooleanExpressionVisitor"""
-    left_result: T = visit(obj.left, visitor=visitor)
-    right_result: T = visit(obj.right, visitor=visitor)
-    return visitor.visit_or(left_result=left_result, right_result=right_result)
-
-
-def bind(schema: Schema, expression: BooleanExpression, case_sensitive: bool) -> BooleanExpression:
-    """Travers over an expression to bind the predicates to the schema
-
-    Args:
-      schema (Schema): A schema to use when binding the expression
-      expression (BooleanExpression): An expression containing UnboundPredicates that can be bound
-      case_sensitive (bool): Whether to consider case when binding a reference to a field in a schema, defaults to True
-
-    Raises:
-        TypeError: In the case a predicate is already bound
-    """
-    return visit(expression, BindVisitor(schema, case_sensitive))
-
-
-class BindVisitor(BooleanExpressionVisitor[BooleanExpression]):
-    """Rewrites a boolean expression by replacing unbound references with references to fields in a struct schema
-
-    Args:
-      schema (Schema): A schema to use when binding the expression
-      case_sensitive (bool): Whether to consider case when binding a reference to a field in a schema, defaults to True
-
-    Raises:
-        TypeError: In the case a predicate is already bound
-    """
-
-    schema: Schema
-    case_sensitive: bool
-
-    def __init__(self, schema: Schema, case_sensitive: bool) -> None:
-        self.schema = schema
-        self.case_sensitive = case_sensitive
-
-    def visit_true(self) -> BooleanExpression:
-        return AlwaysTrue()
-
-    def visit_false(self) -> BooleanExpression:
-        return AlwaysFalse()
-
-    def visit_not(self, child_result: BooleanExpression) -> BooleanExpression:
-        return Not(child=child_result)
-
-    def visit_and(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return And(left=left_result, right=right_result)
-
-    def visit_or(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return Or(left=left_result, right=right_result)
-
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> BooleanExpression:
-        return predicate.bind(self.schema, case_sensitive=self.case_sensitive)
-
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> BooleanExpression:
-        raise TypeError(f"Found already bound predicate: {predicate}")
-
-
-class BoundBooleanExpressionVisitor(BooleanExpressionVisitor[T], ABC):
-    @abstractmethod
-    def visit_in(self, term: BoundTerm[L], literals: Set[L]) -> T:
-        """Visit a bound In predicate"""
-
-    @abstractmethod
-    def visit_not_in(self, term: BoundTerm[L], literals: Set[L]) -> T:
-        """Visit a bound NotIn predicate"""
-
-    @abstractmethod
-    def visit_is_nan(self, term: BoundTerm[L]) -> T:
-        """Visit a bound IsNan predicate"""
-
-    @abstractmethod
-    def visit_not_nan(self, term: BoundTerm[L]) -> T:
-        """Visit a bound NotNan predicate"""
+B = TypeVar("B")
 
-    @abstractmethod
-    def visit_is_null(self, term: BoundTerm[L]) -> T:
-        """Visit a bound IsNull predicate"""
 
-    @abstractmethod
-    def visit_not_null(self, term: BoundTerm[L]) -> T:
-        """Visit a bound NotNull predicate"""
+class Unbound(Generic[B], ABC):
+    """Represents an unbound value expression."""
 
     @abstractmethod
-    def visit_equal(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound Equal predicate"""
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> B:
+        ...
 
+    @property
     @abstractmethod
-    def visit_not_equal(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound NotEqual predicate"""
+    def as_bound(self) -> Type[Bound]:
+        ...
 
-    @abstractmethod
-    def visit_greater_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound GreaterThanOrEqual predicate"""
 
-    @abstractmethod
-    def visit_greater_than(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound GreaterThan predicate"""
+class BoundTerm(Term[L], Bound, ABC):
+    """Represents a bound term."""
 
     @abstractmethod
-    def visit_less_than(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound LessThan predicate"""
+    def ref(self) -> BoundReference[L]:
+        """Returns the bound reference."""
 
     @abstractmethod
-    def visit_less_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> T:
-        """Visit a bound LessThanOrEqual predicate"""
+    def eval(self, struct: StructProtocol) -> L:  # pylint: disable=W0613
+        """Returns the value at the referenced field's position in an object that abides by the StructProtocol."""
 
-    @abstractmethod
-    def visit_true(self) -> T:
-        """Visit a bound True predicate"""
 
-    @abstractmethod
-    def visit_false(self) -> T:
-        """Visit a bound False predicate"""
+class BoundReference(BoundTerm[L]):
+    """A reference bound to a field in a schema.
 
-    @abstractmethod
-    def visit_not(self, child_result: T) -> T:
-        """Visit a bound Not predicate"""
+    Args:
+        field (NestedField): A referenced field in an Iceberg schema.
+        accessor (Accessor): An Accessor object to access the value at the field's position.
+    """
 
-    @abstractmethod
-    def visit_and(self, left_result: T, right_result: T) -> T:
-        """Visit a bound And predicate"""
+    field: NestedField
+    accessor: Accessor
 
-    @abstractmethod
-    def visit_or(self, left_result: T, right_result: T) -> T:
-        """Visit a bound Or predicate"""
+    def __init__(self, field: NestedField, accessor: Accessor):
+        self.field = field
+        self.accessor = accessor
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> T:
-        """Visit an unbound predicate
-        Args:
-            predicate (UnboundPredicate[L]): An unbound predicate
-        Raises:
-            TypeError: This always raises since an unbound predicate is not expected in a bound boolean expression
-        """
-        raise TypeError(f"Not a bound predicate: {predicate}")
+    def eval(self, struct: StructProtocol) -> L:
+        """Returns the value at the referenced field's position in an object that abides by the StructProtocol.
 
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> T:
-        """Visit a bound predicate
         Args:
-            predicate (BoundPredicate[L]): A bound predicate
+            struct (StructProtocol): A row object that abides by the StructProtocol and returns values given a position.
+        Returns:
+            Any: The value at the referenced field's position in `struct`.
         """
-        return visit_bound_predicate(predicate, self)
-
-
-@singledispatch
-def visit_bound_predicate(expr: BoundPredicate[L], _: BooleanExpressionVisitor[T]) -> T:
-    raise TypeError(f"Unknown predicate: {expr}")
-
-
-@visit_bound_predicate.register(BoundIn)
-def _(expr: BoundIn[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_in(term=expr.term, literals=expr.value_set)
+        return self.accessor.get(struct)
 
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the BoundReference class."""
+        return self.field == other.field if isinstance(other, BoundReference) else False
 
-@visit_bound_predicate.register(BoundNotIn)
-def _(expr: BoundNotIn[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_not_in(term=expr.term, literals=expr.value_set)
+    def __repr__(self) -> str:
+        """Returns the string representation of the BoundReference class."""
+        return f"BoundReference(field={repr(self.field)}, accessor={repr(self.accessor)})"
 
+    def ref(self) -> BoundReference[L]:
+        return self
 
-@visit_bound_predicate.register(BoundIsNaN)
-def _(expr: BoundIsNaN[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_is_nan(term=expr.term)
 
+class UnboundTerm(Term[Any], Unbound[BoundTerm[L]], ABC):
+    """Represents an unbound term."""
 
-@visit_bound_predicate.register(BoundNotNaN)
-def _(expr: BoundNotNaN[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_not_nan(term=expr.term)
-
-
-@visit_bound_predicate.register(BoundIsNull)
-def _(expr: BoundIsNull[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_is_null(term=expr.term)
-
-
-@visit_bound_predicate.register(BoundNotNull)
-def _(expr: BoundNotNull[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_not_null(term=expr.term)
-
-
-@visit_bound_predicate.register(BoundEqualTo)
-def _(expr: BoundEqualTo[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_equal(term=expr.term, literal=expr.literal)
-
+    @abstractmethod
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BoundTerm[L]:
+        ...
 
-@visit_bound_predicate.register(BoundNotEqualTo)
-def _(expr: BoundNotEqualTo[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_not_equal(term=expr.term, literal=expr.literal)
 
+class Reference(UnboundTerm[Any]):
+    """A reference not yet bound to a field in a schema.
 
-@visit_bound_predicate.register(BoundGreaterThanOrEqual)
-def _(expr: BoundGreaterThanOrEqual[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    """Visit a bound GreaterThanOrEqual predicate"""
-    return visitor.visit_greater_than_or_equal(term=expr.term, literal=expr.literal)
+    Args:
+        name (str): The name of the field.
 
+    Note:
+        An unbound reference is sometimes referred to as a "named" reference.
+    """
 
-@visit_bound_predicate.register(BoundGreaterThan)
-def _(expr: BoundGreaterThan[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_greater_than(term=expr.term, literal=expr.literal)
+    name: str
 
+    def __init__(self, name: str) -> None:
+        self.name = name
 
-@visit_bound_predicate.register(BoundLessThan)
-def _(expr: BoundLessThan[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_less_than(term=expr.term, literal=expr.literal)
+    def __repr__(self) -> str:
+        """Returns the string representation of the Reference class."""
+        return f"Reference(name={repr(self.name)})"
 
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Reference class."""
+        return self.name == other.name if isinstance(other, Reference) else False
 
-@visit_bound_predicate.register(BoundLessThanOrEqual)
-def _(expr: BoundLessThanOrEqual[L], visitor: BoundBooleanExpressionVisitor[T]) -> T:
-    return visitor.visit_less_than_or_equal(term=expr.term, literal=expr.literal)
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BoundReference[L]:
+        """Bind the reference to an Iceberg schema.
 
+        Args:
+            schema (Schema): An Iceberg schema.
+            case_sensitive (bool): Whether to consider case when binding the reference to the field.
 
-def rewrite_not(expr: BooleanExpression) -> BooleanExpression:
-    return visit(expr, _RewriteNotVisitor())
+        Raises:
+            ValueError: If an empty name is provided.
 
+        Returns:
+            BoundReference: A reference bound to the specific field in the Iceberg schema.
+        """
+        field = schema.find_field(name_or_id=self.name, case_sensitive=case_sensitive)
+        accessor = schema.accessor_for_field(field.field_id)
+        return self.as_bound(field=field, accessor=accessor)  # type: ignore
+
+    @property
+    def as_bound(self) -> Type[BoundReference[L]]:
+        return BoundReference[L]
+
+
+class And(BooleanExpression):
+    """AND operation expression - logical conjunction."""
+
+    left: BooleanExpression
+    right: BooleanExpression
+
+    def __new__(cls, left: BooleanExpression, right: BooleanExpression, *rest: BooleanExpression) -> BooleanExpression:  # type: ignore
+        if rest:
+            return reduce(And, (left, right, *rest))
+        if left is AlwaysFalse() or right is AlwaysFalse():
+            return AlwaysFalse()
+        elif left is AlwaysTrue():
+            return right
+        elif right is AlwaysTrue():
+            return left
+        else:
+            obj = super().__new__(cls)
+            obj.left = left
+            obj.right = right
+            return obj
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the And class."""
+        return self.left == other.left and self.right == other.right if isinstance(other, And) else False
+
+    def __str__(self) -> str:
+        """Returns the string representation of the And class."""
+        return f"And(left={str(self.left)}, right={str(self.right)})"
+
+    def __repr__(self) -> str:
+        """Returns the string representation of the And class."""
+        return f"And(left={repr(self.left)}, right={repr(self.right)})"
+
+    def __invert__(self) -> BooleanExpression:
+        """Transform the Expression into its negated version."""
+        # De Morgan's law: not (A and B) = (not A) or (not B)
+        return Or(~self.left, ~self.right)
+
+    def __getnewargs__(self) -> Tuple[BooleanExpression, BooleanExpression]:
+        """A magic function for pickling the And class."""
+        return (self.left, self.right)
+
+
+class Or(BooleanExpression):
+    """OR operation expression - logical disjunction."""
+
+    left: BooleanExpression
+    right: BooleanExpression
+
+    def __new__(cls, left: BooleanExpression, right: BooleanExpression, *rest: BooleanExpression) -> BooleanExpression:  # type: ignore
+        if rest:
+            return reduce(Or, (left, right, *rest))
+        if left is AlwaysTrue() or right is AlwaysTrue():
+            return AlwaysTrue()
+        elif left is AlwaysFalse():
+            return right
+        elif right is AlwaysFalse():
+            return left
+        else:
+            obj = super().__new__(cls)
+            obj.left = left
+            obj.right = right
+            return obj
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Or class."""
+        return self.left == other.left and self.right == other.right if isinstance(other, Or) else False
+
+    def __repr__(self) -> str:
+        """Returns the string representation of the Or class."""
+        return f"Or(left={repr(self.left)}, right={repr(self.right)})"
+
+    def __invert__(self) -> BooleanExpression:
+        """Transform the Expression into its negated version."""
+        # De Morgan's law: not (A or B) = (not A) and (not B)
+        return And(~self.left, ~self.right)
+
+    def __getnewargs__(self) -> Tuple[BooleanExpression, BooleanExpression]:
+        """A magic function for pickling the Or class."""
+        return (self.left, self.right)
+
+
+class Not(BooleanExpression):
+    """NOT operation expression - logical negation."""
+
+    child: BooleanExpression
+
+    def __new__(cls, child: BooleanExpression) -> BooleanExpression:  # type: ignore
+        if child is AlwaysTrue():
+            return AlwaysFalse()
+        elif child is AlwaysFalse():
+            return AlwaysTrue()
+        elif isinstance(child, Not):
+            return child.child
+        obj = super().__new__(cls)
+        obj.child = child
+        return obj
+
+    def __repr__(self) -> str:
+        """Returns the string representation of the Not class."""
+        return f"Not(child={repr(self.child)})"
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Not class."""
+        return self.child == other.child if isinstance(other, Not) else False
+
+    def __invert__(self) -> BooleanExpression:
+        """Transform the Expression into its negated version."""
+        return self.child
+
+    def __getnewargs__(self) -> Tuple[BooleanExpression]:
+        """A magic function for pickling the Not class."""
+        return (self.child,)
 
-class _RewriteNotVisitor(BooleanExpressionVisitor[BooleanExpression]):
-    """Inverts the negations"""
 
-    def visit_true(self) -> BooleanExpression:
-        return AlwaysTrue()
+class AlwaysTrue(BooleanExpression, Singleton):
+    """TRUE expression."""
 
-    def visit_false(self) -> BooleanExpression:
+    def __invert__(self) -> AlwaysFalse:
+        """Transform the Expression into its negated version."""
         return AlwaysFalse()
 
-    def visit_not(self, child_result: BooleanExpression) -> BooleanExpression:
-        return ~child_result
-
-    def visit_and(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return And(left=left_result, right=right_result)
-
-    def visit_or(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return Or(left=left_result, right=right_result)
+    def __str__(self) -> str:
+        """Returns the string representation of the AlwaysTrue class."""
+        return "AlwaysTrue()"
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> BooleanExpression:
-        return predicate
+    def __repr__(self) -> str:
+        """Returns the string representation of the AlwaysTrue class."""
+        return "AlwaysTrue()"
 
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> BooleanExpression:
-        return predicate
 
+class AlwaysFalse(BooleanExpression, Singleton):
+    """FALSE expression."""
 
-def expression_evaluator(schema: Schema, unbound: BooleanExpression, case_sensitive: bool) -> Callable[[StructProtocol], bool]:
-    return _ExpressionEvaluator(schema, unbound, case_sensitive).eval
-
-
-class _ExpressionEvaluator(BoundBooleanExpressionVisitor[bool]):
-    bound: BooleanExpression
-    struct: StructProtocol
-
-    def __init__(self, schema: Schema, unbound: BooleanExpression, case_sensitive: bool):
-        self.bound = bind(schema, unbound, case_sensitive)
-
-    def eval(self, struct: StructProtocol) -> bool:
-        self.struct = struct
-        return visit(self.bound, self)
-
-    def visit_in(self, term: BoundTerm[L], literals: Set[L]) -> bool:
-        return term.eval(self.struct) in literals
-
-    def visit_not_in(self, term: BoundTerm[L], literals: Set[L]) -> bool:
-        return term.eval(self.struct) not in literals
-
-    def visit_is_nan(self, term: BoundTerm[L]) -> bool:
-        val = term.eval(self.struct)
-        return val != val
-
-    def visit_not_nan(self, term: BoundTerm[L]) -> bool:
-        val = term.eval(self.struct)
-        return val == val
-
-    def visit_is_null(self, term: BoundTerm[L]) -> bool:
-        return term.eval(self.struct) is None
+    def __invert__(self) -> AlwaysTrue:
+        """Transform the Expression into its negated version."""
+        return AlwaysTrue()
 
-    def visit_not_null(self, term: BoundTerm[L]) -> bool:
-        return term.eval(self.struct) is not None
+    def __str__(self) -> str:
+        """Returns the string representation of the AlwaysFalse class."""
+        return "AlwaysFalse()"
 
-    def visit_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) == literal.value
+    def __repr__(self) -> str:
+        """Returns the string representation of the AlwaysFalse class."""
+        return "AlwaysFalse()"
 
-    def visit_not_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) != literal.value
 
-    def visit_greater_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) >= literal.value
+class BoundPredicate(Generic[L], Bound, BooleanExpression, ABC):
+    term: BoundTerm[L]
 
-    def visit_greater_than(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) > literal.value
+    def __init__(self, term: BoundTerm[L]):
+        self.term = term
 
-    def visit_less_than(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) < literal.value
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the BoundPredicate class."""
+        if isinstance(other, BoundPredicate):
+            return self.term == other.term
+        return False
 
-    def visit_less_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        return term.eval(self.struct) <= literal.value
+    @property
+    @abstractmethod
+    def as_unbound(self) -> Type[UnboundPredicate[Any]]:
+        ...
 
-    def visit_true(self) -> bool:
-        return True
 
-    def visit_false(self) -> bool:
-        return False
+class UnboundPredicate(Generic[L], Unbound[BooleanExpression], BooleanExpression, ABC):
+    term: UnboundTerm[Any]
 
-    def visit_not(self, child_result: bool) -> bool:
-        return not child_result
+    def __init__(self, term: Union[str, UnboundTerm[Any]]):
+        self.term = _to_unbound_term(term)
 
-    def visit_and(self, left_result: bool, right_result: bool) -> bool:
-        return left_result and right_result
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the UnboundPredicate class."""
+        return self.term == other.term if isinstance(other, UnboundPredicate) else False
 
-    def visit_or(self, left_result: bool, right_result: bool) -> bool:
-        return left_result or right_result
+    @abstractmethod
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BooleanExpression:
+        ...
 
+    @property
+    @abstractmethod
+    def as_bound(self) -> Type[BoundPredicate[L]]:
+        ...
 
-ROWS_MIGHT_MATCH = True
-ROWS_CANNOT_MATCH = False
-IN_PREDICATE_LIMIT = 200
 
+class UnaryPredicate(UnboundPredicate[Any], ABC):
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BoundUnaryPredicate[Any]:
+        bound_term = self.term.bind(schema, case_sensitive)
+        return self.as_bound(bound_term)
 
-def _from_byte_buffer(field_type: IcebergType, val: bytes) -> Any:
-    if not isinstance(field_type, PrimitiveType):
-        raise ValueError(f"Expected a PrimitiveType, got: {type(field_type)}")
-    return from_bytes(field_type, val)
+    def __repr__(self) -> str:
+        """Returns the string representation of the UnaryPredicate class."""
+        return f"{str(self.__class__.__name__)}(term={repr(self.term)})"
 
+    @property
+    @abstractmethod
+    def as_bound(self) -> Type[BoundUnaryPredicate[Any]]:
+        ...
 
-class _ManifestEvalVisitor(BoundBooleanExpressionVisitor[bool]):
-    partition_fields: List[PartitionFieldSummary]
-    partition_filter: BooleanExpression
 
-    def __init__(self, partition_struct_schema: Schema, partition_filter: BooleanExpression, case_sensitive: bool) -> None:
-        self.partition_filter = bind(partition_struct_schema, rewrite_not(partition_filter), case_sensitive)
+class BoundUnaryPredicate(BoundPredicate[L], ABC):
+    def __repr__(self) -> str:
+        """Returns the string representation of the BoundUnaryPredicate class."""
+        return f"{str(self.__class__.__name__)}(term={repr(self.term)})"
 
-    def eval(self, manifest: ManifestFile) -> bool:
-        if partitions := manifest.partitions:
-            self.partition_fields = partitions
-            return visit(self.partition_filter, self)
+    @property
+    @abstractmethod
+    def as_unbound(self) -> Type[UnaryPredicate]:
+        ...
 
-        # No partition information
-        return ROWS_MIGHT_MATCH
+    def __getnewargs__(self) -> Tuple[BoundTerm[L]]:
+        """A magic function for pickling the BoundUnaryPredicate class."""
+        return (self.term,)
 
-    def visit_in(self, term: BoundTerm[L], literals: Set[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
 
-        if field.lower_bound is None:
-            return ROWS_CANNOT_MATCH
+class BoundIsNull(BoundUnaryPredicate[L]):
+    def __new__(cls, term: BoundTerm[L]) -> BooleanExpression:  # type: ignore  # pylint: disable=W0221
+        if term.ref().field.required:
+            return AlwaysFalse()
+        return super().__new__(cls)
 
-        if len(literals) > IN_PREDICATE_LIMIT:
-            return ROWS_MIGHT_MATCH
+    def __invert__(self) -> BoundNotNull[L]:
+        """Transform the Expression into its negated version."""
+        return BoundNotNull(self.term)
 
-        lower = _from_byte_buffer(term.ref().field.field_type, field.lower_bound)
+    @property
+    def as_unbound(self) -> Type[IsNull]:
+        return IsNull
 
-        if all(lower > val for val in literals):
-            return ROWS_CANNOT_MATCH
 
-        if field.upper_bound is not None:
-            upper = _from_byte_buffer(term.ref().field.field_type, field.upper_bound)
-            if all(upper < val for val in literals):
-                return ROWS_CANNOT_MATCH
+class BoundNotNull(BoundUnaryPredicate[L]):
+    def __new__(cls, term: BoundTerm[L]):  # type: ignore  # pylint: disable=W0221
+        if term.ref().field.required:
+            return AlwaysTrue()
+        return super().__new__(cls)
 
-        return ROWS_MIGHT_MATCH
+    def __invert__(self) -> BoundIsNull[L]:
+        """Transform the Expression into its negated version."""
+        return BoundIsNull(self.term)
 
-    def visit_not_in(self, term: BoundTerm[L], literals: Set[L]) -> bool:
-        # because the bounds are not necessarily a min or max value, this cannot be answered using
-        # them. notIn(col, {X, ...}) with (X, Y) doesn't guarantee that X is a value in col.
-        return ROWS_MIGHT_MATCH
+    @property
+    def as_unbound(self) -> Type[NotNull]:
+        return NotNull
 
-    def visit_is_nan(self, term: BoundTerm[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
 
-        if field.contains_nan is False:
-            return ROWS_CANNOT_MATCH
+class IsNull(UnaryPredicate):
+    def __invert__(self) -> NotNull:
+        """Transform the Expression into its negated version."""
+        return NotNull(self.term)
 
-        return ROWS_MIGHT_MATCH
+    @property
+    def as_bound(self) -> Type[BoundIsNull[L]]:
+        return BoundIsNull[L]
 
-    def visit_not_nan(self, term: BoundTerm[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
 
-        if field.contains_nan is True and field.contains_null is False and field.lower_bound is None:
-            return ROWS_CANNOT_MATCH
+class NotNull(UnaryPredicate):
+    def __invert__(self) -> IsNull:
+        """Transform the Expression into its negated version."""
+        return IsNull(self.term)
 
-        return ROWS_MIGHT_MATCH
+    @property
+    def as_bound(self) -> Type[BoundNotNull[L]]:
+        return BoundNotNull[L]
 
-    def visit_is_null(self, term: BoundTerm[L]) -> bool:
-        pos = term.ref().accessor.position
 
-        if self.partition_fields[pos].contains_null is False:
-            return ROWS_CANNOT_MATCH
+class BoundIsNaN(BoundUnaryPredicate[L]):
+    def __new__(cls, term: BoundTerm[L]) -> BooleanExpression:  # type: ignore  # pylint: disable=W0221
+        bound_type = term.ref().field.field_type
+        if type(bound_type) in {FloatType, DoubleType}:
+            return super().__new__(cls)
+        return AlwaysFalse()
 
-        return ROWS_MIGHT_MATCH
+    def __invert__(self) -> BoundNotNaN[L]:
+        """Transform the Expression into its negated version."""
+        return BoundNotNaN(self.term)
+
+    @property
+    def as_unbound(self) -> Type[IsNaN]:
+        return IsNaN
 
-    def visit_not_null(self, term: BoundTerm[L]) -> bool:
-        pos = term.ref().accessor.position
 
-        # contains_null encodes whether at least one partition value is null,
-        # lowerBound is null if all partition values are null
-        all_null = self.partition_fields[pos].contains_null is True and self.partition_fields[pos].lower_bound is None
+class BoundNotNaN(BoundUnaryPredicate[L]):
+    def __new__(cls, term: BoundTerm[L]) -> BooleanExpression:  # type: ignore  # pylint: disable=W0221
+        bound_type = term.ref().field.field_type
+        if type(bound_type) in {FloatType, DoubleType}:
+            return super().__new__(cls)
+        return AlwaysTrue()
 
-        if all_null and type(term.ref().field.field_type) in {DoubleType, FloatType}:
-            # floating point types may include NaN values, which we check separately.
-            # In case bounds don't include NaN value, contains_nan needs to be checked against.
-            all_null = self.partition_fields[pos].contains_nan is False
+    def __invert__(self) -> BoundIsNaN[L]:
+        """Transform the Expression into its negated version."""
+        return BoundIsNaN(self.term)
 
-        if all_null:
-            return ROWS_CANNOT_MATCH
+    @property
+    def as_unbound(self) -> Type[NotNaN]:
+        return NotNaN
 
-        return ROWS_MIGHT_MATCH
 
-    def visit_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
+class IsNaN(UnaryPredicate):
+    def __invert__(self) -> NotNaN:
+        """Transform the Expression into its negated version."""
+        return NotNaN(self.term)
 
-        if field.lower_bound is None or field.upper_bound is None:
-            # values are all null and literal cannot contain null
-            return ROWS_CANNOT_MATCH
+    @property
+    def as_bound(self) -> Type[BoundIsNaN[L]]:
+        return BoundIsNaN[L]
 
-        lower = _from_byte_buffer(term.ref().field.field_type, field.lower_bound)
 
-        if lower > literal.value:
-            return ROWS_CANNOT_MATCH
+class NotNaN(UnaryPredicate):
+    def __invert__(self) -> IsNaN:
+        """Transform the Expression into its negated version."""
+        return IsNaN(self.term)
 
-        upper = _from_byte_buffer(term.ref().field.field_type, field.upper_bound)
+    @property
+    def as_bound(self) -> Type[BoundNotNaN[L]]:
+        return BoundNotNaN[L]
 
-        if literal.value > upper:
-            return ROWS_CANNOT_MATCH
 
-        return ROWS_MIGHT_MATCH
+class SetPredicate(UnboundPredicate[L], ABC):
+    literals: Set[Literal[L]]
 
-    def visit_not_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        # because the bounds are not necessarily a min or max value, this cannot be answered using
-        # them. notEq(col, X) with (X, Y) doesn't guarantee that X is a value in col.
-        return ROWS_MIGHT_MATCH
+    def __init__(self, term: Union[str, UnboundTerm[Any]], literals: Union[Iterable[L], Iterable[Literal[L]]]):
+        super().__init__(term)
+        self.literals = _to_literal_set(literals)
 
-    def visit_greater_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BoundSetPredicate[L]:
+        bound_term = self.term.bind(schema, case_sensitive)
+        return self.as_bound(bound_term, {lit.to(bound_term.ref().field.field_type) for lit in self.literals})
 
-        if field.upper_bound is None:
-            return ROWS_CANNOT_MATCH
+    def __str__(self) -> str:
+        """Returns the string representation of the SetPredicate class."""
+        # Sort to make it deterministic
+        return f"{str(self.__class__.__name__)}({str(self.term)}, {{{', '.join(sorted([str(literal) for literal in self.literals]))}}})"
 
-        upper = _from_byte_buffer(term.ref().field.field_type, field.upper_bound)
+    def __repr__(self) -> str:
+        """Returns the string representation of the SetPredicate class."""
+        # Sort to make it deterministic
+        return f"{str(self.__class__.__name__)}({repr(self.term)}, {{{', '.join(sorted([repr(literal) for literal in self.literals]))}}})"
 
-        if literal.value > upper:
-            return ROWS_CANNOT_MATCH
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the SetPredicate class."""
+        return self.term == other.term and self.literals == other.literals if isinstance(other, SetPredicate) else False
 
-        return ROWS_MIGHT_MATCH
+    def __getnewargs__(self) -> Tuple[UnboundTerm[L], Set[Literal[L]]]:
+        """A magic function for pickling the SetPredicate class."""
+        return (self.term, self.literals)
 
-    def visit_greater_than(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
+    @property
+    @abstractmethod
+    def as_bound(self) -> Type[BoundSetPredicate[L]]:
+        return BoundSetPredicate[L]
 
-        if field.upper_bound is None:
-            return ROWS_CANNOT_MATCH
 
-        upper = _from_byte_buffer(term.ref().field.field_type, field.upper_bound)
+class BoundSetPredicate(BoundPredicate[L], ABC):
+    literals: Set[Literal[L]]
 
-        if literal.value >= upper:
-            return ROWS_CANNOT_MATCH
+    def __init__(self, term: BoundTerm[L], literals: Set[Literal[L]]):
+        # Since we don't know the type of BoundPredicate[L], we have to ignore this one
+        super().__init__(term)  # type: ignore
+        self.literals = _to_literal_set(literals)  # pylint: disable=W0621
 
-        return ROWS_MIGHT_MATCH
+    @cached_property
+    def value_set(self) -> Set[L]:
+        return {lit.value for lit in self.literals}
 
-    def visit_less_than(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
+    def __str__(self) -> str:
+        """Returns the string representation of the BoundSetPredicate class."""
+        # Sort to make it deterministic
+        return f"{str(self.__class__.__name__)}({str(self.term)}, {{{', '.join(sorted([str(literal) for literal in self.literals]))}}})"
 
-        if field.lower_bound is None:
-            return ROWS_CANNOT_MATCH
+    def __repr__(self) -> str:
+        """Returns the string representation of the BoundSetPredicate class."""
+        # Sort to make it deterministic
+        return f"{str(self.__class__.__name__)}({repr(self.term)}, {{{', '.join(sorted([repr(literal) for literal in self.literals]))}}})"
 
-        lower = _from_byte_buffer(term.ref().field.field_type, field.lower_bound)
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the BoundSetPredicate class."""
+        return self.term == other.term and self.literals == other.literals if isinstance(other, BoundSetPredicate) else False
 
-        if literal.value <= lower:
-            return ROWS_CANNOT_MATCH
+    def __getnewargs__(self) -> Tuple[BoundTerm[L], Set[Literal[L]]]:
+        """A magic function for pickling the BoundSetPredicate class."""
+        return (self.term, self.literals)
 
-        return ROWS_MIGHT_MATCH
+    @property
+    @abstractmethod
+    def as_unbound(self) -> Type[SetPredicate[L]]:
+        ...
 
-    def visit_less_than_or_equal(self, term: BoundTerm[L], literal: Literal[L]) -> bool:
-        pos = term.ref().accessor.position
-        field = self.partition_fields[pos]
 
-        if field.lower_bound is None:
-            return ROWS_CANNOT_MATCH
+class BoundIn(BoundSetPredicate[L]):
+    def __new__(cls, term: BoundTerm[L], literals: Set[Literal[L]]) -> BooleanExpression:  # type: ignore  # pylint: disable=W0221
+        count = len(literals)
+        if count == 0:
+            return AlwaysFalse()
+        elif count == 1:
+            return BoundEqualTo(term, next(iter(literals)))
+        else:
+            return super().__new__(cls)
 
-        lower = _from_byte_buffer(term.ref().field.field_type, field.lower_bound)
+    def __invert__(self) -> BoundNotIn[L]:
+        """Transform the Expression into its negated version."""
+        return BoundNotIn(self.term, self.literals)
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the BoundIn class."""
+        return self.term == other.term and self.literals == other.literals if isinstance(other, BoundIn) else False
+
+    @property
+    def as_unbound(self) -> Type[In[L]]:
+        return In
+
+
+class BoundNotIn(BoundSetPredicate[L]):
+    def __new__(  # type: ignore  # pylint: disable=W0221
+        cls,
+        term: BoundTerm[L],
+        literals: Set[Literal[L]],
+    ) -> BooleanExpression:
+        count = len(literals)
+        if count == 0:
+            return AlwaysTrue()
+        elif count == 1:
+            return BoundNotEqualTo(term, next(iter(literals)))
+        else:
+            return super().__new__(cls)
 
-        if literal.value < lower:
-            return ROWS_CANNOT_MATCH
+    def __invert__(self) -> BoundIn[L]:
+        """Transform the Expression into its negated version."""
+        return BoundIn(self.term, self.literals)
+
+    @property
+    def as_unbound(self) -> Type[NotIn[L]]:
+        return NotIn
+
+
+class In(SetPredicate[L]):
+    def __new__(  # type: ignore  # pylint: disable=W0221
+        cls, term: Union[str, UnboundTerm[Any]], literals: Union[Iterable[L], Iterable[Literal[L]]]
+    ) -> BooleanExpression:
+        literals_set: Set[Literal[L]] = _to_literal_set(literals)
+        count = len(literals_set)
+        if count == 0:
+            return AlwaysFalse()
+        elif count == 1:
+            return EqualTo(term, next(iter(literals)))  # type: ignore
+        else:
+            return super().__new__(cls)
 
-        return ROWS_MIGHT_MATCH
+    def __invert__(self) -> NotIn[L]:
+        """Transform the Expression into its negated version."""
+        return NotIn[L](self.term, self.literals)
+
+    @property
+    def as_bound(self) -> Type[BoundIn[L]]:
+        return BoundIn[L]
+
+
+class NotIn(SetPredicate[L], ABC):
+    def __new__(  # type: ignore  # pylint: disable=W0221
+        cls, term: Union[str, UnboundTerm[Any]], literals: Union[Iterable[L], Iterable[Literal[L]]]
+    ) -> BooleanExpression:
+        literals_set: Set[Literal[L]] = _to_literal_set(literals)
+        count = len(literals_set)
+        if count == 0:
+            return AlwaysTrue()
+        elif count == 1:
+            return NotEqualTo(term, next(iter(literals_set)))
+        else:
+            return super().__new__(cls)
 
-    def visit_true(self) -> bool:
-        return ROWS_MIGHT_MATCH
+    def __invert__(self) -> In[L]:
+        """Transform the Expression into its negated version."""
+        return In[L](self.term, self.literals)
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the NotIn class."""
+        if isinstance(other, NotIn):
+            return self.term == other.term and self.literals == other.literals
+        return False
 
-    def visit_false(self) -> bool:
-        return ROWS_CANNOT_MATCH
+    @property
+    def as_bound(self) -> Type[BoundNotIn[L]]:
+        return BoundNotIn[L]
+
+
+class LiteralPredicate(UnboundPredicate[L], ABC):
+    literal: Literal[L]
+
+    def __init__(self, term: Union[str, UnboundTerm[Any]], literal: Union[L, Literal[L]]):  # pylint: disable=W0621
+        super().__init__(term)
+        self.literal = _to_literal(literal)  # pylint: disable=W0621
+
+    def bind(self, schema: Schema, case_sensitive: bool = True) -> BoundLiteralPredicate[L]:
+        bound_term = self.term.bind(schema, case_sensitive)
+        lit = self.literal.to(bound_term.ref().field.field_type)
+
+        if isinstance(lit, AboveMax):
+            if isinstance(self, (LessThan, LessThanOrEqual, NotEqualTo)):
+                return AlwaysTrue()  # type: ignore
+            elif isinstance(self, (GreaterThan, GreaterThanOrEqual, EqualTo)):
+                return AlwaysFalse()  # type: ignore
+        elif isinstance(lit, BelowMin):
+            if isinstance(self, (GreaterThan, GreaterThanOrEqual, NotEqualTo)):
+                return AlwaysTrue()  # type: ignore
+            elif isinstance(self, (LessThan, LessThanOrEqual, EqualTo)):
+                return AlwaysFalse()  # type: ignore
+
+        return self.as_bound(bound_term, lit)
+
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the LiteralPredicate class."""
+        if isinstance(other, LiteralPredicate):
+            return self.term == other.term and self.literal == other.literal
+        return False
 
-    def visit_not(self, child_result: bool) -> bool:
-        return not child_result
+    def __repr__(self) -> str:
+        """Returns the string representation of the LiteralPredicate class."""
+        return f"{str(self.__class__.__name__)}(term={repr(self.term)}, literal={repr(self.literal)})"
 
-    def visit_and(self, left_result: bool, right_result: bool) -> bool:
-        return left_result and right_result
+    @property
+    @abstractmethod
+    def as_bound(self) -> Type[BoundLiteralPredicate[L]]:
+        ...
 
-    def visit_or(self, left_result: bool, right_result: bool) -> bool:
-        return left_result or right_result
 
+class BoundLiteralPredicate(BoundPredicate[L], ABC):
+    literal: Literal[L]
 
-def manifest_evaluator(
-    partition_spec: PartitionSpec, schema: Schema, partition_filter: BooleanExpression, case_sensitive: bool = True
-) -> Callable[[ManifestFile], bool]:
-    partition_type = partition_spec.partition_type(schema)
-    partition_schema = Schema(*partition_type.fields)
-    evaluator = _ManifestEvalVisitor(partition_schema, partition_filter, case_sensitive)
-    return evaluator.eval
+    def __init__(self, term: BoundTerm[L], literal: Literal[L]):  # pylint: disable=W0621
+        # Since we don't know the type of BoundPredicate[L], we have to ignore this one
+        super().__init__(term)  # type: ignore
+        self.literal = literal  # pylint: disable=W0621
 
+    def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the BoundLiteralPredicate class."""
+        if isinstance(other, BoundLiteralPredicate):
+            return self.term == other.term and self.literal == other.literal
+        return False
 
-class ProjectionEvaluator(BooleanExpressionVisitor[BooleanExpression], ABC):
-    schema: Schema
-    spec: PartitionSpec
-    case_sensitive: bool
+    def __repr__(self) -> str:
+        """Returns the string representation of the BoundLiteralPredicate class."""
+        return f"{str(self.__class__.__name__)}(term={repr(self.term)}, literal={repr(self.literal)})"
 
-    def __init__(self, schema: Schema, spec: PartitionSpec, case_sensitive: bool):
-        self.schema = schema
-        self.spec = spec
-        self.case_sensitive = case_sensitive
+    @property
+    @abstractmethod
+    def as_unbound(self) -> Type[LiteralPredicate[L]]:
+        ...
 
-    def project(self, expr: BooleanExpression) -> BooleanExpression:
-        #  projections assume that there are no NOT nodes in the expression tree. to ensure that this
-        #  is the case, the expression is rewritten to push all NOT nodes down to the expression
-        #  leaf nodes.
-        #  this is necessary to ensure that the default expression returned when a predicate can't be
-        #  projected is correct.
-        return visit(bind(self.schema, rewrite_not(expr), self.case_sensitive), self)
 
-    def visit_true(self) -> BooleanExpression:
-        return AlwaysTrue()
+class BoundEqualTo(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundNotEqualTo[L]:
+        """Transform the Expression into its negated version."""
+        return BoundNotEqualTo[L](self.term, self.literal)
 
-    def visit_false(self) -> BooleanExpression:
-        return AlwaysFalse()
+    @property
+    def as_unbound(self) -> Type[EqualTo[L]]:
+        return EqualTo
 
-    def visit_not(self, child_result: BooleanExpression) -> BooleanExpression:
-        raise ValueError(f"Cannot project not expression, should be rewritten: {child_result}")
 
-    def visit_and(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return And(left_result, right_result)
+class BoundNotEqualTo(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundEqualTo[L]:
+        """Transform the Expression into its negated version."""
+        return BoundEqualTo[L](self.term, self.literal)
 
-    def visit_or(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return Or(left_result, right_result)
+    @property
+    def as_unbound(self) -> Type[NotEqualTo[L]]:
+        return NotEqualTo
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> BooleanExpression:
-        raise ValueError(f"Cannot project unbound predicate: {predicate}")
 
+class BoundGreaterThanOrEqual(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundLessThan[L]:
+        """Transform the Expression into its negated version."""
+        return BoundLessThan[L](self.term, self.literal)
 
-class InclusiveProjection(ProjectionEvaluator):
-    def visit_bound_predicate(self, predicate: BoundPredicate[Any]) -> BooleanExpression:
-        parts = self.spec.fields_by_source_id(predicate.term.ref().field.field_id)
+    @property
+    def as_unbound(self) -> Type[GreaterThanOrEqual[L]]:
+        return GreaterThanOrEqual[L]
 
-        result: BooleanExpression = AlwaysTrue()
-        for part in parts:
-            # consider (d = 2019-01-01) with bucket(7, d) and bucket(5, d)
-            # projections: b1 = bucket(7, '2019-01-01') = 5, b2 = bucket(5, '2019-01-01') = 0
-            # any value where b1 != 5 or any value where b2 != 0 cannot be the '2019-01-01'
-            #
-            # similarly, if partitioning by day(ts) and hour(ts), the more restrictive
-            # projection should be used. ts = 2019-01-01T01:00:00 produces day=2019-01-01 and
-            # hour=2019-01-01-01. the value will be in 2019-01-01-01 and not in 2019-01-01-02.
-            incl_projection = part.transform.project(name=part.name, pred=predicate)
-            if incl_projection is not None:
-                result = And(result, incl_projection)
 
-        return result
+class BoundGreaterThan(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundLessThanOrEqual[L]:
+        """Transform the Expression into its negated version."""
+        return BoundLessThanOrEqual(self.term, self.literal)
 
+    @property
+    def as_unbound(self) -> Type[GreaterThan[L]]:
+        return GreaterThan[L]
 
-def inclusive_projection(
-    schema: Schema, spec: PartitionSpec, case_sensitive: bool = True
-) -> Callable[[BooleanExpression], BooleanExpression]:
-    return InclusiveProjection(schema, spec, case_sensitive).project
 
+class BoundLessThan(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundGreaterThanOrEqual[L]:
+        """Transform the Expression into its negated version."""
+        return BoundGreaterThanOrEqual[L](self.term, self.literal)
 
-class _ColumnNameTranslator(BooleanExpressionVisitor[BooleanExpression]):
-    """Converts the column names with the ones in the actual file
+    @property
+    def as_unbound(self) -> Type[LessThan[L]]:
+        return LessThan[L]
 
-    Args:
-      file_schema (Schema): The schema of the file
-      case_sensitive (bool): Whether to consider case when binding a reference to a field in a schema, defaults to True
 
-    Raises:
-        TypeError: In the case of an UnboundPredicate
-        ValueError: When a column name cannot be found
-    """
+class BoundLessThanOrEqual(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundGreaterThan[L]:
+        """Transform the Expression into its negated version."""
+        return BoundGreaterThan[L](self.term, self.literal)
 
-    file_schema: Schema
-    case_sensitive: bool
+    @property
+    def as_unbound(self) -> Type[LessThanOrEqual[L]]:
+        return LessThanOrEqual[L]
 
-    def __init__(self, file_schema: Schema, case_sensitive: bool) -> None:
-        self.file_schema = file_schema
-        self.case_sensitive = case_sensitive
 
-    def visit_true(self) -> BooleanExpression:
-        return AlwaysTrue()
+class BoundStartsWith(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundNotStartsWith[L]:
+        """Transform the Expression into its negated version."""
+        return BoundNotStartsWith[L](self.term, self.literal)
 
-    def visit_false(self) -> BooleanExpression:
-        return AlwaysFalse()
+    @property
+    def as_unbound(self) -> Type[StartsWith[L]]:
+        return StartsWith[L]
 
-    def visit_not(self, child_result: BooleanExpression) -> BooleanExpression:
-        return Not(child=child_result)
 
-    def visit_and(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return And(left=left_result, right=right_result)
+class BoundNotStartsWith(BoundLiteralPredicate[L]):
+    def __invert__(self) -> BoundStartsWith[L]:
+        """Transform the Expression into its negated version."""
+        return BoundStartsWith[L](self.term, self.literal)
 
-    def visit_or(self, left_result: BooleanExpression, right_result: BooleanExpression) -> BooleanExpression:
-        return Or(left=left_result, right=right_result)
+    @property
+    def as_unbound(self) -> Type[NotStartsWith[L]]:
+        return NotStartsWith[L]
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> BooleanExpression:
-        raise TypeError(f"Expected Bound Predicate, got: {predicate.term}")
-
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> BooleanExpression:
-        file_column_name = self.file_schema.find_column_name(predicate.term.ref().field.field_id)
-
-        if not file_column_name:
-            raise ValueError(f"Not found in file schema: {file_column_name}")
-
-        if isinstance(predicate, BoundUnaryPredicate):
-            return predicate.as_unbound(file_column_name)
-        elif isinstance(predicate, BoundLiteralPredicate):
-            return predicate.as_unbound(file_column_name, predicate.literal)
-        elif isinstance(predicate, BoundSetPredicate):
-            return predicate.as_unbound(file_column_name, predicate.literals)
-        else:
-            raise ValueError(f"Unsupported predicate: {predicate}")
 
+class EqualTo(LiteralPredicate[L]):
+    def __invert__(self) -> NotEqualTo[L]:
+        """Transform the Expression into its negated version."""
+        return NotEqualTo[L](self.term, self.literal)
 
-def translate_column_names(expr: BooleanExpression, file_schema: Schema, case_sensitive: bool) -> BooleanExpression:
-    return visit(expr, _ColumnNameTranslator(file_schema, case_sensitive))
+    @property
+    def as_bound(self) -> Type[BoundEqualTo[L]]:
+        return BoundEqualTo[L]
 
 
-class _ExpressionFieldIDs(BooleanExpressionVisitor[Set[int]]):
-    """Extracts the field IDs used in the BooleanExpression"""
+class NotEqualTo(LiteralPredicate[L]):
+    def __invert__(self) -> EqualTo[L]:
+        """Transform the Expression into its negated version."""
+        return EqualTo[L](self.term, self.literal)
 
-    def visit_true(self) -> Set[int]:
-        return set()
+    @property
+    def as_bound(self) -> Type[BoundNotEqualTo[L]]:
+        return BoundNotEqualTo[L]
 
-    def visit_false(self) -> Set[int]:
-        return set()
 
-    def visit_not(self, child_result: Set[int]) -> Set[int]:
-        return child_result
+class LessThan(LiteralPredicate[L]):
+    def __invert__(self) -> GreaterThanOrEqual[L]:
+        """Transform the Expression into its negated version."""
+        return GreaterThanOrEqual[L](self.term, self.literal)
 
-    def visit_and(self, left_result: Set[int], right_result: Set[int]) -> Set[int]:
-        return left_result.union(right_result)
+    @property
+    def as_bound(self) -> Type[BoundLessThan[L]]:
+        return BoundLessThan[L]
 
-    def visit_or(self, left_result: Set[int], right_result: Set[int]) -> Set[int]:
-        return left_result.union(right_result)
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> Set[int]:
-        raise ValueError("Only works on bound records")
+class GreaterThanOrEqual(LiteralPredicate[L]):
+    def __invert__(self) -> LessThan[L]:
+        """Transform the Expression into its negated version."""
+        return LessThan[L](self.term, self.literal)
 
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> Set[int]:
-        return {predicate.term.ref().field.field_id}
+    @property
+    def as_bound(self) -> Type[BoundGreaterThanOrEqual[L]]:
+        return BoundGreaterThanOrEqual[L]
 
 
-def extract_field_ids(expr: BooleanExpression) -> Set[int]:
-    return visit(expr, _ExpressionFieldIDs())
+class GreaterThan(LiteralPredicate[L]):
+    def __invert__(self) -> LessThanOrEqual[L]:
+        """Transform the Expression into its negated version."""
+        return LessThanOrEqual[L](self.term, self.literal)
 
+    @property
+    def as_bound(self) -> Type[BoundGreaterThan[L]]:
+        return BoundGreaterThan[L]
 
-class _RewriteToDNF(BooleanExpressionVisitor[Tuple[BooleanExpression, ...]]):
-    def visit_true(self) -> Tuple[BooleanExpression, ...]:
-        return (AlwaysTrue(),)
 
-    def visit_false(self) -> Tuple[BooleanExpression, ...]:
-        return (AlwaysFalse(),)
+class LessThanOrEqual(LiteralPredicate[L]):
+    def __invert__(self) -> GreaterThan[L]:
+        """Transform the Expression into its negated version."""
+        return GreaterThan[L](self.term, self.literal)
 
-    def visit_not(self, child_result: Tuple[BooleanExpression, ...]) -> Tuple[BooleanExpression, ...]:
-        raise ValueError(f"Not expressions are not allowed: {child_result}")
+    @property
+    def as_bound(self) -> Type[BoundLessThanOrEqual[L]]:
+        return BoundLessThanOrEqual[L]
 
-    def visit_and(
-        self, left_result: Tuple[BooleanExpression, ...], right_result: Tuple[BooleanExpression, ...]
-    ) -> Tuple[BooleanExpression, ...]:
-        # Distributive law:
-        # ((P OR Q) AND (R OR S)) AND (((P AND R) OR (P AND S)) OR ((Q AND R) OR ((Q AND S)))
-        # A AND (B OR C) = (A AND B) OR (A AND C)
-        # (A OR B) AND C = (A AND C) OR (B AND C)
-        return tuple(And(le, re) for le in left_result for re in right_result)
 
-    def visit_or(
-        self, left_result: Tuple[BooleanExpression, ...], right_result: Tuple[BooleanExpression, ...]
-    ) -> Tuple[BooleanExpression, ...]:
-        return left_result + right_result
+class StartsWith(LiteralPredicate[L]):
+    def __invert__(self) -> NotStartsWith[L]:
+        """Transform the Expression into its negated version."""
+        return NotStartsWith[L](self.term, self.literal)
 
-    def visit_unbound_predicate(self, predicate: UnboundPredicate[L]) -> Tuple[BooleanExpression, ...]:
-        return (predicate,)
+    @property
+    def as_bound(self) -> Type[BoundStartsWith[L]]:
+        return BoundStartsWith[L]
 
-    def visit_bound_predicate(self, predicate: BoundPredicate[L]) -> Tuple[BooleanExpression, ...]:
-        return (predicate,)
 
+class NotStartsWith(LiteralPredicate[L]):
+    def __invert__(self) -> NotStartsWith[L]:
+        """Transform the Expression into its negated version."""
+        return NotStartsWith[L](self.term, self.literal)
 
-def rewrite_to_dnf(expr: BooleanExpression) -> Tuple[BooleanExpression, ...]:
-    # Rewrites an arbitrary boolean expression to disjunctive normal form (DNF):
-    # (A AND NOT(B) AND C) OR (NOT(D) AND E AND F) OR (G)
-    expr_without_not = rewrite_not(expr)
-    return visit(expr_without_not, _RewriteToDNF())
+    @property
+    def as_bound(self) -> Type[BoundNotStartsWith[L]]:
+        return BoundNotStartsWith[L]
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/files.py` & `pyiceberg-0.4.0rc1/pyiceberg/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from enum import Enum, auto
 
 
 class FileContentType(Enum):
-    """An enum that includes all possible content types for an Iceberg data file"""
+    """An enum that includes all possible content types for an Iceberg data file."""
 
     DATA = auto()
     POSITION_DELETES = auto()
     EQUALITY_DELETES = auto()
 
 
 class FileFormat(Enum):
-    """An enum that includes all possible formats for an Iceberg data file"""
+    """An enum that includes all possible formats for an Iceberg data file."""
 
-    ORC = auto()
-    PARQUET = auto()
-    AVRO = auto()
-    METADATA = auto()
+    ORC = "ORC"
+    PARQUET = "PARQUET"
+    AVRO = "AVRO"
+    METADATA = "METADATA"
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/io/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/io/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Base FileIO classes for implementing reading and writing table files
+"""Base FileIO classes for implementing reading and writing table files.
 
 The FileIO abstraction includes a subset of full filesystem implementations. Specifically,
 Iceberg needs to read or write a file at a given location (as a seekable stream), as well
 as check if a file exists. An implementation of the FileIO abstract base class is responsible
 for returning an InputFile instance, an OutputFile instance, and deleting a file given
 its location.
 """
 from __future__ import annotations
 
 import importlib
 import logging
+import warnings
 from abc import ABC, abstractmethod
 from io import SEEK_SET
 from types import TracebackType
 from typing import (
     Dict,
     List,
     Optional,
@@ -40,18 +41,24 @@
 )
 from urllib.parse import urlparse
 
 from pyiceberg.typedef import EMPTY_DICT, Properties
 
 logger = logging.getLogger(__name__)
 
+S3_ENDPOINT = "s3.endpoint"
+S3_ACCESS_KEY_ID = "s3.access-key-id"
+S3_SECRET_ACCESS_KEY = "s3.secret-access-key"
+S3_SESSION_TOKEN = "s3.session-token"
+S3_REGION = "s3.region"
+
 
 @runtime_checkable
 class InputStream(Protocol):
-    """A protocol for the file-like object returned by InputFile.open(...)
+    """A protocol for the file-like object returned by InputFile.open(...).
 
     This outlines the minimally required methods for a seekable input stream returned from an InputFile
     implementation's `open(...)` method. These methods are a subset of IOBase/RawIOBase.
     """
 
     @abstractmethod
     def read(self, size: int = 0) -> bytes:
@@ -66,26 +73,26 @@
         ...
 
     @abstractmethod
     def close(self) -> None:
         ...
 
     def __enter__(self) -> InputStream:
-        ...
+        """Provides setup when opening an InputStream using a 'with' statement."""
 
     @abstractmethod
     def __exit__(
         self, exctype: Optional[Type[BaseException]], excinst: Optional[BaseException], exctb: Optional[TracebackType]
     ) -> None:
-        ...
+        """Performs cleanup when exiting the scope of a 'with' statement."""
 
 
 @runtime_checkable
 class OutputStream(Protocol):  # pragma: no cover
-    """A protocol for the file-like object returned by OutputFile.create(...)
+    """A protocol for the file-like object returned by OutputFile.create(...).
 
     This outlines the minimally required methods for a writable output stream returned from an OutputFile
     implementation's `create(...)` method. These methods are a subset of IOBase/RawIOBase.
     """
 
     @abstractmethod
     def write(self, b: bytes) -> int:
@@ -93,175 +100,173 @@
 
     @abstractmethod
     def close(self) -> None:
         ...
 
     @abstractmethod
     def __enter__(self) -> OutputStream:
-        ...
+        """Provides setup when opening an OutputStream using a 'with' statement."""
 
     @abstractmethod
     def __exit__(
         self, exctype: Optional[Type[BaseException]], excinst: Optional[BaseException], exctb: Optional[TracebackType]
     ) -> None:
-        ...
+        """Performs cleanup when exiting the scope of a 'with' statement."""
 
 
 class InputFile(ABC):
-    """A base class for InputFile implementations
+    """A base class for InputFile implementations.
 
     Args:
-        location(str): A URI or a path to a local file
+        location (str): A URI or a path to a local file.
 
     Attributes:
-        location(str): The URI or path to a local file for an InputFile instance
-        exists(bool): Whether the file exists or not
+        location (str): The URI or path to a local file for an InputFile instance.
+        exists (bool): Whether the file exists or not.
     """
 
     def __init__(self, location: str):
         self._location = location
 
     @abstractmethod
     def __len__(self) -> int:
-        """Returns the total length of the file, in bytes"""
+        """Returns the total length of the file, in bytes."""
 
     @property
     def location(self) -> str:
-        """The fully-qualified location of the input file"""
+        """The fully-qualified location of the input file."""
         return self._location
 
     @abstractmethod
     def exists(self) -> bool:
-        """Checks whether the location exists
-
+        """Checks whether the location exists.
 
         Raises:
-            PermissionError: If the file at self.location cannot be accessed due to a permission error
+            PermissionError: If the file at self.location cannot be accessed due to a permission error.
         """
 
     @abstractmethod
     def open(self, seekable: bool = True) -> InputStream:
-        """This method should return an object that matches the InputStream protocol
+        """This method should return an object that matches the InputStream protocol.
 
         Args:
-            seekable: If the stream should support seek, or if it is consumed sequential
+            seekable: If the stream should support seek, or if it is consumed sequential.
 
         Returns:
-            InputStream: An object that matches the InputStream protocol
+            InputStream: An object that matches the InputStream protocol.
 
         Raises:
-            PermissionError: If the file at self.location cannot be accessed due to a permission error
-            FileNotFoundError: If the file at self.location does not exist
+            PermissionError: If the file at self.location cannot be accessed due to a permission error.
+            FileNotFoundError: If the file at self.location does not exist.
         """
 
 
 class OutputFile(ABC):
-    """A base class for OutputFile implementations
+    """A base class for OutputFile implementations.
 
     Args:
-        location(str): A URI or a path to a local file
+        location (str): A URI or a path to a local file.
 
     Attributes:
-        location(str): The URI or path to a local file for an OutputFile instance
-        exists(bool): Whether the file exists or not
+        location (str): The URI or path to a local file for an OutputFile instance.
+        exists (bool): Whether the file exists or not.
     """
 
     def __init__(self, location: str):
         self._location = location
 
     @abstractmethod
     def __len__(self) -> int:
-        """Returns the total length of the file, in bytes"""
+        """Returns the total length of the file, in bytes."""
 
     @property
     def location(self) -> str:
-        """The fully-qualified location of the output file"""
+        """The fully-qualified location of the output file."""
         return self._location
 
     @abstractmethod
     def exists(self) -> bool:
-        """Checks whether the location exists
-
+        """Checks whether the location exists.
 
         Raises:
-            PermissionError: If the file at self.location cannot be accessed due to a permission error
+            PermissionError: If the file at self.location cannot be accessed due to a permission error.
         """
 
     @abstractmethod
     def to_input_file(self) -> InputFile:
-        """Returns an InputFile for the location of this output file"""
+        """Returns an InputFile for the location of this output file."""
 
     @abstractmethod
     def create(self, overwrite: bool = False) -> OutputStream:
         """This method should return an object that matches the OutputStream protocol.
 
         Args:
-            overwrite(bool): If the file already exists at `self.location`
-            and `overwrite` is False a FileExistsError should be raised
+            overwrite (bool): If the file already exists at `self.location`
+                and `overwrite` is False a FileExistsError should be raised.
 
         Returns:
-            OutputStream: An object that matches the OutputStream protocol
+            OutputStream: An object that matches the OutputStream protocol.
 
         Raises:
-            PermissionError: If the file at self.location cannot be accessed due to a permission error
-            FileExistsError: If the file at self.location already exists and `overwrite=False`
+            PermissionError: If the file at self.location cannot be accessed due to a permission error.
+            FileExistsError: If the file at self.location already exists and `overwrite=False`.
         """
 
 
 class FileIO(ABC):
-    """A base class for FileIO implementations"""
+    """A base class for FileIO implementations."""
 
     properties: Properties
 
     def __init__(self, properties: Properties = EMPTY_DICT):
         self.properties = properties
 
     @abstractmethod
     def new_input(self, location: str) -> InputFile:
-        """Get an InputFile instance to read bytes from the file at the given location
+        """Get an InputFile instance to read bytes from the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
         """
 
     @abstractmethod
     def new_output(self, location: str) -> OutputFile:
-        """Get an OutputFile instance to write bytes to the file at the given location
+        """Get an OutputFile instance to write bytes to the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
         """
 
     @abstractmethod
     def delete(self, location: Union[str, InputFile, OutputFile]) -> None:
-        """Delete the file at the given path
+        """Delete the file at the given path.
 
         Args:
-            location(str, InputFile, OutputFile): A URI or a path to a local file--if an InputFile instance or
-            an OutputFile instance is provided, the location attribute for that instance is used as the URI to delete
+            location (Union[str, InputFile, OutputFile]): A URI or a path to a local file--if an InputFile instance or
+                an OutputFile instance is provided, the location attribute for that instance is used as the URI to delete.
 
         Raises:
-            PermissionError: If the file at location cannot be accessed due to a permission error
-            FileNotFoundError: When the file at the provided location does not exist
+            PermissionError: If the file at location cannot be accessed due to a permission error.
+            FileNotFoundError: When the file at the provided location does not exist.
         """
 
 
 LOCATION = "location"
 WAREHOUSE = "warehouse"
 
 ARROW_FILE_IO = "pyiceberg.io.pyarrow.PyArrowFileIO"
 FSSPEC_FILE_IO = "pyiceberg.io.fsspec.FsspecFileIO"
 
 # Mappings from the Java FileIO impl to a Python one. The list is ordered by preference.
 # If an implementation isn't installed, it will fall back to the next one.
 SCHEMA_TO_FILE_IO: Dict[str, List[str]] = {
-    "s3": [FSSPEC_FILE_IO, ARROW_FILE_IO],
-    "s3a": [FSSPEC_FILE_IO, ARROW_FILE_IO],
-    "s3n": [FSSPEC_FILE_IO, ARROW_FILE_IO],
-    "gcs": [ARROW_FILE_IO],
+    "s3": [ARROW_FILE_IO, FSSPEC_FILE_IO],
+    "s3a": [ARROW_FILE_IO, FSSPEC_FILE_IO],
+    "s3n": [ARROW_FILE_IO, FSSPEC_FILE_IO],
+    "gs": [ARROW_FILE_IO],
     "file": [ARROW_FILE_IO],
     "hdfs": [ARROW_FILE_IO],
     "abfs": [FSSPEC_FILE_IO],
     "abfss": [FSSPEC_FILE_IO],
 }
 
 
@@ -278,42 +283,43 @@
         logger.warning("Could not initialize FileIO: %s", io_impl)
         return None
 
 
 PY_IO_IMPL = "py-io-impl"
 
 
-def _infer_file_io_from_schema(path: str, properties: Properties) -> Optional[FileIO]:
+def _infer_file_io_from_scheme(path: str, properties: Properties) -> Optional[FileIO]:
     parsed_url = urlparse(path)
-    if file_ios := SCHEMA_TO_FILE_IO.get(parsed_url.scheme):
-        for file_io_path in file_ios:
-            if file_io := _import_file_io(file_io_path, properties):
-                return file_io
-    else:
-        logger.warning("No preferred file implementation for schema: %s", parsed_url.scheme)
+    if parsed_url.scheme:
+        if file_ios := SCHEMA_TO_FILE_IO.get(parsed_url.scheme):
+            for file_io_path in file_ios:
+                if file_io := _import_file_io(file_io_path, properties):
+                    return file_io
+        else:
+            warnings.warn(f"No preferred file implementation for scheme: {parsed_url.scheme}")
     return None
 
 
 def load_file_io(properties: Properties = EMPTY_DICT, location: Optional[str] = None) -> FileIO:
     # First look for the py-io-impl property to directly load the class
     if io_impl := properties.get(PY_IO_IMPL):
         if file_io := _import_file_io(io_impl, properties):
             logger.info("Loaded FileIO: %s", io_impl)
             return file_io
         else:
             raise ValueError(f"Could not initialize FileIO: {io_impl}")
 
     # Check the table location
     if location:
-        if file_io := _infer_file_io_from_schema(location, properties):
+        if file_io := _infer_file_io_from_scheme(location, properties):
             return file_io
 
     # Look at the schema of the warehouse
     if warehouse_location := properties.get(WAREHOUSE):
-        if file_io := _infer_file_io_from_schema(warehouse_location, properties):
+        if file_io := _infer_file_io_from_scheme(warehouse_location, properties):
             return file_io
 
     try:
         # Default to PyArrow
         logger.info("Defaulting to PyArrow FileIO")
         from pyiceberg.io.pyarrow import PyArrowFileIO
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/io/fsspec.py` & `pyiceberg-0.4.0rc1/pyiceberg/io/fsspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""FileIO implementation for reading and writing table files that uses fsspec compatible filesystems"""
+"""FileIO implementation for reading and writing table files that uses fsspec compatible filesystems."""
 import errno
 import logging
 import os
 from functools import lru_cache, partial
 from typing import (
     Any,
     Callable,
@@ -27,19 +27,25 @@
 )
 from urllib.parse import urlparse
 
 import requests
 from botocore import UNSIGNED
 from botocore.awsrequest import AWSRequest
 from fsspec import AbstractFileSystem
+from fsspec.implementations.local import LocalFileSystem
 from requests import HTTPError
 
 from pyiceberg.catalog import TOKEN
 from pyiceberg.exceptions import SignError
 from pyiceberg.io import (
+    S3_ACCESS_KEY_ID,
+    S3_ENDPOINT,
+    S3_REGION,
+    S3_SECRET_ACCESS_KEY,
+    S3_SESSION_TOKEN,
     FileIO,
     InputFile,
     InputStream,
     OutputFile,
     OutputStream,
 )
 from pyiceberg.typedef import Properties
@@ -74,22 +80,27 @@
 
     return request
 
 
 SIGNERS: Dict[str, Callable[[Properties, AWSRequest], AWSRequest]] = {"S3V4RestSigner": s3v4_rest_signer}
 
 
+def _file(_: Properties) -> LocalFileSystem:
+    return LocalFileSystem()
+
+
 def _s3(properties: Properties) -> AbstractFileSystem:
     from s3fs import S3FileSystem
 
     client_kwargs = {
-        "endpoint_url": properties.get("s3.endpoint"),
-        "aws_access_key_id": properties.get("s3.access-key-id"),
-        "aws_secret_access_key": properties.get("s3.secret-access-key"),
-        "aws_session_token": properties.get("s3.session-token"),
+        "endpoint_url": properties.get(S3_ENDPOINT),
+        "aws_access_key_id": properties.get(S3_ACCESS_KEY_ID),
+        "aws_secret_access_key": properties.get(S3_SECRET_ACCESS_KEY),
+        "aws_session_token": properties.get(S3_SESSION_TOKEN),
+        "region_name": properties.get(S3_REGION),
     }
     config_kwargs = {}
     register_events: Dict[str, Callable[[Properties], None]] = {}
 
     if signer := properties.get("s3.signer"):
         logger.info("Loading signer %s", signer)
         if singer_func := SIGNERS.get(signer):
@@ -108,173 +119,181 @@
 
     return fs
 
 
 def _adlfs(properties: Properties) -> AbstractFileSystem:
     from adlfs import AzureBlobFileSystem
 
-    fs = AzureBlobFileSystem(**properties)
-    return fs
+    return AzureBlobFileSystem(
+        connection_string=properties.get("adlfs.connection-string"),
+        account_name=properties.get("adlfs.account-name"),
+        account_key=properties.get("adlfs.account-key"),
+        sas_token=properties.get("adlfs.sas-token"),
+        tenant_id=properties.get("adlfs.tenant-id"),
+        client_id=properties.get("adlfs.client-id"),
+        client_secret=properties.get("adlfs.client-secret"),
+    )
 
 
 SCHEME_TO_FS = {
+    "file": _file,
     "s3": _s3,
     "s3a": _s3,
     "s3n": _s3,
     "abfs": _adlfs,
     "abfss": _adlfs,
 }
 
 
 class FsspecInputFile(InputFile):
-    """An input file implementation for the FsspecFileIO
+    """An input file implementation for the FsspecFileIO.
 
     Args:
-        location(str): A URI to a file location
-        fs(AbstractFileSystem): An fsspec filesystem instance
+        location (str): A URI to a file location.
+        fs (AbstractFileSystem): An fsspec filesystem instance.
     """
 
     def __init__(self, location: str, fs: AbstractFileSystem):
         self._fs = fs
         super().__init__(location=location)
 
     def __len__(self) -> int:
-        """Returns the total length of the file, in bytes"""
+        """Returns the total length of the file, in bytes."""
         object_info = self._fs.info(self.location)
         if size := object_info.get("Size"):
             return size
         elif size := object_info.get("size"):
             return size
         raise RuntimeError(f"Cannot retrieve object info: {self.location}")
 
     def exists(self) -> bool:
-        """Checks whether the location exists"""
+        """Checks whether the location exists."""
         return self._fs.lexists(self.location)
 
     def open(self, seekable: bool = True) -> InputStream:
-        """Create an input stream for reading the contents of the file
+        """Create an input stream for reading the contents of the file.
 
         Args:
-            seekable: If the stream should support seek, or if it is consumed sequential
+            seekable: If the stream should support seek, or if it is consumed sequential.
 
         Returns:
-            OpenFile: An fsspec compliant file-like object
+            OpenFile: An fsspec compliant file-like object.
 
         Raises:
-            FileNotFoundError: If the file does not exist
+            FileNotFoundError: If the file does not exist.
         """
         try:
             return self._fs.open(self.location, "rb")
         except FileNotFoundError as e:
             # To have a consistent error handling experience, make sure exception contains missing file location.
             raise e if e.filename else FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), self.location) from e
 
 
 class FsspecOutputFile(OutputFile):
-    """An output file implementation for the FsspecFileIO
+    """An output file implementation for the FsspecFileIO.
 
     Args:
-        location(str): A URI to a file location
-        fs(AbstractFileSystem): An fsspec filesystem instance
+        location (str): A URI to a file location.
+        fs (AbstractFileSystem): An fsspec filesystem instance.
     """
 
     def __init__(self, location: str, fs: AbstractFileSystem):
         self._fs = fs
         super().__init__(location=location)
 
     def __len__(self) -> int:
-        """Returns the total length of the file, in bytes"""
+        """Returns the total length of the file, in bytes."""
         object_info = self._fs.info(self.location)
         if size := object_info.get("Size"):
             return size
         elif size := object_info.get("size"):
             return size
         raise RuntimeError(f"Cannot retrieve object info: {self.location}")
 
     def exists(self) -> bool:
-        """Checks whether the location exists"""
+        """Checks whether the location exists."""
         return self._fs.lexists(self.location)
 
     def create(self, overwrite: bool = False) -> OutputStream:
-        """Create an output stream for reading the contents of the file
+        """Create an output stream for reading the contents of the file.
 
         Args:
-            overwrite(bool): Whether to overwrite the file if it already exists
+            overwrite (bool): Whether to overwrite the file if it already exists.
 
         Returns:
-            OpenFile: An fsspec compliant file-like object
+            OpenFile: An fsspec compliant file-like object.
 
         Raises:
-            FileExistsError: If the file already exists at the location and overwrite is set to False
+            FileExistsError: If the file already exists at the location and overwrite is set to False.
 
         Note:
             If overwrite is set to False, a check is first performed to verify that the file does not exist.
             This is not thread-safe and a possibility does exist that the file can be created by a concurrent
             process after the existence check yet before the output stream is created. In such a case, the default
             behavior will truncate the contents of the existing file when opening the output stream.
         """
         if not overwrite and self.exists():
             raise FileExistsError(f"Cannot create file, file already exists: {self.location}")
         return self._fs.open(self.location, "wb")
 
     def to_input_file(self) -> FsspecInputFile:
-        """Returns a new FsspecInputFile for the location at `self.location`"""
+        """Returns a new FsspecInputFile for the location at `self.location`."""
         return FsspecInputFile(location=self.location, fs=self._fs)
 
 
 class FsspecFileIO(FileIO):
-    """A FileIO implementation that uses fsspec"""
+    """A FileIO implementation that uses fsspec."""
 
     def __init__(self, properties: Properties):
         self._scheme_to_fs = {}
         self._scheme_to_fs.update(SCHEME_TO_FS)
         self.get_fs: Callable[[str], AbstractFileSystem] = lru_cache(self._get_fs)
         super().__init__(properties=properties)
 
     def new_input(self, location: str) -> FsspecInputFile:
-        """Get an FsspecInputFile instance to read bytes from the file at the given location
+        """Get an FsspecInputFile instance to read bytes from the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
 
         Returns:
-            FsspecInputFile: An FsspecInputFile instance for the given location
+            FsspecInputFile: An FsspecInputFile instance for the given location.
         """
         uri = urlparse(location)
         fs = self.get_fs(uri.scheme)
         return FsspecInputFile(location=location, fs=fs)
 
     def new_output(self, location: str) -> FsspecOutputFile:
-        """Get an FsspecOutputFile instance to write bytes to the file at the given location
+        """Get an FsspecOutputFile instance to write bytes to the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
 
         Returns:
-            FsspecOutputFile: An FsspecOutputFile instance for the given location
+            FsspecOutputFile: An FsspecOutputFile instance for the given location.
         """
         uri = urlparse(location)
         fs = self.get_fs(uri.scheme)
         return FsspecOutputFile(location=location, fs=fs)
 
     def delete(self, location: Union[str, InputFile, OutputFile]) -> None:
-        """Delete the file at the given location
+        """Delete the file at the given location.
 
         Args:
-            location(str, InputFile, OutputFile): The URI to the file--if an InputFile instance or an
-            OutputFile instance is provided, the location attribute for that instance is used as the location
-            to delete
+            location (Union[str, InputFile, OutputFile]): The URI to the file--if an InputFile instance or an
+                OutputFile instance is provided, the location attribute for that instance is used as the location
+                to delete.
         """
         if isinstance(location, (InputFile, OutputFile)):
             str_location = location.location  # Use InputFile or OutputFile location
         else:
             str_location = location
 
         uri = urlparse(str_location)
         fs = self.get_fs(uri.scheme)
         fs.rm(str_location)
 
     def _get_fs(self, scheme: str) -> AbstractFileSystem:
-        """Get a filesystem for a specific scheme"""
+        """Get a filesystem for a specific scheme."""
         if scheme not in self._scheme_to_fs:
             raise ValueError(f"No registered filesystem for scheme: {scheme}")
         return self._scheme_to_fs[scheme](self.properties)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/io/memory.py` & `pyiceberg-0.4.0rc1/pyiceberg/io/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Optional, Type
 
 from pyiceberg.io import InputStream
 
 
 class MemoryInputStream(InputStream):
     """
-    Simple in memory stream that we use to store decompressed blocks
+    Simple in memory stream that we use to store decompressed blocks.
 
     Examples:
         >>> stream = MemoryInputStream(b'22memory1925')
         >>> stream.tell()
         0
         >>> stream.read(2)
         b'22'
@@ -71,13 +71,15 @@
         return self.pos
 
     def close(self) -> None:
         del self.buffer
         self.pos = 0
 
     def __enter__(self) -> MemoryInputStream:
+        """Provides setup when opening a MemoryInputStream using a 'with' statement."""
         return self
 
     def __exit__(
         self, exctype: Optional[Type[BaseException]], excinst: Optional[BaseException], exctb: Optional[TracebackType]
     ) -> None:
+        """Performs cleanup when exiting the scope of a 'with' statement."""
         self.close()
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/io/pyarrow.py` & `pyiceberg-0.4.0rc1/pyiceberg/io/pyarrow.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,49 +10,60 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-# pylint: disable=redefined-outer-name,arguments-renamed
-"""FileIO implementation for reading and writing table files that uses pyarrow.fs
+# pylint: disable=redefined-outer-name,arguments-renamed,fixme
+"""FileIO implementation for reading and writing table files that uses pyarrow.fs.
 
 This file contains a FileIO implementation that relies on the filesystem interface provided
 by PyArrow. It relies on PyArrow's `from_uri` method that infers the correct filesystem
 type to use. Theoretically, this allows the supported storage types to grow naturally
 with the pyarrow library.
 """
 from __future__ import annotations
 
+import multiprocessing
 import os
-from functools import lru_cache
+from abc import ABC, abstractmethod
+from functools import lru_cache, singledispatch
+from itertools import chain
 from multiprocessing.pool import ThreadPool
+from multiprocessing.sharedctypes import Synchronized
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Dict,
+    Generic,
     Iterable,
     List,
     Optional,
     Set,
     Tuple,
+    TypeVar,
     Union,
+    cast,
 )
 from urllib.parse import urlparse
 
+import numpy as np
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
-import pyarrow.parquet as pq
+from pyarrow import ChunkedArray
 from pyarrow.fs import (
     FileInfo,
     FileSystem,
     FileType,
+    FSSpecHandler,
     LocalFileSystem,
+    PyFileSystem,
     S3FileSystem,
 )
 
 from pyiceberg.avro.resolver import ResolveError
 from pyiceberg.expressions import (
     AlwaysTrue,
     BooleanExpression,
@@ -63,20 +74,26 @@
     BoundBooleanExpressionVisitor,
     bind,
     extract_field_ids,
     translate_column_names,
 )
 from pyiceberg.expressions.visitors import visit as boolean_expression_visit
 from pyiceberg.io import (
+    S3_ACCESS_KEY_ID,
+    S3_ENDPOINT,
+    S3_REGION,
+    S3_SECRET_ACCESS_KEY,
+    S3_SESSION_TOKEN,
     FileIO,
     InputFile,
     InputStream,
     OutputFile,
     OutputStream,
 )
+from pyiceberg.manifest import DataFile, FileFormat
 from pyiceberg.schema import (
     PartnerAccessor,
     Schema,
     SchemaVisitorPerPrimitiveType,
     SchemaWithPartnerVisitor,
     promote,
     prune_columns,
@@ -110,24 +127,30 @@
 
 if TYPE_CHECKING:
     from pyiceberg.table import FileScanTask, Table
 
 ONE_MEGABYTE = 1024 * 1024
 BUFFER_SIZE = "buffer-size"
 ICEBERG_SCHEMA = b"iceberg.schema"
+FIELD_ID = "field_id"
+DOC = "doc"
+PYARROW_FIELD_ID_KEYS = [b"PARQUET:field_id", b"field_id"]
+PYARROW_FIELD_DOC_KEYS = [b"PARQUET:field_doc", b"field_doc", b"doc"]
+
+T = TypeVar("T")
 
 
 class PyArrowFile(InputFile, OutputFile):
-    """A combined InputFile and OutputFile implementation that uses a pyarrow filesystem to generate pyarrow.lib.NativeFile instances
+    """A combined InputFile and OutputFile implementation that uses a pyarrow filesystem to generate pyarrow.lib.NativeFile instances.
 
     Args:
-        location(str): A URI or a path to a local file
+        location (str): A URI or a path to a local file.
 
     Attributes:
-        location(str): The URI or path to a local file for a PyArrowFile instance
+        location(str): The URI or path to a local file for a PyArrowFile instance.
 
     Examples:
         >>> from pyiceberg.io.pyarrow import PyArrowFile
         >>> # input_file = PyArrowFile("s3://foo/bar.txt")
         >>> # Read the contents of the PyArrowFile instance
         >>> # Make sure that you have permissions to read/write
         >>> # file_content = input_file.open().read()
@@ -145,57 +168,57 @@
     def __init__(self, location: str, path: str, fs: FileSystem, buffer_size: int = ONE_MEGABYTE):
         self._filesystem = fs
         self._path = path
         self._buffer_size = buffer_size
         super().__init__(location=location)
 
     def _file_info(self) -> FileInfo:
-        """Retrieves a pyarrow.fs.FileInfo object for the location
+        """Retrieves a pyarrow.fs.FileInfo object for the location.
 
         Raises:
             PermissionError: If the file at self.location cannot be accessed due to a permission error such as
-                an AWS error code 15
+                an AWS error code 15.
         """
         try:
             file_info = self._filesystem.get_file_info(self._path)
         except OSError as e:
             if e.errno == 13 or "AWS Error [code 15]" in str(e):
                 raise PermissionError(f"Cannot get file info, access denied: {self.location}") from e
             raise  # pragma: no cover - If some other kind of OSError, raise the raw error
 
         if file_info.type == FileType.NotFound:
             raise FileNotFoundError(f"Cannot get file info, file not found: {self.location}")
         return file_info
 
     def __len__(self) -> int:
-        """Returns the total length of the file, in bytes"""
+        """Returns the total length of the file, in bytes."""
         file_info = self._file_info()
         return file_info.size
 
     def exists(self) -> bool:
-        """Checks whether the location exists"""
+        """Checks whether the location exists."""
         try:
             self._file_info()  # raises FileNotFoundError if it does not exist
             return True
         except FileNotFoundError:
             return False
 
     def open(self, seekable: bool = True) -> InputStream:
-        """Opens the location using a PyArrow FileSystem inferred from the location
+        """Opens the location using a PyArrow FileSystem inferred from the location.
 
         Args:
-            seekable: If the stream should support seek, or if it is consumed sequential
+            seekable: If the stream should support seek, or if it is consumed sequential.
 
         Returns:
-            pyarrow.lib.NativeFile: A NativeFile instance for the file located at `self.location`
+            pyarrow.lib.NativeFile: A NativeFile instance for the file located at `self.location`.
 
         Raises:
-            FileNotFoundError: If the file at self.location does not exist
+            FileNotFoundError: If the file at self.location does not exist.
             PermissionError: If the file at self.location cannot be accessed due to a permission error such as
-                an AWS error code 15
+                an AWS error code 15.
         """
         try:
             if seekable:
                 input_file = self._filesystem.open_input_file(self._path)
             else:
                 input_file = self._filesystem.open_input_stream(self._path, buffer_size=self._buffer_size)
         except FileNotFoundError:
@@ -207,24 +230,24 @@
                 raise FileNotFoundError(f"Cannot open file, does not exist: {self.location}") from e
             elif e.errno == 13 or "AWS Error [code 15]" in str(e):
                 raise PermissionError(f"Cannot open file, access denied: {self.location}") from e
             raise  # pragma: no cover - If some other kind of OSError, raise the raw error
         return input_file
 
     def create(self, overwrite: bool = False) -> OutputStream:
-        """Creates a writable pyarrow.lib.NativeFile for this PyArrowFile's location
+        """Creates a writable pyarrow.lib.NativeFile for this PyArrowFile's location.
 
         Args:
-            overwrite(bool): Whether to overwrite the file if it already exists
+            overwrite (bool): Whether to overwrite the file if it already exists.
 
         Returns:
-            pyarrow.lib.NativeFile: A NativeFile instance for the file located at self.location
+            pyarrow.lib.NativeFile: A NativeFile instance for the file located at self.location.
 
         Raises:
-            FileExistsError: If the file already exists at `self.location` and `overwrite` is False
+            FileExistsError: If the file already exists at `self.location` and `overwrite` is False.
 
         Note:
             This retrieves a pyarrow NativeFile by opening an output stream. If overwrite is set to False,
             a check is first performed to verify that the file does not exist. This is not thread-safe and
             a possibility does exist that the file can be created by a concurrent process after the existence
             check yet before the output stream is created. In such a case, the default pyarrow behavior will
             truncate the contents of the existing file when opening the output stream.
@@ -238,15 +261,15 @@
         except OSError as e:
             if e.errno == 13 or "AWS Error [code 15]" in str(e):
                 raise PermissionError(f"Cannot create file, access denied: {self.location}") from e
             raise  # pragma: no cover - If some other kind of OSError, raise the raw error
         return output_file
 
     def to_input_file(self) -> PyArrowFile:
-        """Returns a new PyArrowFile for the location of an existing PyArrowFile instance
+        """Returns a new PyArrowFile for the location of an existing PyArrowFile instance.
 
         This method is included to abide by the OutputFile abstract base class. Since this implementation uses a single
         PyArrowFile class (as opposed to separate InputFile and OutputFile implementations), this method effectively returns
         a copy of the same instance.
         """
         return self
 
@@ -254,70 +277,70 @@
 class PyArrowFileIO(FileIO):
     def __init__(self, properties: Properties = EMPTY_DICT):
         self.get_fs: Callable[[str], FileSystem] = lru_cache(self._get_fs)
         super().__init__(properties=properties)
 
     @staticmethod
     def parse_location(location: str) -> Tuple[str, str]:
-        """Returns the path without the scheme"""
+        """Returns the path without the scheme."""
         uri = urlparse(location)
         return uri.scheme or "file", os.path.abspath(location) if not uri.scheme else f"{uri.netloc}{uri.path}"
 
     def _get_fs(self, scheme: str) -> FileSystem:
         if scheme in {"s3", "s3a", "s3n"}:
             client_kwargs = {
-                "endpoint_override": self.properties.get("s3.endpoint"),
-                "access_key": self.properties.get("s3.access-key-id"),
-                "secret_key": self.properties.get("s3.secret-access-key"),
-                "session_token": self.properties.get("s3.session-token"),
+                "endpoint_override": self.properties.get(S3_ENDPOINT),
+                "access_key": self.properties.get(S3_ACCESS_KEY_ID),
+                "secret_key": self.properties.get(S3_SECRET_ACCESS_KEY),
+                "session_token": self.properties.get(S3_SESSION_TOKEN),
+                "region": self.properties.get(S3_REGION),
             }
             return S3FileSystem(**client_kwargs)
         elif scheme == "file":
             return LocalFileSystem()
         else:
             raise ValueError(f"Unrecognized filesystem type in URI: {scheme}")
 
     def new_input(self, location: str) -> PyArrowFile:
-        """Get a PyArrowFile instance to read bytes from the file at the given location
+        """Get a PyArrowFile instance to read bytes from the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
 
         Returns:
-            PyArrowFile: A PyArrowFile instance for the given location
+            PyArrowFile: A PyArrowFile instance for the given location.
         """
         scheme, path = self.parse_location(location)
         fs = self._get_fs(scheme)
         return PyArrowFile(fs=fs, location=location, path=path, buffer_size=int(self.properties.get(BUFFER_SIZE, ONE_MEGABYTE)))
 
     def new_output(self, location: str) -> PyArrowFile:
-        """Get a PyArrowFile instance to write bytes to the file at the given location
+        """Get a PyArrowFile instance to write bytes to the file at the given location.
 
         Args:
-            location(str): A URI or a path to a local file
+            location (str): A URI or a path to a local file.
 
         Returns:
-            PyArrowFile: A PyArrowFile instance for the given location
+            PyArrowFile: A PyArrowFile instance for the given location.
         """
         scheme, path = self.parse_location(location)
         fs = self._get_fs(scheme)
         return PyArrowFile(fs=fs, location=location, path=path, buffer_size=int(self.properties.get(BUFFER_SIZE, ONE_MEGABYTE)))
 
     def delete(self, location: Union[str, InputFile, OutputFile]) -> None:
-        """Delete the file at the given location
+        """Delete the file at the given location.
 
         Args:
-            location(str, InputFile, OutputFile): The URI to the file--if an InputFile instance or an
-            OutputFile instance is provided, the location attribute for that instance is used as the location
-            to delete
+            location (Union[str, InputFile, OutputFile]): The URI to the file--if an InputFile instance or an OutputFile instance is provided,
+                the location attribute for that instance is used as the location to delete.
 
         Raises:
-            FileNotFoundError: When the file at the provided location does not exist
+            FileNotFoundError: When the file at the provided location does not exist.
             PermissionError: If the file at the provided location cannot be accessed due to a permission error such as
-                an AWS error code 15
+                an AWS error code 15.
         """
         str_location = location.location if isinstance(location, (InputFile, OutputFile)) else location
         scheme, path = self.parse_location(str_location)
         fs = self._get_fs(scheme)
 
         try:
             fs.delete_file(path)
@@ -345,22 +368,25 @@
         return pa.struct(field_results)
 
     def field(self, field: NestedField, field_result: pa.DataType) -> pa.Field:
         return pa.field(
             name=field.name,
             type=field_result,
             nullable=field.optional,
-            metadata={"doc": field.doc, "id": str(field.field_id)} if field.doc else {},
+            metadata={DOC: field.doc, FIELD_ID: str(field.field_id)} if field.doc else {FIELD_ID: str(field.field_id)},
         )
 
-    def list(self, _: ListType, element_result: pa.DataType) -> pa.DataType:
-        return pa.list_(value_type=element_result)
-
-    def map(self, _: MapType, key_result: pa.DataType, value_result: pa.DataType) -> pa.DataType:
-        return pa.map_(key_type=key_result, item_type=value_result)
+    def list(self, list_type: ListType, element_result: pa.DataType) -> pa.DataType:
+        element_field = self.field(list_type.element_field, element_result)
+        return pa.list_(value_type=element_field)
+
+    def map(self, map_type: MapType, key_result: pa.DataType, value_result: pa.DataType) -> pa.DataType:
+        key_field = self.field(map_type.key_field, key_result)
+        value_field = self.field(map_type.value_field, value_result)
+        return pa.map_(key_type=key_field, item_type=value_field)
 
     def visit_fixed(self, fixed_type: FixedType) -> pa.DataType:
         return pa.binary(len(fixed_type))
 
     def visit_decimal(self, decimal_type: DecimalType) -> pa.DataType:
         return pa.decimal128(decimal_type.precision, decimal_type.scale)
 
@@ -388,15 +414,15 @@
     def visit_time(self, _: TimeType) -> pa.DataType:
         return pa.time64("us")
 
     def visit_timestamp(self, _: TimestampType) -> pa.DataType:
         return pa.timestamp(unit="us")
 
     def visit_timestampz(self, _: TimestamptzType) -> pa.DataType:
-        return pa.timestamp(unit="us", tz="+00:00")
+        return pa.timestamp(unit="us", tz="UTC")
 
     def visit_string(self, _: StringType) -> pa.DataType:
         return pa.string()
 
     def visit_uuid(self, _: UUIDType) -> pa.DataType:
         return pa.binary(16)
 
@@ -417,19 +443,19 @@
 
     def visit_not_in(self, term: BoundTerm[pc.Expression], literals: Set[Any]) -> pc.Expression:
         pyarrow_literals = pa.array(literals, type=schema_to_pyarrow(term.ref().field.field_type))
         return ~pc.field(term.ref().field.name).isin(pyarrow_literals)
 
     def visit_is_nan(self, term: BoundTerm[Any]) -> pc.Expression:
         ref = pc.field(term.ref().field.name)
-        return ref.is_null(nan_is_null=True) & ref.is_valid()
+        return pc.is_nan(ref)
 
     def visit_not_nan(self, term: BoundTerm[Any]) -> pc.Expression:
         ref = pc.field(term.ref().field.name)
-        return ~(ref.is_null(nan_is_null=True) & ref.is_valid())
+        return ~pc.is_nan(ref)
 
     def visit_is_null(self, term: BoundTerm[Any]) -> pc.Expression:
         return pc.field(term.ref().field.name).is_null(nan_is_null=False)
 
     def visit_not_null(self, term: BoundTerm[Any]) -> pc.Expression:
         return pc.field(term.ref().field.name).is_valid()
 
@@ -447,14 +473,20 @@
 
     def visit_less_than(self, term: BoundTerm[Any], literal: Literal[Any]) -> pc.Expression:
         return pc.field(term.ref().field.name) < _convert_scalar(literal.value, term.ref().field.field_type)
 
     def visit_less_than_or_equal(self, term: BoundTerm[Any], literal: Literal[Any]) -> pc.Expression:
         return pc.field(term.ref().field.name) <= _convert_scalar(literal.value, term.ref().field.field_type)
 
+    def visit_starts_with(self, term: BoundTerm[Any], literal: Literal[Any]) -> pc.Expression:
+        return pc.starts_with(pc.field(term.ref().field.name), literal.value)
+
+    def visit_not_starts_with(self, term: BoundTerm[Any], literal: Literal[Any]) -> pc.Expression:
+        return ~pc.starts_with(pc.field(term.ref().field.name), literal.value)
+
     def visit_true(self) -> pc.Expression:
         return pc.scalar(True)
 
     def visit_false(self) -> pc.Expression:
         return pc.scalar(False)
 
     def visit_not(self, child_result: pc.Expression) -> pc.Expression:
@@ -467,102 +499,410 @@
         return left_result | right_result
 
 
 def expression_to_pyarrow(expr: BooleanExpression) -> pc.Expression:
     return boolean_expression_visit(expr, _ConvertToArrowExpression())
 
 
-def _file_to_table(
+@lru_cache
+def _get_file_format(file_format: FileFormat, **kwargs: Dict[str, Any]) -> ds.FileFormat:
+    if file_format == FileFormat.PARQUET:
+        return ds.ParquetFileFormat(**kwargs)
+    else:
+        raise ValueError(f"Unsupported file format: {file_format}")
+
+
+def _construct_fragment(fs: FileSystem, data_file: DataFile, file_format_kwargs: Dict[str, Any] = EMPTY_DICT) -> ds.Fragment:
+    _, path = PyArrowFileIO.parse_location(data_file.file_path)
+    return _get_file_format(data_file.file_format, **file_format_kwargs).make_fragment(path, fs)
+
+
+def _read_deletes(fs: FileSystem, data_file: DataFile) -> Dict[str, pa.ChunkedArray]:
+    delete_fragment = _construct_fragment(
+        fs, data_file, file_format_kwargs={"dictionary_columns": ("file_path",), "pre_buffer": True, "buffer_size": ONE_MEGABYTE}
+    )
+    table = ds.Scanner.from_fragment(fragment=delete_fragment).to_table()
+    table = table.unify_dictionaries()
+    return {
+        file.as_py(): table.filter(pc.field("file_path") == file).column("pos")
+        for file in table.column("file_path").chunks[0].dictionary
+    }
+
+
+def _combine_positional_deletes(positional_deletes: List[pa.ChunkedArray], rows: int) -> pa.Array:
+    if len(positional_deletes) == 1:
+        all_chunks = positional_deletes[0]
+    else:
+        all_chunks = pa.chunked_array(chain(*[arr.chunks for arr in positional_deletes]))
+    return np.setdiff1d(np.arange(rows), all_chunks, assume_unique=False)
+
+
+def pyarrow_to_schema(schema: pa.Schema) -> Schema:
+    visitor = _ConvertToIceberg()
+    return visit_pyarrow(schema, visitor)
+
+
+@singledispatch
+def visit_pyarrow(obj: Union[pa.DataType, pa.Schema], visitor: PyArrowSchemaVisitor[T]) -> T:
+    """A generic function for applying a pyarrow schema visitor to any point within a schema.
+
+    The function traverses the schema in post-order fashion.
+
+    Args:
+        obj (Union[pa.DataType, pa.Schema]): An instance of a Schema or an IcebergType.
+        visitor (PyArrowSchemaVisitor[T]): An instance of an implementation of the generic PyarrowSchemaVisitor base class.
+
+    Raises:
+        NotImplementedError: If attempting to visit an unrecognized object type.
+    """
+    raise NotImplementedError("Cannot visit non-type: %s" % obj)
+
+
+@visit_pyarrow.register(pa.Schema)
+def _(obj: pa.Schema, visitor: PyArrowSchemaVisitor[T]) -> Optional[T]:
+    struct_results: List[Optional[T]] = []
+    for field in obj:
+        visitor.before_field(field)
+        struct_result = visit_pyarrow(field.type, visitor)
+        visitor.after_field(field)
+        struct_results.append(struct_result)
+
+    return visitor.schema(obj, struct_results)
+
+
+@visit_pyarrow.register(pa.StructType)
+def _(obj: pa.StructType, visitor: PyArrowSchemaVisitor[T]) -> Optional[T]:
+    struct_results: List[Optional[T]] = []
+    for field in obj:
+        visitor.before_field(field)
+        struct_result = visit_pyarrow(field.type, visitor)
+        visitor.after_field(field)
+        struct_results.append(struct_result)
+
+    return visitor.struct(obj, struct_results)
+
+
+@visit_pyarrow.register(pa.ListType)
+def _(obj: pa.ListType, visitor: PyArrowSchemaVisitor[T]) -> Optional[T]:
+    visitor.before_field(obj.value_field)
+    list_result = visit_pyarrow(obj.value_field.type, visitor)
+    visitor.after_field(obj.value_field)
+    return visitor.list(obj, list_result)
+
+
+@visit_pyarrow.register(pa.MapType)
+def _(obj: pa.MapType, visitor: PyArrowSchemaVisitor[T]) -> Optional[T]:
+    visitor.before_field(obj.key_field)
+    key_result = visit_pyarrow(obj.key_field.type, visitor)
+    visitor.after_field(obj.key_field)
+    visitor.before_field(obj.item_field)
+    value_result = visit_pyarrow(obj.item_field.type, visitor)
+    visitor.after_field(obj.item_field)
+    return visitor.map(obj, key_result, value_result)
+
+
+@visit_pyarrow.register(pa.DataType)
+def _(obj: pa.DataType, visitor: PyArrowSchemaVisitor[T]) -> Optional[T]:
+    if pa.types.is_nested(obj):
+        raise TypeError(f"Expected primitive type, got: {type(obj)}")
+    return visitor.primitive(obj)
+
+
+class PyArrowSchemaVisitor(Generic[T], ABC):
+    def before_field(self, field: pa.Field) -> None:
+        """Override this method to perform an action immediately before visiting a field."""
+
+    def after_field(self, field: pa.Field) -> None:
+        """Override this method to perform an action immediately after visiting a field."""
+
+    @abstractmethod
+    def schema(self, schema: pa.Schema, field_results: List[Optional[T]]) -> Optional[T]:
+        """Visit a schema."""
+
+    @abstractmethod
+    def struct(self, struct: pa.StructType, field_results: List[Optional[T]]) -> Optional[T]:
+        """Visit a struct."""
+
+    @abstractmethod
+    def list(self, list_type: pa.ListType, element_result: Optional[T]) -> Optional[T]:
+        """Visit a list."""
+
+    @abstractmethod
+    def map(self, map_type: pa.MapType, key_result: Optional[T], value_result: Optional[T]) -> Optional[T]:
+        """Visit a map."""
+
+    @abstractmethod
+    def primitive(self, primitive: pa.DataType) -> Optional[T]:
+        """Visit a primitive type."""
+
+
+def _get_field_id(field: pa.Field) -> Optional[int]:
+    for pyarrow_field_id_key in PYARROW_FIELD_ID_KEYS:
+        if field_id_str := field.metadata.get(pyarrow_field_id_key):
+            return int(field_id_str.decode())
+    return None
+
+
+def _get_field_doc(field: pa.Field) -> Optional[str]:
+    for pyarrow_doc_key in PYARROW_FIELD_DOC_KEYS:
+        if doc_str := field.metadata.get(pyarrow_doc_key):
+            return doc_str.decode()
+    return None
+
+
+class _ConvertToIceberg(PyArrowSchemaVisitor[Union[IcebergType, Schema]]):
+    def _convert_fields(self, arrow_fields: Iterable[pa.Field], field_results: List[Optional[IcebergType]]) -> List[NestedField]:
+        fields = []
+        for i, field in enumerate(arrow_fields):
+            field_id = _get_field_id(field)
+            field_doc = _get_field_doc(field)
+            field_type = field_results[i]
+            if field_type is not None and field_id is not None:
+                fields.append(NestedField(field_id, field.name, field_type, required=not field.nullable, doc=field_doc))
+        return fields
+
+    def schema(self, schema: pa.Schema, field_results: List[Optional[IcebergType]]) -> Schema:
+        return Schema(*self._convert_fields(schema, field_results))
+
+    def struct(self, struct: pa.StructType, field_results: List[Optional[IcebergType]]) -> IcebergType:
+        return StructType(*self._convert_fields(struct, field_results))
+
+    def list(self, list_type: pa.ListType, element_result: Optional[IcebergType]) -> Optional[IcebergType]:
+        element_field = list_type.value_field
+        element_id = _get_field_id(element_field)
+        if element_result is not None and element_id is not None:
+            return ListType(element_id, element_result, element_required=not element_field.nullable)
+        return None
+
+    def map(
+        self, map_type: pa.MapType, key_result: Optional[IcebergType], value_result: Optional[IcebergType]
+    ) -> Optional[IcebergType]:
+        key_field = map_type.key_field
+        key_id = _get_field_id(key_field)
+        value_field = map_type.item_field
+        value_id = _get_field_id(value_field)
+        if key_result is not None and value_result is not None and key_id is not None and value_id is not None:
+            return MapType(key_id, key_result, value_id, value_result, value_required=not value_field.nullable)
+        return None
+
+    def primitive(self, primitive: pa.DataType) -> IcebergType:
+        if pa.types.is_boolean(primitive):
+            return BooleanType()
+        elif pa.types.is_int32(primitive):
+            return IntegerType()
+        elif pa.types.is_int64(primitive):
+            return LongType()
+        elif pa.types.is_float32(primitive):
+            return FloatType()
+        elif pa.types.is_float64(primitive):
+            return DoubleType()
+        elif isinstance(primitive, pa.Decimal128Type):
+            primitive = cast(pa.Decimal128Type, primitive)
+            return DecimalType(primitive.precision, primitive.scale)
+        elif pa.types.is_string(primitive):
+            return StringType()
+        elif pa.types.is_date32(primitive):
+            return DateType()
+        elif isinstance(primitive, pa.Time64Type) and primitive.unit == "us":
+            return TimeType()
+        elif pa.types.is_timestamp(primitive):
+            primitive = cast(pa.TimestampType, primitive)
+            if primitive.unit == "us":
+                if primitive.tz == "UTC" or primitive.tz == "+00:00":
+                    return TimestamptzType()
+                elif primitive.tz is None:
+                    return TimestampType()
+        elif pa.types.is_binary(primitive):
+            return BinaryType()
+        elif pa.types.is_fixed_size_binary(primitive):
+            primitive = cast(pa.FixedSizeBinaryType, primitive)
+            return FixedType(primitive.byte_width)
+
+        raise TypeError(f"Unsupported type: {primitive}")
+
+
+def _task_to_table(
     fs: FileSystem,
     task: FileScanTask,
     bound_row_filter: BooleanExpression,
     projected_schema: Schema,
     projected_field_ids: Set[int],
+    positional_deletes: Optional[List[ChunkedArray]],
     case_sensitive: bool,
-) -> pa.Table:
-    _, path = PyArrowFileIO.parse_location(task.file.file_path)
+    rows_counter: Synchronized[int],
+    limit: Optional[int] = None,
+) -> Optional[pa.Table]:
+    if limit and rows_counter.value >= limit:
+        return None
 
-    # Get the schema
-    with fs.open_input_file(path) as fout:
-        parquet_schema = pq.read_schema(fout)
+    _, path = PyArrowFileIO.parse_location(task.file.file_path)
+    arrow_format = ds.ParquetFileFormat(pre_buffer=True, buffer_size=(ONE_MEGABYTE * 8))
+    with fs.open_input_file(path) as fin:
+        fragment = arrow_format.make_fragment(fin)
+        physical_schema = fragment.physical_schema
         schema_raw = None
-        if metadata := parquet_schema.metadata:
+        if metadata := physical_schema.metadata:
             schema_raw = metadata.get(ICEBERG_SCHEMA)
-        if schema_raw is None:
-            raise ValueError(
-                "Iceberg schema is not embedded into the Parquet file, see https://github.com/apache/iceberg/issues/6505"
-            )
-        file_schema = Schema.parse_raw(schema_raw)
+        # TODO: if field_ids are not present, Name Mapping should be implemented to look them up in the table schema,
+        #  see https://github.com/apache/iceberg/issues/7451
+        file_schema = Schema.parse_raw(schema_raw) if schema_raw is not None else pyarrow_to_schema(physical_schema)
+
+        pyarrow_filter = None
+        if bound_row_filter is not AlwaysTrue():
+            translated_row_filter = translate_column_names(bound_row_filter, file_schema, case_sensitive=case_sensitive)
+            bound_file_filter = bind(file_schema, translated_row_filter, case_sensitive=case_sensitive)
+            pyarrow_filter = expression_to_pyarrow(bound_file_filter)
+
+        file_project_schema = prune_columns(file_schema, projected_field_ids, select_full_types=False)
+
+        if file_schema is None:
+            raise ValueError(f"Missing Iceberg schema in Metadata for file: {path}")
+
+        fragment_scanner = ds.Scanner.from_fragment(
+            fragment=fragment,
+            schema=physical_schema,
+            # This will push down the query to Arrow.
+            # But in case there are positional deletes, we have to apply them first
+            filter=pyarrow_filter if not positional_deletes else None,
+            columns=[col.name for col in file_project_schema.columns],
+        )
+
+        if positional_deletes:
+            # Create the mask of indices that we're interested in
+            indices = _combine_positional_deletes(positional_deletes, fragment.count_rows())
+
+            if limit:
+                if pyarrow_filter is not None:
+                    # In case of the filter, we don't exactly know how many rows
+                    # we need to fetch upfront, can be optimized in the future:
+                    # https://github.com/apache/arrow/issues/35301
+                    arrow_table = fragment_scanner.take(indices)
+                    arrow_table = arrow_table.filter(pyarrow_filter)
+                    arrow_table = arrow_table.slice(0, limit)
+                else:
+                    arrow_table = fragment_scanner.take(indices[0:limit])
+            else:
+                arrow_table = fragment_scanner.take(indices)
+                # Apply the user filter
+                if pyarrow_filter is not None:
+                    arrow_table = arrow_table.filter(pyarrow_filter)
+        else:
+            # If there are no deletes, we can just take the head
+            # and the user-filter is already applied
+            if limit:
+                arrow_table = fragment_scanner.head(limit)
+            else:
+                arrow_table = fragment_scanner.to_table()
+
+        if limit:
+            with rows_counter.get_lock():
+                if rows_counter.value >= limit:
+                    return None
+                rows_counter.value += len(arrow_table)
+
+        # If there is no data, we don't have to go through the schema
+        if len(arrow_table) > 0:
+            return to_requested_schema(projected_schema, file_project_schema, arrow_table)
+        else:
+            return None
 
-    pyarrow_filter = None
-    if bound_row_filter is not AlwaysTrue():
-        translated_row_filter = translate_column_names(bound_row_filter, file_schema, case_sensitive=case_sensitive)
-        bound_file_filter = bind(file_schema, translated_row_filter, case_sensitive=case_sensitive)
-        pyarrow_filter = expression_to_pyarrow(bound_file_filter)
-
-    file_project_schema = prune_columns(file_schema, projected_field_ids, select_full_types=False)
-
-    if file_schema is None:
-        raise ValueError(f"Missing Iceberg schema in Metadata for file: {path}")
-
-    # Prune the stuff that we don't need anyway
-    file_project_schema_arrow = schema_to_pyarrow(file_project_schema)
-
-    read_options = {
-        "pre_buffer": True,
-        "use_buffered_stream": True,
-        "buffer_size": 8388608,
-    }
 
-    arrow_table = ds.dataset(
-        source=[path], schema=file_project_schema_arrow, format=ds.ParquetFileFormat(**read_options), filesystem=fs
-    ).to_table(filter=pyarrow_filter)
+def _read_all_delete_files(fs: FileSystem, pool: ThreadPool, tasks: Iterable[FileScanTask]) -> Dict[str, List[ChunkedArray]]:
+    deletes_per_file: Dict[str, List[ChunkedArray]] = {}
+    unique_deletes = set(chain.from_iterable([task.delete_files for task in tasks]))
+    if len(unique_deletes) > 0:
+        deletes_per_files: List[Dict[str, ChunkedArray]] = pool.starmap(
+            func=_read_deletes, iterable=[(fs, delete) for delete in unique_deletes]
+        )
+        for delete in deletes_per_files:
+            for file, arr in delete.items():
+                if file in deletes_per_file:
+                    deletes_per_file[file].append(arr)
+                else:
+                    deletes_per_file[file] = [arr]
 
-    return to_requested_schema(projected_schema, file_project_schema, arrow_table)
+    return deletes_per_file
 
 
 def project_table(
-    tasks: Iterable[FileScanTask], table: Table, row_filter: BooleanExpression, projected_schema: Schema, case_sensitive: bool
+    tasks: Iterable[FileScanTask],
+    table: Table,
+    row_filter: BooleanExpression,
+    projected_schema: Schema,
+    case_sensitive: bool = True,
+    limit: Optional[int] = None,
 ) -> pa.Table:
-    """Resolves the right columns based on the identifier
+    """Resolves the right columns based on the identifier.
 
     Args:
-        tasks(Iterable[FileScanTask]): A URI or a path to a local file
-        table(Table): The table that's being queried
-        row_filter(BooleanExpression): The expression for filtering rows
-        projected_schema(Schema): The output schema
-        case_sensitive(bool): Case sensitivity when looking up column names
+        tasks (Iterable[FileScanTask]): A URI or a path to a local file.
+        table (Table): The table that's being queried.
+        row_filter (BooleanExpression): The expression for filtering rows.
+        projected_schema (Schema): The output schema.
+        case_sensitive (bool): Case sensitivity when looking up column names.
+        limit (Optional[int]): Limit the number of records.
 
     Raises:
-        ResolveError: When an incompatible query is done
+        ResolveError: When an incompatible query is done.
     """
-
+    scheme, _ = PyArrowFileIO.parse_location(table.location())
     if isinstance(table.io, PyArrowFileIO):
-        scheme, _ = PyArrowFileIO.parse_location(table.location())
         fs = table.io.get_fs(scheme)
     else:
-        raise ValueError(f"Expected PyArrowFileIO, got: {table.io}")
+        try:
+            from pyiceberg.io.fsspec import FsspecFileIO
+
+            if isinstance(table.io, FsspecFileIO):
+                fs = PyFileSystem(FSSpecHandler(table.io.get_fs(scheme)))
+            else:
+                raise ValueError(f"Expected PyArrowFileIO or FsspecFileIO, got: {table.io}")
+        except ModuleNotFoundError as e:
+            # When FsSpec is not installed
+            raise ValueError(f"Expected PyArrowFileIO or FsspecFileIO, got: {table.io}") from e
 
     bound_row_filter = bind(table.schema(), row_filter, case_sensitive=case_sensitive)
 
     projected_field_ids = {
         id for id in projected_schema.field_ids if not isinstance(projected_schema.find_type(id), (MapType, ListType))
     }.union(extract_field_ids(bound_row_filter))
 
+    rows_counter = multiprocessing.Value("i", 0)
+
     with ThreadPool() as pool:
-        tables = pool.starmap(
-            func=_file_to_table,
-            iterable=[(fs, task, bound_row_filter, projected_schema, projected_field_ids, case_sensitive) for task in tasks],
-            chunksize=None,  # we could use this to control how to materialize the generator of tasks (we should also make the expression above lazy)
-        )
+        deletes_per_file = _read_all_delete_files(fs, pool, tasks)
+        tables = [
+            table
+            for table in pool.starmap(
+                func=_task_to_table,
+                iterable=[
+                    (
+                        fs,
+                        task,
+                        bound_row_filter,
+                        projected_schema,
+                        projected_field_ids,
+                        deletes_per_file.get(task.file.file_path),
+                        case_sensitive,
+                        rows_counter,
+                        limit,
+                    )
+                    for task in tasks
+                ],
+            )
+            if table is not None
+        ]
 
     if len(tables) > 1:
-        return pa.concat_tables(tables)
+        final_table = pa.concat_tables(tables)
+    elif len(tables) == 1:
+        final_table = tables[0]
     else:
-        return tables[0]
+        final_table = pa.Table.from_batches([], schema=schema_to_pyarrow(projected_schema))
+
+    return final_table.slice(0, limit)
 
 
 def to_requested_schema(requested_schema: Schema, file_schema: Schema, table: pa.Table) -> pa.Table:
     struct_array = visit_with_partner(requested_schema, table, ArrowProjectionVisitor(file_schema), ArrowAccessor(file_schema))
 
     arrays = []
     fields = []
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/partitioning.py` & `pyiceberg-0.4.0rc1/pyiceberg/partitioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 from pyiceberg.types import NestedField, StructType
 
 INITIAL_PARTITION_SPEC_ID = 0
 _PARTITION_DATA_ID_START: int = 1000
 
 
 class PartitionField(IcebergBaseModel):
-    """
-    PartitionField is a single element with name and unique id,
-    It represents how one partition value is derived from the source column via transformation
+    """PartitionField represents how one partition value is derived from the source column via transformation.
 
     Attributes:
-        source_id(int): The source column id of table's schema
-        field_id(int): The partition field id across all the table partition specs
-        transform(Transform): The transform used to produce partition values from source column
-        name(str): The name of this partition field
+        source_id(int): The source column id of table's schema.
+        field_id(int): The partition field id across all the table partition specs.
+        transform(Transform): The transform used to produce partition values from source column.
+        name(str): The name of this partition field.
     """
 
     source_id: int = Field(alias="source-id")
     field_id: int = Field(alias="field-id")
     transform: Transform[Any, Any] = Field()
     name: str = Field()
 
@@ -66,24 +64,25 @@
         if transform is not None:
             data["transform"] = transform
         if name is not None:
             data["name"] = name
         super().__init__(**data)
 
     def __str__(self) -> str:
+        """Returns the string representation of the PartitionField class."""
         return f"{self.field_id}: {self.name}: {self.transform}({self.source_id})"
 
 
 class PartitionSpec(IcebergBaseModel):
     """
-    PartitionSpec captures the transformation from table data to partition values
+    PartitionSpec captures the transformation from table data to partition values.
 
     Attributes:
-        spec_id(int): any change to PartitionSpec will produce a new specId
-        fields(Tuple[PartitionField): list of partition fields to produce partition values
+        spec_id(int): any change to PartitionSpec will produce a new specId.
+        fields(Tuple[PartitionField): list of partition fields to produce partition values.
     """
 
     spec_id: int = Field(alias="spec-id", default=INITIAL_PARTITION_SPEC_ID)
     fields: Tuple[PartitionField, ...] = Field(alias="fields", default_factory=tuple)
 
     def __init__(
         self,
@@ -92,37 +91,38 @@
     ):
         if fields:
             data["fields"] = tuple(fields)
         super().__init__(**data)
 
     def __eq__(self, other: Any) -> bool:
         """
-        Produce a boolean to return True if two objects are considered equal
+        Produce a boolean to return True if two objects are considered equal.
 
         Note:
-            Equality of PartitionSpec is determined by spec_id and partition fields only
+            Equality of PartitionSpec is determined by spec_id and partition fields only.
         """
         if not isinstance(other, PartitionSpec):
             return False
         return self.spec_id == other.spec_id and self.fields == other.fields
 
     def __str__(self) -> str:
         """
-        Produce a human-readable string representation of PartitionSpec
+        Produce a human-readable string representation of PartitionSpec.
 
         Note:
-            Only include list of partition fields in the PartitionSpec's string representation
+            Only include list of partition fields in the PartitionSpec's string representation.
         """
         result_str = "["
         if self.fields:
             result_str += "\n  " + "\n  ".join([str(field) for field in self.fields]) + "\n"
         result_str += "]"
         return result_str
 
     def __repr__(self) -> str:
+        """Returns the string representation of the PartitionSpec class."""
         fields = f"{', '.join(repr(column) for column in self.fields)}, " if self.fields else ""
         return f"PartitionSpec({fields}spec_id={self.spec_id})"
 
     def is_unpartitioned(self) -> bool:
         return not self.fields
 
     @property
@@ -140,43 +140,41 @@
             source_id_to_fields_map[partition_field.source_id] = existing
         return source_id_to_fields_map
 
     def fields_by_source_id(self, field_id: int) -> List[PartitionField]:
         return self.source_id_to_fields_map.get(field_id, [])
 
     def compatible_with(self, other: "PartitionSpec") -> bool:
-        """
-        Produce a boolean to return True if two PartitionSpec are considered compatible
-        """
+        """Produce a boolean to return True if two PartitionSpec are considered compatible."""
         if self == other:
             return True
         if len(self.fields) != len(other.fields):
             return False
         return all(
             this_field.source_id == that_field.source_id
             and this_field.transform == that_field.transform
             and this_field.name == that_field.name
             for this_field, that_field in zip(self.fields, other.fields)
         )
 
     def partition_type(self, schema: Schema) -> StructType:
-        """Produces a struct of the PartitionSpec
+        """Produces a struct of the PartitionSpec.
 
         The partition fields should be optional:
 
         - All partition transforms are required to produce null if the input value is null, so it can
-          happen when the source column is optional
+          happen when the source column is optional.
         - Partition fields may be added later, in which case not all files would have the result field,
           and it may be null.
 
         There is a case where we can guarantee that a partition field in the first and only partition spec
         that uses a required source column will never be null, but it doesn't seem worth tracking this case.
 
-        :param schema: The schema to bind to
-        :return: A StructType that represents the PartitionSpec, with a NestedField for each PartitionField
+        :param schema: The schema to bind to.
+        :return: A StructType that represents the PartitionSpec, with a NestedField for each PartitionField.
         """
         nested_fields = []
         for field in self.fields:
             source_type = schema.find_type(field.source_id)
             result_type = field.transform.result_type(source_type)
             nested_fields.append(NestedField(field.field_id, field.name, result_type, required=False))
         return StructType(*nested_fields)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/schema.py` & `pyiceberg-0.4.0rc1/pyiceberg/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 T = TypeVar("T")
 P = TypeVar("P")
 
 INITIAL_SCHEMA_ID = 0
 
 
 class Schema(IcebergBaseModel):
-    """A table Schema
+    """A table Schema.
 
     Example:
         >>> from pyiceberg import schema
         >>> from pyiceberg import types
     """
 
     type: Literal["struct"] = "struct"
@@ -84,90 +84,94 @@
     def __init__(self, *fields: NestedField, **data: Any):
         if fields:
             data["fields"] = fields
         super().__init__(**data)
         self._name_to_id = index_by_name(self)
 
     def __str__(self) -> str:
+        """Returns the string representation of the Schema class."""
         return "table {\n" + "\n".join(["  " + str(field) for field in self.columns]) + "\n}"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Schema class."""
         return f"Schema({', '.join(repr(column) for column in self.columns)}, schema_id={self.schema_id}, identifier_field_ids={self.identifier_field_ids})"
 
     def __len__(self) -> int:
+        """Returns the length of an instance of the Literal class."""
         return len(self.fields)
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Schema class."""
         if not other:
             return False
 
         if not isinstance(other, Schema):
             return False
 
         if len(self.columns) != len(other.columns):
             return False
 
         identifier_field_ids_is_equal = self.identifier_field_ids == other.identifier_field_ids
-        schema_is_equal = all([lhs == rhs for lhs, rhs in zip(self.columns, other.columns)])
+        schema_is_equal = all(lhs == rhs for lhs, rhs in zip(self.columns, other.columns))
 
         return identifier_field_ids_is_equal and schema_is_equal
 
     @property
     def columns(self) -> Tuple[NestedField, ...]:
-        """A tuple of the top-level fields"""
+        """A tuple of the top-level fields."""
         return self.fields
 
     @cached_property
     def _lazy_id_to_field(self) -> Dict[int, NestedField]:
-        """Returns an index of field ID to NestedField instance
+        """Returns an index of field ID to NestedField instance.
 
         This is calculated once when called for the first time. Subsequent calls to this method will use a cached index.
         """
         return index_by_id(self)
 
     @cached_property
     def _lazy_name_to_id_lower(self) -> Dict[str, int]:
-        """Returns an index of lower-case field names to field IDs
+        """Returns an index of lower-case field names to field IDs.
 
         This is calculated once when called for the first time. Subsequent calls to this method will use a cached index.
         """
         return {name.lower(): field_id for name, field_id in self._name_to_id.items()}
 
     @cached_property
     def _lazy_id_to_name(self) -> Dict[int, str]:
-        """Returns an index of field ID to full name
+        """Returns an index of field ID to full name.
 
         This is calculated once when called for the first time. Subsequent calls to this method will use a cached index.
         """
         return index_name_by_id(self)
 
     @cached_property
     def _lazy_id_to_accessor(self) -> Dict[int, "Accessor"]:
-        """Returns an index of field ID to accessor
+        """Returns an index of field ID to accessor.
 
         This is calculated once when called for the first time. Subsequent calls to this method will use a cached index.
         """
         return build_position_accessors(self)
 
     def as_struct(self) -> StructType:
-        """Returns the schema as a struct"""
+        """Returns the schema as a struct."""
         return StructType(*self.fields)
 
     def find_field(self, name_or_id: Union[str, int], case_sensitive: bool = True) -> NestedField:
-        """Find a field using a field name or field ID
+        """Find a field using a field name or field ID.
 
         Args:
-            name_or_id (str | int): Either a field name or a field ID
+            name_or_id (Union[str, int]): Either a field name or a field ID.
             case_sensitive (bool, optional): Whether to perform a case-sensitive lookup using a field name. Defaults to True.
 
         Raises:
-            ValueError: When the value cannot be found
+            ValueError: When the value cannot be found.
 
         Returns:
-            NestedField: The matched NestedField
+            NestedField: The matched NestedField.
         """
         if isinstance(name_or_id, int):
             if name_or_id not in self._lazy_id_to_field:
                 raise ValueError(f"Could not find field with id: {name_or_id}")
             return self._lazy_id_to_field[name_or_id]
 
         if case_sensitive:
@@ -177,232 +181,242 @@
 
         if field_id is None:
             raise ValueError(f"Could not find field with name {name_or_id}, case_sensitive={case_sensitive}")
 
         return self._lazy_id_to_field[field_id]
 
     def find_type(self, name_or_id: Union[str, int], case_sensitive: bool = True) -> IcebergType:
-        """Find a field type using a field name or field ID
+        """Find a field type using a field name or field ID.
 
         Args:
-            name_or_id (str | int): Either a field name or a field ID
+            name_or_id (Union[str, int]): Either a field name or a field ID.
             case_sensitive (bool, optional): Whether to perform a case-sensitive lookup using a field name. Defaults to True.
 
         Returns:
-            NestedField: The type of the matched NestedField
+            NestedField: The type of the matched NestedField.
         """
         field = self.find_field(name_or_id=name_or_id, case_sensitive=case_sensitive)
         if not field:
             raise ValueError(f"Could not find field with name or id {name_or_id}, case_sensitive={case_sensitive}")
         return field.field_type
 
     @property
     def highest_field_id(self) -> int:
         return visit(self.as_struct(), _FindLastFieldId())
 
     def find_column_name(self, column_id: int) -> Optional[str]:
-        """Find a column name given a column ID
+        """Find a column name given a column ID.
 
         Args:
-            column_id (int): The ID of the column
+            column_id (int): The ID of the column.
 
         Returns:
-            str: The column name (or None if the column ID cannot be found)
+            str: The column name (or None if the column ID cannot be found).
         """
         return self._lazy_id_to_name.get(column_id)
 
+    @property
+    def column_names(self) -> List[str]:
+        """
+        Returns a list of all the column names, including nested fields.
+
+        Excludes short names.
+
+        Returns:
+            List[str]: The column names.
+        """
+        return list(self._lazy_id_to_name.values())
+
     def accessor_for_field(self, field_id: int) -> "Accessor":
-        """Find a schema position accessor given a field ID
+        """Find a schema position accessor given a field ID.
 
         Args:
-            field_id (int): The ID of the field
+            field_id (int): The ID of the field.
 
         Raises:
-            ValueError: When the value cannot be found
+            ValueError: When the value cannot be found.
 
         Returns:
-            Accessor: An accessor for the given field ID
+            Accessor: An accessor for the given field ID.
         """
-
         if field_id not in self._lazy_id_to_accessor:
             raise ValueError(f"Could not find accessor for field with id: {field_id}")
 
         return self._lazy_id_to_accessor[field_id]
 
     def select(self, *names: str, case_sensitive: bool = True) -> "Schema":
-        """Return a new schema instance pruned to a subset of columns
+        """Return a new schema instance pruned to a subset of columns.
 
         Args:
-            names (List[str]): A list of column names
+            names (List[str]): A list of column names.
             case_sensitive (bool, optional): Whether to perform a case-sensitive lookup for each column name. Defaults to True.
 
         Returns:
-            Schema: A new schema with pruned columns
+            Schema: A new schema with pruned columns.
 
         Raises:
-            ValueError: If a column is selected that doesn't exist
+            ValueError: If a column is selected that doesn't exist.
         """
-
         try:
             if case_sensitive:
                 ids = {self._name_to_id[name] for name in names}
             else:
                 ids = {self._lazy_name_to_id_lower[name.lower()] for name in names}
         except KeyError as e:
             raise ValueError(f"Could not find column: {e}") from e
 
         return prune_columns(self, ids)
 
     @property
     def field_ids(self) -> Set[int]:
-        """Returns the IDs of the current schema"""
+        """Returns the IDs of the current schema."""
         return set(self._name_to_id.values())
 
 
 class SchemaVisitor(Generic[T], ABC):
     def before_field(self, field: NestedField) -> None:
-        """Override this method to perform an action immediately before visiting a field"""
+        """Override this method to perform an action immediately before visiting a field."""
 
     def after_field(self, field: NestedField) -> None:
-        """Override this method to perform an action immediately after visiting a field"""
+        """Override this method to perform an action immediately after visiting a field."""
 
     def before_list_element(self, element: NestedField) -> None:
-        """Override this method to perform an action immediately before visiting an element within a ListType"""
+        """Override this method to perform an action immediately before visiting an element within a ListType."""
         self.before_field(element)
 
     def after_list_element(self, element: NestedField) -> None:
-        """Override this method to perform an action immediately after visiting an element within a ListType"""
+        """Override this method to perform an action immediately after visiting an element within a ListType."""
         self.after_field(element)
 
     def before_map_key(self, key: NestedField) -> None:
-        """Override this method to perform an action immediately before visiting a key within a MapType"""
+        """Override this method to perform an action immediately before visiting a key within a MapType."""
         self.before_field(key)
 
     def after_map_key(self, key: NestedField) -> None:
-        """Override this method to perform an action immediately after visiting a key within a MapType"""
+        """Override this method to perform an action immediately after visiting a key within a MapType."""
         self.after_field(key)
 
     def before_map_value(self, value: NestedField) -> None:
-        """Override this method to perform an action immediately before visiting a value within a MapType"""
+        """Override this method to perform an action immediately before visiting a value within a MapType."""
         self.before_field(value)
 
     def after_map_value(self, value: NestedField) -> None:
-        """Override this method to perform an action immediately after visiting a value within a MapType"""
+        """Override this method to perform an action immediately after visiting a value within a MapType."""
         self.after_field(value)
 
     @abstractmethod
     def schema(self, schema: Schema, struct_result: T) -> T:
-        """Visit a Schema"""
+        """Visit a Schema."""
 
     @abstractmethod
     def struct(self, struct: StructType, field_results: List[T]) -> T:
-        """Visit a StructType"""
+        """Visit a StructType."""
 
     @abstractmethod
     def field(self, field: NestedField, field_result: T) -> T:
-        """Visit a NestedField"""
+        """Visit a NestedField."""
 
     @abstractmethod
     def list(self, list_type: ListType, element_result: T) -> T:
-        """Visit a ListType"""
+        """Visit a ListType."""
 
     @abstractmethod
     def map(self, map_type: MapType, key_result: T, value_result: T) -> T:
-        """Visit a MapType"""
+        """Visit a MapType."""
 
     @abstractmethod
     def primitive(self, primitive: PrimitiveType) -> T:
-        """Visit a PrimitiveType"""
+        """Visit a PrimitiveType."""
 
 
 class PreOrderSchemaVisitor(Generic[T], ABC):
     @abstractmethod
     def schema(self, schema: Schema, struct_result: Callable[[], T]) -> T:
-        """Visit a Schema"""
+        """Visit a Schema."""
 
     @abstractmethod
     def struct(self, struct: StructType, field_results: List[Callable[[], T]]) -> T:
-        """Visit a StructType"""
+        """Visit a StructType."""
 
     @abstractmethod
     def field(self, field: NestedField, field_result: Callable[[], T]) -> T:
-        """Visit a NestedField"""
+        """Visit a NestedField."""
 
     @abstractmethod
     def list(self, list_type: ListType, element_result: Callable[[], T]) -> T:
-        """Visit a ListType"""
+        """Visit a ListType."""
 
     @abstractmethod
     def map(self, map_type: MapType, key_result: Callable[[], T], value_result: Callable[[], T]) -> T:
-        """Visit a MapType"""
+        """Visit a MapType."""
 
     @abstractmethod
     def primitive(self, primitive: PrimitiveType) -> T:
-        """Visit a PrimitiveType"""
+        """Visit a PrimitiveType."""
 
 
 class SchemaWithPartnerVisitor(Generic[P, T], ABC):
     def before_field(self, field: NestedField, field_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately before visiting a field"""
+        """Override this method to perform an action immediately before visiting a field."""
 
     def after_field(self, field: NestedField, field_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately after visiting a field"""
+        """Override this method to perform an action immediately after visiting a field."""
 
     def before_list_element(self, element: NestedField, element_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately before visiting an element within a ListType"""
+        """Override this method to perform an action immediately before visiting an element within a ListType."""
         self.before_field(element, element_partner)
 
     def after_list_element(self, element: NestedField, element_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately after visiting an element within a ListType"""
+        """Override this method to perform an action immediately after visiting an element within a ListType."""
         self.after_field(element, element_partner)
 
     def before_map_key(self, key: NestedField, key_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately before visiting a key within a MapType"""
+        """Override this method to perform an action immediately before visiting a key within a MapType."""
         self.before_field(key, key_partner)
 
     def after_map_key(self, key: NestedField, key_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately after visiting a key within a MapType"""
+        """Override this method to perform an action immediately after visiting a key within a MapType."""
         self.after_field(key, key_partner)
 
     def before_map_value(self, value: NestedField, value_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately before visiting a value within a MapType"""
+        """Override this method to perform an action immediately before visiting a value within a MapType."""
         self.before_field(value, value_partner)
 
     def after_map_value(self, value: NestedField, value_partner: Optional[P]) -> None:
-        """Override this method to perform an action immediately after visiting a value within a MapType"""
+        """Override this method to perform an action immediately after visiting a value within a MapType."""
         self.after_field(value, value_partner)
 
     @abstractmethod
     def schema(self, schema: Schema, schema_partner: Optional[P], struct_result: T) -> T:
-        """Visit a schema with a partner"""
+        """Visit a schema with a partner."""
 
     @abstractmethod
     def struct(self, struct: StructType, struct_partner: Optional[P], field_results: List[T]) -> T:
-        """Visit a struct type with a partner"""
+        """Visit a struct type with a partner."""
 
     @abstractmethod
     def field(self, field: NestedField, field_partner: Optional[P], field_result: T) -> T:
-        """Visit a nested field with a partner"""
+        """Visit a nested field with a partner."""
 
     @abstractmethod
     def list(self, list_type: ListType, list_partner: Optional[P], element_result: T) -> T:
-        """Visit a list type with a partner"""
+        """Visit a list type with a partner."""
 
     @abstractmethod
     def map(self, map_type: MapType, map_partner: Optional[P], key_result: T, value_result: T) -> T:
-        """Visit a map type with a partner"""
+        """Visit a map type with a partner."""
 
     @abstractmethod
     def primitive(self, primitive: PrimitiveType, primitive_partner: Optional[P]) -> T:
-        """Visit a primitive type with a partner"""
+        """Visit a primitive type with a partner."""
 
 
 class PrimitiveWithPartnerVisitor(SchemaWithPartnerVisitor[P, T]):
     def primitive(self, primitive: PrimitiveType, primitive_partner: Optional[P]) -> T:
-        """Visit a PrimitiveType"""
+        """Visit a PrimitiveType."""
         if isinstance(primitive, BooleanType):
             return self.visit_boolean(primitive, primitive_partner)
         elif isinstance(primitive, IntegerType):
             return self.visit_integer(primitive, primitive_partner)
         elif isinstance(primitive, LongType):
             return self.visit_long(primitive, primitive_partner)
         elif isinstance(primitive, FloatType):
@@ -428,89 +442,89 @@
         elif isinstance(primitive, BinaryType):
             return self.visit_binary(primitive, primitive_partner)
         else:
             raise ValueError(f"Unknown type: {primitive}")
 
     @abstractmethod
     def visit_boolean(self, boolean_type: BooleanType, partner: Optional[P]) -> T:
-        """Visit a BooleanType"""
+        """Visit a BooleanType."""
 
     @abstractmethod
     def visit_integer(self, integer_type: IntegerType, partner: Optional[P]) -> T:
-        """Visit a IntegerType"""
+        """Visit a IntegerType."""
 
     @abstractmethod
     def visit_long(self, long_type: LongType, partner: Optional[P]) -> T:
-        """Visit a LongType"""
+        """Visit a LongType."""
 
     @abstractmethod
     def visit_float(self, float_type: FloatType, partner: Optional[P]) -> T:
-        """Visit a FloatType"""
+        """Visit a FloatType."""
 
     @abstractmethod
     def visit_double(self, double_type: DoubleType, partner: Optional[P]) -> T:
-        """Visit a DoubleType"""
+        """Visit a DoubleType."""
 
     @abstractmethod
     def visit_decimal(self, decimal_type: DecimalType, partner: Optional[P]) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_date(self, date_type: DateType, partner: Optional[P]) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_time(self, time_type: TimeType, partner: Optional[P]) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_timestamp(self, timestamp_type: TimestampType, partner: Optional[P]) -> T:
-        """Visit a TimestampType"""
+        """Visit a TimestampType."""
 
     @abstractmethod
     def visit_timestampz(self, timestamptz_type: TimestamptzType, partner: Optional[P]) -> T:
-        """Visit a TimestamptzType"""
+        """Visit a TimestamptzType."""
 
     @abstractmethod
     def visit_string(self, string_type: StringType, partner: Optional[P]) -> T:
-        """Visit a StringType"""
+        """Visit a StringType."""
 
     @abstractmethod
     def visit_uuid(self, uuid_type: UUIDType, partner: Optional[P]) -> T:
-        """Visit a UUIDType"""
+        """Visit a UUIDType."""
 
     @abstractmethod
     def visit_fixed(self, fixed_type: FixedType, partner: Optional[P]) -> T:
-        """Visit a FixedType"""
+        """Visit a FixedType."""
 
     @abstractmethod
     def visit_binary(self, binary_type: BinaryType, partner: Optional[P]) -> T:
-        """Visit a BinaryType"""
+        """Visit a BinaryType."""
 
 
 class PartnerAccessor(Generic[P], ABC):
     @abstractmethod
     def schema_partner(self, partner: Optional[P]) -> Optional[P]:
-        """Returns the equivalent of the schema as a struct"""
+        """Returns the equivalent of the schema as a struct."""
 
     @abstractmethod
     def field_partner(self, partner_struct: Optional[P], field_id: int, field_name: str) -> Optional[P]:
-        """Returns the equivalent struct field by name or id in the partner struct"""
+        """Returns the equivalent struct field by name or id in the partner struct."""
 
     @abstractmethod
     def list_element_partner(self, partner_list: Optional[P]) -> Optional[P]:
-        """Returns the equivalent list element in the partner list"""
+        """Returns the equivalent list element in the partner list."""
 
     @abstractmethod
     def map_key_partner(self, partner_map: Optional[P]) -> Optional[P]:
-        """Returns the equivalent map key in the partner map"""
+        """Returns the equivalent map key in the partner map."""
 
     @abstractmethod
     def map_value_partner(self, partner_map: Optional[P]) -> Optional[P]:
-        """Returns the equivalent map value in the partner map"""
+        """Returns the equivalent map value in the partner map."""
 
 
 @singledispatch
 def visit_with_partner(
     schema_or_type: Union[Schema, IcebergType], partner: P, visitor: SchemaWithPartnerVisitor[T, P], accessor: PartnerAccessor[P]
 ) -> T:
     raise ValueError(f"Unsupported type: {schema_or_type}")
@@ -570,15 +584,15 @@
 @visit_with_partner.register(PrimitiveType)
 def _(primitive: PrimitiveType, partner: P, visitor: SchemaWithPartnerVisitor[P, T], _: PartnerAccessor[P]) -> T:
     return visitor.primitive(primitive, partner)
 
 
 class SchemaVisitorPerPrimitiveType(SchemaVisitor[T], ABC):
     def primitive(self, primitive: PrimitiveType) -> T:
-        """Visit a PrimitiveType"""
+        """Visit a PrimitiveType."""
         if isinstance(primitive, FixedType):
             return self.visit_fixed(primitive)
         elif isinstance(primitive, DecimalType):
             return self.visit_decimal(primitive)
         elif isinstance(primitive, BooleanType):
             return self.visit_boolean(primitive)
         elif isinstance(primitive, IntegerType):
@@ -604,333 +618,334 @@
         elif isinstance(primitive, BinaryType):
             return self.visit_binary(primitive)
         else:
             raise ValueError(f"Unknown type: {primitive}")
 
     @abstractmethod
     def visit_fixed(self, fixed_type: FixedType) -> T:
-        """Visit a FixedType"""
+        """Visit a FixedType."""
 
     @abstractmethod
     def visit_decimal(self, decimal_type: DecimalType) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_boolean(self, boolean_type: BooleanType) -> T:
-        """Visit a BooleanType"""
+        """Visit a BooleanType."""
 
     @abstractmethod
     def visit_integer(self, integer_type: IntegerType) -> T:
-        """Visit a IntegerType"""
+        """Visit a IntegerType."""
 
     @abstractmethod
     def visit_long(self, long_type: LongType) -> T:
-        """Visit a LongType"""
+        """Visit a LongType."""
 
     @abstractmethod
     def visit_float(self, float_type: FloatType) -> T:
-        """Visit a FloatType"""
+        """Visit a FloatType."""
 
     @abstractmethod
     def visit_double(self, double_type: DoubleType) -> T:
-        """Visit a DoubleType"""
+        """Visit a DoubleType."""
 
     @abstractmethod
     def visit_date(self, date_type: DateType) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_time(self, time_type: TimeType) -> T:
-        """Visit a DecimalType"""
+        """Visit a DecimalType."""
 
     @abstractmethod
     def visit_timestamp(self, timestamp_type: TimestampType) -> T:
-        """Visit a TimestampType"""
+        """Visit a TimestampType."""
 
     @abstractmethod
     def visit_timestampz(self, timestamptz_type: TimestamptzType) -> T:
-        """Visit a TimestamptzType"""
+        """Visit a TimestamptzType."""
 
     @abstractmethod
     def visit_string(self, string_type: StringType) -> T:
-        """Visit a StringType"""
+        """Visit a StringType."""
 
     @abstractmethod
     def visit_uuid(self, uuid_type: UUIDType) -> T:
-        """Visit a UUIDType"""
+        """Visit a UUIDType."""
 
     @abstractmethod
     def visit_binary(self, binary_type: BinaryType) -> T:
-        """Visit a BinaryType"""
+        """Visit a BinaryType."""
 
 
 @dataclass(init=True, eq=True, frozen=True)
 class Accessor:
-    """An accessor for a specific position in a container that implements the StructProtocol"""
+    """An accessor for a specific position in a container that implements the StructProtocol."""
 
     position: int
     inner: Optional["Accessor"] = None
 
     def __str__(self) -> str:
+        """Returns the string representation of the Accessor class."""
         return f"Accessor(position={self.position},inner={self.inner})"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Accessor class."""
         return self.__str__()
 
     def get(self, container: StructProtocol) -> Any:
-        """Returns the value at self.position in `container`
+        """Returns the value at self.position in `container`.
 
         Args:
-            container(StructProtocol): A container to access at position `self.position`
+            container (StructProtocol): A container to access at position `self.position`.
 
         Returns:
-            Any: The value at position `self.position` in the container
+            Any: The value at position `self.position` in the container.
         """
         pos = self.position
         val = container[pos]
         inner = self
         while inner.inner:
             inner = inner.inner
             val = val[inner.position]
 
         return val
 
 
 @singledispatch
 def visit(obj: Union[Schema, IcebergType], visitor: SchemaVisitor[T]) -> T:
-    """A generic function for applying a schema visitor to any point within a schema
+    """A generic function for applying a schema visitor to any point within a schema.
 
-    The function traverses the schema in post-order fashion
+    The function traverses the schema in post-order fashion.
 
     Args:
-        obj(Schema | IcebergType): An instance of a Schema or an IcebergType
-        visitor (SchemaVisitor[T]): An instance of an implementation of the generic SchemaVisitor base class
+        obj (Union[Schema, IcebergType]): An instance of a Schema or an IcebergType.
+        visitor (SchemaVisitor[T]): An instance of an implementation of the generic SchemaVisitor base class.
 
     Raises:
-        NotImplementedError: If attempting to visit an unrecognized object type
+        NotImplementedError: If attempting to visit an unrecognized object type.
     """
     raise NotImplementedError("Cannot visit non-type: %s" % obj)
 
 
 @visit.register(Schema)
 def _(obj: Schema, visitor: SchemaVisitor[T]) -> T:
-    """Visit a Schema with a concrete SchemaVisitor"""
+    """Visit a Schema with a concrete SchemaVisitor."""
     return visitor.schema(obj, visit(obj.as_struct(), visitor))
 
 
 @visit.register(StructType)
 def _(obj: StructType, visitor: SchemaVisitor[T]) -> T:
-    """Visit a StructType with a concrete SchemaVisitor"""
+    """Visit a StructType with a concrete SchemaVisitor."""
     results = []
 
     for field in obj.fields:
         visitor.before_field(field)
         result = visit(field.field_type, visitor)
         visitor.after_field(field)
         results.append(visitor.field(field, result))
 
     return visitor.struct(obj, results)
 
 
 @visit.register(ListType)
 def _(obj: ListType, visitor: SchemaVisitor[T]) -> T:
-    """Visit a ListType with a concrete SchemaVisitor"""
-
+    """Visit a ListType with a concrete SchemaVisitor."""
     visitor.before_list_element(obj.element_field)
     result = visit(obj.element_type, visitor)
     visitor.after_list_element(obj.element_field)
 
     return visitor.list(obj, result)
 
 
 @visit.register(MapType)
 def _(obj: MapType, visitor: SchemaVisitor[T]) -> T:
-    """Visit a MapType with a concrete SchemaVisitor"""
+    """Visit a MapType with a concrete SchemaVisitor."""
     visitor.before_map_key(obj.key_field)
     key_result = visit(obj.key_type, visitor)
     visitor.after_map_key(obj.key_field)
 
     visitor.before_map_value(obj.value_field)
     value_result = visit(obj.value_type, visitor)
     visitor.after_list_element(obj.value_field)
 
     return visitor.map(obj, key_result, value_result)
 
 
 @visit.register(PrimitiveType)
 def _(obj: PrimitiveType, visitor: SchemaVisitor[T]) -> T:
-    """Visit a PrimitiveType with a concrete SchemaVisitor"""
+    """Visit a PrimitiveType with a concrete SchemaVisitor."""
     return visitor.primitive(obj)
 
 
 @singledispatch
 def pre_order_visit(obj: Union[Schema, IcebergType], visitor: PreOrderSchemaVisitor[T]) -> T:
-    """A generic function for applying a schema visitor to any point within a schema
+    """A generic function for applying a schema visitor to any point within a schema.
 
     The function traverses the schema in pre-order fashion. This is a slimmed down version
     compared to the post-order traversal (missing before and after methods), mostly
     because we don't use the pre-order traversal much.
 
     Args:
-        obj(Schema | IcebergType): An instance of a Schema or an IcebergType
-        visitor (PreOrderSchemaVisitor[T]): An instance of an implementation of the generic PreOrderSchemaVisitor base class
+        obj (Union[Schema, IcebergType]): An instance of a Schema or an IcebergType.
+        visitor (PreOrderSchemaVisitor[T]): An instance of an implementation of the generic PreOrderSchemaVisitor base class.
 
     Raises:
-        NotImplementedError: If attempting to visit an unrecognized object type
+        NotImplementedError: If attempting to visit an unrecognized object type.
     """
     raise NotImplementedError("Cannot visit non-type: %s" % obj)
 
 
 @pre_order_visit.register(Schema)
 def _(obj: Schema, visitor: PreOrderSchemaVisitor[T]) -> T:
-    """Visit a Schema with a concrete PreOrderSchemaVisitor"""
+    """Visit a Schema with a concrete PreOrderSchemaVisitor."""
     return visitor.schema(obj, lambda: pre_order_visit(obj.as_struct(), visitor))
 
 
 @pre_order_visit.register(StructType)
 def _(obj: StructType, visitor: PreOrderSchemaVisitor[T]) -> T:
-    """Visit a StructType with a concrete PreOrderSchemaVisitor"""
+    """Visit a StructType with a concrete PreOrderSchemaVisitor."""
     return visitor.struct(
         obj,
         [
             partial(
                 lambda field: visitor.field(field, partial(lambda field: pre_order_visit(field.field_type, visitor), field)),
                 field,
             )
             for field in obj.fields
         ],
     )
 
 
 @pre_order_visit.register(ListType)
 def _(obj: ListType, visitor: PreOrderSchemaVisitor[T]) -> T:
-    """Visit a ListType with a concrete PreOrderSchemaVisitor"""
+    """Visit a ListType with a concrete PreOrderSchemaVisitor."""
     return visitor.list(obj, lambda: pre_order_visit(obj.element_type, visitor))
 
 
 @pre_order_visit.register(MapType)
 def _(obj: MapType, visitor: PreOrderSchemaVisitor[T]) -> T:
-    """Visit a MapType with a concrete PreOrderSchemaVisitor"""
+    """Visit a MapType with a concrete PreOrderSchemaVisitor."""
     return visitor.map(obj, lambda: pre_order_visit(obj.key_type, visitor), lambda: pre_order_visit(obj.value_type, visitor))
 
 
 @pre_order_visit.register(PrimitiveType)
 def _(obj: PrimitiveType, visitor: PreOrderSchemaVisitor[T]) -> T:
-    """Visit a PrimitiveType with a concrete PreOrderSchemaVisitor"""
+    """Visit a PrimitiveType with a concrete PreOrderSchemaVisitor."""
     return visitor.primitive(obj)
 
 
 class _IndexById(SchemaVisitor[Dict[int, NestedField]]):
-    """A schema visitor for generating a field ID to NestedField index"""
+    """A schema visitor for generating a field ID to NestedField index."""
 
     def __init__(self) -> None:
         self._index: Dict[int, NestedField] = {}
 
     def schema(self, schema: Schema, struct_result: Dict[int, NestedField]) -> Dict[int, NestedField]:
         return self._index
 
     def struct(self, struct: StructType, field_results: List[Dict[int, NestedField]]) -> Dict[int, NestedField]:
         return self._index
 
     def field(self, field: NestedField, field_result: Dict[int, NestedField]) -> Dict[int, NestedField]:
-        """Add the field ID to the index"""
+        """Add the field ID to the index."""
         self._index[field.field_id] = field
         return self._index
 
     def list(self, list_type: ListType, element_result: Dict[int, NestedField]) -> Dict[int, NestedField]:
-        """Add the list element ID to the index"""
+        """Add the list element ID to the index."""
         self._index[list_type.element_field.field_id] = list_type.element_field
         return self._index
 
     def map(
         self, map_type: MapType, key_result: Dict[int, NestedField], value_result: Dict[int, NestedField]
     ) -> Dict[int, NestedField]:
-        """Add the key ID and value ID as individual items in the index"""
+        """Add the key ID and value ID as individual items in the index."""
         self._index[map_type.key_field.field_id] = map_type.key_field
         self._index[map_type.value_field.field_id] = map_type.value_field
         return self._index
 
     def primitive(self, primitive: PrimitiveType) -> Dict[int, NestedField]:
         return self._index
 
 
 def index_by_id(schema_or_type: Union[Schema, IcebergType]) -> Dict[int, NestedField]:
-    """Generate an index of field IDs to NestedField instances
+    """Generate an index of field IDs to NestedField instances.
 
     Args:
-        schema_or_type (Schema | IcebergType): A schema or type to index
+        schema_or_type (Union[Schema, IcebergType]): A schema or type to index.
 
     Returns:
-        Dict[int, NestedField]: An index of field IDs to NestedField instances
+        Dict[int, NestedField]: An index of field IDs to NestedField instances.
     """
     return visit(schema_or_type, _IndexById())
 
 
 class _IndexByName(SchemaVisitor[Dict[str, int]]):
-    """A schema visitor for generating a field name to field ID index"""
+    """A schema visitor for generating a field name to field ID index."""
 
     def __init__(self) -> None:
         self._index: Dict[str, int] = {}
         self._short_name_to_id: Dict[str, int] = {}
         self._combined_index: Dict[str, int] = {}
         self._field_names: List[str] = []
         self._short_field_names: List[str] = []
 
     def before_list_element(self, element: NestedField) -> None:
-        """Short field names omit element when the element is a StructType"""
+        """Short field names omit element when the element is a StructType."""
         if not isinstance(element.field_type, StructType):
             self._short_field_names.append(element.name)
         self._field_names.append(element.name)
 
     def after_list_element(self, element: NestedField) -> None:
         if not isinstance(element.field_type, StructType):
             self._short_field_names.pop()
         self._field_names.pop()
 
     def before_field(self, field: NestedField) -> None:
-        """Store the field name"""
+        """Store the field name."""
         self._field_names.append(field.name)
         self._short_field_names.append(field.name)
 
     def after_field(self, field: NestedField) -> None:
-        """Remove the last field name stored"""
+        """Remove the last field name stored."""
         self._field_names.pop()
         self._short_field_names.pop()
 
     def schema(self, schema: Schema, struct_result: Dict[str, int]) -> Dict[str, int]:
         return self._index
 
     def struct(self, struct: StructType, field_results: List[Dict[str, int]]) -> Dict[str, int]:
         return self._index
 
     def field(self, field: NestedField, field_result: Dict[str, int]) -> Dict[str, int]:
-        """Add the field name to the index"""
+        """Add the field name to the index."""
         self._add_field(field.name, field.field_id)
         return self._index
 
     def list(self, list_type: ListType, element_result: Dict[str, int]) -> Dict[str, int]:
-        """Add the list element name to the index"""
+        """Add the list element name to the index."""
         self._add_field(list_type.element_field.name, list_type.element_field.field_id)
         return self._index
 
     def map(self, map_type: MapType, key_result: Dict[str, int], value_result: Dict[str, int]) -> Dict[str, int]:
-        """Add the key name and value name as individual items in the index"""
+        """Add the key name and value name as individual items in the index."""
         self._add_field(map_type.key_field.name, map_type.key_field.field_id)
         self._add_field(map_type.value_field.name, map_type.value_field.field_id)
         return self._index
 
     def _add_field(self, name: str, field_id: int) -> None:
-        """Add a field name to the index, mapping its full name to its field ID
+        """Add a field name to the index, mapping its full name to its field ID.
 
         Args:
-            name (str): The field name
-            field_id (int): The field ID
+            name (str): The field name.
+            field_id (int): The field ID.
 
         Raises:
-            ValueError: If the field name is already contained in the index
+            ValueError: If the field name is already contained in the index.
         """
         full_name = name
 
         if self._field_names:
             full_name = ".".join([".".join(self._field_names), name])
 
         if full_name in self._index:
@@ -941,64 +956,64 @@
             short_name = ".".join([".".join(self._short_field_names), name])
             self._short_name_to_id[short_name] = field_id
 
     def primitive(self, primitive: PrimitiveType) -> Dict[str, int]:
         return self._index
 
     def by_name(self) -> Dict[str, int]:
-        """Returns an index of combined full and short names
+        """Returns an index of combined full and short names.
 
         Note: Only short names that do not conflict with full names are included.
         """
         combined_index = self._short_name_to_id.copy()
         combined_index.update(self._index)
         return combined_index
 
     def by_id(self) -> Dict[int, str]:
-        """Returns an index of ID to full names"""
+        """Returns an index of ID to full names."""
         id_to_full_name = {value: key for key, value in self._index.items()}
         return id_to_full_name
 
 
 def index_by_name(schema_or_type: Union[Schema, IcebergType]) -> Dict[str, int]:
-    """Generate an index of field names to field IDs
+    """Generate an index of field names to field IDs.
 
     Args:
-        schema_or_type (Schema | IcebergType): A schema or type to index
+        schema_or_type (Union[Schema, IcebergType]): A schema or type to index.
 
     Returns:
-        Dict[str, int]: An index of field names to field IDs
+        Dict[str, int]: An index of field names to field IDs.
     """
     if len(schema_or_type.fields) > 0:
         indexer = _IndexByName()
         visit(schema_or_type, indexer)
         return indexer.by_name()
     else:
         return EMPTY_DICT
 
 
 def index_name_by_id(schema_or_type: Union[Schema, IcebergType]) -> Dict[int, str]:
-    """Generate an index of field IDs full field names
+    """Generate an index of field IDs full field names.
 
     Args:
-        schema_or_type (Schema | IcebergType): A schema or type to index
+        schema_or_type (Union[Schema, IcebergType]): A schema or type to index.
 
     Returns:
-        Dict[str, int]: An index of field IDs to full names
+        Dict[str, int]: An index of field IDs to full names.
     """
     indexer = _IndexByName()
     visit(schema_or_type, indexer)
     return indexer.by_id()
 
 
 Position = int
 
 
 class _BuildPositionAccessors(SchemaVisitor[Dict[Position, Accessor]]):
-    """A schema visitor for generating a field ID to accessor index
+    """A schema visitor for generating a field ID to accessor index.
 
     Example:
         >>> from pyiceberg.schema import Schema
         >>> from pyiceberg.types import *
         >>> schema = Schema(
         ...     NestedField(field_id=2, name="id", field_type=IntegerType(), required=False),
         ...     NestedField(field_id=1, name="data", field_type=StringType(), required=True),
@@ -1052,27 +1067,27 @@
         return {}
 
     def primitive(self, primitive: PrimitiveType) -> Dict[Position, Accessor]:
         return {}
 
 
 def build_position_accessors(schema_or_type: Union[Schema, IcebergType]) -> Dict[int, Accessor]:
-    """Generate an index of field IDs to schema position accessors
+    """Generate an index of field IDs to schema position accessors.
 
     Args:
-        schema_or_type (Schema | IcebergType): A schema or type to index
+        schema_or_type (Union[Schema, IcebergType]): A schema or type to index.
 
     Returns:
-        Dict[int, Accessor]: An index of field IDs to accessors
+        Dict[int, Accessor]: An index of field IDs to accessors.
     """
     return visit(schema_or_type, _BuildPositionAccessors())
 
 
 class _FindLastFieldId(SchemaVisitor[int]):
-    """Traverses the schema to get the highest field-id"""
+    """Traverses the schema to get the highest field-id."""
 
     def schema(self, schema: Schema, struct_result: int) -> int:
         return struct_result
 
     def struct(self, struct: StructType, field_results: List[int]) -> int:
         return max(field_results)
 
@@ -1086,20 +1101,20 @@
         return max(key_result, value_result)
 
     def primitive(self, primitive: PrimitiveType) -> int:
         return 0
 
 
 def assign_fresh_schema_ids(schema: Schema) -> Schema:
-    """Traverses the schema, and sets new IDs"""
+    """Traverses the schema, and sets new IDs."""
     return pre_order_visit(schema, _SetFreshIDs())
 
 
 class _SetFreshIDs(PreOrderSchemaVisitor[IcebergType]):
-    """Traverses the schema and assigns monotonically increasing ids"""
+    """Traverses the schema and assigns monotonically increasing ids."""
 
     counter: itertools.count  # type: ignore
     reserved_ids: Dict[int, int]
 
     def __init__(self, start: int = 1) -> None:
         self.counter = itertools.count(start)
         self.reserved_ids = {}
@@ -1290,22 +1305,22 @@
                 value_type=value_result,
                 value_required=map_type.value_required,
             )
 
 
 @singledispatch
 def promote(file_type: IcebergType, read_type: IcebergType) -> IcebergType:
-    """Promotes reading a file type to a read type
+    """Promotes reading a file type to a read type.
 
     Args:
-        file_type (IcebergType): The type of the Avro file
-        read_type (IcebergType): The requested read type
+        file_type (IcebergType): The type of the Avro file.
+        read_type (IcebergType): The requested read type.
 
     Raises:
-        ResolveError: If attempting to resolve an unrecognized object type
+        ResolveError: If attempting to resolve an unrecognized object type.
     """
     if file_type == read_type:
         return file_type
     else:
         raise ResolveError(f"Cannot promote {file_type} to {read_type}")
 
 
@@ -1348,7 +1363,16 @@
     if isinstance(read_type, DecimalType):
         if file_type.precision <= read_type.precision and file_type.scale == file_type.scale:
             return read_type
         else:
             raise ResolveError(f"Cannot reduce precision from {file_type} to {read_type}")
     else:
         raise ResolveError(f"Cannot promote an decimal to {read_type}")
+
+
+@promote.register(FixedType)
+def _(file_type: FixedType, read_type: IcebergType) -> IcebergType:
+    if isinstance(read_type, UUIDType) and len(file_type) == 16:
+        # Since pyarrow reads parquet UUID as fixed 16-byte binary, the promotion is needed to ensure read compatibility
+        return read_type
+    else:
+        raise ResolveError(f"Cannot promote {file_type} to {read_type}")
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/serializers.py` & `pyiceberg-0.4.0rc1/pyiceberg/serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,54 +19,54 @@
 import json
 
 from pyiceberg.io import InputFile, InputStream, OutputFile
 from pyiceberg.table.metadata import TableMetadata, TableMetadataUtil
 
 
 class FromByteStream:
-    """A collection of methods that deserialize dictionaries into Iceberg objects"""
+    """A collection of methods that deserialize dictionaries into Iceberg objects."""
 
     @staticmethod
     def table_metadata(byte_stream: InputStream, encoding: str = "utf-8") -> TableMetadata:
-        """Instantiate a TableMetadata object from a byte stream
+        """Instantiate a TableMetadata object from a byte stream.
 
         Args:
-            byte_stream: A file-like byte stream object
-            encoding (default "utf-8"): The byte encoder to use for the reader
+            byte_stream: A file-like byte stream object.
+            encoding (default "utf-8"): The byte encoder to use for the reader.
         """
         reader = codecs.getreader(encoding)
         metadata = json.load(reader(byte_stream))
         return TableMetadataUtil.parse_obj(metadata)
 
 
 class FromInputFile:
-    """A collection of methods that deserialize InputFiles into Iceberg objects"""
+    """A collection of methods that deserialize InputFiles into Iceberg objects."""
 
     @staticmethod
     def table_metadata(input_file: InputFile, encoding: str = "utf-8") -> TableMetadata:
-        """Create a TableMetadata instance from an input file
+        """Create a TableMetadata instance from an input file.
 
         Args:
-            input_file (InputFile): A custom implementation of the iceberg.io.file.InputFile abstract base class
-            encoding (str): Encoding to use when loading bytestream
+            input_file (InputFile): A custom implementation of the iceberg.io.file.InputFile abstract base class.
+            encoding (str): Encoding to use when loading bytestream.
 
         Returns:
-            TableMetadata: A table metadata instance
+            TableMetadata: A table metadata instance.
 
         """
         with input_file.open() as input_stream:
             return FromByteStream.table_metadata(byte_stream=input_stream, encoding=encoding)
 
 
 class ToOutputFile:
-    """A collection of methods that serialize Iceberg objects into files given an OutputFile instance"""
+    """A collection of methods that serialize Iceberg objects into files given an OutputFile instance."""
 
     @staticmethod
     def table_metadata(metadata: TableMetadata, output_file: OutputFile, overwrite: bool = False) -> None:
-        """Write a TableMetadata instance to an output file
+        """Write a TableMetadata instance to an output file.
 
         Args:
-            output_file (OutputFile): A custom implementation of the iceberg.io.file.OutputFile abstract base class
+            output_file (OutputFile): A custom implementation of the iceberg.io.file.OutputFile abstract base class.
             overwrite (bool): Where to overwrite the file if it already exists. Defaults to `False`.
         """
         with output_file.create(overwrite=overwrite) as output_stream:
             output_stream.write(metadata.json().encode("utf-8"))
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/table/__init__.py` & `pyiceberg-0.4.0rc1/tests/table/test_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,353 +10,370 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-from __future__ import annotations
+# pylint:disable=redefined-outer-name
+from typing import Any, Dict
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from functools import cached_property
-from itertools import chain
-from multiprocessing.pool import ThreadPool
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    TypeVar,
-)
-
-from pydantic import Field
+import pytest
+from sortedcontainers import SortedList
 
+from pyiceberg.catalog.noop import NoopCatalog
 from pyiceberg.expressions import (
     AlwaysTrue,
     And,
-    BooleanExpression,
-    visitors,
+    EqualTo,
+    In,
 )
-from pyiceberg.expressions.visitors import inclusive_projection
-from pyiceberg.io import FileIO
-from pyiceberg.io.pyarrow import project_table
+from pyiceberg.io import PY_IO_IMPL, load_file_io
 from pyiceberg.manifest import (
     DataFile,
-    ManifestContent,
-    ManifestFile,
-    files,
+    DataFileContent,
+    FileFormat,
+    ManifestEntry,
+    ManifestEntryStatus,
 )
-from pyiceberg.partitioning import PartitionSpec
+from pyiceberg.partitioning import PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.table.metadata import TableMetadata
-from pyiceberg.table.snapshots import Snapshot, SnapshotLogEntry
-from pyiceberg.table.sorting import SortOrder
-from pyiceberg.typedef import (
-    EMPTY_DICT,
-    Identifier,
-    KeyDefaultDict,
-    Properties,
+from pyiceberg.table import StaticTable, Table, _match_deletes_to_datafile
+from pyiceberg.table.metadata import INITIAL_SEQUENCE_NUMBER, TableMetadataV2
+from pyiceberg.table.snapshots import (
+    Operation,
+    Snapshot,
+    SnapshotLogEntry,
+    Summary,
 )
-
-if TYPE_CHECKING:
-    import pandas as pd
-    import pyarrow as pa
-    from duckdb import DuckDBPyConnection
-
-
-class Table:
-    identifier: Identifier = Field()
-    metadata: TableMetadata = Field()
-    metadata_location: str = Field()
-    io: FileIO
-
-    def __init__(self, identifier: Identifier, metadata: TableMetadata, metadata_location: str, io: FileIO) -> None:
-        self.identifier = identifier
-        self.metadata = metadata
-        self.metadata_location = metadata_location
-        self.io = io
-
-    def refresh(self) -> Table:
-        """Refresh the current table metadata"""
-        raise NotImplementedError("To be implemented")
-
-    def name(self) -> Identifier:
-        """Return the identifier of this table"""
-        return self.identifier
-
-    def scan(
-        self,
-        row_filter: Optional[BooleanExpression] = None,
-        selected_fields: Tuple[str] = ("*",),
-        case_sensitive: bool = True,
-        snapshot_id: Optional[int] = None,
-        options: Properties = EMPTY_DICT,
-    ) -> TableScan[Any]:
-        return DataScan(
-            table=self,
-            row_filter=row_filter or AlwaysTrue(),
-            selected_fields=selected_fields,
-            case_sensitive=case_sensitive,
-            snapshot_id=snapshot_id,
-            options=options,
-        )
-
-    def schema(self) -> Schema:
-        """Return the schema for this table"""
-        return next(schema for schema in self.metadata.schemas if schema.schema_id == self.metadata.current_schema_id)
-
-    def schemas(self) -> Dict[int, Schema]:
-        """Return a dict of the schema of this table"""
-        return {schema.schema_id: schema for schema in self.metadata.schemas}
-
-    def spec(self) -> PartitionSpec:
-        """Return the partition spec of this table"""
-        return next(spec for spec in self.metadata.partition_specs if spec.spec_id == self.metadata.default_spec_id)
-
-    def specs(self) -> Dict[int, PartitionSpec]:
-        """Return a dict the partition specs this table"""
-        return {spec.spec_id: spec for spec in self.metadata.partition_specs}
-
-    def sort_order(self) -> SortOrder:
-        """Return the sort order of this table"""
-        return next(
-            sort_order for sort_order in self.metadata.sort_orders if sort_order.order_id == self.metadata.default_sort_order_id
-        )
-
-    def sort_orders(self) -> Dict[int, SortOrder]:
-        """Return a dict of the sort orders of this table"""
-        return {sort_order.order_id: sort_order for sort_order in self.metadata.sort_orders}
-
-    def location(self) -> str:
-        """Return the table's base location."""
-        return self.metadata.location
-
-    def current_snapshot(self) -> Optional[Snapshot]:
-        """Get the current snapshot for this table, or None if there is no current snapshot."""
-        if snapshot_id := self.metadata.current_snapshot_id:
-            return self.snapshot_by_id(snapshot_id)
-        return None
-
-    def snapshot_by_id(self, snapshot_id: int) -> Optional[Snapshot]:
-        """Get the snapshot of this table with the given id, or None if there is no matching snapshot."""
-        try:
-            return next(snapshot for snapshot in self.metadata.snapshots if snapshot.snapshot_id == snapshot_id)
-        except StopIteration:
-            return None
-
-    def snapshot_by_name(self, name: str) -> Optional[Snapshot]:
-        """Returns the snapshot referenced by the given name or null if no such reference exists."""
-        if ref := self.metadata.refs.get(name):
-            return self.snapshot_by_id(ref.snapshot_id)
-        return None
-
-    def history(self) -> List[SnapshotLogEntry]:
-        """Get the snapshot history of this table."""
-        return self.metadata.snapshot_log
-
-    def __eq__(self, other: Any) -> bool:
-        return (
-            self.identifier == other.identifier
-            and self.metadata == other.metadata
-            and self.metadata_location == other.metadata_location
-            if isinstance(other, Table)
-            else False
-        )
-
-
-S = TypeVar("S", bound="TableScan", covariant=True)  # type: ignore
+from pyiceberg.table.sorting import (
+    NullOrder,
+    SortDirection,
+    SortField,
+    SortOrder,
+)
+from pyiceberg.transforms import BucketTransform, IdentityTransform
+from pyiceberg.types import LongType, NestedField
 
 
-class TableScan(Generic[S], ABC):
-    table: Table
-    row_filter: BooleanExpression
-    selected_fields: Tuple[str]
-    case_sensitive: bool
-    snapshot_id: Optional[int]
-    options: Properties
-
-    def __init__(
-        self,
-        table: Table,
-        row_filter: Optional[BooleanExpression] = None,
-        selected_fields: Tuple[str] = ("*",),
-        case_sensitive: bool = True,
-        snapshot_id: Optional[int] = None,
-        options: Properties = EMPTY_DICT,
-    ):
-        self.table = table
-        self.row_filter = row_filter or AlwaysTrue()
-        self.selected_fields = selected_fields
-        self.case_sensitive = case_sensitive
-        self.snapshot_id = snapshot_id
-        self.options = options
-
-    def snapshot(self) -> Optional[Snapshot]:
-        if self.snapshot_id:
-            return self.table.snapshot_by_id(self.snapshot_id)
-        return self.table.current_snapshot()
-
-    def projection(self) -> Schema:
-        snapshot_schema = self.table.schema()
-        if snapshot := self.snapshot():
-            if snapshot_schema_id := snapshot.schema_id:
-                snapshot_schema = self.table.schemas()[snapshot_schema_id]
-
-        if "*" in self.selected_fields:
-            return snapshot_schema
-
-        return snapshot_schema.select(*self.selected_fields, case_sensitive=self.case_sensitive)
-
-    @abstractmethod
-    def plan_files(self) -> Iterator[ScanTask]:
-        ...
-
-    @abstractmethod
-    def to_arrow(self) -> pa.Table:
-        ...
-
-    @abstractmethod
-    def to_pandas(self, **kwargs: Any) -> pd.DataFrame:
-        ...
-
-    def update(self: S, **overrides: Any) -> S:
-        """Creates a copy of this table scan with updated fields."""
-        return type(self)(**{**self.__dict__, **overrides})
-
-    def use_ref(self, name: str) -> S:
-        if self.snapshot_id:
-            raise ValueError(f"Cannot override ref, already set snapshot id={self.snapshot_id}")
-        if snapshot := self.table.snapshot_by_name(name):
-            return self.update(snapshot_id=snapshot.snapshot_id)
-
-        raise ValueError(f"Cannot scan unknown ref={name}")
-
-    def select(self, *field_names: str) -> S:
-        if "*" in self.selected_fields:
-            return self.update(selected_fields=field_names)
-        return self.update(selected_fields=tuple(set(self.selected_fields).intersection(set(field_names))))
-
-    def filter(self, new_row_filter: BooleanExpression) -> S:
-        return self.update(row_filter=And(self.row_filter, new_row_filter))
-
-    def with_case_sensitive(self, case_sensitive: bool = True) -> S:
-        return self.update(case_sensitive=case_sensitive)
-
-
-class ScanTask(ABC):
-    pass
-
-
-@dataclass(init=False)
-class FileScanTask(ScanTask):
-    file: DataFile
-    start: int
-    length: int
-
-    def __init__(self, data_file: DataFile, start: Optional[int] = None, length: Optional[int] = None):
-        self.file = data_file
-        self.start = start or 0
-        self.length = length or data_file.file_size_in_bytes
-
-
-def _check_content(file: DataFile) -> DataFile:
-    try:
-        if file.content == ManifestContent.DELETES:
-            raise ValueError("PyIceberg does not support deletes: https://github.com/apache/iceberg/issues/6568")
-        return file
-    except AttributeError:
-        # If the attribute is not there, it is a V1 record
-        return file
-
-
-def _open_manifest(io: FileIO, manifest: ManifestFile, partition_filter: Callable[[DataFile], bool]) -> List[FileScanTask]:
-    all_files = files(io.new_input(manifest.manifest_path))
-    matching_partition_files = filter(partition_filter, all_files)
-    matching_partition_data_files = map(_check_content, matching_partition_files)
-    return [FileScanTask(file) for file in matching_partition_data_files]
-
-
-class DataScan(TableScan["DataScan"]):
-    def __init__(
-        self,
-        table: Table,
-        row_filter: Optional[BooleanExpression] = None,
-        selected_fields: Tuple[str] = ("*",),
-        case_sensitive: bool = True,
-        snapshot_id: Optional[int] = None,
-        options: Properties = EMPTY_DICT,
-    ):
-        super().__init__(table, row_filter, selected_fields, case_sensitive, snapshot_id, options)
-
-    def _build_partition_projection(self, spec_id: int) -> BooleanExpression:
-        project = inclusive_projection(self.table.schema(), self.table.specs()[spec_id])
-        return project(self.row_filter)
-
-    @cached_property
-    def partition_filters(self) -> KeyDefaultDict[int, BooleanExpression]:
-        return KeyDefaultDict(self._build_partition_projection)
-
-    def _build_manifest_evaluator(self, spec_id: int) -> Callable[[ManifestFile], bool]:
-        spec = self.table.specs()[spec_id]
-        return visitors.manifest_evaluator(spec, self.table.schema(), self.partition_filters[spec_id], self.case_sensitive)
-
-    def _build_partition_evaluator(self, spec_id: int) -> Callable[[DataFile], bool]:
-        spec = self.table.specs()[spec_id]
-        partition_type = spec.partition_type(self.table.schema())
-        partition_schema = Schema(*partition_type.fields)
-        partition_expr = self.partition_filters[spec_id]
-
-        evaluator = visitors.expression_evaluator(partition_schema, partition_expr, self.case_sensitive)
-        return lambda data_file: evaluator(data_file.partition)
-
-    def plan_files(self) -> Iterator[FileScanTask]:
-        snapshot = self.snapshot()
-        if not snapshot:
-            return iter([])
-
-        io = self.table.io
-
-        # step 1: filter manifests using partition summaries
-        # the filter depends on the partition spec used to write the manifest file, so create a cache of filters for each spec id
-
-        manifest_evaluators: Dict[int, Callable[[ManifestFile], bool]] = KeyDefaultDict(self._build_manifest_evaluator)
-
-        manifests = [
-            manifest_file
-            for manifest_file in snapshot.manifests(io)
-            if manifest_evaluators[manifest_file.partition_spec_id](manifest_file)
-        ]
-
-        # step 2: filter the data files in each manifest
-        # this filter depends on the partition spec used to write the manifest file
-
-        partition_evaluators: Dict[int, Callable[[DataFile], bool]] = KeyDefaultDict(self._build_partition_evaluator)
-
-        with ThreadPool() as pool:
-            return chain(
-                *pool.starmap(
-                    func=_open_manifest,
-                    iterable=[(io, manifest, partition_evaluators[manifest.partition_spec_id]) for manifest in manifests],
-                )
-            )
-
-    def to_arrow(self) -> pa.Table:
-        return project_table(
-            self.plan_files(), self.table, self.row_filter, self.projection(), case_sensitive=self.case_sensitive
+@pytest.fixture
+def table(example_table_metadata_v2: Dict[str, Any]) -> Table:
+    table_metadata = TableMetadataV2(**example_table_metadata_v2)
+    return Table(
+        identifier=("database", "table"),
+        metadata=table_metadata,
+        metadata_location=f"{table_metadata.location}/uuid.metadata.json",
+        io=load_file_io(),
+        catalog=NoopCatalog("NoopCatalog"),
+    )
+
+
+@pytest.fixture
+def static_table(metadata_location: str) -> StaticTable:
+    return StaticTable.from_metadata(metadata_location)
+
+
+def test_schema(table: Table) -> None:
+    assert table.schema() == Schema(
+        NestedField(field_id=1, name="x", field_type=LongType(), required=True),
+        NestedField(field_id=2, name="y", field_type=LongType(), required=True, doc="comment"),
+        NestedField(field_id=3, name="z", field_type=LongType(), required=True),
+        schema_id=1,
+        identifier_field_ids=[1, 2],
+    )
+
+
+def test_schemas(table: Table) -> None:
+    assert table.schemas() == {
+        0: Schema(
+            NestedField(field_id=1, name="x", field_type=LongType(), required=True),
+            schema_id=0,
+            identifier_field_ids=[],
+        ),
+        1: Schema(
+            NestedField(field_id=1, name="x", field_type=LongType(), required=True),
+            NestedField(field_id=2, name="y", field_type=LongType(), required=True, doc="comment"),
+            NestedField(field_id=3, name="z", field_type=LongType(), required=True),
+            schema_id=1,
+            identifier_field_ids=[1, 2],
+        ),
+    }
+
+
+def test_spec(table: Table) -> None:
+    assert table.spec() == PartitionSpec(
+        PartitionField(source_id=1, field_id=1000, transform=IdentityTransform(), name="x"), spec_id=0
+    )
+
+
+def test_specs(table: Table) -> None:
+    assert table.specs() == {
+        0: PartitionSpec(PartitionField(source_id=1, field_id=1000, transform=IdentityTransform(), name="x"), spec_id=0)
+    }
+
+
+def test_sort_order(table: Table) -> None:
+    assert table.sort_order() == SortOrder(
+        SortField(source_id=2, transform=IdentityTransform(), direction=SortDirection.ASC, null_order=NullOrder.NULLS_FIRST),
+        SortField(
+            source_id=3,
+            transform=BucketTransform(num_buckets=4),
+            direction=SortDirection.DESC,
+            null_order=NullOrder.NULLS_LAST,
+        ),
+        order_id=3,
+    )
+
+
+def test_sort_orders(table: Table) -> None:
+    assert table.sort_orders() == {
+        3: SortOrder(
+            SortField(source_id=2, transform=IdentityTransform(), direction=SortDirection.ASC, null_order=NullOrder.NULLS_FIRST),
+            SortField(
+                source_id=3,
+                transform=BucketTransform(num_buckets=4),
+                direction=SortDirection.DESC,
+                null_order=NullOrder.NULLS_LAST,
+            ),
+            order_id=3,
         )
+    }
 
-    def to_pandas(self, **kwargs: Any) -> pd.DataFrame:
-        return self.to_arrow().to_pandas(**kwargs)
 
-    def to_duckdb(self, table_name: str, connection: Optional[DuckDBPyConnection] = None) -> DuckDBPyConnection:
-        import duckdb
+def test_location(table: Table) -> None:
+    assert table.location() == "s3://bucket/test/location"
 
-        con = connection or duckdb.connect(database=":memory:")
-        con.register(table_name, self.to_arrow())
 
-        return con
+def test_current_snapshot(table: Table) -> None:
+    assert table.current_snapshot() == Snapshot(
+        snapshot_id=3055729675574597004,
+        parent_snapshot_id=3051729675574597004,
+        sequence_number=1,
+        timestamp_ms=1555100955770,
+        manifest_list="s3://a/b/2.avro",
+        summary=Summary(operation=Operation.APPEND),
+        schema_id=1,
+    )
+
+
+def test_snapshot_by_id(table: Table) -> None:
+    assert table.snapshot_by_id(3055729675574597004) == Snapshot(
+        snapshot_id=3055729675574597004,
+        parent_snapshot_id=3051729675574597004,
+        sequence_number=1,
+        timestamp_ms=1555100955770,
+        manifest_list="s3://a/b/2.avro",
+        summary=Summary(operation=Operation.APPEND),
+        schema_id=1,
+    )
+
+
+def test_snapshot_by_id_does_not_exist(table: Table) -> None:
+    assert table.snapshot_by_id(-1) is None
+
+
+def test_snapshot_by_name(table: Table) -> None:
+    assert table.snapshot_by_name("test") == Snapshot(
+        snapshot_id=3051729675574597004,
+        parent_snapshot_id=None,
+        sequence_number=0,
+        timestamp_ms=1515100955770,
+        manifest_list="s3://a/b/1.avro",
+        summary=Summary(operation=Operation.APPEND),
+        schema_id=None,
+    )
+
+
+def test_snapshot_by_name_does_not_exist(table: Table) -> None:
+    assert table.snapshot_by_name("doesnotexist") is None
+
+
+def test_history(table: Table) -> None:
+    assert table.history() == [
+        SnapshotLogEntry(snapshot_id="3051729675574597004", timestamp_ms=1515100955770),
+        SnapshotLogEntry(snapshot_id="3055729675574597004", timestamp_ms=1555100955770),
+    ]
+
+
+def test_table_scan_select(table: Table) -> None:
+    scan = table.scan()
+    assert scan.selected_fields == ("*",)
+    assert scan.select("a", "b").selected_fields == ("a", "b")
+    assert scan.select("a", "c").select("a").selected_fields == ("a",)
+
+
+def test_table_scan_row_filter(table: Table) -> None:
+    scan = table.scan()
+    assert scan.row_filter == AlwaysTrue()
+    assert scan.filter(EqualTo("x", 10)).row_filter == EqualTo("x", 10)
+    assert scan.filter(EqualTo("x", 10)).filter(In("y", (10, 11))).row_filter == And(EqualTo("x", 10), In("y", (10, 11)))
+
+
+def test_table_scan_ref(table: Table) -> None:
+    scan = table.scan()
+    assert scan.use_ref("test").snapshot_id == 3051729675574597004
+
+
+def test_table_scan_ref_does_not_exists(table: Table) -> None:
+    scan = table.scan()
+
+    with pytest.raises(ValueError) as exc_info:
+        _ = scan.use_ref("boom")
+
+    assert "Cannot scan unknown ref=boom" in str(exc_info.value)
+
+
+def test_table_scan_projection_full_schema(table: Table) -> None:
+    scan = table.scan()
+    assert scan.select("x", "y", "z").projection() == Schema(
+        NestedField(field_id=1, name="x", field_type=LongType(), required=True),
+        NestedField(field_id=2, name="y", field_type=LongType(), required=True, doc="comment"),
+        NestedField(field_id=3, name="z", field_type=LongType(), required=True),
+        schema_id=1,
+        identifier_field_ids=[1, 2],
+    )
+
+
+def test_table_scan_projection_single_column(table: Table) -> None:
+    scan = table.scan()
+    assert scan.select("y").projection() == Schema(
+        NestedField(field_id=2, name="y", field_type=LongType(), required=True, doc="comment"),
+        schema_id=1,
+        identifier_field_ids=[2],
+    )
+
+
+def test_table_scan_projection_single_column_case_sensitive(table: Table) -> None:
+    scan = table.scan()
+    assert scan.with_case_sensitive(False).select("Y").projection() == Schema(
+        NestedField(field_id=2, name="y", field_type=LongType(), required=True, doc="comment"),
+        schema_id=1,
+        identifier_field_ids=[2],
+    )
+
+
+def test_table_scan_projection_unknown_column(table: Table) -> None:
+    scan = table.scan()
+
+    with pytest.raises(ValueError) as exc_info:
+        _ = scan.select("a").projection()
+
+    assert "Could not find column: 'a'" in str(exc_info.value)
+
+
+def test_static_table_same_as_table(table: Table, static_table: StaticTable) -> None:
+    assert isinstance(static_table, Table)
+    assert static_table.metadata == table.metadata
+
+
+def test_static_table_io_does_not_exist(metadata_location: str) -> None:
+    with pytest.raises(ValueError):
+        StaticTable.from_metadata(metadata_location, {PY_IO_IMPL: "pyiceberg.does.not.exist.FileIO"})
+
+
+def test_match_deletes_to_datafile() -> None:
+    data_entry = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=1,
+        data_file=DataFile(
+            content=DataFileContent.DATA,
+            file_path="s3://bucket/0000.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+        ),
+    )
+    delete_entry_1 = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=0,  # Older than the data
+        data_file=DataFile(
+            content=DataFileContent.POSITION_DELETES,
+            file_path="s3://bucket/0001-delete.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+        ),
+    )
+    delete_entry_2 = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=3,
+        data_file=DataFile(
+            content=DataFileContent.POSITION_DELETES,
+            file_path="s3://bucket/0002-delete.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+            # We don't really care about the tests here
+            value_counts={},
+            null_value_counts={},
+            nan_value_counts={},
+            lower_bounds={},
+            upper_bounds={},
+        ),
+    )
+    assert _match_deletes_to_datafile(
+        data_entry,
+        SortedList(iterable=[delete_entry_1, delete_entry_2], key=lambda entry: entry.sequence_number or INITIAL_SEQUENCE_NUMBER),
+    ) == {
+        delete_entry_2.data_file,
+    }
+
+
+def test_match_deletes_to_datafile_duplicate_number() -> None:
+    data_entry = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=1,
+        data_file=DataFile(
+            content=DataFileContent.DATA,
+            file_path="s3://bucket/0000.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+        ),
+    )
+    delete_entry_1 = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=3,
+        data_file=DataFile(
+            content=DataFileContent.POSITION_DELETES,
+            file_path="s3://bucket/0001-delete.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+            # We don't really care about the tests here
+            value_counts={},
+            null_value_counts={},
+            nan_value_counts={},
+            lower_bounds={},
+            upper_bounds={},
+        ),
+    )
+    delete_entry_2 = ManifestEntry(
+        status=ManifestEntryStatus.ADDED,
+        sequence_number=3,
+        data_file=DataFile(
+            content=DataFileContent.POSITION_DELETES,
+            file_path="s3://bucket/0002-delete.parquet",
+            file_format=FileFormat.PARQUET,
+            partition={},
+            record_count=3,
+            file_size_in_bytes=3,
+            # We don't really care about the tests here
+            value_counts={},
+            null_value_counts={},
+            nan_value_counts={},
+            lower_bounds={},
+            upper_bounds={},
+        ),
+    )
+    assert _match_deletes_to_datafile(
+        data_entry,
+        SortedList(iterable=[delete_entry_1, delete_entry_2], key=lambda entry: entry.sequence_number or INITIAL_SEQUENCE_NUMBER),
+    ) == {
+        delete_entry_1.data_file,
+        delete_entry_2.data_file,
+    }
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/table/metadata.py` & `pyiceberg-0.4.0rc1/pyiceberg/table/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,53 +53,55 @@
 
 INITIAL_SEQUENCE_NUMBER = 0
 INITIAL_SPEC_ID = 0
 DEFAULT_SCHEMA_ID = 0
 
 
 def check_schemas(values: Dict[str, Any]) -> Dict[str, Any]:
-    """Validator to check if the current-schema-id is actually present in schemas"""
+    """Validator to check if the current-schema-id is actually present in schemas."""
     current_schema_id = values[CURRENT_SCHEMA_ID]
 
     for schema in values[SCHEMAS]:
         if schema.schema_id == current_schema_id:
             return values
 
     raise ValidationError(f"current-schema-id {current_schema_id} can't be found in the schemas")
 
 
 def check_partition_specs(values: Dict[str, Any]) -> Dict[str, Any]:
-    """Validator to check if the default-spec-id is present in partition-specs"""
+    """Validator to check if the default-spec-id is present in partition-specs."""
     default_spec_id = values["default_spec_id"]
 
     partition_specs: List[PartitionSpec] = values[PARTITION_SPECS]
     for spec in partition_specs:
         if spec.spec_id == default_spec_id:
             return values
 
     raise ValidationError(f"default-spec-id {default_spec_id} can't be found")
 
 
 def check_sort_orders(values: Dict[str, Any]) -> Dict[str, Any]:
-    """Validator to check if the default_sort_order_id is present in sort-orders"""
+    """Validator to check if the default_sort_order_id is present in sort-orders."""
     default_sort_order_id: int = values["default_sort_order_id"]
 
     if default_sort_order_id != UNSORTED_SORT_ORDER_ID:
         sort_orders: List[SortOrder] = values[SORT_ORDERS]
         for sort_order in sort_orders:
             if sort_order.order_id == default_sort_order_id:
                 return values
 
         raise ValidationError(f"default-sort-order-id {default_sort_order_id} can't be found in {sort_orders}")
     return values
 
 
 class TableMetadataCommonFields(IcebergBaseModel):
-    """Metadata for an Iceberg table as specified in the Apache Iceberg
-    spec (https://iceberg.apache.org/spec/#iceberg-table-spec)"""
+    """Metadata for an Iceberg table as specified in the Apache Iceberg spec.
+
+    https://iceberg.apache.org/spec/#iceberg-table-spec
+    """
 
     @root_validator(skip_on_failure=True)
     def cleanup_snapshot_id(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if data[CURRENT_SNAPSHOT_ID] == -1:
             # We treat -1 and None the same, by cleaning this up
             # in a pre-validator, we can simplify the logic later on
             data[CURRENT_SNAPSHOT_ID] = None
@@ -193,77 +195,77 @@
     The map keys are the unique snapshot reference names in the table,
     and the map values are snapshot reference objects.
     There is always a main branch reference pointing to the
     current-snapshot-id even if the refs map is null."""
 
 
 class TableMetadataV1(TableMetadataCommonFields, IcebergBaseModel):
-    """Represents version 1 of the Table Metadata
+    """Represents version 1 of the Table Metadata.
 
     More information about the specification:
     https://iceberg.apache.org/spec/#version-1-analytic-data-tables
     """
 
     # When we read a V1 format-version, we'll make sure to populate the fields
     # for V2 as well. This makes it easier downstream because we can just
     # assume that everything is a TableMetadataV2.
     # When writing, we should stick to the same version that it was,
     # because bumping the version should be an explicit operation that is up
     # to the owner of the table.
 
     @root_validator
     def set_v2_compatible_defaults(cls, data: Dict[str, Any]) -> Dict[str, Any]:
-        """Sets default values to be compatible with the format v2
+        """Sets default values to be compatible with the format v2.
 
         Args:
-            data: The raw arguments when initializing a V1 TableMetadata
+            data: The raw arguments when initializing a V1 TableMetadata.
 
         Returns:
-            The TableMetadata with the defaults applied
+            The TableMetadata with the defaults applied.
         """
         # When the schema doesn't have an ID
         if data.get("schema") and "schema_id" not in data["schema"]:
             data["schema"]["schema_id"] = DEFAULT_SCHEMA_ID
 
         return data
 
     @root_validator(skip_on_failure=True)
     def construct_schemas(cls, data: Dict[str, Any]) -> Dict[str, Any]:
-        """Converts the schema into schemas
+        """Converts the schema into schemas.
 
         For V1 schemas is optional, and if they aren't set, we'll set them
         in this validator. This was we can always use the schemas when reading
         table metadata, and we don't have to worry if it is a v1 or v2 format.
 
         Args:
-            data: The raw data after validation, meaning that the aliases are applied
+            data: The raw data after validation, meaning that the aliases are applied.
 
         Returns:
-            The TableMetadata with the schemas set, if not provided
+            The TableMetadata with the schemas set, if not provided.
         """
         if not data.get("schemas"):
             schema = data["schema_"]
             data["schemas"] = [schema]
         else:
             check_schemas(data)
         return data
 
     @root_validator(skip_on_failure=True)
     def construct_partition_specs(cls, data: Dict[str, Any]) -> Dict[str, Any]:
-        """Converts the partition_spec into partition_specs
+        """Converts the partition_spec into partition_specs.
 
         For V1 partition_specs is optional, and if they aren't set, we'll set them
         in this validator. This was we can always use the partition_specs when reading
         table metadata, and we don't have to worry if it is a v1 or v2 format.
 
         Args:
-            data: The raw data after validation, meaning that the aliases are applied
+            data: The raw data after validation, meaning that the aliases are applied.
 
         Returns:
-            The TableMetadata with the partition_specs set, if not provided
+            The TableMetadata with the partition_specs set, if not provided.
         """
         if not data.get(PARTITION_SPECS):
             fields = data[PARTITION_SPEC]
             migrated_spec = PartitionSpec(*fields)
             data[PARTITION_SPECS] = [migrated_spec]
             data[DEFAULT_SPEC_ID] = migrated_spec.spec_id
         else:
@@ -273,24 +275,24 @@
             if partition_specs := data.get(PARTITION_SPECS):
                 data["last_partition_id"] = max(spec.last_assigned_field_id for spec in partition_specs)
 
         return data
 
     @root_validator(skip_on_failure=True)
     def set_sort_orders(cls, data: Dict[str, Any]) -> Dict[str, Any]:
-        """Sets the sort_orders if not provided
+        """Sets the sort_orders if not provided.
 
         For V1 sort_orders is optional, and if they aren't set, we'll set them
         in this validator.
 
         Args:
-            data: The raw data after validation, meaning that the aliases are applied
+            data: The raw data after validation, meaning that the aliases are applied.
 
         Returns:
-            The TableMetadata with the sort_orders set, if not provided
+            The TableMetadata with the sort_orders set, if not provided.
         """
         if not data.get(SORT_ORDERS):
             data[SORT_ORDERS] = [UNSORTED_SORT_ORDER]
         else:
             check_sort_orders(data)
         return data
 
@@ -302,26 +304,26 @@
     format_version: Literal[1] = Field(alias="format-version")
     """An integer version number for the format. Currently, this can be 1 or 2
     based on the spec. Implementations must throw an exception if a table’s
     version is higher than the supported version."""
 
     schema_: Schema = Field(alias="schema")
     """The table’s current schema. (Deprecated: use schemas and
-    current-schema-id instead)"""
+    current-schema-id instead)."""
 
     partition_spec: List[Dict[str, Any]] = Field(alias="partition-spec")
     """The table’s current partition spec, stored as only fields.
     Note that this is used by writers to partition data, but is
     not used when reading because reads use the specs stored in
     manifest files. (Deprecated: use partition-specs and default-spec-id
-    instead)"""
+    instead)."""
 
 
 class TableMetadataV2(TableMetadataCommonFields, IcebergBaseModel):
-    """Represents version 2 of the Table Metadata
+    """Represents version 2 of the Table Metadata.
 
     This extends Version 1 with row-level deletes, and adds some additional
     information to the schema, such as all the historical schemas, partition-specs,
     sort-orders.
 
     For more information:
     https://iceberg.apache.org/spec/#version-2-row-level-deletes
@@ -370,15 +372,15 @@
         default_sort_order_id=fresh_sort_order.order_id,
         properties=properties,
         last_partition_id=fresh_partition_spec.last_assigned_field_id,
     )
 
 
 class TableMetadataUtil:
-    """Helper class for parsing TableMetadata"""
+    """Helper class for parsing TableMetadata."""
 
     # Once this has been resolved, we can simplify this: https://github.com/samuelcolvin/pydantic/issues/3846
     # TableMetadata = Annotated[TableMetadata, Field(alias="format-version", discriminator="format-version")]
 
     @staticmethod
     def parse_obj(data: Dict[str, Any]) -> TableMetadata:
         if "format-version" not in data:
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/table/refs.py` & `pyiceberg-0.4.0rc1/pyiceberg/table/refs.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 class SnapshotRefType(str, Enum):
     BRANCH = "branch"
     TAG = "tag"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the SnapshotRefType class."""
         return f"SnapshotRefType.{self.name}"
 
 
 class SnapshotRef(IcebergBaseModel):
     snapshot_id: int = Field(alias="snapshot-id")
     snapshot_ref_type: SnapshotRefType = Field(alias="type")
     min_snapshots_to_keep: Optional[int] = Field(alias="min-snapshots-to-keep", default=None)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/table/snapshots.py` & `pyiceberg-0.4.0rc1/pyiceberg/table/snapshots.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,34 +29,36 @@
 from pyiceberg.manifest import ManifestFile, read_manifest_list
 from pyiceberg.typedef import IcebergBaseModel
 
 OPERATION = "operation"
 
 
 class Operation(Enum):
-    """Describes the operation
+    """Describes the operation.
 
     Possible operation values are:
         - append: Only data files were added and no files were removed.
         - replace: Data and delete files were added and removed without changing table data; i.e., compaction, changing the data file format, or relocating data files.
         - overwrite: Data and delete files were added and removed in a logical overwrite operation.
         - delete: Data files were removed and their contents logically deleted and/or delete files were added to delete rows.
     """
 
     APPEND = "append"
     REPLACE = "replace"
     OVERWRITE = "overwrite"
     DELETE = "delete"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Operation class."""
         return f"Operation.{self.name}"
 
 
 class Summary(IcebergBaseModel):
-    """
+    """A class that stores the summary information for a Snapshot.
+
     The snapshot summary’s operation field is used by some operations,
     like snapshot expiration, to skip processing certain snapshots.
     """
 
     __root__: Dict[str, Union[str, Operation]]
     _additional_properties: Dict[str, str] = PrivateAttr()
 
@@ -87,28 +89,30 @@
             raise ValueError(f"Unknown type of operation: {operation}")
 
     @property
     def additional_properties(self) -> Dict[str, str]:
         return self._additional_properties
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Summary class."""
         repr_properties = f", **{repr(self._additional_properties)}" if self._additional_properties else ""
         return f"Summary({repr(self.operation)}{repr_properties})"
 
 
 class Snapshot(IcebergBaseModel):
     snapshot_id: int = Field(alias="snapshot-id")
     parent_snapshot_id: Optional[int] = Field(alias="parent-snapshot-id")
     sequence_number: Optional[int] = Field(alias="sequence-number", default=None)
     timestamp_ms: int = Field(alias="timestamp-ms")
     manifest_list: Optional[str] = Field(alias="manifest-list", description="Location of the snapshot's manifest list file")
     summary: Optional[Summary] = Field()
     schema_id: Optional[int] = Field(alias="schema-id", default=None)
 
     def __str__(self) -> str:
+        """Returns the string representation of the Snapshot class."""
         operation = f"{self.summary.operation}: " if self.summary else ""
         parent_id = f", parent_id={self.parent_snapshot_id}" if self.parent_snapshot_id else ""
         schema_id = f", schema_id={self.schema_id}" if self.schema_id is not None else ""
         result_str = f"{operation}id={self.snapshot_id}{parent_id}{schema_id}"
         return result_str
 
     def manifests(self, io: FileIO) -> List[ManifestFile]:
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/table/sorting.py` & `pyiceberg-0.4.0rc1/pyiceberg/table/sorting.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,40 +34,44 @@
 
 
 class SortDirection(Enum):
     ASC = "asc"
     DESC = "desc"
 
     def __str__(self) -> str:
+        """Returns the string representation of the SortDirection class."""
         return self.name
 
     def __repr__(self) -> str:
+        """Returns the string representation of the SortDirection class."""
         return f"SortDirection.{self.name}"
 
 
 class NullOrder(Enum):
     NULLS_FIRST = "nulls-first"
     NULLS_LAST = "nulls-last"
 
     def __str__(self) -> str:
+        """Returns the string representation of the NullOrder class."""
         return self.name.replace("_", " ")
 
     def __repr__(self) -> str:
+        """Returns the string representation of the NullOrder class."""
         return f"NullOrder.{self.name}"
 
 
 class SortField(IcebergBaseModel):
-    """Sort order field
+    """Sort order field.
 
     Args:
-      source_id (int): Source column id from the table’s schema
+      source_id (int): Source column id from the table’s schema.
       transform (str): Transform that is used to produce values to be sorted on from the source column.
                        This is the same transform as described in partition transforms.
-      direction (SortDirection): Sort direction, that can only be either asc or desc
-      null_order (NullOrder): Null order that describes the order of null values when sorted. Can only be either nulls-first or nulls-last
+      direction (SortDirection): Sort direction, that can only be either asc or desc.
+      null_order (NullOrder): Null order that describes the order of null values when sorted. Can only be either nulls-first or nulls-last.
     """
 
     def __init__(
         self,
         source_id: Optional[int] = None,
         transform: Optional[Union[Transform[Any, Any], Callable[[IcebergType], Transform[Any, Any]]]] = None,
         direction: Optional[SortDirection] = None,
@@ -93,34 +97,37 @@
 
     source_id: int = Field(alias="source-id")
     transform: Transform[Any, Any] = Field()
     direction: SortDirection = Field()
     null_order: NullOrder = Field(alias="null-order")
 
     def __str__(self) -> str:
+        """Returns the string representation of the SortField class."""
         if type(self.transform) == IdentityTransform:
             # In the case of an identity transform, we can omit the transform
             return f"{self.source_id} {self.direction} {self.null_order}"
         else:
             return f"{self.transform}({self.source_id}) {self.direction} {self.null_order}"
 
 
 INITIAL_SORT_ORDER_ID = 1
 
 
 class SortOrder(IcebergBaseModel):
-    """Describes how the data is sorted within the table
+    """Describes how the data is sorted within the table.
 
     Users can sort their data within partitions by columns to gain performance.
 
     The order of the sort fields within the list defines the order in which the sort is applied to the data.
 
     Args:
+      fields (List[SortField]): The fields how the table is sorted.
+
+    Keyword Args:
       order_id (int): An unique id of the sort-order of a table.
-      fields (List[SortField]): The fields how the table is sorted
     """
 
     order_id: int = Field(alias="order-id", default=INITIAL_SORT_ORDER_ID)
     fields: List[SortField] = Field(default_factory=list)
 
     def __init__(self, *fields: SortField, **data: Any):
         if fields:
@@ -128,21 +135,23 @@
         super().__init__(**data)
 
     @property
     def is_unsorted(self) -> bool:
         return len(self.fields) == 0
 
     def __str__(self) -> str:
+        """Returns the string representation of the SortOrder class."""
         result_str = "["
         if self.fields:
             result_str += "\n  " + "\n  ".join([str(field) for field in self.fields]) + "\n"
         result_str += "]"
         return result_str
 
     def __repr__(self) -> str:
+        """Returns the string representation of the SortOrder class."""
         fields = f"{', '.join(repr(column) for column in self.fields)}, " if self.fields else ""
         return f"SortOrder({fields}order_id={self.order_id})"
 
 
 UNSORTED_SORT_ORDER_ID = 0
 UNSORTED_SORT_ORDER = SortOrder(order_id=UNSORTED_SORT_ORDER_ID)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/transforms.py` & `pyiceberg-0.4.0rc1/pyiceberg/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,22 +38,26 @@
     BoundGreaterThan,
     BoundGreaterThanOrEqual,
     BoundIn,
     BoundLessThan,
     BoundLessThanOrEqual,
     BoundLiteralPredicate,
     BoundNotIn,
+    BoundNotStartsWith,
     BoundPredicate,
     BoundSetPredicate,
+    BoundStartsWith,
     BoundTerm,
     BoundUnaryPredicate,
     EqualTo,
     GreaterThanOrEqual,
     LessThanOrEqual,
+    NotStartsWith,
     Reference,
+    StartsWith,
     UnboundPredicate,
 )
 from pyiceberg.expressions.literals import (
     DateLiteral,
     DecimalLiteral,
     Literal,
     LongLiteral,
@@ -93,29 +97,30 @@
 HOUR = "hour"
 
 BUCKET_PARSER = ParseNumberFromBrackets(BUCKET)
 TRUNCATE_PARSER = ParseNumberFromBrackets(TRUNCATE)
 
 
 def _transform_literal(func: Callable[[L], L], lit: Literal[L]) -> Literal[L]:
-    """Small helper to upwrap the value from the literal, and wrap it again"""
+    """Small helper to upwrap the value from the literal, and wrap it again."""
     return literal(func(lit.value))
 
 
 class Transform(IcebergBaseModel, ABC, Generic[S, T]):
     """Transform base class for concrete transforms.
 
     A base class to transform values and project predicates on partition values.
     This class is not used directly. Instead, use one of module method to create the child classes.
     """
 
     __root__: str = Field()
 
     @classmethod
     def __get_validators__(cls) -> Generator[AnyCallable, None, None]:
+        """Called to validate the input of the Transform class."""
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v: Any) -> IcebergBaseModel:
@@ -169,24 +174,26 @@
         return str(value) if value is not None else "null"
 
     @property
     def dedup_name(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
+        """Returns the string representation of the Transform class."""
         return self.__root__
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Transform class."""
         if isinstance(other, Transform):
             return self.__root__ == other.__root__
         return False
 
 
 class BucketTransform(Transform[S, int]):
-    """Base Transform class to transform a value into a bucket partition value
+    """Base Transform class to transform a value into a bucket partition value.
 
     Transforms are parameterized by a number of buckets. Bucket partition transforms use a 32-bit
     hash of the source value to produce a positive value by mod the bucket number.
 
     Args:
       num_buckets (int): The number of buckets.
     """
@@ -274,14 +281,15 @@
             raise ValueError(f"Unknown type {source}")
 
         if bucket:
             return lambda v: (hash_func(v) & IntegerType.max) % self._num_buckets if v else None
         return hash_func
 
     def __repr__(self) -> str:
+        """Returns the string representation of the BucketTransform class."""
         return f"BucketTransform(num_buckets={self._num_buckets})"
 
 
 class TimeResolution(IntEnum):
     YEAR = 6
     MONTH = 5
     WEEK = 4
@@ -368,14 +376,15 @@
     def granularity(self) -> TimeResolution:
         return TimeResolution.YEAR
 
     def to_human_string(self, _: IcebergType, value: Optional[S]) -> str:
         return datetime.to_human_year(value) if isinstance(value, int) else "null"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the YearTransform class."""
         return "YearTransform()"
 
 
 class MonthTransform(TimeTransform[S]):
     """Transforms a datetime value into a month value.
 
     Example:
@@ -414,14 +423,15 @@
     def granularity(self) -> TimeResolution:
         return TimeResolution.MONTH
 
     def to_human_string(self, _: IcebergType, value: Optional[S]) -> str:
         return datetime.to_human_month(value) if isinstance(value, int) else "null"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the MonthTransform class."""
         return "MonthTransform()"
 
 
 class DayTransform(TimeTransform[S]):
     """Transforms a datetime value into a day value.
 
     Example:
@@ -463,14 +473,15 @@
     def granularity(self) -> TimeResolution:
         return TimeResolution.DAY
 
     def to_human_string(self, _: IcebergType, value: Optional[S]) -> str:
         return datetime.to_human_day(value) if isinstance(value, int) else "null"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the DayTransform class."""
         return "DayTransform()"
 
 
 class HourTransform(TimeTransform[S]):
     """Transforms a datetime value into a hour value.
 
     Example:
@@ -502,19 +513,20 @@
     def granularity(self) -> TimeResolution:
         return TimeResolution.HOUR
 
     def to_human_string(self, _: IcebergType, value: Optional[S]) -> str:
         return datetime.to_human_hour(value) if isinstance(value, int) else "null"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the HourTransform class."""
         return "HourTransform()"
 
 
 def _base64encode(buffer: bytes) -> str:
-    """Converts bytes to base64 string"""
+    """Converts bytes to base64 string."""
     return base64.b64encode(buffer).decode("ISO-8859-1")
 
 
 class IdentityTransform(Transform[S, S]):
     """Transforms a value into itself.
 
     Example:
@@ -547,33 +559,36 @@
             raise ValueError(f"Could not project: {pred}")
 
     @property
     def preserves_order(self) -> bool:
         return True
 
     def satisfies_order_of(self, other: Transform[S, T]) -> bool:
-        """ordering by value is the same as long as the other preserves order"""
+        """Ordering by value is the same as long as the other preserves order."""
         return other.preserves_order
 
     def to_human_string(self, source_type: IcebergType, value: Optional[S]) -> str:
         return _human_string(value, source_type) if value is not None else "null"
 
     def __str__(self) -> str:
+        """Returns the string representation of the IdentityTransform class."""
         return "identity"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the IdentityTransform class."""
         return "IdentityTransform()"
 
 
 class TruncateTransform(Transform[S, S]):
     """A transform for truncating a value to a specified width.
+
     Args:
-      width (int): The truncate width, should be positive
+      width (int): The truncate width, should be positive.
     Raises:
-      ValueError: If a type is provided that is incompatible with a Truncate transform
+      ValueError: If a type is provided that is incompatible with a Truncate transform.
     """
 
     __root__: str = Field()
     _source_type: IcebergType = PrivateAttr()
     _width: PositiveInt = PrivateAttr()
 
     def __init__(self, width: int, **data: Any):
@@ -596,17 +611,14 @@
 
     def project(self, name: str, pred: BoundPredicate[L]) -> Optional[UnboundPredicate[Any]]:
         field_type = pred.term.ref().field.field_type
 
         if isinstance(pred.term, BoundTransform):
             return _project_transform_predicate(self, name, pred)
 
-        # Implement startswith and notstartswith for string (and probably binary)
-        # https://github.com/apache/iceberg/issues/6112
-
         if isinstance(pred, BoundUnaryPredicate):
             return pred.as_unbound(Reference(name))
         elif isinstance(pred, BoundIn):
             return _set_apply_transform(name, pred, self.transform(field_type))
         elif isinstance(field_type, (IntegerType, LongType, DecimalType)):
             if isinstance(pred, BoundLiteralPredicate):
                 return _truncate_number(name, pred, self.transform(field_type))
@@ -658,14 +670,15 @@
             return "null"
         elif isinstance(value, bytes):
             return _base64encode(value)
         else:
             return str(value)
 
     def __repr__(self) -> str:
+        """Returns the string representation of the TruncateTransform class."""
         return f"TruncateTransform(width={self._width})"
 
 
 @singledispatch
 def _human_string(value: Any, _type: IcebergType) -> str:
     return str(value)
 
@@ -702,20 +715,21 @@
 
 @_int_to_human_string.register(TimestamptzType)
 def _(_type: IcebergType, value: int) -> str:
     return datetime.to_human_timestamptz(value)
 
 
 class UnknownTransform(Transform[S, T]):
-    """A transform that represents when an unknown transform is provided
+    """A transform that represents when an unknown transform is provided.
+
     Args:
-      source_type (IcebergType): An Iceberg `Type`
-      transform (str): A string name of a transform
-    Raises:
-      AttributeError: If the apply method is called.
+      transform (str): A string name of a transform.
+
+    Keyword Args:
+      source_type (IcebergType): An Iceberg `Type`.
     """
 
     __root__: LiteralType["unknown"] = Field(default="unknown")  # noqa: F821
     _transform: str = PrivateAttr()
 
     def __init__(self, transform: str, **data: Any):
         super().__init__(**data)
@@ -730,19 +744,20 @@
     def result_type(self, source: IcebergType) -> StringType:
         return StringType()
 
     def project(self, name: str, pred: BoundPredicate[L]) -> Optional[UnboundPredicate[Any]]:
         return None
 
     def __repr__(self) -> str:
+        """Returns the string representation of the UnknownTransform class."""
         return f"UnknownTransform(transform={repr(self._transform)})"
 
 
 class VoidTransform(Transform[S, None], Singleton):
-    """A transform that always returns None"""
+    """A transform that always returns None."""
 
     __root__ = "void"
 
     def transform(self, source: IcebergType) -> Callable[[Optional[S]], Optional[T]]:
         return lambda v: None
 
     def can_transform(self, _: IcebergType) -> bool:
@@ -754,14 +769,15 @@
     def project(self, name: str, pred: BoundPredicate[L]) -> Optional[UnboundPredicate[Any]]:
         return None
 
     def to_human_string(self, _: IcebergType, value: Optional[S]) -> str:
         return "null"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the VoidTransform class."""
         return "VoidTransform()"
 
 
 def _truncate_number(
     name: str, pred: BoundLiteralPredicate[L], transform: Callable[[Optional[L]], Optional[L]]
 ) -> Optional[UnboundPredicate[Any]]:
     boundary = pred.literal
@@ -790,14 +806,18 @@
 
     if type(pred) in {BoundLessThan, BoundLessThanOrEqual}:
         return LessThanOrEqual(Reference(name), _transform_literal(transform, boundary))
     elif type(pred) in {BoundGreaterThan, BoundGreaterThanOrEqual}:
         return GreaterThanOrEqual(Reference(name), _transform_literal(transform, boundary))
     if isinstance(pred, BoundEqualTo):
         return EqualTo(Reference(name), _transform_literal(transform, boundary))
+    elif isinstance(pred, BoundStartsWith):
+        return StartsWith(Reference(name), _transform_literal(transform, boundary))
+    elif isinstance(pred, BoundNotStartsWith):
+        return NotStartsWith(Reference(name), _transform_literal(transform, boundary))
     else:
         return None
 
 
 def _project_transform_predicate(
     transform: Transform[Any, Any], partition_name: str, pred: BoundPredicate[L]
 ) -> Optional[UnboundPredicate[Any]]:
@@ -823,14 +843,14 @@
     if isinstance(pred, BoundSetPredicate):
         return pred.as_unbound(Reference(name), {_transform_literal(transform, literal) for literal in literals})
     else:
         raise ValueError(f"Unknown BoundSetPredicate: {pred}")
 
 
 class BoundTransform(BoundTerm[L]):
-    """A transform expression"""
+    """A transform expression."""
 
     transform: Transform[L, Any]
 
     def __init__(self, term: BoundTerm[L], transform: Transform[L, Any]):
         self.term: BoundTerm[L] = term
         self.transform = transform
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/typedef.py` & `pyiceberg-0.4.0rc1/pyiceberg/typedef.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 if TYPE_CHECKING:
     from pyiceberg.types import StructType
 
 
 class FrozenDict(Dict[Any, Any]):
     def __setitem__(self, instance: Any, value: Any) -> None:
+        """Used for assigning a value to a FrozenDict."""
         raise AttributeError("FrozenDict does not support assignment")
 
     def update(self, *args: Any, **kwargs: Any) -> None:
         raise AttributeError("FrozenDict does not support .update()")
 
 
 EMPTY_DICT = FrozenDict()
@@ -57,14 +58,15 @@
 # from https://stackoverflow.com/questions/2912231/is-there-a-clever-way-to-pass-the-key-to-defaultdicts-default-factory
 class KeyDefaultDict(Dict[K, V]):
     def __init__(self, default_factory: Callable[[K], V]):
         super().__init__()
         self.default_factory = default_factory
 
     def __missing__(self, key: K) -> V:
+        """Defines behavior if you access a non-existent key in a KeyDefaultDict."""
         val = self.default_factory(key)
         self[key] = val
         return val
 
 
 Identifier = Tuple[str, ...]
 Properties = Dict[str, str]
@@ -72,23 +74,23 @@
 
 # Represents the literal value
 L = TypeVar("L", str, bool, int, float, bytes, UUID, Decimal, covariant=True)
 
 
 @runtime_checkable
 class StructProtocol(Protocol):  # pragma: no cover
-    """A generic protocol used by accessors to get and set at positions of an object"""
+    """A generic protocol used by accessors to get and set at positions of an object."""
 
     @abstractmethod
     def __getitem__(self, pos: int) -> Any:
-        ...
+        """Used for fetching a value from a StructProtocol."""
 
     @abstractmethod
     def __setitem__(self, pos: int, value: Any) -> None:
-        ...
+        """Used for assigning a value to a StructProtocol."""
 
 
 class IcebergBaseModel(BaseModel):
     """
     This class extends the Pydantic BaseModel to set default values by overriding them.
 
     This is because we always want to set by_alias to True. In Python, the dash can't
@@ -128,30 +130,34 @@
     _position_to_field_name: Dict[int, str]
 
     def __init__(self, *data: Any, struct: Optional[StructType] = None, **named_data: Any) -> None:
         if struct is not None:
             self._position_to_field_name = {idx: field.name for idx, field in enumerate(struct.fields)}
         elif named_data:
             # Order of named_data is preserved (PEP 468) so this can be used to generate the position dict
-            self._position_to_field_name = {idx: name for idx, name in enumerate(named_data.keys())}
+            self._position_to_field_name = dict(enumerate(named_data.keys()))
         else:
             self._position_to_field_name = {idx: f"field{idx + 1}" for idx in range(len(data))}
 
         for idx, d in enumerate(data):
             self[idx] = d
 
         for field_name, d in named_data.items():
             self.__setattr__(field_name, d)
 
     def __setitem__(self, pos: int, value: Any) -> None:
+        """Used for assigning a value to a Record."""
         self.__setattr__(self._position_to_field_name[pos], value)
 
     def __getitem__(self, pos: int) -> Any:
+        """Used for fetching a value from a Record."""
         return self.__getattribute__(self._position_to_field_name[pos])
 
     def __eq__(self, other: Any) -> bool:
+        """Returns the equality of two instances of the Record class."""
         if not isinstance(other, Record):
             return False
         return self.__dict__ == other.__dict__
 
     def __repr__(self) -> str:
+        """Returns the string representation of the Record class."""
         return f"{self.__class__.__name__}[{', '.join(f'{key}={repr(value)}' for key, value in self.__dict__.items() if not key.startswith('_'))}]"
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/types.py` & `pyiceberg-0.4.0rc1/pyiceberg/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Data types used in describing Iceberg schemas
+"""Data types used in describing Iceberg schemas.
 
 This module implements the data types described in the Iceberg specification for Iceberg schemas. To
 describe an Iceberg table schema, these classes can be used in the construction of a StructType instance.
 
 Example:
     >>> str(StructType(
     ...     NestedField(1, "required_field", StringType(), True),
@@ -51,25 +51,26 @@
 
 DECIMAL_REGEX = re.compile(r"decimal\((\d+),\s*(\d+)\)")
 FIXED = "fixed"
 FIXED_PARSER = ParseNumberFromBrackets(FIXED)
 
 
 class IcebergType(IcebergBaseModel, Singleton):
-    """Base type for all Iceberg Types
+    """Base type for all Iceberg Types.
 
     Example:
         >>> str(IcebergType())
         'IcebergType()'
         >>> repr(IcebergType())
         'IcebergType()'
     """
 
     @classmethod
     def __get_validators__(cls) -> Generator[AnyCallable, None, None]:
+        """Called to validate the input of the IcebergType class."""
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v: Any) -> IcebergType:
@@ -103,27 +104,30 @@
 
     @property
     def is_struct(self) -> bool:
         return isinstance(self, StructType)
 
 
 class PrimitiveType(IcebergType):
-    """Base class for all Iceberg Primitive Types"""
+    """Base class for all Iceberg Primitive Types."""
 
     __root__: str = Field()
 
     def __repr__(self) -> str:
+        """Returns the string representation of the PrimitiveType class."""
         return f"{type(self).__name__}()"
 
     def __str__(self) -> str:
+        """Returns the string representation of the PrimitiveType class."""
         return self.__root__
 
 
 class FixedType(PrimitiveType):
     """A fixed data type in Iceberg.
+
     Example:
         >>> FixedType(8)
         FixedType(length=8)
         >>> FixedType(8) == FixedType(8)
         True
         >>> FixedType(19) == FixedType(25)
         False
@@ -137,22 +141,29 @@
         return FixedType(length=FIXED_PARSER.match(str_repr))
 
     def __init__(self, length: int):
         super().__init__(__root__=f"fixed[{length}]")
         self._len = length
 
     def __len__(self) -> int:
+        """Returns the length of an instance of the FixedType class."""
         return self._len
 
     def __repr__(self) -> str:
+        """Returns the string representation of the FixedType class."""
         return f"FixedType(length={self._len})"
 
+    def __getnewargs__(self) -> Tuple[int]:
+        """A magic function for pickling the FixedType class."""
+        return (self._len,)
+
 
 class DecimalType(PrimitiveType):
     """A fixed data type in Iceberg.
+
     Example:
         >>> DecimalType(32, 3)
         DecimalType(precision=32, scale=3)
         >>> DecimalType(8, 3) == DecimalType(8, 3)
         True
     """
 
@@ -184,16 +195,21 @@
         return self._precision
 
     @property
     def scale(self) -> int:
         return self._scale
 
     def __repr__(self) -> str:
+        """Returns the string representation of the DecimalType class."""
         return f"DecimalType(precision={self._precision}, scale={self._scale})"
 
+    def __getnewargs__(self) -> Tuple[int, int]:
+        """A magic function for pickling the DecimalType class."""
+        return (self._precision, self._scale)
+
 
 class NestedField(IcebergType):
     """Represents a field of a struct, a map key, a map value, or a list element.
 
     This is where field IDs, names, docs, and nullability are tracked.
 
     Example:
@@ -215,45 +231,53 @@
     """
 
     field_id: int = Field(alias="id")
     name: str = Field()
     field_type: IcebergType = Field(alias="type")
     required: bool = Field(default=True)
     doc: Optional[str] = Field(default=None, repr=False)
+    initial_default: Any = Field(alias="initial-default", repr=False)
 
     def __init__(
         self,
         field_id: Optional[int] = None,
         name: Optional[str] = None,
         field_type: Optional[IcebergType] = None,
         required: bool = True,
         doc: Optional[str] = None,
+        initial_default: Optional[Any] = None,
         **data: Any,
     ):
         # We need an init when we want to use positional arguments, but
         # need also to support the aliases.
         data["field_id"] = data["id"] if "id" in data else field_id
         data["name"] = name
         data["field_type"] = data["type"] if "type" in data else field_type
         data["required"] = required
         data["doc"] = doc
+        data["initial_default"] = initial_default
         super().__init__(**data)
 
     def __str__(self) -> str:
+        """Returns the string representation of the NestedField class."""
         doc = "" if not self.doc else f" ({self.doc})"
         req = "required" if self.required else "optional"
         return f"{self.field_id}: {self.name}: {req} {self.field_type}{doc}"
 
+    def __getnewargs__(self) -> Tuple[int, str, IcebergType, bool, Optional[str]]:
+        """A magic function for pickling the NestedField class."""
+        return (self.field_id, self.name, self.field_type, self.required, self.doc)
+
     @property
     def optional(self) -> bool:
         return not self.required
 
 
 class StructType(IcebergType):
-    """A struct type in Iceberg
+    """A struct type in Iceberg.
 
     Example:
         >>> str(StructType(
         ...     NestedField(1, "required_field", StringType(), True),
         ...     NestedField(2, "optional_field", IntegerType())
         ... ))
         'struct<1: required_field: optional string, 2: optional_field: optional int>'
@@ -271,25 +295,32 @@
     def field(self, field_id: int) -> Optional[NestedField]:
         for field in self.fields:
             if field.field_id == field_id:
                 return field
         return None
 
     def __str__(self) -> str:
+        """Returns the string representation of the StructType class."""
         return f"struct<{', '.join(map(str, self.fields))}>"
 
     def __repr__(self) -> str:
+        """Returns the string representation of the StructType class."""
         return f"StructType(fields=({', '.join(map(repr, self.fields))},))"
 
     def __len__(self) -> int:
+        """Returns the length of an instance of the StructType class."""
         return len(self.fields)
 
+    def __getnewargs__(self) -> Tuple[NestedField, ...]:
+        """A magic function for pickling the StructType class."""
+        return self.fields
+
 
 class ListType(IcebergType):
-    """A list type in Iceberg
+    """A list type in Iceberg.
 
     Example:
         >>> ListType(element_id=3, element_type=StringType(), element_required=True)
         ListType(element_id=3, element_type=StringType(), element_required=True)
     """
 
     class Config:
@@ -312,19 +343,24 @@
             required=data["element_required"],
             field_id=data["element_id"],
             field_type=data["element_type"],
         )
         super().__init__(**data)
 
     def __str__(self) -> str:
+        """Returns the string representation of the ListType class."""
         return f"list<{self.element_type}>"
 
+    def __getnewargs__(self) -> Tuple[int, IcebergType, bool]:
+        """A magic function for pickling the ListType class."""
+        return (self.element_id, self.element_type, self.element_required)
+
 
 class MapType(IcebergType):
-    """A map type in Iceberg
+    """A map type in Iceberg.
 
     Example:
         >>> MapType(key_id=1, key_type=StringType(), value_id=2, value_type=IntegerType(), value_required=True)
         MapType(key_id=1, key_type=StringType(), value_id=2, value_type=IntegerType(), value_required=True)
     """
 
     type: Literal["map"] = "map"
@@ -357,16 +393,21 @@
         data["key_field"] = NestedField(name="key", field_id=data["key_id"], field_type=data["key_type"], required=True)
         data["value_field"] = NestedField(
             name="value", field_id=data["value_id"], field_type=data["value_type"], required=data["value_required"]
         )
         super().__init__(**data)
 
     def __str__(self) -> str:
+        """Returns the string representation of the MapType class."""
         return f"map<{self.key_type}, {self.value_type}>"
 
+    def __getnewargs__(self) -> Tuple[int, IcebergType, int, IcebergType, bool]:
+        """A magic function for pickling the MapType class."""
+        return (self.key_id, self.key_type, self.value_id, self.value_type, self.value_required)
+
 
 class BooleanType(PrimitiveType):
     """A boolean data type in Iceberg can be represented using an instance of this class.
 
     Example:
         >>> column_foo = BooleanType()
         >>> isinstance(column_foo, BooleanType)
@@ -375,193 +416,204 @@
         BooleanType()
     """
 
     __root__ = "boolean"
 
 
 class IntegerType(PrimitiveType):
-    """An Integer data type in Iceberg can be represented using an instance of this class. Integers in Iceberg are
-    32-bit signed and can be promoted to Longs.
+    """An Integer data type in Iceberg can be represented using an instance of this class.
+
+    Integers in Iceberg are 32-bit signed and can be promoted to Longs.
 
     Example:
         >>> column_foo = IntegerType()
         >>> isinstance(column_foo, IntegerType)
         True
 
     Attributes:
         max (int): The maximum allowed value for Integers, inherited from the canonical Iceberg implementation
-          in Java (returns `2147483647`)
+            in Java (returns `2147483647`)
         min (int): The minimum allowed value for Integers, inherited from the canonical Iceberg implementation
-          in Java (returns `-2147483648`)
+            in Java (returns `-2147483648`)
     """
 
     max: ClassVar[int] = 2147483647
     min: ClassVar[int] = -2147483648
 
     __root__ = "int"
 
 
 class LongType(PrimitiveType):
-    """A Long data type in Iceberg can be represented using an instance of this class. Longs in Iceberg are
-    64-bit signed integers.
+    """A Long data type in Iceberg can be represented using an instance of this class.
+
+    Longs in Iceberg are 64-bit signed integers.
 
     Example:
         >>> column_foo = LongType()
         >>> isinstance(column_foo, LongType)
         True
         >>> column_foo
         LongType()
         >>> str(column_foo)
         'long'
 
     Attributes:
         max (int): The maximum allowed value for Longs, inherited from the canonical Iceberg implementation
-          in Java. (returns `9223372036854775807`)
+            in Java. (returns `9223372036854775807`)
         min (int): The minimum allowed value for Longs, inherited from the canonical Iceberg implementation
-          in Java (returns `-9223372036854775808`)
+            in Java (returns `-9223372036854775808`)
     """
 
     max: ClassVar[int] = 9223372036854775807
     min: ClassVar[int] = -9223372036854775808
 
     __root__ = "long"
 
 
 class FloatType(PrimitiveType):
-    """A Float data type in Iceberg can be represented using an instance of this class. Floats in Iceberg are
-    32-bit IEEE 754 floating points and can be promoted to Doubles.
+    """A Float data type in Iceberg can be represented using an instance of this class.
+
+    Floats in Iceberg are 32-bit IEEE 754 floating points and can be promoted to Doubles.
 
     Example:
         >>> column_foo = FloatType()
         >>> isinstance(column_foo, FloatType)
         True
         >>> column_foo
         FloatType()
 
     Attributes:
         max (float): The maximum allowed value for Floats, inherited from the canonical Iceberg implementation
-          in Java. (returns `3.4028235e38`)
+            in Java. (returns `3.4028235e38`)
         min (float): The minimum allowed value for Floats, inherited from the canonical Iceberg implementation
-          in Java (returns `-3.4028235e38`)
+            in Java (returns `-3.4028235e38`)
     """
 
     max: ClassVar[float] = 3.4028235e38
     min: ClassVar[float] = -3.4028235e38
 
     __root__ = "float"
 
 
 class DoubleType(PrimitiveType):
-    """A Double data type in Iceberg can be represented using an instance of this class. Doubles in Iceberg are
-    64-bit IEEE 754 floating points.
+    """A Double data type in Iceberg can be represented using an instance of this class.
+
+    Doubles in Iceberg are 64-bit IEEE 754 floating points.
 
     Example:
         >>> column_foo = DoubleType()
         >>> isinstance(column_foo, DoubleType)
         True
         >>> column_foo
         DoubleType()
     """
 
     __root__ = "double"
 
 
 class DateType(PrimitiveType):
-    """A Date data type in Iceberg can be represented using an instance of this class. Dates in Iceberg are
-    calendar dates without a timezone or time.
+    """A Date data type in Iceberg can be represented using an instance of this class.
+
+    Dates in Iceberg are calendar dates without a timezone or time.
 
     Example:
         >>> column_foo = DateType()
         >>> isinstance(column_foo, DateType)
         True
         >>> column_foo
         DateType()
     """
 
     __root__ = "date"
 
 
 class TimeType(PrimitiveType):
-    """A Time data type in Iceberg can be represented using an instance of this class. Times in Iceberg
-    have microsecond precision and are a time of day without a date or timezone.
+    """A Time data type in Iceberg can be represented using an instance of this class.
+
+    Times in Iceberg have microsecond precision and are a time of day without a date or timezone.
 
     Example:
         >>> column_foo = TimeType()
         >>> isinstance(column_foo, TimeType)
         True
         >>> column_foo
         TimeType()
     """
 
     __root__ = "time"
 
 
 class TimestampType(PrimitiveType):
-    """A Timestamp data type in Iceberg can be represented using an instance of this class. Timestamps in
-    Iceberg have microsecond precision and include a date and a time of day without a timezone.
+    """A Timestamp data type in Iceberg can be represented using an instance of this class.
+
+    Timestamps in Iceberg have microsecond precision and include a date and a time of day without a timezone.
 
     Example:
         >>> column_foo = TimestampType()
         >>> isinstance(column_foo, TimestampType)
         True
         >>> column_foo
         TimestampType()
     """
 
     __root__ = "timestamp"
 
 
 class TimestamptzType(PrimitiveType):
-    """A Timestamptz data type in Iceberg can be represented using an instance of this class. Timestamptzs in
-    Iceberg are stored as UTC and include a date and a time of day with a timezone.
+    """A Timestamptz data type in Iceberg can be represented using an instance of this class.
+
+    Timestamptzs in Iceberg are stored as UTC and include a date and a time of day with a timezone.
 
     Example:
         >>> column_foo = TimestamptzType()
         >>> isinstance(column_foo, TimestamptzType)
         True
         >>> column_foo
         TimestamptzType()
     """
 
     __root__ = "timestamptz"
 
 
 class StringType(PrimitiveType):
-    """A String data type in Iceberg can be represented using an instance of this class. Strings in
-    Iceberg are arbitrary-length character sequences and are encoded with UTF-8.
+    """A String data type in Iceberg can be represented using an instance of this class.
+
+    Strings in Iceberg are arbitrary-length character sequences and are encoded with UTF-8.
 
     Example:
         >>> column_foo = StringType()
         >>> isinstance(column_foo, StringType)
         True
         >>> column_foo
         StringType()
     """
 
     __root__ = "string"
 
 
 class UUIDType(PrimitiveType):
-    """A UUID data type in Iceberg can be represented using an instance of this class. UUIDs in
-    Iceberg are universally unique identifiers.
+    """A UUID data type in Iceberg can be represented using an instance of this class.
+
+    UUIDs in Iceberg are universally unique identifiers.
 
     Example:
         >>> column_foo = UUIDType()
         >>> isinstance(column_foo, UUIDType)
         True
         >>> column_foo
         UUIDType()
     """
 
     __root__ = "uuid"
 
 
 class BinaryType(PrimitiveType):
-    """A Binary data type in Iceberg can be represented using an instance of this class. Binaries in
-    Iceberg are arbitrary-length byte arrays.
+    """A Binary data type in Iceberg can be represented using an instance of this class.
+
+    Binaries in Iceberg are arbitrary-length byte arrays.
 
     Example:
         >>> column_foo = BinaryType()
         >>> isinstance(column_foo, BinaryType)
         True
         >>> column_foo
         BinaryType()
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/__init__.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/bin_packing.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/bin_packing.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
     def add(self, item: T, weight: int) -> None:
         self.bin_weight += weight
         self.items.append(item)
 
 
 class PackingIterator(Generic[T]):
-
     bins: List[Bin[T]]
 
     def __init__(
         self,
         items: Iterable[T],
         target_weight: int,
         lookback: int,
@@ -61,17 +60,19 @@
         self.target_weight = target_weight
         self.lookback = lookback
         self.weight_func = weight_func
         self.largest_bin_first = largest_bin_first
         self.bins = []
 
     def __iter__(self) -> PackingIterator[T]:
+        """Returns an iterator for the PackingIterator class."""
         return self
 
     def __next__(self) -> List[T]:
+        """Returns the next item when iterating over the PackingIterator class."""
         while True:
             try:
                 item = next(self.items)
                 weight = self.weight_func(item)
                 bin_ = self.find_bin(weight)
                 if bin_ is not None:
                     bin_.add(item, weight)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/config.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import logging
 import os
 from typing import List, Optional
 
-import yaml
+import strictyaml
 
 from pyiceberg.typedef import FrozenDict, RecursiveDict
 
 PYICEBERG = "pyiceberg_"
+DEFAULT = "default"
 CATALOG = "catalog"
-HOME = "HOME"
+DEFAULT_CATALOG = f"{DEFAULT}-{CATALOG}"
 PYICEBERG_HOME = "PYICEBERG_HOME"
 PYICEBERG_YML = ".pyiceberg.yaml"
 
 logger = logging.getLogger(__name__)
 
 
 def merge_config(lhs: RecursiveDict, rhs: RecursiveDict) -> RecursiveDict:
-    """merges right-hand side into the left-hand side"""
+    """Merges right-hand side into the left-hand side."""
     new_config = lhs.copy()
     for rhs_key, rhs_value in rhs.items():
         if rhs_key in new_config:
             lhs_value = new_config[rhs_key]
             if isinstance(lhs_value, dict) and isinstance(rhs_value, dict):
                 # If they are both dicts, then we have to go deeper
                 new_config[rhs_key] = merge_config(lhs_value, rhs_value)
@@ -47,62 +48,63 @@
             # New key
             new_config[rhs_key] = rhs_value
 
     return new_config
 
 
 def _lowercase_dictionary_keys(input_dict: RecursiveDict) -> RecursiveDict:
-    """Lowers all the keys of a dictionary in a recursive manner, to make the lookup case-insensitive"""
+    """Lowers all the keys of a dictionary in a recursive manner, to make the lookup case-insensitive."""
     return {k.lower(): _lowercase_dictionary_keys(v) if isinstance(v, dict) else v for k, v in input_dict.items()}
 
 
 class Config:
     config: RecursiveDict
 
     def __init__(self) -> None:
         config = self._from_configuration_files() or {}
         config = merge_config(config, self._from_environment_variables(config))
         self.config = FrozenDict(**config)
 
     @staticmethod
     def _from_configuration_files() -> Optional[RecursiveDict]:
-        """Loads the first configuration file that its finds
+        """Loads the first configuration file that its finds.
 
         Will first look in the PYICEBERG_HOME env variable,
         and then in the home directory.
         """
 
         def _load_yaml(directory: Optional[str]) -> Optional[RecursiveDict]:
             if directory:
-                path = f"{directory.rstrip('/')}/{PYICEBERG_YML}"
+                path = os.path.join(directory, PYICEBERG_YML)
                 if os.path.isfile(path):
                     with open(path, encoding="utf-8") as f:
-                        file_config = yaml.safe_load(f)
-                        file_config_lowercase = _lowercase_dictionary_keys(file_config)
-                        return file_config_lowercase
+                        yml_str = f.read()
+                    file_config = strictyaml.load(yml_str).data
+                    file_config_lowercase = _lowercase_dictionary_keys(file_config)
+                    return file_config_lowercase
             return None
 
         # Give priority to the PYICEBERG_HOME directory
         if pyiceberg_home_config := _load_yaml(os.environ.get(PYICEBERG_HOME)):
             return pyiceberg_home_config
         # Look into the home directory
-        if pyiceberg_home_config := _load_yaml(os.environ.get(HOME)):
+        if pyiceberg_home_config := _load_yaml(os.path.expanduser("~")):
             return pyiceberg_home_config
         # Didn't find a config
         return None
 
     @staticmethod
     def _from_environment_variables(config: RecursiveDict) -> RecursiveDict:
-        """Reads the environment variables, to check if there are any prepended by PYICEBERG_
+        """Reads the environment variables, to check if there are any prepended by PYICEBERG_.
 
         Args:
-            config: Existing configuration that's being amended with configuration from environment variables
+            config: Existing configuration that's being amended with configuration from environment variables.
 
         Returns:
-            Amended configuration
+            Amended configuration.
         """
 
         def set_property(_config: RecursiveDict, path: List[str], config_value: str) -> None:
             while len(path) > 0:
                 element = path.pop(0)
                 if len(path) == 0:
                     # We're at the end
@@ -125,14 +127,26 @@
                 key = env_var_lower[len(PYICEBERG) :]
                 parts = key.split("__")
                 parts_normalized = [part.replace("_", "-") for part in parts]
                 set_property(config, parts_normalized, config_value)
 
         return config
 
+    def get_default_catalog_name(self) -> str:
+        """Returns the default catalog name.
+
+        Returns: The name of the default catalog in `default-catalog`.
+                 Returns `default` when the key cannot be found in the config file.
+        """
+        if default_catalog_name := self.config.get(DEFAULT_CATALOG):
+            if not isinstance(default_catalog_name, str):
+                raise ValueError(f"Default catalog name should be a str: {default_catalog_name}")
+            return default_catalog_name
+        return DEFAULT
+
     def get_catalog_config(self, catalog_name: str) -> Optional[RecursiveDict]:
         if CATALOG in self.config:
             catalog_name_lower = catalog_name.lower()
             catalogs = self.config[CATALOG]
             if not isinstance(catalogs, dict):
                 raise ValueError(f"Catalog configurations needs to be an object: {catalog_name}")
             if catalog_name_lower in catalogs:
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/datetime.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
-"""Helper methods for working with date/time representations
-"""
+"""Helper methods for working with date/time representations."""
 from __future__ import annotations
 
 import re
 from datetime import (
     date,
     datetime,
     time,
@@ -30,126 +29,126 @@
 EPOCH_TIMESTAMP = datetime.fromisoformat("1970-01-01T00:00:00.000000")
 ISO_TIMESTAMP = re.compile(r"\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d(.\d{1,6})?")
 EPOCH_TIMESTAMPTZ = datetime.fromisoformat("1970-01-01T00:00:00.000000+00:00")
 ISO_TIMESTAMPTZ = re.compile(r"\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d(.\d{1,6})?[-+]\d\d:\d\d")
 
 
 def micros_to_days(timestamp: int) -> int:
-    """Converts a timestamp in microseconds to a date in days"""
+    """Converts a timestamp in microseconds to a date in days."""
     return timedelta(microseconds=timestamp).days
 
 
 def micros_to_time(micros: int) -> time:
-    """Converts a timestamp in microseconds to a time"""
+    """Converts a timestamp in microseconds to a time."""
     micros, microseconds = divmod(micros, 1000000)
     micros, seconds = divmod(micros, 60)
     micros, minutes = divmod(micros, 60)
     hours = micros
     return time(hour=hours, minute=minutes, second=seconds, microsecond=microseconds)
 
 
 def date_str_to_days(date_str: str) -> int:
-    """Converts an ISO-8601 formatted date to days from 1970-01-01"""
+    """Converts an ISO-8601 formatted date to days from 1970-01-01."""
     return (date.fromisoformat(date_str) - EPOCH_DATE).days
 
 
 def date_to_days(date_val: date) -> int:
-    """Converts a Python date object to days from 1970-01-01"""
+    """Converts a Python date object to days from 1970-01-01."""
     return (date_val - EPOCH_DATE).days
 
 
 def days_to_date(days: int) -> date:
-    """Creates a date from the number of days from 1970-01-01"""
+    """Creates a date from the number of days from 1970-01-01."""
     return EPOCH_DATE + timedelta(days)
 
 
 def time_to_micros(time_str: str) -> int:
-    """Converts an ISO-8601 formatted time to microseconds from midnight"""
+    """Converts an ISO-8601 formatted time to microseconds from midnight."""
     t = time.fromisoformat(time_str)
     return (((t.hour * 60 + t.minute) * 60) + t.second) * 1_000_000 + t.microsecond
 
 
 def datetime_to_micros(dt: datetime) -> int:
-    """Converts a datetime to microseconds from 1970-01-01T00:00:00.000000"""
+    """Converts a datetime to microseconds from 1970-01-01T00:00:00.000000."""
     if dt.tzinfo:
         delta = dt - EPOCH_TIMESTAMPTZ
     else:
         delta = dt - EPOCH_TIMESTAMP
     return (delta.days * 86400 + delta.seconds) * 1_000_000 + delta.microseconds
 
 
 def timestamp_to_micros(timestamp_str: str) -> int:
-    """Converts an ISO-9601 formatted timestamp without zone to microseconds from 1970-01-01T00:00:00.000000"""
+    """Converts an ISO-9601 formatted timestamp without zone to microseconds from 1970-01-01T00:00:00.000000."""
     if ISO_TIMESTAMP.fullmatch(timestamp_str):
         return datetime_to_micros(datetime.fromisoformat(timestamp_str))
     if ISO_TIMESTAMPTZ.fullmatch(timestamp_str):
         # When we can match a timestamp without a zone, we can give a more specific error
         raise ValueError(f"Zone offset provided, but not expected: {timestamp_str}")
     raise ValueError(f"Invalid timestamp without zone: {timestamp_str} (must be ISO-8601)")
 
 
 def timestamptz_to_micros(timestamptz_str: str) -> int:
-    """Converts an ISO-8601 formatted timestamp with zone to microseconds from 1970-01-01T00:00:00.000000+00:00"""
+    """Converts an ISO-8601 formatted timestamp with zone to microseconds from 1970-01-01T00:00:00.000000+00:00."""
     if ISO_TIMESTAMPTZ.fullmatch(timestamptz_str):
         return datetime_to_micros(datetime.fromisoformat(timestamptz_str))
     if ISO_TIMESTAMP.fullmatch(timestamptz_str):
         # When we can match a timestamp without a zone, we can give a more specific error
         raise ValueError(f"Missing zone offset: {timestamptz_str} (must be ISO-8601)")
     raise ValueError(f"Invalid timestamp with zone: {timestamptz_str} (must be ISO-8601)")
 
 
 def micros_to_timestamp(micros: int) -> datetime:
-    """Converts microseconds from epoch to a timestamp"""
+    """Converts microseconds from epoch to a timestamp."""
     dt = timedelta(microseconds=micros)
     return EPOCH_TIMESTAMP + dt
 
 
 def micros_to_timestamptz(micros: int) -> datetime:
-    """Converts microseconds from epoch to an utc timestamp"""
+    """Converts microseconds from epoch to an utc timestamp."""
     dt = timedelta(microseconds=micros)
     return EPOCH_TIMESTAMPTZ + dt
 
 
 def to_human_year(year_ordinal: int) -> str:
-    """Converts a DateType value to human string"""
+    """Converts a DateType value to human string."""
     return f"{EPOCH_TIMESTAMP.year + year_ordinal:0=4d}"
 
 
 def to_human_month(month_ordinal: int) -> str:
-    """Converts a DateType value to human string"""
+    """Converts a DateType value to human string."""
     return f"{EPOCH_TIMESTAMP.year + month_ordinal // 12:0=4d}-{1 + month_ordinal % 12:0=2d}"
 
 
 def to_human_day(day_ordinal: int) -> str:
-    """Converts a DateType value to human string"""
+    """Converts a DateType value to human string."""
     return (EPOCH_DATE + timedelta(days=day_ordinal)).isoformat()
 
 
 def to_human_hour(hour_ordinal: int) -> str:
-    """Converts a DateType value to human string"""
+    """Converts a DateType value to human string."""
     return (EPOCH_TIMESTAMP + timedelta(hours=hour_ordinal)).isoformat("-", "hours")
 
 
 def to_human_time(micros_from_midnight: int) -> str:
-    """Converts a TimeType value to human string"""
+    """Converts a TimeType value to human string."""
     return micros_to_time(micros_from_midnight).isoformat()
 
 
 def to_human_timestamptz(timestamp_micros: int) -> str:
-    """Converts a TimestamptzType value to human string"""
+    """Converts a TimestamptzType value to human string."""
     return (EPOCH_TIMESTAMPTZ + timedelta(microseconds=timestamp_micros)).isoformat()
 
 
 def to_human_timestamp(timestamp_micros: int) -> str:
-    """Converts a TimestampType value to human string"""
+    """Converts a TimestampType value to human string."""
     return (EPOCH_TIMESTAMP + timedelta(microseconds=timestamp_micros)).isoformat()
 
 
 def micros_to_hours(micros: int) -> int:
-    """Converts a timestamp in microseconds to hours from 1970-01-01T00:00"""
+    """Converts a timestamp in microseconds to hours from 1970-01-01T00:00."""
     return micros // 3_600_000_000
 
 
 def days_to_months(days: int) -> int:
     d = days_to_date(days)
     return (d.year - EPOCH_DATE.year) * 12 + (d.month - EPOCH_DATE.month)
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/decimal.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/decimal.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,80 +11,80 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-"""Helper methods for working with Python Decimals
-"""
+"""Helper methods for working with Python Decimals."""
 from decimal import Decimal
 from typing import Union
 
 
 def decimal_to_unscaled(value: Decimal) -> int:
-    """Get an unscaled value given a Decimal value
+    """Get an unscaled value given a Decimal value.
 
     Args:
-        value (Decimal): A Decimal instance
+        value (Decimal): A Decimal instance.
 
     Returns:
-        int: The unscaled value
+        int: The unscaled value.
     """
     sign, digits, _ = value.as_tuple()
     return int(Decimal((sign, digits, 0)).to_integral_value())
 
 
 def unscaled_to_decimal(unscaled: int, scale: int) -> Decimal:
-    """Get a scaled Decimal value given an unscaled value and a scale
+    """Get a scaled Decimal value given an unscaled value and a scale.
 
     Args:
-        unscaled (int): An unscaled value
-        scale (int): A scale to set for the returned Decimal instance
+        unscaled (int): An unscaled value.
+        scale (int): A scale to set for the returned Decimal instance.
 
     Returns:
-        Decimal: A scaled Decimal instance
+        Decimal: A scaled Decimal instance.
     """
     sign, digits, _ = Decimal(unscaled).as_tuple()
     return Decimal((sign, digits, -scale))
 
 
 def bytes_required(value: Union[int, Decimal]) -> int:
-    """Returns the minimum number of bytes needed to serialize a decimal or unscaled value
+    """Returns the minimum number of bytes needed to serialize a decimal or unscaled value.
 
     Args:
-        value (int | Decimal): a Decimal value or unscaled int value
+        value (int | Decimal): a Decimal value or unscaled int value.
 
     Returns:
-        int: the minimum number of bytes needed to serialize the value
+        int: the minimum number of bytes needed to serialize the value.
     """
     if isinstance(value, int):
         return (value.bit_length() + 7) // 8
     elif isinstance(value, Decimal):
         return (decimal_to_unscaled(value).bit_length() + 7) // 8
 
     raise ValueError(f"Unsupported value: {value}")
 
 
 def decimal_to_bytes(value: Decimal) -> bytes:
-    """Returns a byte representation of a decimal
+    """Returns a byte representation of a decimal.
 
     Args:
-        value (Decimal): a decimal value
+        value (Decimal): a decimal value.
     Returns:
-        bytes: the unscaled value of the Decimal as bytes
+        bytes: the unscaled value of the Decimal as bytes.
     """
     unscaled_value = decimal_to_unscaled(value)
     return unscaled_value.to_bytes(bytes_required(unscaled_value), byteorder="big", signed=True)
 
 
 def truncate_decimal(value: Decimal, width: int) -> Decimal:
-    """Get a truncated Decimal value given a decimal value and a width
+    """Get a truncated Decimal value given a decimal value and a width.
+
     Args:
-        value (Decimal): a decimal value
-        width (int): A width for the returned Decimal instance
+        value (Decimal): a decimal value.
+        width (int): A width for the returned Decimal instance.
     Returns:
-        Decimal: A truncated Decimal instance
+        Decimal: A truncated Decimal instance.
     """
     unscaled_value = decimal_to_unscaled(value)
     applied_value = unscaled_value - (((unscaled_value % width) + width) % width)
-    return unscaled_to_decimal(applied_value, -value.as_tuple().exponent)
+    return unscaled_to_decimal(applied_value, abs(int(value.as_tuple().exponent)))
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/deprecated.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/deprecated.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 #  under the License.
 import functools
 import warnings
 from typing import Any, Callable, Optional
 
 
 def deprecated(deprecated_in: str, removed_in: str, help_message: Optional[str] = None) -> Callable:  # type: ignore
-    """This is a decorator which can be used to mark functions
-    as deprecated. It will result in a warning being emitted
-    when the function is used."""
+    """A decorator which can be used to mark functions as deprecated.
 
+    Adding this will result in a warning being emitted when the function is used.
+    """
     if help_message is not None:
         help_message = f" {help_message}."
 
     def decorator(func: Callable):  # type: ignore
         @functools.wraps(func)
         def new_func(*args: Any, **kwargs: Any) -> Any:
             warnings.simplefilter("always", DeprecationWarning)  # turn off filter
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/parsing.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  specific language governing permissions and limitations
 #  under the License.
 import re
 from re import Pattern
 
 
 class ParseNumberFromBrackets:
-    """Extracts the size from a string in the form of prefix[22]"""
+    """Extracts the size from a string in the form of prefix[22]."""
 
     regex: Pattern  # type: ignore
     prefix: str
 
     def __init__(self, prefix: str):
         self.prefix = prefix
         self.regex = re.compile(rf"{prefix}\[(\d+)\]")
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/schema_conversion.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/schema_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Utility class for converting between Avro and Iceberg schemas"""
-from __future__ import annotations
-
+"""Utility class for converting between Avro and Iceberg schemas."""
 import logging
 from typing import (
     Any,
     Dict,
     List,
     Tuple,
     Union,
@@ -47,40 +45,40 @@
     TimestampType,
     TimeType,
     UUIDType,
 )
 
 logger = logging.getLogger(__name__)
 
-PRIMITIVE_FIELD_TYPE_MAPPING: dict[str, PrimitiveType] = {
+PRIMITIVE_FIELD_TYPE_MAPPING: Dict[str, PrimitiveType] = {
     "boolean": BooleanType(),
     "bytes": BinaryType(),
     "double": DoubleType(),
     "float": FloatType(),
     "int": IntegerType(),
     "long": LongType(),
     "string": StringType(),
     "enum": StringType(),
 }
 
-LOGICAL_FIELD_TYPE_MAPPING: dict[tuple[str, str], PrimitiveType] = {
+LOGICAL_FIELD_TYPE_MAPPING: Dict[Tuple[str, str], PrimitiveType] = {
     ("date", "int"): DateType(),
     ("time-millis", "int"): TimeType(),
     ("timestamp-millis", "long"): TimestampType(),
     ("time-micros", "int"): TimeType(),
     ("timestamp-micros", "long"): TimestampType(),
     ("uuid", "fixed"): UUIDType(),
 }
 
 
 class AvroSchemaConversion:
-    def avro_to_iceberg(self, avro_schema: dict[str, Any]) -> Schema:
-        """Converts an Apache Avro into an Apache Iceberg schema equivalent
+    def avro_to_iceberg(self, avro_schema: Dict[str, Any]) -> Schema:
+        """Converts an Apache Avro into an Apache Iceberg schema equivalent.
 
-        This expects to have field id's to be encoded in the Avro schema::
+        This expects to have field id's to be encoded in the Avro schema:
 
             {
                 "type": "record",
                 "name": "manifest_file",
                 "fields": [
                     {"name": "manifest_path", "type": "string", "doc": "Location URI with FS scheme", "field-id": 500},
                     {"name": "manifest_length", "type": "long", "doc": "Total file size in bytes", "field-id": 501}
@@ -107,45 +105,45 @@
             ...     ),
             ...     schema_id=1
             ... )
             >>> avro_schema == iceberg_schema
             True
 
         Args:
-            avro_schema (Dict[str, Any]): The JSON decoded Avro schema
+            avro_schema (Dict[str, Any]): The JSON decoded Avro schema.
 
         Returns:
-            Equivalent Iceberg schema
+            Equivalent Iceberg schema.
         """
         return Schema(*[self._convert_field(field) for field in avro_schema["fields"]], schema_id=1)
 
     def _resolve_union(
         self, type_union: Union[Dict[str, str], List[Union[str, Dict[str, str]]], str]
     ) -> Tuple[Union[str, Dict[str, Any]], bool]:
         """
-        Converts Unions into their type and resolves if the field is required
+        Converts Unions into their type and resolves if the field is required.
 
         Examples:
             >>> AvroSchemaConversion()._resolve_union('str')
             ('str', True)
             >>> AvroSchemaConversion()._resolve_union(['null', 'str'])
             ('str', False)
             >>> AvroSchemaConversion()._resolve_union([{'type': 'str'}])
             ({'type': 'str'}, True)
             >>> AvroSchemaConversion()._resolve_union(['null', {'type': 'str'}])
             ({'type': 'str'}, False)
 
         Args:
-            type_union: The field, can be a string 'str', list ['null', 'str'], or dict {"type": 'str'}
+            type_union: The field, can be a string 'str', list ['null', 'str'], or dict {"type": 'str'}.
 
         Returns:
-            A tuple containing the type and if required
+            A tuple containing the type and if required.
 
         Raises:
-            TypeError: In the case non-optional union types are encountered
+            TypeError: In the case non-optional union types are encountered.
         """
         avro_types: Union[Dict[str, str], List[Union[Dict[str, str], str]]]
         if isinstance(type_union, str):
             # It is a primitive and required
             return type_union, True
         elif isinstance(type_union, dict):
             # It is a context and required
@@ -167,21 +165,21 @@
             raise TypeError("Only null-unions are supported")
 
         # Filter the null value and return the type
         return list(filter(lambda t: t != "null", avro_types))[0], False
 
     def _convert_schema(self, avro_type: Union[str, Dict[str, Any]]) -> IcebergType:
         """
-        Resolves the Avro type
+        Resolves the Avro type.
 
         Args:
-            avro_type: The Avro type, can be simple or complex
+            avro_type: The Avro type, can be simple or complex.
 
         Returns:
-            The equivalent IcebergType
+            The equivalent IcebergType.
 
         Raises:
             ValueError: When there are unknown types
         """
         if isinstance(avro_type, str) and avro_type in PRIMITIVE_FIELD_TYPE_MAPPING:
             return PRIMITIVE_FIELD_TYPE_MAPPING[avro_type]
         elif isinstance(avro_type, dict):
@@ -203,39 +201,39 @@
                 elif isinstance(type_identifier, str) and type_identifier in PRIMITIVE_FIELD_TYPE_MAPPING:
                     return PRIMITIVE_FIELD_TYPE_MAPPING[type_identifier]
                 else:
                     raise TypeError(f"Unknown type: {avro_type}")
         else:
             raise TypeError(f"Unknown type: {avro_type}")
 
-    def _convert_field(self, field: dict[str, Any]) -> NestedField:
-        """
-        Converts an Avro field into an Iceberg equivalent field
+    def _convert_field(self, field: Dict[str, Any]) -> NestedField:
+        """Converts an Avro field into an Iceberg equivalent field.
+
         Args:
-            field: The Avro field
+            field: The Avro field.
 
         Returns:
-            The Iceberg equivalent field
+            The Iceberg equivalent field.
         """
         if "field-id" not in field:
             raise ValueError(f"Cannot convert field, missing field-id: {field}")
 
         plain_type, required = self._resolve_union(field["type"])
 
         return NestedField(
             field_id=field["field-id"],
             name=field["name"],
             field_type=self._convert_schema(plain_type),
             required=required,
             doc=field.get("doc"),
         )
 
-    def _convert_record_type(self, record_type: dict[str, Any]) -> StructType:
+    def _convert_record_type(self, record_type: Dict[str, Any]) -> StructType:
         """
-        Converts the fields from a record into an Iceberg struct
+        Converts the fields from a record into an Iceberg struct.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> record_type = {
             ...     "type": "record",
             ...     "name": "r508",
             ...     "fields": [{
@@ -270,39 +268,40 @@
             ...         ),
             ...     )
             ... )
             >>> expected == actual
             True
 
         Args:
-            record_type: The record type itself
+            record_type: The record type itself.
 
-        Returns:
+        Returns: A StructType.
         """
         if record_type["type"] != "record":
             raise ValueError(f"Expected record type, got: {record_type}")
 
         return StructType(*[self._convert_field(field) for field in record_type["fields"]])
 
-    def _convert_array_type(self, array_type: dict[str, Any]) -> ListType:
+    def _convert_array_type(self, array_type: Dict[str, Any]) -> ListType:
         if "element-id" not in array_type:
             raise ValueError(f"Cannot convert array-type, missing element-id: {array_type}")
 
         plain_type, element_required = self._resolve_union(array_type["items"])
 
         return ListType(
             element_id=array_type["element-id"],
             element_type=self._convert_schema(plain_type),
             element_required=element_required,
         )
 
-    def _convert_map_type(self, map_type: dict[str, Any]) -> MapType:
-        """
+    def _convert_map_type(self, map_type: Dict[str, Any]) -> MapType:
+        """Converts an avro map type into an Iceberg MapType.
+
         Args:
-            map_type: The dict that describes the Avro map type
+            map_type: The dict that describes the Avro map type.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> avro_field = {
             ...     "type": "map",
             ...     "values": ["null", "long"],
             ...     "key-id": 101,
@@ -315,66 +314,67 @@
             ...     value_id=102,
             ...     value_type=LongType(),
             ...     value_required=True
             ... )
             >>> actual == expected
             True
 
-        Returns: A MapType
+        Returns: A MapType.
         """
         value_type, value_required = self._resolve_union(map_type["values"])
         return MapType(
             key_id=map_type["key-id"],
             # Avro only supports string keys
             key_type=StringType(),
             value_id=map_type["value-id"],
             value_type=self._convert_schema(value_type),
             value_required=value_required,
         )
 
-    def _convert_logical_type(self, avro_logical_type: dict[str, Any]) -> IcebergType:
-        """
-        Convert a schema with a logical type annotation. For the decimal and map
-        we need to fetch more keys from the dict, and for the simple ones we can just
-        look it up in the mapping.
+    def _convert_logical_type(self, avro_logical_type: Dict[str, Any]) -> IcebergType:
+        """Convert a schema with a logical type annotation into an IcebergType.
+
+        For the decimal and map we need to fetch more keys from the dict, and for
+        the simple ones we can just look it up in the mapping.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> avro_logical_type = {
             ...     "type": "int",
             ...     "logicalType": "date"
             ... }
             >>> actual = AvroSchemaConversion()._convert_logical_type(avro_logical_type)
             >>> actual == DateType()
             True
 
         Args:
-            avro_logical_type: The logical type
+            avro_logical_type: The logical type.
 
         Returns:
-            The converted logical type
+            The converted logical type.
 
         Raises:
-            ValueError: When the logical type is unknown
+            ValueError: When the logical type is unknown.
         """
         logical_type = avro_logical_type["logicalType"]
         physical_type = avro_logical_type["type"]
         if logical_type == "decimal":
             return self._convert_logical_decimal_type(avro_logical_type)
         elif logical_type == "map":
             return self._convert_logical_map_type(avro_logical_type)
         elif (logical_type, physical_type) in LOGICAL_FIELD_TYPE_MAPPING:
             return LOGICAL_FIELD_TYPE_MAPPING[(logical_type, physical_type)]
         else:
             raise ValueError(f"Unknown logical/physical type combination: {avro_logical_type}")
 
-    def _convert_logical_decimal_type(self, avro_type: dict[str, Any]) -> DecimalType:
-        """
+    def _convert_logical_decimal_type(self, avro_type: Dict[str, Any]) -> DecimalType:
+        """Converts an avro type to an Iceberg DecimalType.
+
         Args:
-            avro_type: The Avro type
+            avro_type: The Avro type.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> avro_decimal_type = {
             ...     "type": "bytes",
             ...     "logicalType": "decimal",
             ...     "precision": 19,
@@ -385,25 +385,25 @@
             ...     precision=19,
             ...     scale=25
             ... )
             >>> actual == expected
             True
 
         Returns:
-            A Iceberg DecimalType
+            A Iceberg DecimalType.
         """
         return DecimalType(precision=avro_type["precision"], scale=avro_type["scale"])
 
-    def _convert_logical_map_type(self, avro_type: dict[str, Any]) -> MapType:
-        """
-        In the case where a map hasn't a key as a type you can use a logical map to
-        still encode this in Avro
+    def _convert_logical_map_type(self, avro_type: Dict[str, Any]) -> MapType:
+        """Converts an avro map type to an Iceberg MapType.
+
+        In the case where a map hasn't a key as a type you can use a logical map to still encode this in Avro.
 
         Args:
-            avro_type: The Avro Type
+            avro_type: The Avro Type.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> avro_type = {
             ...     "type": "array",
             ...     "logicalType": "map",
             ...     "items": {
@@ -426,43 +426,45 @@
             >>> actual == expected
             True
 
         .. _Apache Iceberg specification:
             https://iceberg.apache.org/spec/#appendix-a-format-specific-requirements
 
         Returns:
-            The logical map
+            The logical map.
         """
         fields = avro_type["items"]["fields"]
         if len(fields) != 2:
             raise ValueError(f'Invalid key-value pair schema: {avro_type["items"]}')
         key = self._convert_field(list(filter(lambda f: f["name"] == "key", fields))[0])
         value = self._convert_field(list(filter(lambda f: f["name"] == "value", fields))[0])
         return MapType(
             key_id=key.field_id,
             key_type=key.field_type,
             value_id=value.field_id,
             value_type=value.field_type,
             value_required=value.required,
         )
 
-    def _convert_fixed_type(self, avro_type: dict[str, Any]) -> FixedType:
+    def _convert_fixed_type(self, avro_type: Dict[str, Any]) -> FixedType:
         """
-        https://avro.apache.org/docs/current/spec.html#Fixed
+        Converts Avro Type to the equivalent Iceberg fixed type.
+
+        - https://avro.apache.org/docs/current/spec.html#Fixed
 
         Args:
-            avro_type: The Avro Type
+            avro_type: The Avro type.
 
         Examples:
             >>> from pyiceberg.utils.schema_conversion import AvroSchemaConversion
             >>> avro_fixed_type = {
             ...     "name": "md5",
             ...     "type": "fixed",
             ...     "size": 16
             ... }
             >>> FixedType(length=16) == AvroSchemaConversion()._convert_fixed_type(avro_fixed_type)
             True
 
         Returns:
-            An Iceberg equivalent fixed type
+            An Iceberg equivalent fixed type.
         """
         return FixedType(length=avro_type["size"])
```

### Comparing `pyiceberg-0.3.0rc2/pyiceberg/utils/singleton.py` & `pyiceberg-0.4.0rc1/pyiceberg/utils/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 """
-This is a singleton metaclass that can be used to cache and re-use existing objects
+This is a singleton metaclass that can be used to cache and re-use existing objects.
 
 In the Iceberg codebase we have a lot of objects that are stateless (for example Types such as StringType,
 BooleanType etc). FixedTypes have arguments (eg. Fixed[22]) that we also make part of the key when caching
 the newly created object.
 
 The Singleton uses a metaclass which essentially defines a new type. When the Type gets created, it will first
 evaluate the `__call__` method with all the arguments. If we already initialized a class earlier, we'll just
```

### Comparing `pyiceberg-0.3.0rc2/pyproject.toml` & `pyiceberg-0.4.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,110 +10,98 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
 [tool.poetry]
 name = "pyiceberg"
-version = "0.3.0rc2"
+version = "0.4.0rc1"
 readme = "README.md"
 homepage = "https://iceberg.apache.org/"
 repository = "https://github.com/apache/iceberg/"
 description = "Apache Iceberg is an open table format for huge analytic datasets"
 authors = ["Apache Software Foundation <dev@iceberg.apache.org>"]
 license = "Apache License 2.0"
-
 classifiers = [
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+  "License :: OSI Approved :: Apache Software License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11"
 ]
-
 packages = [
-    { include = "pyiceberg" },
-    { from = "vendor", include = "fb303" },
-    { from = "vendor", include = "hive_metastore" },
-    { include = "tests", format = "sdist" },
-    { include = "Makefile", format = "sdist" },
-    { include = "NOTICE", format = ["sdist", "wheel"] }
-]
-
-include = [
-    {path = "dev", format = "sdist"}
+  { include = "pyiceberg" },
+  { from = "vendor", include = "fb303" },
+  { from = "vendor", include = "hive_metastore" },
+  { include = "tests", format = "sdist" },
+  { include = "Makefile", format = "sdist" },
+  { include = "NOTICE", format = ["sdist", "wheel"] }
 ]
+include = [{ path = "dev", format = "sdist" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-mmhash3 = "3.0.1"
-requests = "2.28.2"
-click = "8.1.3"
-rich = "13.2.0"
-pyyaml = "6.0.0"
-
-pydantic = "1.10.4"
-fsspec = "2023.1.0"
-
-pyparsing = "3.0.9"
-
-zstandard = "0.19.0"
-
-pyarrow = { version = "10.0.1", optional = true }
-
-pandas = { version = "1.5.3", optional = true }
-
-duckdb = { version = "0.6.1", optional = true }
-
-python-snappy = { version = "0.6.1", optional = true }
-
-thrift = { version = "0.16.0", optional = true }
-
-boto3 = {version = "1.24.59", optional = true}
-
-# The versions of the fsspec implementations should run in sync with fsspec above
-s3fs = { version = "2023.1.0", optional = true }
-adlfs = { version = "2023.1.0", optional = true }
+mmhash3 = ">=3.0.0,<4.0.0"
+requests = ">=2.20.0,<3.0.0"
+click = ">=7.1.1,<9.0.0"
+rich = ">=10.11.0,<14.0.0"
+strictyaml = ">=1.7.0,<2.0.0" # CVE-2020-14343 was fixed in 5.4.
+pydantic = ">=1.9.0,<2.0.0"
+sortedcontainers = "2.4.0"
+fsspec = ">=2021.09.0,<2024.1.0" # `lexists()` was implemented in 2021.09.0. Upper bound set arbitrarily, to be reassessed in early 2024.
+pyparsing = ">=3.0.7,<4.0.0" # The `min` keyword argument for `delimited_list()` was added in 3.0.7.
+zstandard = ">=0.13.0,<1.0.0"
+pyarrow = { version = ">=9.0.0,<13.0.0", optional = true }
+pandas = { version = ">=1.0.0,<3.0.0", optional = true }
+duckdb = { version = ">=0.5.0,<1.0.0", optional = true }
+ray = { version = ">=2.0.0,<3.0.0", optional = true }
+python-snappy = { version = ">=0.6.0,<1.0.0", optional = true }
+thrift = { version = ">=0.13.0,<1.0.0", optional = true }
+boto3 = { version = ">=1.17.106", optional = true }
+s3fs = { version = ">=2021.08.0,<2024.1.0", optional = true } # Upper bound set arbitrarily, to be reassessed in early 2024.
+adlfs = { version = ">=2021.07.0,<2024.1.0", optional = true } # Upper bound set arbitrarily, to be reassessed in early 2024.
 
 [tool.poetry.dev-dependencies]
-pytest = "7.2.1"
+pytest = "7.4.0"
 pytest-checkdocs = "2.9.0"
-pre-commit = "2.21.0"
-fastavro = "1.7.0"
-coverage = { version = "^7.0.5", extras = ["toml"] }
-requests-mock = "1.10.0"
-moto = "^4.1.0"
-typing-extensions = '4.4.0'
+pre-commit = "3.3.3"
+fastavro = "1.7.4"
+coverage = { version = "^7.2.3", extras = ["toml"] }
+requests-mock = "1.11.0"
+moto = "^4.1.12"
+typing-extensions = "^4.6.3"
 
 [tool.poetry.scripts]
 pyiceberg = "pyiceberg.cli.console:run"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 pyarrow = ["pyarrow"]
 pandas = ["pandas", "pyarrow"]
 duckdb = ["duckdb", "pyarrow"]
+ray = ["ray", "pyarrow", "pandas"]
 snappy = ["python-snappy"]
 hive = ["thrift"]
 s3fs = ["s3fs"]
 glue = ["boto3"]
 adlfs = ["adlfs"]
+dynamodb = ["boto3"]
+zstandard = ["zstandard"]
 
 [tool.pytest.ini_options]
 markers = [
-    "s3: marks a test as requiring access to s3 compliant storage (use with --aws-access-key-id, --aws-secret-access-key, and --endpoint-url args)",
-    "adlfs: marks a test as requiring access to adlfs compliant storage (use with --adlfs.account-name, --adlfs.account-key, and --adlfs.endpoint args)"
+  "s3: marks a test as requiring access to s3 compliant storage (use with --aws-access-key-id, --aws-secret-access-key, and --endpoint-url args)",
+  "adlfs: marks a test as requiring access to adlfs compliant storage (use with --adlfs.account-name, --adlfs.account-key, and --adlfs.endpoint args)",
+  "integration: marks integration tests against Apache Spark"
 ]
 
 [tool.black]
 line-length = 130
 target-version = ['py38']
 
 [tool.isort]
@@ -232,12 +220,32 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "duckdb.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "ray.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "pyparsing.*"
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = "pyspark.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "strictyaml.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "sortedcontainers.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "numpy.*"
+ignore_missing_imports = true
+
 [tool.coverage.run]
 source = ['pyiceberg/']
```

### Comparing `pyiceberg-0.3.0rc2/tests/avro/test_decoder.py` & `pyiceberg-0.4.0rc1/tests/avro/test_decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/avro/test_file.py` & `pyiceberg-0.4.0rc1/tests/avro/test_file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/avro/test_reader.py` & `pyiceberg-0.4.0rc1/tests/avro/test_reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/avro/test_resolver.py` & `pyiceberg-0.4.0rc1/tests/avro/test_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import pytest
 from pydantic import Field
 
 from pyiceberg.avro.file import AvroFile
 from pyiceberg.avro.reader import (
     DecimalReader,
+    DefaultReader,
     DoubleReader,
     FloatReader,
     IntegerReader,
     MapReader,
     StringReader,
     StructReader,
 )
@@ -276,7 +277,27 @@
             NestedField(4, "d", IntegerType(), required=False),
         )
 
         with AvroFile[Ints](PyArrowFileIO().new_input(tmp_avro_file), MANIFEST_ENTRY_SCHEMA, {-1: Ints}) as reader:
             records = list(reader)
 
     assert repr(records) == "[Ints[c=3, d=None]]"
+
+
+def test_resolver_initial_value() -> None:
+    write_schema = Schema(
+        NestedField(1, "name", StringType()),
+        schema_id=1,
+    )
+    read_schema = Schema(
+        NestedField(2, "something", StringType(), required=False, initial_default="vo"),
+        schema_id=2,
+    )
+
+    assert resolve(write_schema, read_schema) == StructReader(
+        (
+            (None, StringReader()),  # The one we skip
+            (0, DefaultReader("vo")),
+        ),
+        Record,
+        read_schema.as_struct(),
+    )
```

### Comparing `pyiceberg-0.3.0rc2/tests/catalog/integration_test_glue.py` & `pyiceberg-0.4.0rc1/tests/catalog/integration_test_glue.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-import os
-from typing import Generator, Optional
+from typing import Generator, List
 
 import boto3
 import pytest
 from botocore.exceptions import ClientError
 
 from pyiceberg.catalog import Catalog
 from pyiceberg.catalog.glue import GlueCatalog
@@ -28,154 +27,103 @@
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchNamespaceError,
     NoSuchTableError,
     TableAlreadyExistsError,
 )
 from pyiceberg.schema import Schema
-from tests.catalog.test_glue import (
-    get_random_database_name,
-    get_random_databases,
-    get_random_table_name,
-    get_random_tables,
-)
+from tests.conftest import clean_up, get_bucket_name, get_s3_path
 
-# The number of random characters in generated table/database name
-RANDOM_LENGTH = 20
 # The number of tables/databases used in list_table/namespace test
 LIST_TEST_NUMBER = 2
 
 
-def get_bucket_name() -> str:
-    """
-    Set the environment variable AWS_TEST_BUCKET for a default bucket to test
-    """
-    bucket_name = os.getenv("AWS_TEST_BUCKET")
-    if bucket_name is None:
-        raise ValueError("Please specify a bucket to run the test by setting environment variable AWS_TEST_BUCKET")
-    return bucket_name
-
-
-def get_s3_path(bucket_name: str, database_name: Optional[str] = None, table_name: Optional[str] = None) -> str:
-    result_path = f"s3://{bucket_name}"
-    if database_name is not None:
-        result_path += f"/{database_name}.db"
-
-    if table_name is not None:
-        result_path += f"/{table_name}"
-    return result_path
-
-
-@pytest.fixture(name="s3", scope="module")
-def fixture_s3_client() -> boto3.client:
-    yield boto3.client("s3")
-
-
 @pytest.fixture(name="glue", scope="module")
 def fixture_glue_client() -> boto3.client:
     yield boto3.client("glue")
 
 
-def clean_up(test_catalog: Catalog) -> None:
-    """Clean all databases and tables created during the integration test"""
-    for database_tuple in test_catalog.list_namespaces():
-        database_name = database_tuple[0]
-        if "my_iceberg_database-" in database_name:
-            for identifier in test_catalog.list_tables(database_name):
-                test_catalog.purge_table(identifier)
-            test_catalog.drop_namespace(database_name)
-
-
 @pytest.fixture(name="test_catalog", scope="module")
 def fixture_test_catalog() -> Generator[Catalog, None, None]:
-    """The pre- and post-setting of aws integration test"""
+    """The pre- and post-setting of aws integration test."""
     test_catalog = GlueCatalog("glue", warehouse=get_s3_path(get_bucket_name()))
     yield test_catalog
     clean_up(test_catalog)
 
 
-def test_create_table(test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_create_table(
+    test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema, table_name: str, database_name: str
+) -> None:
     identifier = (database_name, table_name)
     test_catalog.create_namespace(database_name)
     test_catalog.create_table(identifier, table_schema_nested, get_s3_path(get_bucket_name(), database_name, table_name))
     table = test_catalog.load_table(identifier)
     assert table.identifier == identifier
     metadata_location = table.metadata_location.split(get_bucket_name())[1][1:]
     s3.head_object(Bucket=get_bucket_name(), Key=metadata_location)
 
 
-def test_create_table_with_invalid_location(table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_create_table_with_invalid_location(table_schema_nested: Schema, table_name: str, database_name: str) -> None:
     identifier = (database_name, table_name)
     test_catalog_no_warehouse = GlueCatalog("glue")
     test_catalog_no_warehouse.create_namespace(database_name)
     with pytest.raises(ValueError):
         test_catalog_no_warehouse.create_table(identifier, table_schema_nested)
     test_catalog_no_warehouse.drop_namespace(database_name)
 
 
-def test_create_table_with_default_location(test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_create_table_with_default_location(
+    test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema, table_name: str, database_name: str
+) -> None:
     identifier = (database_name, table_name)
     test_catalog.create_namespace(database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     table = test_catalog.load_table(identifier)
     assert table.identifier == identifier
     metadata_location = table.metadata_location.split(get_bucket_name())[1][1:]
     s3.head_object(Bucket=get_bucket_name(), Key=metadata_location)
 
 
-def test_create_table_with_invalid_database(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
+def test_create_table_with_invalid_database(test_catalog: Catalog, table_schema_nested: Schema, table_name: str) -> None:
     identifier = ("invalid", table_name)
     with pytest.raises(NoSuchNamespaceError):
         test_catalog.create_table(identifier, table_schema_nested)
 
 
-def test_create_duplicated_table(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_create_duplicated_table(test_catalog: Catalog, table_schema_nested: Schema, table_name: str, database_name: str) -> None:
     test_catalog.create_namespace(database_name)
     test_catalog.create_table((database_name, table_name), table_schema_nested)
     with pytest.raises(TableAlreadyExistsError):
         test_catalog.create_table((database_name, table_name), table_schema_nested)
 
 
-def test_load_table(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_load_table(test_catalog: Catalog, table_schema_nested: Schema, table_name: str, database_name: str) -> None:
     identifier = (database_name, table_name)
     test_catalog.create_namespace(database_name)
     table = test_catalog.create_table(identifier, table_schema_nested)
     loaded_table = test_catalog.load_table(identifier)
     assert table.identifier == loaded_table.identifier
     assert table.metadata_location == loaded_table.metadata_location
     assert table.metadata == loaded_table.metadata
 
 
-def test_list_tables(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    test_tables = get_random_tables(LIST_TEST_NUMBER)
-    database_name = get_random_database_name()
+def test_list_tables(test_catalog: Catalog, table_schema_nested: Schema, database_name: str, table_list: List[str]) -> None:
     test_catalog.create_namespace(database_name)
-    for table_name in test_tables:
+    for table_name in table_list:
         test_catalog.create_table((database_name, table_name), table_schema_nested)
     identifier_list = test_catalog.list_tables(database_name)
     assert len(identifier_list) == LIST_TEST_NUMBER
-    for table_name in test_tables:
+    for table_name in table_list:
         assert (database_name, table_name) in identifier_list
 
 
-def test_rename_table(test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
-    new_database_name = get_random_database_name()
+def test_rename_table(
+    test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema, table_name: str, database_name: str
+) -> None:
+    new_database_name = f"{database_name}_new"
     test_catalog.create_namespace(database_name)
     test_catalog.create_namespace(new_database_name)
     new_table_name = f"rename-{table_name}"
     identifier = (database_name, table_name)
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
     new_identifier = (new_database_name, new_table_name)
@@ -185,97 +133,88 @@
     assert new_table.metadata_location == table.metadata_location
     metadata_location = new_table.metadata_location.split(get_bucket_name())[1][1:]
     s3.head_object(Bucket=get_bucket_name(), Key=metadata_location)
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
 
 
-def test_drop_table(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_drop_table(test_catalog: Catalog, table_schema_nested: Schema, table_name: str, database_name: str) -> None:
     identifier = (database_name, table_name)
     test_catalog.create_namespace(database_name)
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
     test_catalog.drop_table(identifier)
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
 
 
-def test_purge_table(test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_purge_table(
+    test_catalog: Catalog, s3: boto3.client, table_schema_nested: Schema, table_name: str, database_name: str
+) -> None:
     identifier = (database_name, table_name)
     test_catalog.create_namespace(database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     table = test_catalog.load_table(identifier)
     assert table.identifier == identifier
     metadata_location = table.metadata_location.split(get_bucket_name())[1][1:]
     s3.head_object(Bucket=get_bucket_name(), Key=metadata_location)
     test_catalog.purge_table(identifier)
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
     with pytest.raises(ClientError):
         s3.head_object(Bucket=get_bucket_name(), Key=metadata_location)
 
 
-def test_create_namespace(test_catalog: Catalog) -> None:
-    database_name = get_random_database_name()
+def test_create_namespace(test_catalog: Catalog, database_name: str) -> None:
     test_catalog.create_namespace(database_name)
     assert (database_name,) in test_catalog.list_namespaces()
 
 
-def test_create_duplicate_namespace(test_catalog: Catalog) -> None:
-    database_name = get_random_database_name()
+def test_create_duplicate_namespace(test_catalog: Catalog, database_name: str) -> None:
     test_catalog.create_namespace(database_name)
     with pytest.raises(NamespaceAlreadyExistsError):
         test_catalog.create_namespace(database_name)
 
 
-def test_create_namespace_with_comment_and_location(test_catalog: Catalog) -> None:
-    database_name = get_random_database_name()
+def test_create_namespace_with_comment_and_location(test_catalog: Catalog, database_name: str) -> None:
     test_location = get_s3_path(get_bucket_name(), database_name)
     test_properties = {
         "comment": "this is a test description",
         "location": test_location,
     }
     test_catalog.create_namespace(namespace=database_name, properties=test_properties)
     loaded_database_list = test_catalog.list_namespaces()
     assert (database_name,) in loaded_database_list
     properties = test_catalog.load_namespace_properties(database_name)
     assert properties["comment"] == "this is a test description"
     assert properties["location"] == test_location
 
 
-def test_list_namespaces(test_catalog: Catalog) -> None:
-    database_list = get_random_databases(LIST_TEST_NUMBER)
+def test_list_namespaces(test_catalog: Catalog, database_list: List[str]) -> None:
     for database_name in database_list:
         test_catalog.create_namespace(database_name)
     db_list = test_catalog.list_namespaces()
     for database_name in database_list:
         assert (database_name,) in db_list
     assert len(test_catalog.list_namespaces(list(database_list)[0])) == 0
 
 
-def test_drop_namespace(test_catalog: Catalog, table_schema_nested: Schema) -> None:
-    table_name = get_random_table_name()
-    database_name = get_random_database_name()
+def test_drop_namespace(test_catalog: Catalog, table_schema_nested: Schema, database_name: str, table_name: str) -> None:
     test_catalog.create_namespace(database_name)
     assert (database_name,) in test_catalog.list_namespaces()
     test_catalog.create_table((database_name, table_name), table_schema_nested)
     with pytest.raises(NamespaceNotEmptyError):
         test_catalog.drop_namespace(database_name)
     test_catalog.drop_table((database_name, table_name))
     test_catalog.drop_namespace(database_name)
     assert (database_name,) not in test_catalog.list_namespaces()
 
 
-def test_load_namespace_properties(test_catalog: Catalog) -> None:
+def test_load_namespace_properties(test_catalog: Catalog, database_name: str) -> None:
     warehouse_location = get_s3_path(get_bucket_name())
-    database_name = get_random_database_name()
     test_properties = {
         "comment": "this is a test description",
         "location": f"{warehouse_location}/{database_name}.db",
         "test_property1": "1",
         "test_property2": "2",
         "test_property3": "3",
     }
@@ -283,32 +222,29 @@
     test_catalog.create_namespace(database_name, test_properties)
     listed_properties = test_catalog.load_namespace_properties(database_name)
     for k, v in listed_properties.items():
         assert k in test_properties
         assert v == test_properties[k]
 
 
-def test_load_empty_namespace_properties(test_catalog: Catalog) -> None:
-    database_name = get_random_database_name()
+def test_load_empty_namespace_properties(test_catalog: Catalog, database_name: str) -> None:
     test_catalog.create_namespace(database_name)
     listed_properties = test_catalog.load_namespace_properties(database_name)
     assert listed_properties == {}
 
 
-def test_load_default_namespace_properties(test_catalog: Catalog, glue: boto3.client) -> None:
-    database_name = get_random_database_name()
+def test_load_default_namespace_properties(test_catalog: Catalog, glue: boto3.client, database_name: str) -> None:
     # simulate creating database with default settings through AWS Glue Web Console
     glue.create_database(DatabaseInput={"Name": database_name})
     listed_properties = test_catalog.load_namespace_properties(database_name)
     assert listed_properties == {}
 
 
-def test_update_namespace_properties(test_catalog: Catalog) -> None:
+def test_update_namespace_properties(test_catalog: Catalog, database_name: str) -> None:
     warehouse_location = get_s3_path(get_bucket_name())
-    database_name = get_random_database_name()
     test_properties = {
         "comment": "this is a test description",
         "location": f"{warehouse_location}/{database_name}.db",
         "test_property1": "1",
         "test_property2": "2",
         "test_property3": "3",
     }
```

### Comparing `pyiceberg-0.3.0rc2/tests/catalog/test_base.py` & `pyiceberg-0.4.0rc1/tests/catalog/test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+# pylint:disable=redefined-outer-name
 
 from typing import (
     Dict,
     List,
     Optional,
     Set,
     Union,
@@ -37,15 +38,15 @@
     NoSuchNamespaceError,
     NoSuchTableError,
     TableAlreadyExistsError,
 )
 from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.table import Table
+from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table
 from pyiceberg.table.metadata import TableMetadataV1
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.transforms import IdentityTransform
 from pyiceberg.typedef import EMPTY_DICT
 
 
 class InMemoryCatalog(Catalog):
@@ -64,15 +65,14 @@
         identifier: Union[str, Identifier],
         schema: Schema,
         location: Optional[str] = None,
         partition_spec: PartitionSpec = UNPARTITIONED_PARTITION_SPEC,
         sort_order: SortOrder = UNSORTED_SORT_ORDER,
         properties: Properties = EMPTY_DICT,
     ) -> Table:
-
         identifier = Catalog.identifier_to_tuple(identifier)
         namespace = Catalog.namespace_from(identifier)
 
         if identifier in self.__tables:
             raise TableAlreadyExistsError(f"Table already exists: {identifier}")
         else:
             if namespace not in self.__namespaces:
@@ -99,18 +99,22 @@
                         "properties": {},
                         "current-snapshot-id": -1,
                         "snapshots": [{"snapshot-id": 1925, "timestamp-ms": 1602638573822}],
                     }
                 ),
                 metadata_location=f's3://warehouse/{"/".join(identifier)}/metadata/metadata.json',
                 io=load_file_io(),
+                catalog=self,
             )
             self.__tables[identifier] = table
             return table
 
+    def _commit_table(self, table_request: CommitTableRequest) -> CommitTableResponse:
+        raise NotImplementedError
+
     def load_table(self, identifier: Union[str, Identifier]) -> Table:
         identifier = Catalog.identifier_to_tuple(identifier)
         try:
             return self.__tables[identifier]
         except KeyError as error:
             raise NoSuchTableError(f"Table does not exist: {identifier}") from error
 
@@ -137,14 +141,15 @@
             self.__namespaces[to_namespace] = {}
 
         self.__tables[to_identifier] = Table(
             identifier=to_identifier,
             metadata=table.metadata,
             metadata_location=table.metadata_location,
             io=load_file_io(),
+            catalog=self,
         )
         return self.__tables[to_identifier]
 
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         namespace = Catalog.identifier_to_tuple(namespace)
         if namespace in self.__namespaces:
             raise NamespaceAlreadyExistsError(f"Namespace already exists: {namespace}")
@@ -202,14 +207,19 @@
         expected_to_change = removed.difference(removals or set())
 
         return PropertiesUpdateSummary(
             removed=list(removed or []), updated=list(updates.keys() if updates else []), missing=list(expected_to_change)
         )
 
 
+@pytest.fixture
+def catalog() -> InMemoryCatalog:
+    return InMemoryCatalog("test.in.memory.catalog", **{"test.key": "test.value"})
+
+
 TEST_TABLE_IDENTIFIER = ("com", "organization", "department", "my_table")
 TEST_TABLE_NAMESPACE = ("com", "organization", "department")
 TEST_TABLE_NAME = "my_table"
 TEST_TABLE_SCHEMA = Schema(schema_id=1)
 TEST_TABLE_LOCATION = "protocol://some/location"
 TEST_TABLE_PARTITION_SPEC = PartitionSpec(PartitionField(name="x", transform=IdentityTransform(), source_id=1, field_id=1000))
 TEST_TABLE_PROPERTIES = {"key1": "value1", "key2": "value2"}
```

### Comparing `pyiceberg-0.3.0rc2/tests/catalog/test_glue.py` & `pyiceberg-0.4.0rc1/tests/catalog/test_glue.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
-import random
-import re
-import string
-from typing import Set
+from typing import List
+from unittest import mock
 
 import pytest
 from moto import mock_glue
 
 from pyiceberg.catalog.glue import GlueCatalog
 from pyiceberg.exceptions import (
     NamespaceAlreadyExistsError,
@@ -29,248 +27,204 @@
     NoSuchIcebergTableError,
     NoSuchNamespaceError,
     NoSuchPropertyException,
     NoSuchTableError,
     TableAlreadyExistsError,
 )
 from pyiceberg.schema import Schema
-
-BUCKET_NAME = "test_bucket"
-RANDOM_LENGTH = 20
-LIST_TEST_NUMBER = 100
-table_metadata_location_regex = re.compile(
-    r"""s3://test_bucket/my_iceberg_database-[a-z]{20}.db/
-    my_iceberg_table-[a-z]{20}/metadata/
-    00000-[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}.metadata.json""",
-    re.X,
-)
-
-
-def get_random_table_name() -> str:
-    prefix = "my_iceberg_table-"
-    random_tag = "".join(random.choice(string.ascii_letters) for _ in range(RANDOM_LENGTH))
-    return (prefix + random_tag).lower()
-
-
-def get_random_tables(n: int) -> Set[str]:
-    return {get_random_table_name() for _ in range(n)}
-
-
-def get_random_database_name() -> str:
-    prefix = "my_iceberg_database-"
-    random_tag = "".join(random.choice(string.ascii_letters) for _ in range(RANDOM_LENGTH))
-    return (prefix + random_tag).lower()
-
-
-def get_random_databases(n: int) -> Set[str]:
-    return {get_random_database_name() for _ in range(n)}
-
-
-@pytest.fixture(name="_bucket_initialize")
-def fixture_s3_bucket(_s3) -> None:  # type: ignore
-    _s3.create_bucket(Bucket=BUCKET_NAME)
+from tests.conftest import BUCKET_NAME, TABLE_METADATA_LOCATION_REGEX
 
 
 @mock_glue
 def test_create_table_with_database_location(
-    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
 ) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name, properties={"location": f"s3://{BUCKET_NAME}/{database_name}.db"})
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
 
 
 @mock_glue
 def test_create_table_with_default_warehouse(
-    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
 ) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}"})
     test_catalog.create_namespace(namespace=database_name)
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
 
 
 @mock_glue
 def test_create_table_with_given_location(
-    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
 ) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name)
     table = test_catalog.create_table(
         identifier=identifier, schema=table_schema_nested, location=f"s3://{BUCKET_NAME}/{database_name}.db/{table_name}"
     )
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
 
 
 @mock_glue
-def test_create_table_with_no_location(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_create_table_with_no_location(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name)
     with pytest.raises(ValueError):
         test_catalog.create_table(identifier=identifier, schema=table_schema_nested)
 
 
 @mock_glue
-def test_create_table_with_strips(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_create_table_with_strips(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name, properties={"location": f"s3://{BUCKET_NAME}/{database_name}.db/"})
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
-    identifier = (database_name, table_name)
-    test_catalog_strip = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}/")
-    test_catalog_strip.create_namespace(namespace=database_name)
-    table_strip = test_catalog_strip.create_table(identifier, table_schema_nested)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
+
+
+@mock_glue
+def test_create_table_with_strips_bucket_root(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
+    identifier = (database_name, table_name)
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
+    test_catalog.create_namespace(namespace=database_name)
+    table_strip = test_catalog.create_table(identifier, table_schema_nested)
     assert table_strip.identifier == identifier
-    assert table_metadata_location_regex.match(table_strip.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table_strip.metadata_location)
 
 
 @mock_glue
-def test_create_table_with_no_database(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_create_table_with_no_database(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     with pytest.raises(NoSuchNamespaceError):
         test_catalog.create_table(identifier=identifier, schema=table_schema_nested)
 
 
 @mock_glue
-def test_create_duplicated_table(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_create_duplicated_table(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     with pytest.raises(TableAlreadyExistsError):
         test_catalog.create_table(identifier, table_schema_nested)
 
 
 @mock_glue
-def test_load_table(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_load_table(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     table = test_catalog.load_table(identifier)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
 
 
 @mock_glue
-def test_load_non_exist_table(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_load_non_exist_table(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str, table_name: str) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
 
 
 @mock_glue
-def test_drop_table(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_drop_table(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     table = test_catalog.load_table(identifier)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
     test_catalog.drop_table(identifier)
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
 
 
 @mock_glue
-def test_drop_non_exist_table(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_drop_non_exist_table(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str, table_name: str) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     with pytest.raises(NoSuchTableError):
         test_catalog.drop_table(identifier)
 
 
 @mock_glue
-def test_rename_table(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
-    new_table_name = get_random_table_name()
+def test_rename_table(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
+    new_table_name = f"{table_name}_new"
     identifier = (database_name, table_name)
     new_identifier = (database_name, new_table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     table = test_catalog.create_table(identifier, table_schema_nested)
     assert table.identifier == identifier
-    assert table_metadata_location_regex.match(table.metadata_location)
+    assert TABLE_METADATA_LOCATION_REGEX.match(table.metadata_location)
     test_catalog.rename_table(identifier, new_identifier)
     new_table = test_catalog.load_table(new_identifier)
     assert new_table.identifier == new_identifier
     # the metadata_location should not change
     assert new_table.metadata_location == table.metadata_location
     # old table should be dropped
     with pytest.raises(NoSuchTableError):
         test_catalog.load_table(identifier)
 
 
 @mock_glue
-def test_rename_table_no_params(_glue, _bucket_initialize: None, _patch_aiobotocore: None) -> None:  # type: ignore
-    database_name = get_random_database_name()
-    new_database_name = get_random_database_name()
-    table_name = get_random_table_name()
-    new_table_name = get_random_table_name()
+def test_rename_table_no_params(_glue, _bucket_initialize: None, _patch_aiobotocore: None, database_name: str, table_name: str) -> None:  # type: ignore
+    new_database_name = f"{database_name}_new"
+    new_table_name = f"{table_name}_new"
     identifier = (database_name, table_name)
     new_identifier = (new_database_name, new_table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_namespace(namespace=new_database_name)
     _glue.create_table(
         DatabaseName=database_name,
         TableInput={"Name": table_name, "TableType": "EXTERNAL_TABLE", "Parameters": {"table_type": "iceberg"}},
     )
     with pytest.raises(NoSuchPropertyException):
         test_catalog.rename_table(identifier, new_identifier)
 
 
 @mock_glue
-def test_rename_non_iceberg_table(_glue, _bucket_initialize: None, _patch_aiobotocore: None) -> None:  # type: ignore
-    database_name = get_random_database_name()
-    new_database_name = get_random_database_name()
-    table_name = get_random_table_name()
-    new_table_name = get_random_table_name()
+def test_rename_non_iceberg_table(_glue, _bucket_initialize: None, _patch_aiobotocore: None, database_name: str, table_name: str) -> None:  # type: ignore
+    new_database_name = f"{database_name}_new"
+    new_table_name = f"{table_name}_new"
     identifier = (database_name, table_name)
     new_identifier = (new_database_name, new_table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_namespace(namespace=new_database_name)
     _glue.create_table(
         DatabaseName=database_name,
         TableInput={
             "Name": table_name,
             "TableType": "EXTERNAL_TABLE",
@@ -278,196 +232,212 @@
         },
     )
     with pytest.raises(NoSuchIcebergTableError):
         test_catalog.rename_table(identifier, new_identifier)
 
 
 @mock_glue
-def test_list_tables(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_list = get_random_tables(LIST_TEST_NUMBER)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+def test_list_tables(
+    _bucket_initialize: None,
+    _patch_aiobotocore: None,
+    table_schema_nested: Schema,
+    database_name: str,
+    table_name: str,
+    table_list: List[str],
+) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     for table_name in table_list:
         test_catalog.create_table((database_name, table_name), table_schema_nested)
     loaded_table_list = test_catalog.list_tables(database_name)
     for table_name in table_list:
         assert (database_name, table_name) in loaded_table_list
 
 
 @mock_glue
-def test_list_namespaces(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_list = get_random_databases(LIST_TEST_NUMBER)
-    test_catalog = GlueCatalog("glue")
+def test_list_namespaces(_bucket_initialize: None, _patch_aiobotocore: None, database_list: List[str]) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     for database_name in database_list:
         test_catalog.create_namespace(namespace=database_name)
     loaded_database_list = test_catalog.list_namespaces()
     for database_name in database_list:
         assert (database_name,) in loaded_database_list
 
 
 @mock_glue
-def test_create_namespace_no_properties(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_create_namespace_no_properties(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name)
     loaded_database_list = test_catalog.list_namespaces()
     assert len(loaded_database_list) == 1
     assert (database_name,) in loaded_database_list
     properties = test_catalog.load_namespace_properties(database_name)
     assert properties == {}
 
 
 @mock_glue
-def test_create_namespace_with_comment_and_location(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
+def test_create_namespace_with_comment_and_location(
+    _bucket_initialize: None, _patch_aiobotocore: None, database_name: str
+) -> None:
     test_location = f"s3://{BUCKET_NAME}/{database_name}.db"
     test_properties = {
         "comment": "this is a test description",
         "location": test_location,
     }
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name, properties=test_properties)
     loaded_database_list = test_catalog.list_namespaces()
     assert len(loaded_database_list) == 1
     assert (database_name,) in loaded_database_list
     properties = test_catalog.load_namespace_properties(database_name)
     assert properties["comment"] == "this is a test description"
     assert properties["location"] == test_location
 
 
 @mock_glue
-def test_create_duplicated_namespace(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_create_duplicated_namespace(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name)
     loaded_database_list = test_catalog.list_namespaces()
     assert len(loaded_database_list) == 1
     assert (database_name,) in loaded_database_list
     with pytest.raises(NamespaceAlreadyExistsError):
         test_catalog.create_namespace(namespace=database_name, properties={"test": "test"})
 
 
 @mock_glue
-def test_drop_namespace(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_drop_namespace(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(namespace=database_name)
     loaded_database_list = test_catalog.list_namespaces()
     assert len(loaded_database_list) == 1
     assert (database_name,) in loaded_database_list
     test_catalog.drop_namespace(database_name)
     loaded_database_list = test_catalog.list_namespaces()
     assert len(loaded_database_list) == 0
 
 
 @mock_glue
-def test_drop_non_empty_namespace(_bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema) -> None:
-    database_name = get_random_database_name()
-    table_name = get_random_table_name()
+def test_drop_non_empty_namespace(
+    _bucket_initialize: None, _patch_aiobotocore: None, table_schema_nested: Schema, database_name: str, table_name: str
+) -> None:
     identifier = (database_name, table_name)
-    test_catalog = GlueCatalog("glue", warehouse=f"s3://{BUCKET_NAME}")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO", "warehouse": f"s3://{BUCKET_NAME}/"})
     test_catalog.create_namespace(namespace=database_name)
     test_catalog.create_table(identifier, table_schema_nested)
     assert len(test_catalog.list_tables(database_name)) == 1
     with pytest.raises(NamespaceNotEmptyError):
         test_catalog.drop_namespace(database_name)
 
 
 @mock_glue
-def test_drop_non_exist_namespace(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_drop_non_exist_namespace(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     with pytest.raises(NoSuchNamespaceError):
         test_catalog.drop_namespace(database_name)
 
 
 @mock_glue
-def test_load_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
+def test_load_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
     test_location = f"s3://{BUCKET_NAME}/{database_name}.db"
     test_properties = {
         "comment": "this is a test description",
         "location": test_location,
         "test_property1": "1",
         "test_property2": "2",
         "test_property3": "3",
     }
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(database_name, test_properties)
     listed_properties = test_catalog.load_namespace_properties(database_name)
     for k, v in listed_properties.items():
         assert k in test_properties
         assert v == test_properties[k]
 
 
 @mock_glue
-def test_load_non_exist_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_load_non_exist_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     with pytest.raises(NoSuchNamespaceError):
         test_catalog.load_namespace_properties(database_name)
 
 
 @mock_glue
-def test_update_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
+def test_update_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
     test_properties = {
         "comment": "this is a test description",
         "location": f"s3://{BUCKET_NAME}/{database_name}.db",
         "test_property1": "1",
         "test_property2": "2",
         "test_property3": "3",
     }
     removals = {"test_property1", "test_property2", "test_property3", "should_not_removed"}
     updates = {"test_property4": "4", "test_property5": "5", "comment": "updated test description"}
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(database_name, test_properties)
     update_report = test_catalog.update_namespace_properties(database_name, removals, updates)
     for k in updates.keys():
         assert k in update_report.updated
     for k in removals:
         if k == "should_not_removed":
             assert k in update_report.missing
         else:
             assert k in update_report.removed
     assert "updated test description" == test_catalog.load_namespace_properties(database_name)["comment"]
     test_catalog.drop_namespace(database_name)
 
 
 @mock_glue
-def test_load_empty_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
-    test_catalog = GlueCatalog("glue")
+def test_load_empty_namespace_properties(_bucket_initialize: None, _patch_aiobotocore: None, database_name: str) -> None:
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(database_name)
     listed_properties = test_catalog.load_namespace_properties(database_name)
     assert listed_properties == {}
 
 
 @mock_glue
-def test_load_default_namespace_properties(_glue, _bucket_initialize, _patch_aiobotocore) -> None:  # type: ignore
-    database_name = get_random_database_name()
+def test_load_default_namespace_properties(_glue, _bucket_initialize, _patch_aiobotocore, database_name: str) -> None:  # type: ignore
     # simulate creating database with default settings through AWS Glue Web Console
     _glue.create_database(DatabaseInput={"Name": database_name})
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     listed_properties = test_catalog.load_namespace_properties(database_name)
     assert listed_properties == {}
 
 
 @mock_glue
-def test_update_namespace_properties_overlap_update_removal(_bucket_initialize: None, _patch_aiobotocore: None) -> None:
-    database_name = get_random_database_name()
+def test_update_namespace_properties_overlap_update_removal(
+    _bucket_initialize: None, _patch_aiobotocore: None, database_name: str
+) -> None:
     test_properties = {
         "comment": "this is a test description",
         "location": f"s3://{BUCKET_NAME}/{database_name}.db",
         "test_property1": "1",
         "test_property2": "2",
         "test_property3": "3",
     }
     removals = {"test_property1", "test_property2", "test_property3", "should_not_removed"}
     updates = {"test_property1": "4", "test_property5": "5", "comment": "updated test description"}
-    test_catalog = GlueCatalog("glue")
+    test_catalog = GlueCatalog("glue", **{"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"})
     test_catalog.create_namespace(database_name, test_properties)
     with pytest.raises(ValueError):
         test_catalog.update_namespace_properties(database_name, removals, updates)
     # should not modify the properties
     assert test_catalog.load_namespace_properties(database_name) == test_properties
+
+
+@mock_glue
+def test_passing_profile_name() -> None:
+    session_properties = {
+        "aws_secret_key_id": "abc",
+        "aws_secret_access_key": "def",
+        "aws_session_token": "ghi",
+        "region_name": "eu-central-1",
+        "profile_name": "sandbox",
+    }
+    test_properties = {"type": "glue"}
+    test_properties.update(session_properties)
+
+    with mock.patch("boto3.Session") as mock_session:
+        test_catalog = GlueCatalog("glue", **test_properties)
+
+    mock_session.assert_called_with(**session_properties)
+    assert test_catalog.glue is mock_session().client()
```

### Comparing `pyiceberg-0.3.0rc2/tests/catalog/test_hive.py` & `pyiceberg-0.4.0rc1/tests/catalog/test_hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 # pylint: disable=protected-access,redefined-outer-name
 import json
 import uuid
-from typing import Any, Dict
 from unittest.mock import MagicMock, patch
 
 import pytest
 from hive_metastore.ttypes import AlreadyExistsException
 from hive_metastore.ttypes import Database as HiveDatabase
 from hive_metastore.ttypes import (
     FieldSchema,
@@ -38,18 +37,16 @@
 from pyiceberg.catalog.hive import HiveCatalog, _construct_hive_storage_descriptor
 from pyiceberg.exceptions import (
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchNamespaceError,
     NoSuchTableError,
 )
-from pyiceberg.io.pyarrow import PyArrowFileIO
 from pyiceberg.partitioning import PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.serializers import ToOutputFile
 from pyiceberg.table.metadata import TableMetadataUtil, TableMetadataV2
 from pyiceberg.table.refs import SnapshotRef, SnapshotRefType
 from pyiceberg.table.snapshots import (
     MetadataLogEntry,
     Operation,
     Snapshot,
     SnapshotLogEntry,
@@ -71,20 +68,15 @@
 )
 
 HIVE_CATALOG_NAME = "hive"
 HIVE_METASTORE_FAKE_URL = "thrift://unknown:9083"
 
 
 @pytest.fixture
-def hive_table(tmp_path_factory: pytest.TempPathFactory, example_table_metadata_v2: Dict[str, Any]) -> HiveTable:
-    metadata_path = str(tmp_path_factory.mktemp("metadata") / f"{uuid.uuid4()}.metadata.json")
-    metadata = TableMetadataV2(**example_table_metadata_v2)
-
-    ToOutputFile.table_metadata(metadata, PyArrowFileIO().new_output(location=str(metadata_path)), True)
-
+def hive_table(metadata_location: str) -> HiveTable:
     return HiveTable(
         tableName="new_tabl2e",
         dbName="default",
         owner="fokkodriesprong",
         createTime=1659092339,
         lastAccessTime=1659092,
         retention=0,
@@ -115,15 +107,15 @@
             storedAsSubDirectories=False,
         ),
         partitionKeys=[],
         parameters={
             "EXTERNAL": "TRUE",
             "transient_lastDdlTime": "1659092339",
             "table_type": "ICEBERG",
-            "metadata_location": metadata_path,
+            "metadata_location": metadata_location,
         },
         viewOriginalText=None,
         viewExpandedText=None,
         tableType="EXTERNAL_TABLE",
         privileges=None,
         temporary=False,
         rewriteEnabled=False,
@@ -700,8 +692,8 @@
     # Set this one to None, so we'll fall back to the properties
     hive_database.locationUri = None
 
     catalog._client = MagicMock()
     catalog._client.__enter__().get_database.return_value = hive_database
 
     location = catalog._resolve_table_location(None, "database", "table")
-    assert location == "/tmp/warehouse/database/table"
+    assert location == "/tmp/warehouse/database.db/table"
```

### Comparing `pyiceberg-0.3.0rc2/tests/catalog/test_rest.py` & `pyiceberg-0.4.0rc1/tests/catalog/test_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
             "expires_in": 86400,
             "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
         },
         status_code=200,
         request_headers=OAUTH_TEST_HEADERS,
     )
     assert (
-        RestCatalog("rest", uri=TEST_URI, credential=TEST_CREDENTIALS).session.headers["Authorization"] == f"Bearer {TEST_TOKEN}"
+        RestCatalog("rest", uri=TEST_URI, credential=TEST_CREDENTIALS)._session.headers["Authorization"]  # pylint: disable=W0212
+        == f"Bearer {TEST_TOKEN}"
     )
 
 
 def test_config_200(requests_mock: Mocker) -> None:
     requests_mock.get(
         f"{TEST_URI}v1/config",
         json={"defaults": {}, "overrides": {}},
@@ -157,14 +158,29 @@
         status_code=200,
         request_headers=TEST_HEADERS,
     )
 
     assert RestCatalog("rest", uri=TEST_URI, token=TEST_TOKEN).list_tables(namespace) == [("examples", "fooshare")]
 
 
+def test_list_tables_200_sigv4(rest_mock: Mocker) -> None:
+    namespace = "examples"
+    rest_mock.get(
+        f"{TEST_URI}v1/namespaces/{namespace}/tables",
+        json={"identifiers": [{"namespace": ["examples"], "name": "fooshare"}]},
+        status_code=200,
+        request_headers=TEST_HEADERS,
+    )
+
+    assert RestCatalog("rest", **{"uri": TEST_URI, "token": TEST_TOKEN, "rest.sigv4-enabled": "true"}).list_tables(namespace) == [
+        ("examples", "fooshare")
+    ]
+    assert rest_mock.called
+
+
 def test_list_tables_404(rest_mock: Mocker) -> None:
     namespace = "examples"
     rest_mock.get(
         f"{TEST_URI}v1/namespaces/{namespace}/tables",
         json={
             "error": {
                 "message": "Namespace does not exist: personal in warehouse 8bcb0838-50fc-472d-9ddb-8feb89ef5f1e",
@@ -388,15 +404,16 @@
                 ],
             },
             "config": {"client.factory": "io.tabular.iceberg.catalog.TabularAwsClientFactory", "region": "us-west-2"},
         },
         status_code=200,
         request_headers=TEST_HEADERS,
     )
-    actual = RestCatalog("rest", uri=TEST_URI, token=TEST_TOKEN).load_table(("fokko", "table"))
+    catalog = RestCatalog("rest", uri=TEST_URI, token=TEST_TOKEN)
+    actual = catalog.load_table(("fokko", "table"))
     expected = Table(
         identifier=("rest", "fokko", "table"),
         metadata_location="s3://warehouse/database/table/metadata/00001-5f2f8166-244c-4eae-ac36-384ecdec81fc.gz.metadata.json",
         metadata=TableMetadataV1(
             location="s3://warehouse/database/table",
             table_uuid=UUID("b55d9dda-6561-423a-8bfc-787980ce421f"),
             last_updated_ms=1646787054459,
@@ -464,14 +481,15 @@
                 NestedField(field_id=2, name="data", field_type=StringType(), required=False),
                 schema_id=0,
                 identifier_field_ids=[],
             ),
             partition_spec=[],
         ),
         io=load_file_io(),
+        catalog=catalog,
     )
     assert actual == expected
 
 
 def test_load_table_404(rest_mock: Mocker) -> None:
     rest_mock.get(
         f"{TEST_URI}v1/namespaces/fokko/tables/does_not_exists",
@@ -565,15 +583,16 @@
                 "client.factory": "io.tabular.iceberg.catalog.TabularAwsClientFactory",
                 "region": "us-west-2",
             },
         },
         status_code=200,
         request_headers=TEST_HEADERS,
     )
-    table = RestCatalog("rest", uri=TEST_URI, token=TEST_TOKEN).create_table(
+    catalog = RestCatalog("rest", uri=TEST_URI, token=TEST_TOKEN)
+    table = catalog.create_table(
         identifier=("fokko", "fokko2"),
         schema=table_schema_simple,
         location=None,
         partition_spec=PartitionSpec(
             PartitionField(source_id=1, field_id=1000, transform=TruncateTransform(width=3), name="id"), spec_id=1
         ),
         sort_order=SortOrder(SortField(source_id=2, transform=IdentityTransform())),
@@ -619,14 +638,15 @@
                 NestedField(field_id=3, name="baz", field_type=BooleanType(), required=False),
                 schema_id=0,
                 identifier_field_ids=[2],
             ),
             partition_spec=[],
         ),
         io=load_file_io(),
+        catalog=catalog,
     )
 
 
 def test_create_table_409(rest_mock: Mocker, table_schema_simple: Schema) -> None:
     rest_mock.post(
         f"{TEST_URI}v1/namespaces/fokko/tables",
         json={
```

### Comparing `pyiceberg-0.3.0rc2/tests/cli/test_console.py` & `pyiceberg-0.4.0rc1/tests/cli/test_console.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,25 +22,87 @@
     Union,
 )
 from unittest import mock
 
 from click.testing import CliRunner
 
 from pyiceberg.catalog import Catalog, PropertiesUpdateSummary
+from pyiceberg.catalog.noop import NoopCatalog
 from pyiceberg.cli.console import run
 from pyiceberg.exceptions import NoSuchNamespaceError, NoSuchTableError
 from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.table import Table
+from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table
 from pyiceberg.table.metadata import TableMetadataV2
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 from pyiceberg.utils.config import Config
-from tests.conftest import EXAMPLE_TABLE_METADATA_V2
+
+EXAMPLE_TABLE_METADATA_V2 = {
+    "format-version": 2,
+    "table-uuid": "9c12d441-03fe-4693-9a96-a0705ddf69c1",
+    "location": "s3://bucket/test/location",
+    "last-sequence-number": 34,
+    "last-updated-ms": 1602638573590,
+    "last-column-id": 3,
+    "current-schema-id": 1,
+    "schemas": [
+        {"type": "struct", "schema-id": 0, "fields": [{"id": 1, "name": "x", "required": True, "type": "long"}]},
+        {
+            "type": "struct",
+            "schema-id": 1,
+            "identifier-field-ids": [1, 2],
+            "fields": [
+                {"id": 1, "name": "x", "required": True, "type": "long"},
+                {"id": 2, "name": "y", "required": True, "type": "long", "doc": "comment"},
+                {"id": 3, "name": "z", "required": True, "type": "long"},
+            ],
+        },
+    ],
+    "default-spec-id": 0,
+    "partition-specs": [{"spec-id": 0, "fields": [{"name": "x", "transform": "identity", "source-id": 1, "field-id": 1000}]}],
+    "last-partition-id": 1000,
+    "default-sort-order-id": 3,
+    "sort-orders": [
+        {
+            "order-id": 3,
+            "fields": [
+                {"transform": "identity", "source-id": 2, "direction": "asc", "null-order": "nulls-first"},
+                {"transform": "bucket[4]", "source-id": 3, "direction": "desc", "null-order": "nulls-last"},
+            ],
+        }
+    ],
+    "properties": {"read.split.target.size": 134217728},
+    "current-snapshot-id": 3055729675574597004,
+    "snapshots": [
+        {
+            "snapshot-id": 3051729675574597004,
+            "timestamp-ms": 1515100955770,
+            "sequence-number": 0,
+            "summary": {"operation": "append"},
+            "manifest-list": "s3://a/b/1.avro",
+        },
+        {
+            "snapshot-id": 3055729675574597004,
+            "parent-snapshot-id": 3051729675574597004,
+            "timestamp-ms": 1555100955770,
+            "sequence-number": 1,
+            "summary": {"operation": "append"},
+            "manifest-list": "s3://a/b/2.avro",
+            "schema-id": 1,
+        },
+    ],
+    "snapshot-log": [
+        {"snapshot-id": 3051729675574597004, "timestamp-ms": 1515100955770},
+        {"snapshot-id": 3055729675574597004, "timestamp-ms": 1555100955770},
+    ],
+    "metadata-log": [{"metadata-file": "s3://bucket/.../v1.json", "timestamp-ms": 1515100}],
+    "refs": {"test": {"snapshot-id": 3051729675574597004, "type": "tag", "max-ref-age-ms": 10000000}},
+}
 
 
 class MockCatalog(Catalog):
     def create_table(
         self,
         identifier: Union[str, Identifier],
         schema: Schema,
@@ -50,24 +112,29 @@
         properties: Properties = EMPTY_DICT,
     ) -> Table:
         return Table(
             identifier=Catalog.identifier_to_tuple(identifier),
             metadata_location="s3://tmp/",
             metadata=TableMetadataV2(**EXAMPLE_TABLE_METADATA_V2),
             io=load_file_io(),
+            catalog=self,
         )
 
+    def _commit_table(self, table_request: CommitTableRequest) -> CommitTableResponse:
+        raise NotImplementedError
+
     def load_table(self, identifier: Union[str, Identifier]) -> Table:
         tuple_identifier = Catalog.identifier_to_tuple(identifier)
         if tuple_identifier == ("default", "foo"):
             return Table(
                 identifier=tuple_identifier,
                 metadata_location="s3://tmp/",
                 metadata=TableMetadataV2(**EXAMPLE_TABLE_METADATA_V2),
                 io=load_file_io(),
+                catalog=NoopCatalog("NoopCatalog"),
             )
         else:
             raise NoSuchTableError(f"Table does not exist: {'.'.join(tuple_identifier)}")
 
     def drop_table(self, identifier: Union[str, Identifier]) -> None:
         tuple_identifier = Catalog.identifier_to_tuple(identifier)
         if tuple_identifier == ("default", "foo"):
@@ -82,14 +149,15 @@
         tuple_identifier = Catalog.identifier_to_tuple(from_identifier)
         if tuple_identifier == ("default", "foo"):
             return Table(
                 identifier=tuple_identifier,
                 metadata_location="s3://tmp/",
                 metadata=TableMetadataV2(**EXAMPLE_TABLE_METADATA_V2),
                 io=load_file_io(),
+                catalog=NoopCatalog("NoopCatalog"),
             )
         else:
             raise NoSuchTableError(f"Table does not exist: {from_identifier}")
 
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         return None
 
@@ -132,15 +200,14 @@
 
 
 MOCK_CATALOG = MockCatalog("production", uri="http://somewhere")
 MOCK_ENVIRONMENT = {"PYICEBERG_CATALOG__PRODUCTION__URI": "test://doesnotexist"}
 
 
 def test_missing_uri(empty_home_dir_path: str) -> None:
-
     # mock to prevent parsing ~/.pyiceberg.yaml or {PYICEBERG_HOME}/.pyiceberg.yaml
     with mock.patch.dict(os.environ, {"HOME": empty_home_dir_path, "PYICEBERG_HOME": empty_home_dir_path}):
         with mock.patch("pyiceberg.catalog._ENV_CONFIG", Config()):
             runner = CliRunner()
             result = runner.invoke(run, ["list"])
             assert result.exit_code == 1
             assert (
```

### Comparing `pyiceberg-0.3.0rc2/tests/cli/test_output.py` & `pyiceberg-0.4.0rc1/tests/cli/test_output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/conftest.py` & `pyiceberg-0.4.0rc1/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,55 +21,73 @@
 to any pytest function.
 
 In the case where the fixture must be used in a pytest.mark.parametrize decorator, the string representation can be used
 and the built-in pytest fixture request should be used as an additional argument in the function. The fixture can then be
 retrieved using `request.getfixturevalue(fixture_name)`.
 """
 import os
+import re
+import string
+import uuid
+from random import choice
 from tempfile import TemporaryDirectory
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
+    List,
+    Optional,
 )
 from unittest.mock import MagicMock
 from urllib.parse import urlparse
 
 import aiobotocore.awsrequest
 import aiobotocore.endpoint
 import aiohttp
 import aiohttp.client_reqrep
 import aiohttp.typedefs
 import boto3
 import botocore.awsrequest
 import botocore.model
+import pyarrow as pa
 import pytest
-from moto import mock_glue, mock_s3
+from moto import mock_dynamodb, mock_glue, mock_s3
+from pyarrow import parquet as pq
 
 from pyiceberg import schema
+from pyiceberg.catalog import Catalog
 from pyiceberg.io import OutputFile, OutputStream, fsspec
 from pyiceberg.io.fsspec import FsspecFileIO
 from pyiceberg.io.pyarrow import PyArrowFile, PyArrowFileIO
+from pyiceberg.manifest import DataFile, FileFormat
 from pyiceberg.schema import Schema
+from pyiceberg.serializers import ToOutputFile
+from pyiceberg.table import FileScanTask
+from pyiceberg.table.metadata import TableMetadataV2
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DoubleType,
     FloatType,
     IntegerType,
     ListType,
     LongType,
     MapType,
     NestedField,
     StringType,
     StructType,
 )
-from tests.catalog.test_base import InMemoryCatalog
+
+
+def pytest_collection_modifyitems(items: List[pytest.Item]) -> None:
+    for item in items:
+        if not any(item.iter_markers()):
+            item.add_marker("unmarked")
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     # S3 options
     parser.addoption(
         "--s3.endpoint", action="store", default="http://localhost:9000", help="The S3 endpoint URL for tests marked as s3"
     )
@@ -306,17 +324,20 @@
 
 
 @pytest.fixture
 def example_table_metadata_v2() -> Dict[str, Any]:
     return EXAMPLE_TABLE_METADATA_V2
 
 
-@pytest.fixture
-def catalog() -> InMemoryCatalog:
-    return InMemoryCatalog("test.in.memory.catalog", **{"test.key": "test.value"})
+@pytest.fixture(scope="session")
+def metadata_location(tmp_path_factory: pytest.TempPathFactory) -> str:
+    metadata_location = str(tmp_path_factory.mktemp("metadata") / f"{uuid.uuid4()}.metadata.json")
+    metadata = TableMetadataV2(**EXAMPLE_TABLE_METADATA_V2)
+    ToOutputFile.table_metadata(metadata, PyArrowFileIO().new_output(location=metadata_location), overwrite=True)
+    return metadata_location
 
 
 manifest_entry_records = [
     {
         "status": 1,
         "snapshot_id": 8744736658442914487,
         "data_file": {
@@ -564,15 +585,15 @@
             "key_metadata": None,
             "split_offsets": [4],
             "sort_order_id": 0,
         },
     },
 ]
 
-manifest_file_records = [
+manifest_file_records_v1 = [
     {
         "manifest_path": "/home/iceberg/warehouse/nyc/taxis_partitioned/metadata/0125c686-8aa6-4502-bdcc-b6d17ca41a3b-m0.avro",
         "manifest_length": 7989,
         "partition_spec_id": 0,
         "added_snapshot_id": 9182715666859759686,
         "added_data_files_count": 3,
         "existing_data_files_count": 0,
@@ -582,17 +603,39 @@
         ],
         "added_rows_count": 237993,
         "existing_rows_count": 0,
         "deleted_rows_count": 0,
     }
 ]
 
+manifest_file_records_v2 = [
+    {
+        "manifest_path": "/home/iceberg/warehouse/nyc/taxis_partitioned/metadata/0125c686-8aa6-4502-bdcc-b6d17ca41a3b-m0.avro",
+        "manifest_length": 7989,
+        "partition_spec_id": 0,
+        "content": 1,
+        "sequence_number": 3,
+        "min_sequence_number": 3,
+        "added_snapshot_id": 9182715666859759686,
+        "added_files_count": 3,
+        "existing_files_count": 0,
+        "deleted_files_count": 0,
+        "added_rows_count": 237993,
+        "existing_rows_count": 0,
+        "deleted_rows_count": 0,
+        "partitions": [
+            {"contains_null": True, "contains_nan": False, "lower_bound": b"\x01\x00\x00\x00", "upper_bound": b"\x02\x00\x00\x00"}
+        ],
+        "key_metadata": b"\x19\x25",
+    }
+]
+
 
 @pytest.fixture(scope="session")
-def avro_schema_manifest_file() -> Dict[str, Any]:
+def avro_schema_manifest_file_v1() -> Dict[str, Any]:
     return {
         "type": "record",
         "name": "manifest_file",
         "fields": [
             {"name": "manifest_path", "type": "string", "doc": "Location URI with FS scheme", "field-id": 500},
             {"name": "manifest_length", "type": "long", "doc": "Total file size in bytes", "field-id": 501},
             {"name": "partition_spec_id", "type": "int", "doc": "Spec ID used to write", "field-id": 502},
@@ -686,14 +729,93 @@
                 "field-id": 514,
             },
         ],
     }
 
 
 @pytest.fixture(scope="session")
+def avro_schema_manifest_file_v2() -> Dict[str, Any]:
+    return {
+        "type": "record",
+        "name": "manifest_file",
+        "fields": [
+            {"name": "manifest_path", "type": "string", "doc": "Location URI with FS scheme", "field-id": 500},
+            {"name": "manifest_length", "type": "long", "doc": "Total file size in bytes", "field-id": 501},
+            {"name": "partition_spec_id", "type": "int", "doc": "Spec ID used to write", "field-id": 502},
+            {"name": "content", "type": "int", "doc": "Contents of the manifest: 0=data, 1=deletes", "field-id": 517},
+            {
+                "name": "sequence_number",
+                "type": ["null", "long"],
+                "doc": "Sequence number when the manifest was added",
+                "field-id": 515,
+            },
+            {
+                "name": "min_sequence_number",
+                "type": ["null", "long"],
+                "doc": "Lowest sequence number in the manifest",
+                "field-id": 516,
+            },
+            {"name": "added_snapshot_id", "type": "long", "doc": "Snapshot ID that added the manifest", "field-id": 503},
+            {"name": "added_files_count", "type": "int", "doc": "Added entry count", "field-id": 504},
+            {"name": "existing_files_count", "type": "int", "doc": "Existing entry count", "field-id": 505},
+            {"name": "deleted_files_count", "type": "int", "doc": "Deleted entry count", "field-id": 506},
+            {"name": "added_rows_count", "type": "long", "doc": "Added rows count", "field-id": 512},
+            {"name": "existing_rows_count", "type": "long", "doc": "Existing rows count", "field-id": 513},
+            {"name": "deleted_rows_count", "type": "long", "doc": "Deleted rows count", "field-id": 514},
+            {
+                "name": "partitions",
+                "type": [
+                    "null",
+                    {
+                        "type": "array",
+                        "items": {
+                            "type": "record",
+                            "name": "r508",
+                            "fields": [
+                                {
+                                    "name": "contains_null",
+                                    "type": "boolean",
+                                    "doc": "True if any file has a null partition value",
+                                    "field-id": 509,
+                                },
+                                {
+                                    "name": "contains_nan",
+                                    "type": ["null", "boolean"],
+                                    "doc": "True if any file has a nan partition value",
+                                    "default": None,
+                                    "field-id": 518,
+                                },
+                                {
+                                    "name": "lower_bound",
+                                    "type": ["null", "bytes"],
+                                    "doc": "Partition lower bound for all files",
+                                    "default": None,
+                                    "field-id": 510,
+                                },
+                                {
+                                    "name": "upper_bound",
+                                    "type": ["null", "bytes"],
+                                    "doc": "Partition upper bound for all files",
+                                    "default": None,
+                                    "field-id": 511,
+                                },
+                            ],
+                        },
+                        "element-id": 508,
+                    },
+                ],
+                "doc": "Summary for each partition",
+                "default": None,
+                "field-id": 507,
+            },
+        ],
+    }
+
+
+@pytest.fixture(scope="session")
 def avro_schema_manifest_entry() -> Dict[str, Any]:
     return {
         "type": "record",
         "name": "manifest_entry",
         "fields": [
             {"name": "status", "type": "int", "field-id": 0},
             {"name": "snapshot_id", "type": ["null", "long"], "default": None, "field-id": 1},
@@ -900,27 +1022,30 @@
 
 @pytest.fixture(scope="session")
 def simple_map() -> MapType:
     return MapType(key_id=19, key_type=StringType(), value_id=25, value_type=DoubleType(), value_required=False)
 
 
 class LocalOutputFile(OutputFile):
-    """An OutputFile implementation for local files (for test use only)"""
+    """An OutputFile implementation for local files (for test use only)."""
 
     def __init__(self, location: str) -> None:
         parsed_location = urlparse(location)  # Create a ParseResult from the uri
-        if parsed_location.scheme and parsed_location.scheme != "file":  # Validate that a uri is provided with a scheme of `file`
+        if (
+            parsed_location.scheme and parsed_location.scheme != "file"
+        ):  # Validate that an uri is provided with a scheme of `file`
             raise ValueError("LocalOutputFile location must have a scheme of `file`")
         elif parsed_location.netloc:
             raise ValueError(f"Network location is not allowed for LocalOutputFile: {parsed_location.netloc}")
 
         super().__init__(location=location)
         self._path = parsed_location.path
 
     def __len__(self) -> int:
+        """Returns the length of an instance of the LocalOutputFile class."""
         return os.path.getsize(self._path)
 
     def exists(self) -> bool:
         return os.path.exists(self._path)
 
     def to_input_file(self) -> PyArrowFile:
         return PyArrowFileIO().new_input(location=self.location)
@@ -942,28 +1067,46 @@
         tmp_avro_file = tmpdir + "/manifest.avro"
         with open(tmp_avro_file, "wb") as out:
             writer(out, parsed_schema, manifest_entry_records)
         yield tmp_avro_file
 
 
 @pytest.fixture(scope="session")
-def generated_manifest_file_file(
-    avro_schema_manifest_file: Dict[str, Any], generated_manifest_entry_file: str
+def generated_manifest_file_file_v1(
+    avro_schema_manifest_file_v1: Dict[str, Any], generated_manifest_entry_file: str
+) -> Generator[str, None, None]:
+    from fastavro import parse_schema, writer
+
+    parsed_schema = parse_schema(avro_schema_manifest_file_v1)
+
+    # Make sure that a valid manifest_path is set
+    manifest_file_records_v1[0]["manifest_path"] = generated_manifest_entry_file
+
+    with TemporaryDirectory() as tmpdir:
+        tmp_avro_file = tmpdir + "/manifest.avro"
+        with open(tmp_avro_file, "wb") as out:
+            writer(out, parsed_schema, manifest_file_records_v1)
+        yield tmp_avro_file
+
+
+@pytest.fixture(scope="session")
+def generated_manifest_file_file_v2(
+    avro_schema_manifest_file_v2: Dict[str, Any], generated_manifest_entry_file: str
 ) -> Generator[str, None, None]:
     from fastavro import parse_schema, writer
 
-    parsed_schema = parse_schema(avro_schema_manifest_file)
+    parsed_schema = parse_schema(avro_schema_manifest_file_v2)
 
     # Make sure that a valid manifest_path is set
-    manifest_file_records[0]["manifest_path"] = generated_manifest_entry_file
+    manifest_file_records_v2[0]["manifest_path"] = generated_manifest_entry_file
 
     with TemporaryDirectory() as tmpdir:
         tmp_avro_file = tmpdir + "/manifest.avro"
         with open(tmp_avro_file, "wb") as out:
-            writer(out, parsed_schema, manifest_file_records)
+            writer(out, parsed_schema, manifest_file_records_v2)
         yield tmp_avro_file
 
 
 @pytest.fixture(scope="session")
 def iceberg_manifest_entry_schema() -> Schema:
     return Schema(
         NestedField(field_id=0, name="status", field_type=IntegerType(), required=True),
@@ -1143,17 +1286,17 @@
         "s3.access-key-id": request.config.getoption("--s3.access-key-id"),
         "s3.secret-access-key": request.config.getoption("--s3.secret-access-key"),
     }
     return fsspec.FsspecFileIO(properties=properties)
 
 
 class MockAWSResponse(aiobotocore.awsrequest.AioAWSResponse):
-    """
-    A mocked aws response implementation (for test use only)
-    See https://github.com/aio-libs/aiobotocore/issues/755
+    """A mocked aws response implementation (for test use only).
+
+    See https://github.com/aio-libs/aiobotocore/issues/755.
     """
 
     def __init__(self, response: botocore.awsrequest.AWSResponse) -> None:
         self._moto_response = response
         self.status_code = response.status_code
         self.raw = MockHttpClientResponse(response)
 
@@ -1162,17 +1305,17 @@
         return self._moto_response.content
 
     async def _text_prop(self) -> str:
         return self._moto_response.text
 
 
 class MockHttpClientResponse(aiohttp.client_reqrep.ClientResponse):
-    """
-    A mocked http client response implementation (for test use only)
-    See https://github.com/aio-libs/aiobotocore/issues/755
+    """A mocked http client response implementation (for test use only).
+
+    See https://github.com/aio-libs/aiobotocore/issues/755.
     """
 
     def __init__(self, response: botocore.awsrequest.AWSResponse) -> None:
         async def read(*_: Any) -> bytes:
             # streaming/range requests. used by s3fs
             return response.content
 
@@ -1183,17 +1326,17 @@
     @property
     def raw_headers(self) -> aiohttp.typedefs.RawHeaders:
         # Return the headers encoded the way that aiobotocore expects them
         return {k.encode("utf-8"): str(v).encode("utf-8") for k, v in self.response.headers.items()}.items()
 
 
 def patch_aiobotocore() -> None:
-    """
-    Patch aiobotocore to work with moto
-    See https://github.com/aio-libs/aiobotocore/issues/755
+    """Patch aiobotocore to work with moto.
+
+    See https://github.com/aio-libs/aiobotocore/issues/755.
     """
 
     def factory(original: Callable) -> Callable:  # type: ignore
         def patched_convert_to_response_dict(  # type: ignore
             http_response: botocore.awsrequest.AWSResponse, operation_model: botocore.model.OperationModel
         ):
             return original(MockAWSResponse(http_response), operation_model)
@@ -1201,17 +1344,17 @@
         return patched_convert_to_response_dict
 
     aiobotocore.endpoint.convert_to_response_dict = factory(aiobotocore.endpoint.convert_to_response_dict)
 
 
 @pytest.fixture(name="_patch_aiobotocore")
 def fixture_aiobotocore():  # type: ignore
-    """
-    Patch aiobotocore to work with moto
-    pending close of this issue: https://github.com/aio-libs/aiobotocore/issues/755
+    """Patch aiobotocore to work with moto.
+
+    pending close of this issue: https://github.com/aio-libs/aiobotocore/issues/755.
     """
     stored_method = aiobotocore.endpoint.convert_to_response_dict
     yield patch_aiobotocore()
     # restore the changed method after the fixture is destroyed
     aiobotocore.endpoint.convert_to_response_dict = stored_method
 
 
@@ -1232,42 +1375,143 @@
     os.environ.pop("AWS_SECURITY_TOKEN")
     os.environ.pop("AWS_SESSION_TOKEN")
     os.environ.pop("AWS_DEFAULT_REGION")
 
 
 @pytest.fixture(name="_s3")
 def fixture_s3(_aws_credentials: None) -> Generator[boto3.client, None, None]:
-    """Mocked S3 client"""
+    """Mocked S3 client."""
     with mock_s3():
         yield boto3.client("s3", region_name="us-east-1")
 
 
 @pytest.fixture(name="_glue")
 def fixture_glue(_aws_credentials: None) -> Generator[boto3.client, None, None]:
-    """Mocked glue client"""
+    """Mocked glue client."""
     with mock_glue():
         yield boto3.client("glue", region_name="us-east-1")
 
 
+@pytest.fixture(name="_dynamodb")
+def fixture_dynamodb(_aws_credentials: None) -> Generator[boto3.client, None, None]:
+    """Mocked DynamoDB client."""
+    with mock_dynamodb():
+        yield boto3.client("dynamodb", region_name="us-east-1")
+
+
 @pytest.fixture
 def adlfs_fsspec_fileio(request: pytest.FixtureRequest) -> Generator[FsspecFileIO, None, None]:
     from azure.storage.blob import BlobServiceClient
 
     azurite_url = request.config.getoption("--adlfs.endpoint")
     azurite_account_name = request.config.getoption("--adlfs.account-name")
     azurite_account_key = request.config.getoption("--adlfs.account-key")
     azurite_connection_string = f"DefaultEndpointsProtocol=http;AccountName={azurite_account_name};AccountKey={azurite_account_key};BlobEndpoint={azurite_url}/{azurite_account_name};"
     properties = {
-        "connection_string": azurite_connection_string,
-        "account_name": azurite_account_name,
+        "adlfs.connection-string": azurite_connection_string,
+        "adlfs.account-name": azurite_account_name,
     }
 
     bbs = BlobServiceClient.from_connection_string(conn_str=azurite_connection_string)
     bbs.create_container("tests")
     yield fsspec.FsspecFileIO(properties=properties)
     bbs.delete_container("tests")
 
 
 @pytest.fixture(scope="session")
 def empty_home_dir_path(tmp_path_factory: pytest.TempPathFactory) -> str:
     home_path = str(tmp_path_factory.mktemp("home"))
     return home_path
+
+
+RANDOM_LENGTH = 20
+NUM_TABLES = 2
+
+
+@pytest.fixture()
+def table_name() -> str:
+    prefix = "my_iceberg_table-"
+    random_tag = "".join(choice(string.ascii_letters) for _ in range(RANDOM_LENGTH))
+    return (prefix + random_tag).lower()
+
+
+@pytest.fixture()
+def table_list(table_name: str) -> List[str]:
+    return [f"{table_name}_{idx}" for idx in range(NUM_TABLES)]
+
+
+@pytest.fixture()
+def database_name() -> str:
+    prefix = "my_iceberg_database-"
+    random_tag = "".join(choice(string.ascii_letters) for _ in range(RANDOM_LENGTH))
+    return (prefix + random_tag).lower()
+
+
+@pytest.fixture()
+def database_list(database_name: str) -> List[str]:
+    return [f"{database_name}_{idx}" for idx in range(NUM_TABLES)]
+
+
+BUCKET_NAME = "test_bucket"
+TABLE_METADATA_LOCATION_REGEX = re.compile(
+    r"""s3://test_bucket/my_iceberg_database-[a-z]{20}.db/
+    my_iceberg_table-[a-z]{20}/metadata/
+    00000-[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}.metadata.json""",
+    re.X,
+)
+
+
+@pytest.fixture(name="_bucket_initialize")
+def fixture_s3_bucket(_s3) -> None:  # type: ignore
+    _s3.create_bucket(Bucket=BUCKET_NAME)
+
+
+def get_bucket_name() -> str:
+    """Set the environment variable AWS_TEST_BUCKET for a default bucket to test."""
+    bucket_name = os.getenv("AWS_TEST_BUCKET")
+    if bucket_name is None:
+        raise ValueError("Please specify a bucket to run the test by setting environment variable AWS_TEST_BUCKET")
+    return bucket_name
+
+
+def get_s3_path(bucket_name: str, database_name: Optional[str] = None, table_name: Optional[str] = None) -> str:
+    result_path = f"s3://{bucket_name}"
+    if database_name is not None:
+        result_path += f"/{database_name}.db"
+
+    if table_name is not None:
+        result_path += f"/{table_name}"
+    return result_path
+
+
+@pytest.fixture(name="s3", scope="module")
+def fixture_s3_client() -> boto3.client:
+    yield boto3.client("s3")
+
+
+def clean_up(test_catalog: Catalog) -> None:
+    """Clean all databases and tables created during the integration test."""
+    for database_tuple in test_catalog.list_namespaces():
+        database_name = database_tuple[0]
+        if "my_iceberg_database-" in database_name:
+            for identifier in test_catalog.list_tables(database_name):
+                test_catalog.purge_table(identifier)
+            test_catalog.drop_namespace(database_name)
+
+
+@pytest.fixture
+def data_file(table_schema_simple: Schema, tmp_path: str) -> str:
+    table = pa.table(
+        {"foo": ["a", "b", "c"], "bar": [1, 2, 3], "baz": [True, False, None]},
+        metadata={"iceberg.schema": table_schema_simple.json()},
+    )
+
+    file_path = f"{tmp_path}/0000-data.parquet"
+    pq.write_table(table=table, where=file_path)
+    return file_path
+
+
+@pytest.fixture
+def example_task(data_file: str) -> FileScanTask:
+    return FileScanTask(
+        data_file=DataFile(file_path=data_file, file_format=FileFormat.PARQUET, file_size_in_bytes=1925),
+    )
```

### Comparing `pyiceberg-0.3.0rc2/tests/expressions/test_expressions.py` & `pyiceberg-0.4.0rc1/tests/expressions/test_expressions.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # pylint:disable=redefined-outer-name,eval-used
 
+import pickle
 import uuid
 from decimal import Decimal
 from typing import Any
 
 import pytest
 from typing_extensions import assert_type
 
@@ -675,62 +676,69 @@
 
 
 def test_bound_reference(field: NestedField, accessor: Accessor) -> None:
     bound_ref = BoundReference(field=field, accessor=accessor)
     assert str(bound_ref) == f"BoundReference(field={repr(field)}, accessor={repr(accessor)})"
     assert repr(bound_ref) == f"BoundReference(field={repr(field)}, accessor={repr(accessor)})"
     assert bound_ref == eval(repr(bound_ref))
+    assert bound_ref == pickle.loads(pickle.dumps(bound_ref))
 
 
 def test_reference() -> None:
     abc = "abc"
     ref = Reference(abc)
     assert str(ref) == "Reference(name='abc')"
     assert repr(ref) == "Reference(name='abc')"
     assert ref == eval(repr(ref))
+    assert ref == pickle.loads(pickle.dumps(ref))
 
 
 def test_and() -> None:
     null = IsNull(Reference("a"))
     nan = IsNaN(Reference("b"))
     and_ = And(null, nan)
     assert str(and_) == f"And(left={str(null)}, right={str(nan)})"
     assert repr(and_) == f"And(left={repr(null)}, right={repr(nan)})"
     assert and_ == eval(repr(and_))
+    assert and_ == pickle.loads(pickle.dumps(and_))
 
 
 def test_or() -> None:
     null = IsNull(Reference("a"))
     nan = IsNaN(Reference("b"))
     or_ = Or(null, nan)
     assert str(or_) == f"Or(left={str(null)}, right={str(nan)})"
     assert repr(or_) == f"Or(left={repr(null)}, right={repr(nan)})"
     assert or_ == eval(repr(or_))
+    assert or_ == pickle.loads(pickle.dumps(or_))
 
 
 def test_not() -> None:
     null = IsNull(Reference("a"))
-    or_ = Not(null)
-    assert str(or_) == f"Not(child={str(null)})"
-    assert repr(or_) == f"Not(child={repr(null)})"
-    assert or_ == eval(repr(or_))
+    not_ = Not(null)
+    assert str(not_) == f"Not(child={str(null)})"
+    assert repr(not_) == f"Not(child={repr(null)})"
+    assert not_ == eval(repr(not_))
+    assert not_ == pickle.loads(pickle.dumps(not_))
 
 
 def test_always_true() -> None:
     always_true = AlwaysTrue()
     assert str(always_true) == "AlwaysTrue()"
     assert repr(always_true) == "AlwaysTrue()"
     assert always_true == eval(repr(always_true))
+    assert always_true == pickle.loads(pickle.dumps(always_true))
 
 
 def test_always_false() -> None:
     always_false = AlwaysFalse()
     assert str(always_false) == "AlwaysFalse()"
     assert repr(always_false) == "AlwaysFalse()"
     assert always_false == eval(repr(always_false))
+    assert always_false == pickle.loads(pickle.dumps(always_false))
 
 
 def test_bound_reference_field_property() -> None:
     field = NestedField(field_id=1, name="foo", field_type=StringType(), required=False)
     position1_accessor = Accessor(position=1)
     bound_ref = BoundReference(field=field, accessor=position1_accessor)
     assert bound_ref.field == NestedField(field_id=1, name="foo", field_type=StringType(), required=False)
@@ -752,176 +760,198 @@
 
 def test_is_null() -> None:
     ref = Reference("a")
     is_null = IsNull(ref)
     assert str(is_null) == f"IsNull(term={str(ref)})"
     assert repr(is_null) == f"IsNull(term={repr(ref)})"
     assert is_null == eval(repr(is_null))
+    assert is_null == pickle.loads(pickle.dumps(is_null))
 
 
 def test_not_null() -> None:
     ref = Reference("a")
     non_null = NotNull(ref)
     assert str(non_null) == f"NotNull(term={str(ref)})"
     assert repr(non_null) == f"NotNull(term={repr(ref)})"
     assert non_null == eval(repr(non_null))
+    assert non_null == pickle.loads(pickle.dumps(non_null))
 
 
 def test_bound_is_nan(accessor: Accessor) -> None:
     # We need a FloatType here
     term = BoundReference[float](
         field=NestedField(field_id=1, name="foo", field_type=FloatType(), required=False),
         accessor=accessor,
     )
     bound_is_nan = BoundIsNaN(term)
     assert str(bound_is_nan) == f"BoundIsNaN(term={str(term)})"
     assert repr(bound_is_nan) == f"BoundIsNaN(term={repr(term)})"
     assert bound_is_nan == eval(repr(bound_is_nan))
+    assert bound_is_nan == pickle.loads(pickle.dumps(bound_is_nan))
 
 
 def test_bound_is_not_nan(accessor: Accessor) -> None:
     # We need a FloatType here
     term = BoundReference[float](
         field=NestedField(field_id=1, name="foo", field_type=FloatType(), required=False),
         accessor=accessor,
     )
     bound_not_nan = BoundNotNaN(term)
     assert str(bound_not_nan) == f"BoundNotNaN(term={str(term)})"
     assert repr(bound_not_nan) == f"BoundNotNaN(term={repr(term)})"
     assert bound_not_nan == eval(repr(bound_not_nan))
+    assert bound_not_nan == pickle.loads(pickle.dumps(bound_not_nan))
 
 
 def test_is_nan() -> None:
     ref = Reference("a")
     is_nan = IsNaN(ref)
     assert str(is_nan) == f"IsNaN(term={str(ref)})"
     assert repr(is_nan) == f"IsNaN(term={repr(ref)})"
     assert is_nan == eval(repr(is_nan))
+    assert is_nan == pickle.loads(pickle.dumps(is_nan))
 
 
 def test_not_nan() -> None:
     ref = Reference("a")
     not_nan = NotNaN(ref)
     assert str(not_nan) == f"NotNaN(term={str(ref)})"
     assert repr(not_nan) == f"NotNaN(term={repr(ref)})"
     assert not_nan == eval(repr(not_nan))
+    assert not_nan == pickle.loads(pickle.dumps(not_nan))
 
 
 def test_bound_in(term: BoundReference[Any]) -> None:
     bound_in = BoundIn(term, {literal("a"), literal("b"), literal("c")})
     assert str(bound_in) == f"BoundIn({str(term)}, {{a, b, c}})"
     assert repr(bound_in) == f"BoundIn({repr(term)}, {{literal('a'), literal('b'), literal('c')}})"
     assert bound_in == eval(repr(bound_in))
+    assert bound_in == pickle.loads(pickle.dumps(bound_in))
 
 
 def test_bound_not_in(term: BoundReference[Any]) -> None:
     bound_not_in = BoundNotIn(term, {literal("a"), literal("b"), literal("c")})
     assert str(bound_not_in) == f"BoundNotIn({str(term)}, {{a, b, c}})"
     assert repr(bound_not_in) == f"BoundNotIn({repr(term)}, {{literal('a'), literal('b'), literal('c')}})"
     assert bound_not_in == eval(repr(bound_not_in))
+    assert bound_not_in == pickle.loads(pickle.dumps(bound_not_in))
 
 
 def test_in() -> None:
     ref = Reference("a")
     unbound_in = In(ref, {"a", "b", "c"})
     assert str(unbound_in) == f"In({str(ref)}, {{a, b, c}})"
     assert repr(unbound_in) == f"In({repr(ref)}, {{literal('a'), literal('b'), literal('c')}})"
     assert unbound_in == eval(repr(unbound_in))
+    assert unbound_in == pickle.loads(pickle.dumps(unbound_in))
 
 
 def test_not_in() -> None:
     ref = Reference("a")
     not_in = NotIn(ref, {"a", "b", "c"})
     assert str(not_in) == f"NotIn({str(ref)}, {{a, b, c}})"
     assert repr(not_in) == f"NotIn({repr(ref)}, {{literal('a'), literal('b'), literal('c')}})"
     assert not_in == eval(repr(not_in))
+    assert not_in == pickle.loads(pickle.dumps(not_in))
 
 
 def test_bound_equal_to(term: BoundReference[Any]) -> None:
     bound_equal_to = BoundEqualTo(term, literal("a"))
     assert str(bound_equal_to) == f"BoundEqualTo(term={str(term)}, literal=literal('a'))"
     assert repr(bound_equal_to) == f"BoundEqualTo(term={repr(term)}, literal=literal('a'))"
     assert bound_equal_to == eval(repr(bound_equal_to))
+    assert bound_equal_to == pickle.loads(pickle.dumps(bound_equal_to))
 
 
 def test_bound_not_equal_to(term: BoundReference[Any]) -> None:
     bound_not_equal_to = BoundNotEqualTo(term, literal("a"))
     assert str(bound_not_equal_to) == f"BoundNotEqualTo(term={str(term)}, literal=literal('a'))"
     assert repr(bound_not_equal_to) == f"BoundNotEqualTo(term={repr(term)}, literal=literal('a'))"
     assert bound_not_equal_to == eval(repr(bound_not_equal_to))
+    assert bound_not_equal_to == pickle.loads(pickle.dumps(bound_not_equal_to))
 
 
 def test_bound_greater_than_or_equal_to(term: BoundReference[Any]) -> None:
     bound_greater_than_or_equal_to = BoundGreaterThanOrEqual(term, literal("a"))
     assert str(bound_greater_than_or_equal_to) == f"BoundGreaterThanOrEqual(term={str(term)}, literal=literal('a'))"
     assert repr(bound_greater_than_or_equal_to) == f"BoundGreaterThanOrEqual(term={repr(term)}, literal=literal('a'))"
     assert bound_greater_than_or_equal_to == eval(repr(bound_greater_than_or_equal_to))
+    assert bound_greater_than_or_equal_to == pickle.loads(pickle.dumps(bound_greater_than_or_equal_to))
 
 
 def test_bound_greater_than(term: BoundReference[Any]) -> None:
     bound_greater_than = BoundGreaterThan(term, literal("a"))
     assert str(bound_greater_than) == f"BoundGreaterThan(term={str(term)}, literal=literal('a'))"
     assert repr(bound_greater_than) == f"BoundGreaterThan(term={repr(term)}, literal=literal('a'))"
     assert bound_greater_than == eval(repr(bound_greater_than))
+    assert bound_greater_than == pickle.loads(pickle.dumps(bound_greater_than))
 
 
 def test_bound_less_than(term: BoundReference[Any]) -> None:
     bound_less_than = BoundLessThan(term, literal("a"))
     assert str(bound_less_than) == f"BoundLessThan(term={str(term)}, literal=literal('a'))"
     assert repr(bound_less_than) == f"BoundLessThan(term={repr(term)}, literal=literal('a'))"
     assert bound_less_than == eval(repr(bound_less_than))
+    assert bound_less_than == pickle.loads(pickle.dumps(bound_less_than))
 
 
 def test_bound_less_than_or_equal(term: BoundReference[Any]) -> None:
     bound_less_than_or_equal = BoundLessThanOrEqual(term, literal("a"))
     assert str(bound_less_than_or_equal) == f"BoundLessThanOrEqual(term={str(term)}, literal=literal('a'))"
     assert repr(bound_less_than_or_equal) == f"BoundLessThanOrEqual(term={repr(term)}, literal=literal('a'))"
     assert bound_less_than_or_equal == eval(repr(bound_less_than_or_equal))
+    assert bound_less_than_or_equal == pickle.loads(pickle.dumps(bound_less_than_or_equal))
 
 
 def test_equal_to() -> None:
     equal_to = EqualTo(Reference("a"), literal("a"))
     assert str(equal_to) == "EqualTo(term=Reference(name='a'), literal=literal('a'))"
     assert repr(equal_to) == "EqualTo(term=Reference(name='a'), literal=literal('a'))"
     assert equal_to == eval(repr(equal_to))
+    assert equal_to == pickle.loads(pickle.dumps(equal_to))
 
 
 def test_not_equal_to() -> None:
     not_equal_to = NotEqualTo(Reference("a"), literal("a"))
     assert str(not_equal_to) == "NotEqualTo(term=Reference(name='a'), literal=literal('a'))"
     assert repr(not_equal_to) == "NotEqualTo(term=Reference(name='a'), literal=literal('a'))"
     assert not_equal_to == eval(repr(not_equal_to))
+    assert not_equal_to == pickle.loads(pickle.dumps(not_equal_to))
 
 
 def test_greater_than_or_equal_to() -> None:
     greater_than_or_equal_to = GreaterThanOrEqual(Reference("a"), literal("a"))
     assert str(greater_than_or_equal_to) == "GreaterThanOrEqual(term=Reference(name='a'), literal=literal('a'))"
     assert repr(greater_than_or_equal_to) == "GreaterThanOrEqual(term=Reference(name='a'), literal=literal('a'))"
     assert greater_than_or_equal_to == eval(repr(greater_than_or_equal_to))
+    assert greater_than_or_equal_to == pickle.loads(pickle.dumps(greater_than_or_equal_to))
 
 
 def test_greater_than() -> None:
     greater_than = GreaterThan(Reference("a"), literal("a"))
     assert str(greater_than) == "GreaterThan(term=Reference(name='a'), literal=literal('a'))"
     assert repr(greater_than) == "GreaterThan(term=Reference(name='a'), literal=literal('a'))"
     assert greater_than == eval(repr(greater_than))
+    assert greater_than == pickle.loads(pickle.dumps(greater_than))
 
 
 def test_less_than() -> None:
     less_than = LessThan(Reference("a"), literal("a"))
     assert str(less_than) == "LessThan(term=Reference(name='a'), literal=literal('a'))"
     assert repr(less_than) == "LessThan(term=Reference(name='a'), literal=literal('a'))"
     assert less_than == eval(repr(less_than))
+    assert less_than == pickle.loads(pickle.dumps(less_than))
 
 
 def test_less_than_or_equal() -> None:
     less_than_or_equal = LessThanOrEqual(Reference("a"), literal("a"))
     assert str(less_than_or_equal) == "LessThanOrEqual(term=Reference(name='a'), literal=literal('a'))"
     assert repr(less_than_or_equal) == "LessThanOrEqual(term=Reference(name='a'), literal=literal('a'))"
     assert less_than_or_equal == eval(repr(less_than_or_equal))
+    assert less_than_or_equal == pickle.loads(pickle.dumps(less_than_or_equal))
 
 
 def test_bound_reference_eval(table_schema_simple: Schema) -> None:
     """Test creating a BoundReference and evaluating it on a StructProtocol"""
     struct = Record(struct=table_schema_simple.as_struct())
 
     struct[0] = "foovalue"
```

### Comparing `pyiceberg-0.3.0rc2/tests/expressions/test_literals.py` & `pyiceberg-0.4.0rc1/tests/expressions/test_literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -380,14 +380,28 @@
     decimal_str = literal("34.560")
     decimal_lit = decimal_str.to(DecimalType(9, 3))
 
     assert 3 == abs(decimal_lit.value.as_tuple().exponent)  # type: ignore
     assert Decimal("34.560").as_tuple() == decimal_lit.value.as_tuple()  # type: ignore
 
 
+def test_string_to_boolean_literal() -> None:
+    assert literal(True) == literal("true").to(BooleanType())
+    assert literal(True) == literal("True").to(BooleanType())
+    assert literal(False) == literal("false").to(BooleanType())
+    assert literal(False) == literal("False").to(BooleanType())
+
+
+def test_invalid_string_to_boolean_literal() -> None:
+    invalid_boolean_str = literal("unknown")
+    with pytest.raises(ValueError) as e:
+        _ = invalid_boolean_str.to(BooleanType())
+    assert "Could not convert unknown into a boolean" in str(e.value)
+
+
 # MISC
 
 
 def test_python_date_conversion() -> None:
     one_day_str = "2022-03-28"
 
     from_str_lit = literal(one_day_str).to(DateType())
@@ -688,15 +702,15 @@
         ],
     )
 
 
 def test_invalid_string_conversions() -> None:
     assert_invalid_conversions(
         literal("abc"),
-        [BooleanType(), FloatType(), DoubleType(), FixedType(1), BinaryType()],
+        [FloatType(), DoubleType(), FixedType(1), BinaryType()],
     )
 
 
 def test_invalid_uuid_conversions() -> None:
     assert_invalid_conversions(
         literal(uuid.uuid4()),
         [
```

### Comparing `pyiceberg-0.3.0rc2/tests/expressions/test_parser.py` & `pyiceberg-0.4.0rc1/tests/expressions/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     LessThan,
     LessThanOrEqual,
     Not,
     NotEqualTo,
     NotIn,
     NotNaN,
     NotNull,
+    NotStartsWith,
     Or,
+    StartsWith,
     parser,
 )
 
 
 def test_true() -> None:
     assert AlwaysTrue() == parser.parse("true")
 
@@ -145,7 +147,15 @@
 
 
 def test_and_or_with_parens() -> None:
     assert And(NotNull("x"), Or(LessThan("x", 5), GreaterThan("x", 10))) == parser.parse("x is not null and (x < 5 or 10 < x)")
     assert Or(IsNull("x"), And(GreaterThanOrEqual("x", 5), Not(LessThan("x", 10)))) == parser.parse(
         "(x is null) or (5 <= x) and not(x < 10)"
     )
+
+
+def test_starts_with() -> None:
+    assert StartsWith("x", "data") == parser.parse("x LIKE 'data'")
+
+
+def test_not_starts_with() -> None:
+    assert NotStartsWith("x", "data") == parser.parse("x NOT LIKE 'data'")
```

### Comparing `pyiceberg-0.3.0rc2/tests/expressions/test_projection.py` & `pyiceberg-0.4.0rc1/tests/expressions/test_projection.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/expressions/test_visitors.py` & `pyiceberg-0.4.0rc1/tests/expressions/test_visitors.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,47 +34,54 @@
     BoundIsNull,
     BoundLessThan,
     BoundLessThanOrEqual,
     BoundNotEqualTo,
     BoundNotIn,
     BoundNotNaN,
     BoundNotNull,
+    BoundNotStartsWith,
     BoundPredicate,
     BoundReference,
+    BoundStartsWith,
     BoundTerm,
     EqualTo,
     GreaterThan,
     GreaterThanOrEqual,
     In,
     IsNaN,
     IsNull,
     LessThan,
     LessThanOrEqual,
     Not,
     NotEqualTo,
     NotIn,
     NotNaN,
     NotNull,
+    NotStartsWith,
     Or,
     Reference,
+    StartsWith,
     UnboundPredicate,
 )
 from pyiceberg.expressions.literals import Literal, literal
 from pyiceberg.expressions.visitors import (
     BindVisitor,
     BooleanExpressionVisitor,
     BoundBooleanExpressionVisitor,
     _ManifestEvalVisitor,
+    expression_evaluator,
+    expression_to_plain_format,
     rewrite_not,
     rewrite_to_dnf,
     visit,
     visit_bound_predicate,
 )
 from pyiceberg.manifest import ManifestFile, PartitionFieldSummary
 from pyiceberg.schema import Accessor, Schema
+from pyiceberg.typedef import Record
 from pyiceberg.types import (
     DoubleType,
     FloatType,
     IcebergType,
     IntegerType,
     NestedField,
     PrimitiveType,
@@ -200,14 +207,22 @@
         self.visit_history.append("AND")
         return self.visit_history
 
     def visit_or(self, left_result: List[str], right_result: List[str]) -> List[str]:
         self.visit_history.append("OR")
         return self.visit_history
 
+    def visit_starts_with(self, term: BoundTerm[Any], literal: Literal[Any]) -> List[str]:
+        self.visit_history.append("STARTS_WITH")
+        return self.visit_history
+
+    def visit_not_starts_with(self, term: BoundTerm[Any], literal: Literal[Any]) -> List[str]:
+        self.visit_history.append("NOT_STARTS_WITH")
+        return self.visit_history
+
 
 def test_boolean_expression_visitor() -> None:
     """Test post-order traversal of boolean expression visit method"""
     expr = And(
         Or(Not(EqualTo("a", 1)), Not(NotEqualTo("b", 0)), EqualTo("a", 1), NotEqualTo("b", 0)),
         Not(EqualTo("a", 1)),
         NotEqualTo("b", 0),
@@ -775,14 +790,40 @@
     )
     visitor = FooBoundBooleanExpressionVisitor()
     with pytest.raises(TypeError) as exc_info:
         visit(bound_expression, visitor=visitor)
     assert "Not a bound predicate" in str(exc_info.value)
 
 
+def test_bound_boolean_expression_visitor_starts_with() -> None:
+    bound_expression = BoundStartsWith(
+        term=BoundReference(
+            field=NestedField(field_id=1, name="foo", field_type=StringType(), required=False),
+            accessor=Accessor(position=0, inner=None),
+        ),
+        literal=literal("foo"),
+    )
+    visitor = FooBoundBooleanExpressionVisitor()
+    result = visit(bound_expression, visitor=visitor)
+    assert result == ["STARTS_WITH"]
+
+
+def test_bound_boolean_expression_visitor_not_starts_with() -> None:
+    bound_expression = BoundNotStartsWith(
+        term=BoundReference(
+            field=NestedField(field_id=1, name="foo", field_type=StringType(), required=False),
+            accessor=Accessor(position=0, inner=None),
+        ),
+        literal=literal("foo"),
+    )
+    visitor = FooBoundBooleanExpressionVisitor()
+    result = visit(bound_expression, visitor=visitor)
+    assert result == ["NOT_STARTS_WITH"]
+
+
 def _to_byte_buffer(field_type: IcebergType, val: Any) -> bytes:
     if not isinstance(field_type, PrimitiveType):
         raise ValueError(f"Expected a PrimitiveType, got: {type(field_type)}")
     return to_bytes(field_type, val)
 
 
 def _to_manifest_file(*partitions: PartitionFieldSummary) -> ManifestFile:
@@ -1354,35 +1395,133 @@
     ), "Should read: in on some nulls column"
 
     assert _ManifestEvalVisitor(schema, NotIn(Reference("no_nulls"), ("abc", "def")), case_sensitive=True).eval(
         manifest
     ), "Should read: in on no nulls column"
 
 
+def test_string_starts_with(schema: Schema, manifest: ManifestFile) -> None:
+    assert _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "aa"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "dddd"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "z"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, StartsWith(Reference("no_nulls"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert not _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "zzzz"), case_sensitive=False).eval(
+        manifest
+    ), "Should skip: range doesn't match"
+
+    assert not _ManifestEvalVisitor(schema, StartsWith(Reference("some_nulls"), "1"), case_sensitive=False).eval(
+        manifest
+    ), "Should skip: range doesn't match"
+
+
+def test_string_not_starts_with(schema: Schema, manifest: ManifestFile) -> None:
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "aa"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "dddd"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "z"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("no_nulls"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "zzzz"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("some_nulls"), "1"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("all_same_value_or_null"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("all_same_value_or_null"), "aa"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("all_same_value_or_null"), "A"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    #    Iceberg does not implement SQL's 3-way boolean logic, so the choice of an all null column
+    #    matching is
+    #    by definition in order to surface more values to the query engine to allow it to make its own
+    #    decision.
+    assert _ManifestEvalVisitor(schema, NotStartsWith(Reference("all_nulls_missing_nan"), "A"), case_sensitive=False).eval(
+        manifest
+    ), "Should read: range matches"
+
+    assert not _ManifestEvalVisitor(schema, NotStartsWith(Reference("no_nulls_same_value_a"), "a"), case_sensitive=False).eval(
+        manifest
+    ), "Should not read: all values start with the prefix"
+
+
 def test_rewrite_not_equal_to() -> None:
     assert rewrite_not(Not(EqualTo(Reference("x"), 34.56))) == NotEqualTo(Reference("x"), 34.56)
 
 
 def test_rewrite_not_not_equal_to() -> None:
     assert rewrite_not(Not(NotEqualTo(Reference("x"), 34.56))) == EqualTo(Reference("x"), 34.56)
 
 
 def test_rewrite_not_in() -> None:
     assert rewrite_not(Not(In(Reference("x"), (34.56,)))) == NotIn(Reference("x"), (34.56,))
 
 
 def test_rewrite_and() -> None:
-    assert rewrite_not(Not(And(EqualTo(Reference("x"), 34.56), EqualTo(Reference("y"), 34.56),))) == Or(
+    assert rewrite_not(
+        Not(
+            And(
+                EqualTo(Reference("x"), 34.56),
+                EqualTo(Reference("y"), 34.56),
+            )
+        )
+    ) == Or(
         NotEqualTo(term=Reference(name="x"), literal=34.56),
         NotEqualTo(term=Reference(name="y"), literal=34.56),
     )
 
 
 def test_rewrite_or() -> None:
-    assert rewrite_not(Not(Or(EqualTo(Reference("x"), 34.56), EqualTo(Reference("y"), 34.56),))) == And(
+    assert rewrite_not(
+        Not(
+            Or(
+                EqualTo(Reference("x"), 34.56),
+                EqualTo(Reference("y"), 34.56),
+            )
+        )
+    ) == And(
         NotEqualTo(term=Reference(name="x"), literal=34.56),
         NotEqualTo(term=Reference(name="y"), literal=34.56),
     )
 
 
 def test_rewrite_always_false() -> None:
     assert rewrite_not(Not(AlwaysFalse())) == AlwaysTrue()
@@ -1447,7 +1586,46 @@
     expr = And(Not(EqualTo("Q", "b")), EqualTo("R", "c"))
     assert rewrite_to_dnf(expr) == (And(NotEqualTo("Q", "b"), EqualTo("R", "c")),)
 
 
 def test_to_dnf_not_and() -> None:
     expr = Not(And(Not(EqualTo("Q", "b")), EqualTo("R", "c")))
     assert rewrite_to_dnf(expr) == (EqualTo("Q", "b"), NotEqualTo("R", "c"))
+
+
+def test_dnf_to_dask(table_schema_simple: Schema) -> None:
+    expr = (
+        BoundGreaterThan[str](
+            term=BoundReference(table_schema_simple.find_field(1), table_schema_simple.accessor_for_field(1)),
+            literal=literal("hello"),
+        ),
+        And(
+            BoundIn[int](
+                term=BoundReference(table_schema_simple.find_field(2), table_schema_simple.accessor_for_field(2)),
+                literals={literal(1), literal(2), literal(3)},
+            ),
+            BoundEqualTo[bool](
+                term=BoundReference(table_schema_simple.find_field(3), table_schema_simple.accessor_for_field(3)),
+                literal=literal(True),
+            ),
+        ),
+    )
+    assert expression_to_plain_format(expr) == [[("foo", ">", "hello")], [("bar", "in", {1, 2, 3}), ("baz", "==", True)]]
+
+
+def test_expression_evaluator_null() -> None:
+    struct = Record(a=None)
+    schema = Schema(NestedField(1, "a", IntegerType(), required=False), schema_id=1)
+    assert expression_evaluator(schema, In("a", {1, 2, 3}), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, NotIn("a", {1, 2, 3}), case_sensitive=True)(struct) is True
+    assert expression_evaluator(schema, IsNaN("a"), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, NotNaN("a"), case_sensitive=True)(struct) is True
+    assert expression_evaluator(schema, IsNull("a"), case_sensitive=True)(struct) is True
+    assert expression_evaluator(schema, NotNull("a"), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, EqualTo("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, NotEqualTo("a", 1), case_sensitive=True)(struct) is True
+    assert expression_evaluator(schema, GreaterThanOrEqual("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, GreaterThan("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, LessThanOrEqual("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, LessThan("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, StartsWith("a", 1), case_sensitive=True)(struct) is False
+    assert expression_evaluator(schema, NotStartsWith("a", 1), case_sensitive=True)(struct) is True
```

### Comparing `pyiceberg-0.3.0rc2/tests/io/test_fsspec.py` & `pyiceberg-0.4.0rc1/tests/io/test_fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/io/test_io.py` & `pyiceberg-0.4.0rc1/tests/io/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 import pytest
 
 from pyiceberg.io import (
     ARROW_FILE_IO,
     PY_IO_IMPL,
     _import_file_io,
+    _infer_file_io_from_scheme,
     load_file_io,
 )
-from pyiceberg.io.fsspec import FsspecFileIO
 from pyiceberg.io.pyarrow import PyArrowFileIO
 
 
 def test_custom_local_input_file() -> None:
     """Test initializing an InputFile implementation to read a local file"""
     with tempfile.TemporaryDirectory() as tmpdirname:
         file_location = os.path.join(tmpdirname, "foo.txt")
@@ -273,15 +273,15 @@
     with pytest.raises(ValueError) as exc_info:
         load_file_io({PY_IO_IMPL: "pyiceberg.does.not.exist.FileIO"})
 
     assert "Could not initialize FileIO: pyiceberg.does.not.exist.FileIO" in str(exc_info.value)
 
 
 def test_load_file_io_warehouse() -> None:
-    assert isinstance(load_file_io({"warehouse": "s3://some-path/"}), FsspecFileIO)
+    assert isinstance(load_file_io({"warehouse": "s3://some-path/"}), PyArrowFileIO)
 
 
 def test_load_file_io_location() -> None:
     assert isinstance(load_file_io({"location": "s3://some-path/"}), PyArrowFileIO)
 
 
 def test_load_file_io_location_no_schema() -> None:
@@ -299,7 +299,15 @@
     io = load_file_io({}, "test://some-path/")
     assert io.properties == {}
 
 
 def test_gibberish_table_location_file_io() -> None:
     # For testing the selection logic
     assert isinstance(load_file_io({}, "gibberish"), PyArrowFileIO)
+
+
+def test_infer_file_io_from_schema_unknown() -> None:
+    # When we have an unknown scheme, we would like to know
+    with pytest.warns(UserWarning) as w:
+        _infer_file_io_from_scheme("unknown://bucket/path/", {})
+
+    assert str(w[0].message) == "No preferred file implementation for scheme: unknown"
```

### Comparing `pyiceberg-0.3.0rc2/tests/io/test_pyarrow.py` & `pyiceberg-0.4.0rc1/tests/io/test_pyarrow.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 import tempfile
 from typing import Any, List, Optional
 from unittest.mock import MagicMock, patch
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pytest
-from pyarrow.fs import FileType
+from pyarrow.fs import FileType, LocalFileSystem
 
 from pyiceberg.avro.resolver import ResolveError
+from pyiceberg.catalog.noop import NoopCatalog
 from pyiceberg.expressions import (
     AlwaysFalse,
     AlwaysTrue,
     And,
     BooleanExpression,
     BoundEqualTo,
     BoundGreaterThan,
@@ -40,30 +41,33 @@
     BoundIsNull,
     BoundLessThan,
     BoundLessThanOrEqual,
     BoundNotEqualTo,
     BoundNotIn,
     BoundNotNaN,
     BoundNotNull,
+    BoundNotStartsWith,
     BoundReference,
+    BoundStartsWith,
     GreaterThan,
     Not,
     Or,
     literal,
 )
-from pyiceberg.io import InputStream, OutputStream
+from pyiceberg.io import InputStream, OutputStream, load_file_io
 from pyiceberg.io.pyarrow import (
     PyArrowFile,
     PyArrowFileIO,
     _ConvertToArrowSchema,
+    _read_deletes,
     expression_to_pyarrow,
     project_table,
     schema_to_pyarrow,
 )
-from pyiceberg.manifest import DataFile, FileFormat
+from pyiceberg.manifest import DataFile, DataFileContent, FileFormat
 from pyiceberg.partitioning import PartitionSpec
 from pyiceberg.schema import Schema, visit
 from pyiceberg.table import FileScanTask, Table
 from pyiceberg.table.metadata import TableMetadataV2
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
@@ -297,32 +301,66 @@
 
         assert "Cannot delete file, does not exist:" in str(exc_info.value)
 
 
 def test_schema_to_pyarrow_schema(table_schema_nested: Schema) -> None:
     actual = schema_to_pyarrow(table_schema_nested)
     expected = """foo: string
+  -- field metadata --
+  field_id: '1'
 bar: int32 not null
+  -- field metadata --
+  field_id: '2'
 baz: bool
-qux: list<item: string> not null
-  child 0, item: string
+  -- field metadata --
+  field_id: '3'
+qux: list<element: string not null> not null
+  child 0, element: string not null
+    -- field metadata --
+    field_id: '5'
+  -- field metadata --
+  field_id: '4'
 quux: map<string, map<string, int32>> not null
-  child 0, entries: struct<key: string not null, value: map<string, int32>> not null
+  child 0, entries: struct<key: string not null, value: map<string, int32> not null> not null
       child 0, key: string not null
-      child 1, value: map<string, int32>
-          child 0, entries: struct<key: string not null, value: int32> not null
+      -- field metadata --
+      field_id: '7'
+      child 1, value: map<string, int32> not null
+          child 0, entries: struct<key: string not null, value: int32 not null> not null
               child 0, key: string not null
-              child 1, value: int32
-location: list<item: struct<latitude: float, longitude: float>> not null
-  child 0, item: struct<latitude: float, longitude: float>
+          -- field metadata --
+          field_id: '9'
+              child 1, value: int32 not null
+          -- field metadata --
+          field_id: '10'
+      -- field metadata --
+      field_id: '8'
+  -- field metadata --
+  field_id: '6'
+location: list<element: struct<latitude: float, longitude: float> not null> not null
+  child 0, element: struct<latitude: float, longitude: float> not null
       child 0, latitude: float
+      -- field metadata --
+      field_id: '13'
       child 1, longitude: float
+      -- field metadata --
+      field_id: '14'
+    -- field metadata --
+    field_id: '12'
+  -- field metadata --
+  field_id: '11'
 person: struct<name: string, age: int32 not null>
   child 0, name: string
-  child 1, age: int32 not null"""
+    -- field metadata --
+    field_id: '16'
+  child 1, age: int32 not null
+    -- field metadata --
+    field_id: '17'
+  -- field metadata --
+  field_id: '15'"""
     assert repr(actual) == expected
 
 
 def test_fixed_type_to_pyarrow() -> None:
     length = 22
     iceberg_type = FixedType(length)
     assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.binary(length)
@@ -373,15 +411,15 @@
 def test_timestamp_type_to_pyarrow() -> None:
     iceberg_type = TimestampType()
     assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.timestamp(unit="us")
 
 
 def test_timestamptz_type_to_pyarrow() -> None:
     iceberg_type = TimestamptzType()
-    assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.timestamp(unit="us", tz="+00:00")
+    assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.timestamp(unit="us", tz="UTC")
 
 
 def test_string_type_to_pyarrow() -> None:
     iceberg_type = StringType()
     assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.string()
 
 
@@ -389,40 +427,45 @@
     iceberg_type = BinaryType()
     assert visit(iceberg_type, _ConvertToArrowSchema()) == pa.binary()
 
 
 def test_struct_type_to_pyarrow(table_schema_simple: Schema) -> None:
     expected = pa.struct(
         [
-            pa.field("foo", pa.string(), nullable=True, metadata={"id": "1"}),
-            pa.field("bar", pa.int32(), nullable=False, metadata={"id": "2"}),
-            pa.field("baz", pa.bool_(), nullable=True, metadata={"id": "3"}),
+            pa.field("foo", pa.string(), nullable=True, metadata={"field_id": "1"}),
+            pa.field("bar", pa.int32(), nullable=False, metadata={"field_id": "2"}),
+            pa.field("baz", pa.bool_(), nullable=True, metadata={"field_id": "3"}),
         ]
     )
     assert visit(table_schema_simple.as_struct(), _ConvertToArrowSchema()) == expected
 
 
 def test_map_type_to_pyarrow() -> None:
     iceberg_map = MapType(
         key_id=1,
         key_type=IntegerType(),
         value_id=2,
         value_type=StringType(),
         value_required=True,
     )
-    assert visit(iceberg_map, _ConvertToArrowSchema()) == pa.map_(pa.int32(), pa.string())
+    assert visit(iceberg_map, _ConvertToArrowSchema()) == pa.map_(
+        pa.field("key", pa.int32(), nullable=False, metadata={"field_id": "1"}),
+        pa.field("value", pa.string(), nullable=False, metadata={"field_id": "2"}),
+    )
 
 
 def test_list_type_to_pyarrow() -> None:
     iceberg_map = ListType(
         element_id=1,
         element_type=IntegerType(),
         element_required=True,
     )
-    assert visit(iceberg_map, _ConvertToArrowSchema()) == pa.list_(pa.int32())
+    assert visit(iceberg_map, _ConvertToArrowSchema()) == pa.list_(
+        pa.field("element", pa.int32(), nullable=False, metadata={"field_id": "1"})
+    )
 
 
 @pytest.fixture
 def bound_reference(table_schema_simple: Schema) -> BoundReference[str]:
     return BoundReference(table_schema_simple.find_field(1), table_schema_simple.accessor_for_field(1))
 
 
@@ -444,25 +487,19 @@
 
 
 def test_expr_not_null_to_pyarrow(bound_reference: BoundReference[str]) -> None:
     assert repr(expression_to_pyarrow(BoundNotNull(bound_reference))) == "<pyarrow.compute.Expression is_valid(foo)>"
 
 
 def test_expr_is_nan_to_pyarrow(bound_double_reference: BoundReference[str]) -> None:
-    assert (
-        repr(expression_to_pyarrow(BoundIsNaN(bound_double_reference)))
-        == "<pyarrow.compute.Expression (is_null(foo, {nan_is_null=true}) and is_valid(foo))>"
-    )
+    assert repr(expression_to_pyarrow(BoundIsNaN(bound_double_reference))) == "<pyarrow.compute.Expression is_nan(foo)>"
 
 
 def test_expr_not_nan_to_pyarrow(bound_double_reference: BoundReference[str]) -> None:
-    assert (
-        repr(expression_to_pyarrow(BoundNotNaN(bound_double_reference)))
-        == "<pyarrow.compute.Expression invert((is_null(foo, {nan_is_null=true}) and is_valid(foo)))>"
-    )
+    assert repr(expression_to_pyarrow(BoundNotNaN(bound_double_reference))) == "<pyarrow.compute.Expression invert(is_nan(foo))>"
 
 
 def test_expr_equal_to_pyarrow(bound_reference: BoundReference[str]) -> None:
     assert (
         repr(expression_to_pyarrow(BoundEqualTo(bound_reference, literal("hello"))))
         == '<pyarrow.compute.Expression (foo == "hello")>'
     )
@@ -525,14 +562,28 @@
         """<pyarrow.compute.Expression invert(is_in(foo, {value_set=string:[
   "hello",
   "world"
 ], skip_nulls=false}))>""",
     )
 
 
+def test_expr_starts_with_to_pyarrow(bound_reference: BoundReference[str]) -> None:
+    assert (
+        repr(expression_to_pyarrow(BoundStartsWith(bound_reference, literal("he"))))
+        == '<pyarrow.compute.Expression starts_with(foo, {pattern="he", ignore_case=false})>'
+    )
+
+
+def test_expr_not_starts_with_to_pyarrow(bound_reference: BoundReference[str]) -> None:
+    assert (
+        repr(expression_to_pyarrow(BoundNotStartsWith(bound_reference, literal("he"))))
+        == '<pyarrow.compute.Expression invert(starts_with(foo, {pattern="he", ignore_case=false}))>'
+    )
+
+
 def test_and_to_pyarrow(bound_reference: BoundReference[str]) -> None:
     assert (
         repr(expression_to_pyarrow(And(BoundEqualTo(bound_reference, literal("hello")), BoundIsNull(bound_reference))))
         == '<pyarrow.compute.Expression ((foo == "hello") and is_null(foo, {nan_is_null=false}))>'
     )
 
 
@@ -745,29 +796,37 @@
 
 def project(
     schema: Schema, files: List[str], expr: Optional[BooleanExpression] = None, table_schema: Optional[Schema] = None
 ) -> pa.Table:
     return project_table(
         [
             FileScanTask(
-                DataFile(file_path=file, file_format=FileFormat.PARQUET, partition={}, record_count=3, file_size_in_bytes=3)
+                DataFile(
+                    content=DataFileContent.DATA,
+                    file_path=file,
+                    file_format=FileFormat.PARQUET,
+                    partition={},
+                    record_count=3,
+                    file_size_in_bytes=3,
+                )
             )
             for file in files
         ],
         Table(
             ("namespace", "table"),
             metadata=TableMetadataV2(
                 location="file://a/b/",
                 last_column_id=1,
                 format_version=2,
                 schemas=[table_schema or schema],
                 partition_specs=[PartitionSpec()],
             ),
             metadata_location="file://a/b/c.json",
             io=PyArrowFileIO(),
+            catalog=NoopCatalog("NoopCatalog"),
         ),
         expr or AlwaysTrue(),
         schema,
         case_sensitive=True,
     )
 
 
@@ -803,27 +862,36 @@
         assert actual.as_py() == expected
 
     for actual, expected in zip(result_table.columns[2], [None, None, None]):
         assert actual.as_py() == expected
 
     for actual, expected in zip(result_table.columns[3], [None, None, None]):
         assert actual.as_py() == expected
-
     assert (
         repr(result_table.schema)
         == """id: int32
-list: list<item: int32>
-  child 0, item: int32
+list: list<element: int32>
+  child 0, element: int32
+    -- field metadata --
+    field_id: '21'
 map: map<int32, string>
   child 0, entries: struct<key: int32 not null, value: string> not null
       child 0, key: int32 not null
+      -- field metadata --
+      field_id: '31'
       child 1, value: string
+      -- field metadata --
+      field_id: '32'
 location: struct<lat: double, lon: double>
   child 0, lat: double
-  child 1, lon: double"""
+    -- field metadata --
+    field_id: '41'
+  child 1, lon: double
+    -- field metadata --
+    field_id: '42'"""
     )
 
 
 def test_read_list(schema_list: Schema, file_list: str) -> None:
     result_table = project(schema_list, [file_list])
 
     assert len(result_table.columns[0]) == 3
@@ -859,21 +927,24 @@
             required=False,
         )
     )
     result_table = project(schema, [file_int])
     # Everything should be None
     for r in result_table.columns[0]:
         assert r.as_py() is None
-
     assert (
         repr(result_table.schema)
         == """id: map<int32, string>
   child 0, entries: struct<key: int32 not null, value: string> not null
       child 0, key: int32 not null
-      child 1, value: string"""
+      -- field metadata --
+      field_id: '3'
+      child 1, value: string
+      -- field metadata --
+      field_id: '4'"""
     )
 
 
 def test_projection_add_column_struct_required(file_int: str) -> None:
     schema = Schema(
         # A new ID
         NestedField(
@@ -909,15 +980,20 @@
     assert len(result_table.columns[0]) == 6
     assert repr(result_table.schema) == "id: int32"
 
 
 def test_projection_filter(schema_int: Schema, file_int: str) -> None:
     result_table = project(schema_int, [file_int], GreaterThan("id", 4))
     assert len(result_table.columns[0]) == 0
-    assert repr(result_table.schema) == "id: int32"
+    assert (
+        repr(result_table.schema)
+        == """id: int32
+  -- field metadata --
+  field_id: '1'"""
+    )
 
 
 def test_projection_filter_renamed_column(file_int: str) -> None:
     schema = Schema(
         # Reuses the id 1
         NestedField(1, "other_id", IntegerType())
     )
@@ -1085,15 +1161,19 @@
     for actual, expected in zip(result_table.columns[0], [None, None, None]):
         assert actual.as_py() == expected
     assert len(result_table.columns[0]) == 3
     assert (
         repr(result_table.schema)
         == """location: struct<lat: double, long: double>
   child 0, lat: double
-  child 1, long: double"""
+    -- field metadata --
+    field_id: '41'
+  child 1, long: double
+    -- field metadata --
+    field_id: '42'"""
     )
 
 
 def test_projection_filter_on_unprojected_field(schema_int_str: Schema, file_int_str: str) -> None:
     schema = Schema(NestedField(1, "id", IntegerType()))
 
     result_table = project(schema, [file_int_str], GreaterThan("data", "1"), schema_int_str)
@@ -1110,7 +1190,143 @@
 def test_projection_filter_on_unknown_field(schema_int_str: Schema, file_int_str: str) -> None:
     schema = Schema(NestedField(1, "id", IntegerType()))
 
     with pytest.raises(ValueError) as exc_info:
         _ = project(schema, [file_int_str], GreaterThan("unknown_field", "1"), schema_int_str)
 
     assert "Could not find field with name unknown_field, case_sensitive=True" in str(exc_info.value)
+
+
+@pytest.fixture
+def deletes_file(tmp_path: str, example_task: FileScanTask) -> str:
+    path = example_task.file.file_path
+    table = pa.table({"file_path": [path, path, path], "pos": [1, 3, 5]})
+
+    deletes_file_path = f"{tmp_path}/deletes.parquet"
+    pq.write_table(table, deletes_file_path)
+
+    return deletes_file_path
+
+
+def test_read_deletes(deletes_file: str, example_task: FileScanTask) -> None:
+    deletes = _read_deletes(LocalFileSystem(), DataFile(file_path=deletes_file, file_format=FileFormat.PARQUET))
+    assert set(deletes.keys()) == {example_task.file.file_path}
+    assert list(deletes.values())[0] == pa.chunked_array([[1, 3, 5]])
+
+
+def test_delete(deletes_file: str, example_task: FileScanTask, table_schema_simple: Schema) -> None:
+    metadata_location = "file://a/b/c.json"
+    example_task_with_delete = FileScanTask(
+        data_file=example_task.file,
+        delete_files={DataFile(content=DataFileContent.POSITION_DELETES, file_path=deletes_file, file_format=FileFormat.PARQUET)},
+    )
+
+    with_deletes = project_table(
+        tasks=[example_task_with_delete],
+        table=Table(
+            ("namespace", "table"),
+            metadata=TableMetadataV2(
+                location=metadata_location,
+                last_column_id=1,
+                format_version=2,
+                current_schema_id=1,
+                schemas=[table_schema_simple],
+                partition_specs=[PartitionSpec()],
+            ),
+            metadata_location=metadata_location,
+            io=load_file_io(),
+            catalog=NoopCatalog("noop"),
+        ),
+        row_filter=AlwaysTrue(),
+        projected_schema=table_schema_simple,
+    )
+
+    assert (
+        str(with_deletes)
+        == """pyarrow.Table
+foo: string
+bar: int64 not null
+baz: bool
+----
+foo: [["a","c"]]
+bar: [[1,3]]
+baz: [[true,null]]"""
+    )
+
+
+def test_delete_duplicates(deletes_file: str, example_task: FileScanTask, table_schema_simple: Schema) -> None:
+    metadata_location = "file://a/b/c.json"
+    example_task_with_delete = FileScanTask(
+        data_file=example_task.file,
+        delete_files={
+            DataFile(content=DataFileContent.POSITION_DELETES, file_path=deletes_file, file_format=FileFormat.PARQUET),
+            DataFile(content=DataFileContent.POSITION_DELETES, file_path=deletes_file, file_format=FileFormat.PARQUET),
+        },
+    )
+
+    with_deletes = project_table(
+        tasks=[example_task_with_delete],
+        table=Table(
+            ("namespace", "table"),
+            metadata=TableMetadataV2(
+                location=metadata_location,
+                last_column_id=1,
+                format_version=2,
+                current_schema_id=1,
+                schemas=[table_schema_simple],
+                partition_specs=[PartitionSpec()],
+            ),
+            metadata_location=metadata_location,
+            io=load_file_io(),
+            catalog=NoopCatalog("noop"),
+        ),
+        row_filter=AlwaysTrue(),
+        projected_schema=table_schema_simple,
+    )
+
+    assert (
+        str(with_deletes)
+        == """pyarrow.Table
+foo: string
+bar: int64 not null
+baz: bool
+----
+foo: [["a","c"]]
+bar: [[1,3]]
+baz: [[true,null]]"""
+    )
+
+
+def test_pyarrow_wrap_fsspec(example_task: FileScanTask, table_schema_simple: Schema) -> None:
+    metadata_location = "file://a/b/c.json"
+    projection = project_table(
+        [example_task],
+        Table(
+            ("namespace", "table"),
+            metadata=TableMetadataV2(
+                location=metadata_location,
+                last_column_id=1,
+                format_version=2,
+                current_schema_id=1,
+                schemas=[table_schema_simple],
+                partition_specs=[PartitionSpec()],
+            ),
+            metadata_location=metadata_location,
+            io=load_file_io(properties={"py-io-impl": "pyiceberg.io.fsspec.FsspecFileIO"}, location=metadata_location),
+            catalog=NoopCatalog("NoopCatalog"),
+        ),
+        case_sensitive=True,
+        projected_schema=table_schema_simple,
+        row_filter=AlwaysTrue(),
+    )
+
+    assert (
+        str(projection)
+        == """pyarrow.Table
+foo: string
+bar: int64 not null
+baz: bool
+----
+foo: [["a","b","c"]]
+bar: [[1,2,3]]
+baz: [[true,false,null]]"""
+    )
```

### Comparing `pyiceberg-0.3.0rc2/tests/table/test_metadata.py` & `pyiceberg-0.4.0rc1/tests/table/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/table/test_partitioning.py` & `pyiceberg-0.4.0rc1/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/table/test_refs.py` & `pyiceberg-0.4.0rc1/tests/table/test_refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/table/test_snapshots.py` & `pyiceberg-0.4.0rc1/tests/table/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/table/test_sorting.py` & `pyiceberg-0.4.0rc1/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/test_conversions.py` & `pyiceberg-0.4.0rc1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/test_schema.py` & `pyiceberg-0.4.0rc1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/test_transforms.py` & `pyiceberg-0.4.0rc1/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,26 @@
     BoundGreaterThan,
     BoundGreaterThanOrEqual,
     BoundIn,
     BoundLessThan,
     BoundLessThanOrEqual,
     BoundNotIn,
     BoundNotNull,
+    BoundNotStartsWith,
     BoundReference,
+    BoundStartsWith,
     EqualTo,
     GreaterThanOrEqual,
     In,
     LessThanOrEqual,
     NotIn,
     NotNull,
+    NotStartsWith,
     Reference,
+    StartsWith,
 )
 from pyiceberg.expressions.literals import (
     DateLiteral,
     DecimalLiteral,
     TimestampLiteral,
     literal,
 )
@@ -418,15 +422,14 @@
     assert not void_transform.satisfies_order_of(BucketTransform(100))
     assert void_transform.to_human_string(StringType(), "test") == "null"
     assert void_transform.dedup_name == "void"
 
 
 class TestType(IcebergBaseModel):
     __root__: Transform[Any, Any]
-    __test__ = False
 
 
 def test_bucket_transform_serialize() -> None:
     assert BucketTransform(num_buckets=22).json() == '"bucket[22]"'
 
 
 def test_bucket_transform_deserialize() -> None:
@@ -765,42 +768,40 @@
 def test_projection_identity_unary(bound_reference_timestamp: BoundReference[int]) -> None:
     assert IdentityTransform().project("name", BoundNotNull(term=bound_reference_timestamp)) == NotNull(term="name")
 
 
 def test_projection_identity_literal(bound_reference_timestamp: BoundReference[int]) -> None:
     assert IdentityTransform().project(
         "name", BoundEqualTo(term=bound_reference_timestamp, literal=TimestampLiteral(TIMESTAMP_EXAMPLE))
-    ) == EqualTo(
-        term="name", literal=TimestampLiteral(TIMESTAMP_EXAMPLE)  # type: ignore
-    )
+    ) == EqualTo(term="name", literal=TimestampLiteral(TIMESTAMP_EXAMPLE))
 
 
 def test_projection_identity_set_in(bound_reference_timestamp: BoundReference[int]) -> None:
     assert IdentityTransform().project(
         "name",
         BoundIn(
             term=bound_reference_timestamp,
             literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},
         ),
     ) == In(
         term="name",
-        literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},  # type: ignore
+        literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},
     )
 
 
 def test_projection_identity_set_not_in(bound_reference_timestamp: BoundReference[int]) -> None:
     assert IdentityTransform().project(
         "name",
         BoundNotIn(
             term=bound_reference_timestamp,
             literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},
         ),
     ) == NotIn(
         term="name",
-        literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},  # type: ignore
+        literals={TimestampLiteral(TIMESTAMP_EXAMPLE + HOUR_IN_MICROSECONDS), TimestampLiteral(TIMESTAMP_EXAMPLE)},
     )
 
 
 def test_projection_truncate_string_unary(bound_reference_str: BoundReference[str]) -> None:
     assert TruncateTransform(2).project("name", BoundNotNull(term=bound_reference_str)) == NotNull(term="name")
 
 
@@ -895,7 +896,19 @@
     ) == In(
         term="name",
         literals={
             Decimal("19.24"),
             Decimal("18.14999999999999857891452847979962825775146484374"),
         },
     )
+
+
+def test_projection_truncate_string_starts_with(bound_reference_str: BoundReference[str]) -> None:
+    assert TruncateTransform(2).project(
+        "name", BoundStartsWith(term=bound_reference_str, literal=literal("hello"))
+    ) == StartsWith(term="name", literal=literal("he"))
+
+
+def test_projection_truncate_string_not_starts_with(bound_reference_str: BoundReference[str]) -> None:
+    assert TruncateTransform(2).project(
+        "name", BoundNotStartsWith(term=bound_reference_str, literal=literal("hello"))
+    ) == NotStartsWith(term="name", literal=literal("he"))
```

### Comparing `pyiceberg-0.3.0rc2/tests/test_typedef.py` & `pyiceberg-0.4.0rc1/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/test_types.py` & `pyiceberg-0.4.0rc1/tests/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # pylint: disable=W0123,W0613
+import pickle
 from typing import Type
 
 import pytest
 from pydantic import ValidationError
 
 from pyiceberg.typedef import IcebergBaseModel
 from pyiceberg.types import (
@@ -59,14 +60,15 @@
     (12, BinaryType),
 ]
 
 
 @pytest.mark.parametrize("input_index, input_type", non_parameterized_types)
 def test_repr_primitive_types(input_index: int, input_type: Type[PrimitiveType]) -> None:
     assert isinstance(eval(repr(input_type())), input_type)
+    assert input_type == pickle.loads(pickle.dumps(input_type))
 
 
 @pytest.mark.parametrize(
     "input_type, result",
     [
         (BooleanType(), True),
         (IntegerType(), True),
@@ -105,25 +107,27 @@
     type_var = FixedType(length=5)
     assert len(type_var) == 5
     assert str(type_var) == "fixed[5]"
     assert repr(type_var) == "FixedType(length=5)"
     assert str(type_var) == str(eval(repr(type_var)))
     assert type_var == FixedType(5)
     assert type_var != FixedType(6)
+    assert type_var == pickle.loads(pickle.dumps(type_var))
 
 
 def test_decimal_type() -> None:
     type_var = DecimalType(precision=9, scale=2)
     assert type_var.precision == 9
     assert type_var.scale == 2
     assert str(type_var) == "decimal(9, 2)"
     assert repr(type_var) == "DecimalType(precision=9, scale=2)"
     assert str(type_var) == str(eval(repr(type_var)))
     assert type_var == DecimalType(9, 2)
     assert type_var != DecimalType(9, 3)
+    assert type_var == pickle.loads(pickle.dumps(type_var))
 
 
 def test_struct_type() -> None:
     type_var = StructType(
         NestedField(1, "optional_field", IntegerType(), required=True),
         NestedField(2, "required_field", FixedType(5), required=False),
         NestedField(
@@ -136,14 +140,15 @@
             required=False,
         ),
     )
     assert len(type_var.fields) == 3
     assert str(type_var) == str(eval(repr(type_var)))
     assert type_var == eval(repr(type_var))
     assert type_var != StructType(NestedField(1, "optional_field", IntegerType(), required=True))
+    assert type_var == pickle.loads(pickle.dumps(type_var))
 
 
 def test_list_type() -> None:
     type_var = ListType(
         1,
         StructType(
             NestedField(2, "optional_field", DecimalType(8, 2), required=True),
@@ -159,26 +164,28 @@
     assert type_var != ListType(
         1,
         StructType(
             NestedField(2, "optional_field", DecimalType(8, 2), required=True),
         ),
         True,
     )
+    assert type_var == pickle.loads(pickle.dumps(type_var))
 
 
 def test_map_type() -> None:
     type_var = MapType(1, DoubleType(), 2, UUIDType(), False)
     assert isinstance(type_var.key_field.field_type, DoubleType)
     assert type_var.key_field.field_id == 1
     assert isinstance(type_var.value_field.field_type, UUIDType)
     assert type_var.value_field.field_id == 2
     assert str(type_var) == str(eval(repr(type_var)))
     assert type_var == eval(repr(type_var))
     assert type_var != MapType(1, LongType(), 2, UUIDType(), False)
     assert type_var != MapType(1, DoubleType(), 2, StringType(), True)
+    assert type_var == pickle.loads(pickle.dumps(type_var))
 
 
 def test_nested_field() -> None:
     field_var = NestedField(
         1,
         "optional_field1",
         StructType(
@@ -196,14 +203,15 @@
         required=True,
     )
     assert field_var.required
     assert not field_var.optional
     assert field_var.field_id == 1
     assert isinstance(field_var.field_type, StructType)
     assert str(field_var) == str(eval(repr(field_var)))
+    assert field_var == pickle.loads(pickle.dumps(field_var))
 
 
 @pytest.mark.parametrize("input_index,input_type", non_parameterized_types)
 @pytest.mark.parametrize("check_index,check_type", non_parameterized_types)
 def test_non_parameterized_type_equality(
     input_index: int, input_type: Type[PrimitiveType], check_index: int, check_type: Type[PrimitiveType]
 ) -> None:
```

### Comparing `pyiceberg-0.3.0rc2/tests/test_version.py` & `pyiceberg-0.4.0rc1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_bin_packing.py` & `pyiceberg-0.4.0rc1/tests/utils/test_bin_packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ],
 )
 def test_bin_packing(splits: List[int], lookback: int, split_size: int, open_cost: int) -> None:
     def weight_func(x: int) -> int:
         return max(x, open_cost)
 
     item_list_sums: List[int] = [sum(item) for item in PackingIterator(splits, split_size, lookback, weight_func)]
-    assert all([split_size >= item_sum >= 0 for item_sum in item_list_sums])
+    assert all(split_size >= item_sum >= 0 for item_sum in item_list_sums)
 
 
 @pytest.mark.parametrize(
     "splits, target_weight, lookback, largest_bin_first, expected_lists",
     [
         (
             [36, 36, 36, 36, 73, 110, 128],
```

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_config.py` & `pyiceberg-0.4.0rc1/tests/utils/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import os
 from unittest import mock
 
 import pytest
-import yaml
+from strictyaml import as_document
 
 from pyiceberg.utils.config import Config, _lowercase_dictionary_keys
 
 EXAMPLE_ENV = {"PYICEBERG_CATALOG__PRODUCTION__URI": "https://service.io/api"}
 
 
 def test_config() -> None:
@@ -39,15 +39,16 @@
 def test_from_environment_variables_uppercase() -> None:
     assert Config().get_catalog_config("PRODUCTION") == {"uri": "https://service.io/api"}
 
 
 def test_from_configuration_files(tmp_path_factory: pytest.TempPathFactory) -> None:
     config_path = str(tmp_path_factory.mktemp("config"))
     with open(f"{config_path}/.pyiceberg.yaml", "w", encoding="utf-8") as file:
-        yaml.dump({"catalog": {"production": {"uri": "https://service.io/api"}}}, file)
+        yaml_str = as_document({"catalog": {"production": {"uri": "https://service.io/api"}}}).as_yaml()
+        file.write(yaml_str)
 
     os.environ["PYICEBERG_HOME"] = config_path
     assert Config().get_catalog_config("production") == {"uri": "https://service.io/api"}
 
 
 def test_lowercase_dictionary_keys() -> None:
     uppercase_keys = {"UPPER": {"NESTED_UPPER": {"YES"}}}
```

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_deprecated.py` & `pyiceberg-0.4.0rc1/tests/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_manifest.py` & `pyiceberg-0.4.0rc1/tests/utils/test_manifest.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,37 +15,41 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from pyiceberg.io import load_file_io
 from pyiceberg.io.pyarrow import PyArrowFileIO
 from pyiceberg.manifest import (
     DataFile,
+    DataFileContent,
     FileFormat,
+    ManifestContent,
     ManifestEntryStatus,
+    ManifestFile,
     PartitionFieldSummary,
-    read_manifest_entry,
     read_manifest_list,
 )
 from pyiceberg.table import Snapshot
 from pyiceberg.table.snapshots import Operation, Summary
 
 
 def test_read_manifest_entry(generated_manifest_entry_file: str) -> None:
-    input_file = PyArrowFileIO().new_input(location=generated_manifest_entry_file)
-    manifest_entries = list(read_manifest_entry(input_file))
+    manifest = ManifestFile(
+        manifest_path=generated_manifest_entry_file, manifest_length=0, partition_spec_id=0, sequence_number=None, partitions=[]
+    )
+    manifest_entries = manifest.fetch_manifest_entry(PyArrowFileIO())
     manifest_entry = manifest_entries[0]
 
     assert manifest_entry.status == ManifestEntryStatus.ADDED
     assert manifest_entry.snapshot_id == 8744736658442914487
-    assert manifest_entry.sequence_number is None
+    assert manifest_entry.data_sequence_number is None
     assert isinstance(manifest_entry.data_file, DataFile)
 
     data_file = manifest_entry.data_file
 
-    assert data_file.content is None
+    assert data_file.content is DataFileContent.DATA
     assert (
         data_file.file_path
         == "/home/iceberg/warehouse/nyc/taxis_partitioned/data/VendorID=null/00000-633-d8a4223e-dc97-45a1-86e1-adaba6e8abd7-00001.parquet"
     )
     assert data_file.file_format == FileFormat.PARQUET
     assert repr(data_file.partition) == "Record[VendorID=1, tpep_pickup_datetime=1925]"
     assert data_file.record_count == 19513
@@ -146,16 +150,16 @@
     }
     assert data_file.key_metadata is None
     assert data_file.split_offsets == [4]
     assert data_file.equality_ids is None
     assert data_file.sort_order_id == 0
 
 
-def test_read_manifest_list(generated_manifest_file_file: str) -> None:
-    input_file = PyArrowFileIO().new_input(generated_manifest_file_file)
+def test_read_manifest_list(generated_manifest_file_file_v1: str) -> None:
+    input_file = PyArrowFileIO().new_input(generated_manifest_file_file_v1)
     manifest_list = list(read_manifest_list(input_file))[0]
 
     assert manifest_list.manifest_length == 7989
     assert manifest_list.partition_spec_id == 0
     assert manifest_list.added_snapshot_id == 9182715666859759686
     assert manifest_list.added_files_count == 3
     assert manifest_list.existing_files_count == 0
@@ -172,32 +176,82 @@
     assert partitions_summary.upper_bound == b"\x02\x00\x00\x00"
 
     assert manifest_list.added_rows_count == 237993
     assert manifest_list.existing_rows_count == 0
     assert manifest_list.deleted_rows_count == 0
 
 
-def test_read_manifest(generated_manifest_file_file: str) -> None:
-    io = load_file_io({})
+def test_read_manifest_v1(generated_manifest_file_file_v1: str) -> None:
+    io = load_file_io()
+
+    snapshot = Snapshot(
+        snapshot_id=25,
+        parent_snapshot_id=19,
+        timestamp_ms=1602638573590,
+        manifest_list=generated_manifest_file_file_v1,
+        summary=Summary(Operation.APPEND),
+        schema_id=3,
+    )
+    manifest_list = snapshot.manifests(io)[0]
+
+    assert manifest_list.manifest_length == 7989
+    assert manifest_list.partition_spec_id == 0
+    assert manifest_list.content == ManifestContent.DATA
+    assert manifest_list.sequence_number == 0
+    assert manifest_list.min_sequence_number == 0
+    assert manifest_list.added_snapshot_id == 9182715666859759686
+    assert manifest_list.added_files_count == 3
+    assert manifest_list.existing_files_count == 0
+    assert manifest_list.deleted_files_count == 0
+    assert manifest_list.added_rows_count == 237993
+    assert manifest_list.existing_rows_count == 0
+    assert manifest_list.deleted_rows_count == 0
+    assert manifest_list.key_metadata is None
+
+    assert isinstance(manifest_list.partitions, list)
+
+    partition = manifest_list.partitions[0]
+
+    assert isinstance(partition, PartitionFieldSummary)
+
+    assert partition.contains_null is True
+    assert partition.contains_nan is False
+    assert partition.lower_bound == b"\x01\x00\x00\x00"
+    assert partition.upper_bound == b"\x02\x00\x00\x00"
+
+    entries = manifest_list.fetch_manifest_entry(io)
+
+    assert isinstance(entries, list)
+
+    entry = entries[0]
+
+    assert entry.data_sequence_number == 0
+    assert entry.file_sequence_number == 0
+    assert entry.snapshot_id == 8744736658442914487
+    assert entry.status == ManifestEntryStatus.ADDED
+
+
+def test_read_manifest_v2(generated_manifest_file_file_v2: str) -> None:
+    io = load_file_io()
 
     snapshot = Snapshot(
         snapshot_id=25,
         parent_snapshot_id=19,
         timestamp_ms=1602638573590,
-        manifest_list=generated_manifest_file_file,
+        manifest_list=generated_manifest_file_file_v2,
         summary=Summary(Operation.APPEND),
         schema_id=3,
     )
     manifest_list = snapshot.manifests(io)[0]
 
     assert manifest_list.manifest_length == 7989
     assert manifest_list.partition_spec_id == 0
-    assert manifest_list.content is None
-    assert manifest_list.sequence_number is None
-    assert manifest_list.min_sequence_number is None
+    assert manifest_list.content == ManifestContent.DELETES
+    assert manifest_list.sequence_number == 3
+    assert manifest_list.min_sequence_number == 3
     assert manifest_list.added_snapshot_id == 9182715666859759686
     assert manifest_list.added_files_count == 3
     assert manifest_list.existing_files_count == 0
     assert manifest_list.deleted_files_count == 0
     assert manifest_list.added_rows_count == 237993
     assert manifest_list.existing_rows_count == 0
     assert manifest_list.deleted_rows_count == 0
@@ -209,7 +263,18 @@
 
     assert isinstance(partition, PartitionFieldSummary)
 
     assert partition.contains_null is True
     assert partition.contains_nan is False
     assert partition.lower_bound == b"\x01\x00\x00\x00"
     assert partition.upper_bound == b"\x02\x00\x00\x00"
+
+    entries = manifest_list.fetch_manifest_entry(io)
+
+    assert isinstance(entries, list)
+
+    entry = entries[0]
+
+    assert entry.data_sequence_number == 3
+    assert entry.file_sequence_number == 3
+    assert entry.snapshot_id == 8744736658442914487
+    assert entry.status == ManifestEntryStatus.ADDED
```

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_schema_conversion.py` & `pyiceberg-0.4.0rc1/tests/utils/test_schema_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     NestedField,
     StringType,
     StructType,
 )
 from pyiceberg.utils.schema_conversion import AvroSchemaConversion
 
 
-def test_iceberg_to_avro(avro_schema_manifest_file: Dict[str, Any]) -> None:
-    iceberg_schema = AvroSchemaConversion().avro_to_iceberg(avro_schema_manifest_file)
+def test_iceberg_to_avro(avro_schema_manifest_file_v1: Dict[str, Any]) -> None:
+    iceberg_schema = AvroSchemaConversion().avro_to_iceberg(avro_schema_manifest_file_v1)
     expected_iceberg_schema = Schema(
         NestedField(
             field_id=500, name="manifest_path", field_type=StringType(), required=True, doc="Location URI with FS scheme"
         ),
         NestedField(field_id=501, name="manifest_length", field_type=LongType(), required=True, doc="Total file size in bytes"),
         NestedField(field_id=502, name="partition_spec_id", field_type=IntegerType(), required=True, doc="Spec ID used to write"),
         NestedField(
```

### Comparing `pyiceberg-0.3.0rc2/tests/utils/test_singleton.py` & `pyiceberg-0.4.0rc1/tests/utils/test_singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/fb303/FacebookService.py` & `pyiceberg-0.4.0rc1/vendor/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/fb303/__init__.py` & `pyiceberg-0.4.0rc1/vendor/fb303/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/fb303/constants.py` & `pyiceberg-0.4.0rc1/vendor/fb303/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/fb303/ttypes.py` & `pyiceberg-0.4.0rc1/vendor/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/hive_metastore/ThriftHiveMetastore.py` & `pyiceberg-0.4.0rc1/vendor/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/hive_metastore/__init__.py` & `pyiceberg-0.4.0rc1/vendor/hive_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/hive_metastore/constants.py` & `pyiceberg-0.4.0rc1/vendor/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/vendor/hive_metastore/ttypes.py` & `pyiceberg-0.4.0rc1/vendor/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.3.0rc2/PKG-INFO` & `pyiceberg-0.4.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: pyiceberg
-Version: 0.3.0rc2
+Version: 0.4.0rc1
 Summary: Apache Iceberg is an open table format for huge analytic datasets
 Home-page: https://iceberg.apache.org/
 License: Apache-2.0
 Author: Apache Software Foundation
 Author-email: dev@iceberg.apache.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: adlfs
 Provides-Extra: duckdb
+Provides-Extra: dynamodb
 Provides-Extra: glue
 Provides-Extra: hive
 Provides-Extra: pandas
 Provides-Extra: pyarrow
+Provides-Extra: ray
 Provides-Extra: s3fs
 Provides-Extra: snappy
-Requires-Dist: adlfs (==2023.1.0); extra == "adlfs"
-Requires-Dist: boto3 (==1.24.59); extra == "glue"
-Requires-Dist: click (==8.1.3)
-Requires-Dist: duckdb (==0.6.1); extra == "duckdb"
-Requires-Dist: fsspec (==2023.1.0)
-Requires-Dist: mmhash3 (==3.0.1)
-Requires-Dist: pandas (==1.5.3); extra == "pandas"
-Requires-Dist: pyarrow (==10.0.1); extra == "pyarrow" or extra == "pandas" or extra == "duckdb"
-Requires-Dist: pydantic (==1.10.4)
-Requires-Dist: pyparsing (==3.0.9)
-Requires-Dist: python-snappy (==0.6.1); extra == "snappy"
-Requires-Dist: pyyaml (==6.0.0)
-Requires-Dist: requests (==2.28.2)
-Requires-Dist: rich (==13.2.0)
-Requires-Dist: s3fs (==2023.1.0); extra == "s3fs"
-Requires-Dist: thrift (==0.16.0); extra == "hive"
-Requires-Dist: zstandard (==0.19.0)
+Provides-Extra: zstandard
+Requires-Dist: adlfs (>=2021.07.0,<2024.1.0) ; extra == "adlfs"
+Requires-Dist: boto3 (>=1.17.106) ; extra == "glue" or extra == "dynamodb"
+Requires-Dist: click (>=7.1.1,<9.0.0)
+Requires-Dist: duckdb (>=0.5.0,<1.0.0) ; extra == "duckdb"
+Requires-Dist: fsspec (>=2021.09.0,<2024.1.0)
+Requires-Dist: mmhash3 (>=3.0.0,<4.0.0)
+Requires-Dist: pandas (>=1.0.0,<3.0.0) ; extra == "pandas" or extra == "ray"
+Requires-Dist: pyarrow (>=9.0.0,<13.0.0) ; extra == "pyarrow" or extra == "pandas" or extra == "duckdb" or extra == "ray"
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pyparsing (>=3.0.7,<4.0.0)
+Requires-Dist: python-snappy (>=0.6.0,<1.0.0) ; extra == "snappy"
+Requires-Dist: ray (>=2.0.0,<3.0.0) ; extra == "ray"
+Requires-Dist: requests (>=2.20.0,<3.0.0)
+Requires-Dist: rich (>=10.11.0,<14.0.0)
+Requires-Dist: s3fs (>=2021.08.0,<2024.1.0) ; extra == "s3fs"
+Requires-Dist: sortedcontainers (==2.4.0)
+Requires-Dist: strictyaml (>=1.7.0,<2.0.0)
+Requires-Dist: thrift (>=0.13.0,<1.0.0) ; extra == "hive"
+Requires-Dist: zstandard (>=0.13.0,<1.0.0) ; extra == "zstandard"
 Project-URL: Repository, https://github.com/apache/iceberg/
 Description-Content-Type: text/markdown
 
 <!--
  - Licensed to the Apache Software Foundation (ASF) under one or more
  - contributor license agreements.  See the NOTICE file distributed with
  - this work for additional information regarding copyright ownership.
```

