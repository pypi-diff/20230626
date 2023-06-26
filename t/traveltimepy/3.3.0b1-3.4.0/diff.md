# Comparing `tmp/traveltimepy-3.3.0b1.tar.gz` & `tmp/traveltimepy-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traveltimepy-3.3.0b1.tar", last modified: Mon May 29 08:59:50 2023, max compression
+gzip compressed data, was "traveltimepy-3.4.0.tar", last modified: Mon Jun 26 13:24:29 2023, max compression
```

## Comparing `traveltimepy-3.3.0b1.tar` & `traveltimepy-3.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24259 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.537338 traveltimepy-3.3.0b1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/time_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.541339 traveltimepy-3.3.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/geocoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/map_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/postcodes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/routes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_fast_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_proto_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_map_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-29 08:59:39.000000 traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastRequest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-29 08:59:39.000000 traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastResponse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/accept_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/traveltimepy/dto/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/traveltimepy/dto/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/map_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/transportation.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/proto_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.972760 traveltimepy-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-06-26 13:24:29.972760 traveltimepy-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.964759 traveltimepy-3.4.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/benchmarks/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/benchmarks/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 13:24:29.976760 traveltimepy-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.968759 traveltimepy-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/geocoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/map_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/postcodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/routes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/time_filter_fast_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/time_filter_proto_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/time_filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/tests/time_map_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.968759 traveltimepy-3.4.0/traveltimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 13:24:17.000000 traveltimepy-3.4.0/traveltimepy/TimeFilterFastRequest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 13:24:17.000000 traveltimepy-3.4.0/traveltimepy/TimeFilterFastResponse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/accept_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.968759 traveltimepy-3.4.0/traveltimepy/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.972760 traveltimepy-3.4.0/traveltimepy/dto/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/postcodes_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/requests/time_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.972760 traveltimepy-3.4.0/traveltimepy/dto/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/responses/zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/dto/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/proto_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 13:24:11.000000 traveltimepy-3.4.0/traveltimepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:24:29.968759 traveltimepy-3.4.0/traveltimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 13:24:29.000000 traveltimepy-3.4.0/traveltimepy.egg-info/top_level.txt
```

### Comparing `traveltimepy-3.3.0b1/LICENSE` & `traveltimepy-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/PKG-INFO` & `traveltimepy-3.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: traveltimepy
-Version: 3.3.0b1
-Summary: "Python Interface to Travel Time."
-Author: TravelTime
-License: MIT
-Keywords: traveltimepy,api,maps
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Travel Time Python SDK
 
 [![PyPI version](https://badge.fury.io/py/traveltimepy.svg)](https://badge.fury.io/py/traveltimepy) [![Unit Tests](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml/badge.svg)](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml) [![Python support](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue)
 
 [Travel Time](https://docs.traveltime.com/api/overview/introduction) Python SDK helps users find locations by journey
 time rather than using ‘as the crow flies’ distance.  
 Time-based searching gives users more opportunities for personalisation and delivers a more relevant search.
@@ -61,34 +50,14 @@
 
 ```python
 from traveltimepy import TravelTimeSdk
 
 sdk = TravelTimeSdk(app_id="YOUR_APP_ID", api_key="YOUR_APP_KEY")
 ```
 
-### Synchronous calls
-
-Each method below has its own synchronous version.
-
-#### Example:
-
-```python
-from datetime import datetime
-
-from traveltimepy import Driving, Coordinates, TravelTimeSdk
-
-sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
-
-res = sdk.time_map(
-    coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
-    arrival_time=datetime.now(),
-    transportation=Driving()
-)
-```
-
 ### [Isochrones (Time Map)](https://docs.traveltime.com/api/reference/isochrones)
 
 Given origin coordinates, find shapes of zones reachable within corresponding travel time.
 
 #### Takes:
 
 * coordinates: List[Coordinates] - Isochrones coordinates.
```

### Comparing `traveltimepy-3.3.0b1/README.md` & `traveltimepy-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: traveltimepy
+Version: 3.4.0
+Summary: "Python Interface to Travel Time."
+Author: TravelTime
+License: MIT
+Keywords: traveltimepy,api,maps
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Travel Time Python SDK
 
 [![PyPI version](https://badge.fury.io/py/traveltimepy.svg)](https://badge.fury.io/py/traveltimepy) [![Unit Tests](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml/badge.svg)](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml) [![Python support](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue)
 
 [Travel Time](https://docs.traveltime.com/api/overview/introduction) Python SDK helps users find locations by journey
 time rather than using ‘as the crow flies’ distance.  
 Time-based searching gives users more opportunities for personalisation and delivers a more relevant search.
@@ -50,34 +61,14 @@
 
 ```python
 from traveltimepy import TravelTimeSdk
 
 sdk = TravelTimeSdk(app_id="YOUR_APP_ID", api_key="YOUR_APP_KEY")
 ```
 
-### Synchronous calls
-
-Each method below has its own synchronous version.
-
-#### Example:
-
-```python
-from datetime import datetime
-
-from traveltimepy import Driving, Coordinates, TravelTimeSdk
-
-sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
-
-res = sdk.time_map(
-    coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
-    arrival_time=datetime.now(),
-    transportation=Driving()
-)
-```
-
 ### [Isochrones (Time Map)](https://docs.traveltime.com/api/reference/isochrones)
 
 Given origin coordinates, find shapes of zones reachable within corresponding travel time.
 
 #### Takes:
 
 * coordinates: List[Coordinates] - Isochrones coordinates.
```

### Comparing `traveltimepy-3.3.0b1/benchmarks/common.py` & `traveltimepy-3.4.0/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/benchmarks/time_filter.py` & `traveltimepy-3.4.0/benchmarks/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/benchmarks/time_map.py` & `traveltimepy-3.4.0/benchmarks/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/setup.cfg` & `traveltimepy-3.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 	typing-extensions
 	geojson-pydantic
 	dacite
 	certifi >= 2021.5.30
 	aiohttp
 	aiolimiter
 	aiohttp-retry
-	protobuf == 3.20.3
+	protobuf == 4.21.12
 test_require = 
 	pytest
+	pytest-asyncio
 
 [flake8]
 per-file-ignores = __init__.py:F401
 max-line-length = 88
 extend-ignore = 
 	E203,
 exclude =
```

### Comparing `traveltimepy-3.3.0b1/tests/conftest.py` & `traveltimepy-3.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/tests/routes_test.py` & `traveltimepy-3.4.0/tests/routes_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+import pytest
 from datetime import datetime
 
 from traveltimepy import PublicTransport
 
 
-def test_departures(sdk, locations):
-    results = sdk.routes(
+@pytest.mark.asyncio
+async def test_departures(sdk, locations):
+    results = await sdk.routes_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
     )
     assert len(results) == 2
 
 
-def test_arrivals(sdk, locations):
-    results = sdk.routes(
+@pytest.mark.asyncio
+async def test_arrivals(sdk, locations):
+    results = await sdk.routes_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
```

### Comparing `traveltimepy-3.3.0b1/tests/supported_locations.py` & `traveltimepy-3.4.0/tests/supported_locations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import pytest
+
 from traveltimepy import Location, Coordinates
 
 
-def test_supported_locations(sdk):
+@pytest.mark.asyncio
+async def test_supported_locations(sdk):
     locations = [
         Location(id="Kaunas", coords=Coordinates(lat=54.900008, lng=23.957734)),
         Location(id="London", coords=Coordinates(lat=51.506756, lng=-0.12805)),
         Location(id="Bangkok", coords=Coordinates(lat=13.761866, lng=100.544818)),
         Location(id="Lisbon", coords=Coordinates(lat=38.721869, lng=-9.138549)),
         Location(id="Unsupported", coords=Coordinates(lat=68.721869, lng=-9.138549)),
     ]
-    response = sdk.supported_locations(locations)
+    response = await sdk.supported_locations_async(locations)
     assert len(response.locations) == 4
     assert len(response.unsupported_locations) == 1
```

### Comparing `traveltimepy-3.3.0b1/tests/time_filter_fast_test.py` & `traveltimepy-3.4.0/tests/time_filter_fast_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import pytest
+
 from traveltimepy.dto.requests.time_filter_fast import Transportation
 
 
-def test_one_to_many(sdk, locations):
-    results = sdk.time_filter_fast(
+@pytest.mark.asyncio
+async def test_one_to_many(sdk, locations):
+    results = await sdk.time_filter_fast_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=Transportation(type="public_transport"),
     )
 
     assert len(results) > 0
 
 
-def test_many_to_one(sdk, locations):
-    results = sdk.time_filter_fast(
+@pytest.mark.asyncio
+async def test_many_to_one(sdk, locations):
+    results = await sdk.time_filter_fast_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=Transportation(type="public_transport"),
         one_to_many=False,
```

### Comparing `traveltimepy-3.3.0b1/tests/time_filter_proto_test.py` & `traveltimepy-3.4.0/tests/time_filter_proto_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/tests/time_filter_test.py` & `traveltimepy-3.4.0/tests/time_filter_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+import pytest
 from datetime import datetime
 
 from traveltimepy import PublicTransport
 
 
-def test_departures(sdk, locations):
-    results = sdk.time_filter(
+@pytest.mark.asyncio
+async def test_departures(sdk, locations):
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
     )
     assert len(results) == 2
 
 
-def test_arrivals(sdk, locations):
-    results = sdk.time_filter(
+@pytest.mark.asyncio
+async def test_arrivals(sdk, locations):
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
```

### Comparing `traveltimepy-3.3.0b1/tests/time_map_test.py` & `traveltimepy-3.4.0/tests/time_map_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,58 @@
+import pytest
 from datetime import datetime
 
 from traveltimepy import Coordinates, Driving
 
 
-def test_departures(sdk):
-    results = sdk.time_map(
+@pytest.mark.asyncio
+async def test_departures(sdk):
+    results = await sdk.time_map_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
         transportation=Driving(),
     )
     assert len(results) == 2
 
 
-def test_arrivals(sdk):
-    results = sdk.time_map(
+@pytest.mark.asyncio
+async def test_arrivals(sdk):
+    results = await sdk.time_map_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
         transportation=Driving(),
     )
     assert len(results) == 2
 
 
-def test_union_departures(sdk):
-    result = sdk.union(
+@pytest.mark.asyncio
+async def test_union_departures(sdk):
+    result = await sdk.union_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
         transportation=Driving(),
     )
     assert len(result.shapes) > 0
 
 
-def test_intersection_arrivals(sdk):
-    result = sdk.intersection(
+@pytest.mark.asyncio
+async def test_intersection_arrivals(sdk):
+    result = await sdk.intersection_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
         transportation=Driving(),
```

### Comparing `traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastRequest_pb2.py` & `traveltimepy-3.4.0/traveltimepy/TimeFilterFastRequest_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastResponse_pb2.py` & `traveltimepy-3.4.0/traveltimepy/TimeFilterFastResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/__init__.py` & `traveltimepy-3.4.0/traveltimepy/__init__.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/common.py` & `traveltimepy-3.4.0/traveltimepy/dto/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/postcodes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes_zones.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/postcodes_zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/routes.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/supported_locations.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_fast.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_proto.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/time_filter_proto.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_map.py` & `traveltimepy-3.4.0/traveltimepy/dto/requests/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter.py` & `traveltimepy-3.4.0/traveltimepy/dto/responses/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_fast.py` & `traveltimepy-3.4.0/traveltimepy/dto/responses/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/responses/zones.py` & `traveltimepy-3.4.0/traveltimepy/dto/responses/zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/dto/transportation.py` & `traveltimepy-3.4.0/traveltimepy/dto/transportation.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/http.py` & `traveltimepy-3.4.0/traveltimepy/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,26 +73,14 @@
 def _window_size(rate_limit: int):
     if rate_limit >= DEFAULT_SPLIT_SIZE:
         return DEFAULT_SPLIT_SIZE
     else:
         return rate_limit
 
 
-def send_post(
-    response_class: Type[T],
-    path: str,
-    headers: Dict[str, str],
-    request: TravelTimeRequest,
-    sdk_params: SdkParams,
-) -> T:
-    return asyncio.run(
-        send_post_async(response_class, path, headers, request, sdk_params)
-    )
-
-
 async def send_get_async(
     response_class: Type[T],
     path: str,
     headers: Dict[str, str],
     sdk_params: SdkParams,
     params: Dict[str, str] = None,
 ) -> T:
@@ -105,26 +93,14 @@
                 url=f"https://{sdk_params.host}/v4/{path}",
                 headers=headers,
                 params=params,
             ) as resp:
                 return await _process_response(response_class, resp)
 
 
-def send_get(
-    response_class: Type[T],
-    path: str,
-    headers: Dict[str, str],
-    sdk_params: SdkParams,
-    params: Dict[str, str] = None,
-) -> T:
-    return asyncio.run(
-        send_get_async(response_class, path, headers, sdk_params, params)
-    )
-
-
 async def _process_response(response_class: Type[T], response: ClientResponse) -> T:
     text = await response.text()
     if response.status != 200:
         parsed = parse_raw_as(ResponseError, text)
         msg = (
             f"Travel Time API request failed: {parsed.description}\n"
             f"Error code: {parsed.error_code}\n"
```

### Comparing `traveltimepy-3.3.0b1/traveltimepy/itertools.py` & `traveltimepy-3.4.0/traveltimepy/itertools.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/mapper.py` & `traveltimepy-3.4.0/traveltimepy/mapper.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/proto_http.py` & `traveltimepy-3.4.0/traveltimepy/proto_http.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0b1/traveltimepy/sdk.py` & `traveltimepy-3.4.0/traveltimepy/sdk.py`

 * *Files 23% similar despite different names*

```diff
@@ -57,17 +57,15 @@
     create_time_map,
     create_intersection,
     create_union,
 )
 
 from traveltimepy.proto_http import send_proto, send_proto_async
 from traveltimepy.http import (
-    send_get,
     send_get_async,
-    send_post,
     send_post_async,
     SdkParams,
 )
 
 from geojson_pydantic import FeatureCollection
 
 
@@ -116,61 +114,23 @@
                 range,
             ),
             self._sdk_params,
         )
 
         return resp.results
 
-    def time_filter(
-        self,
-        locations: List[Location],
-        search_ids: Dict[str, List[str]],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        departure_time: Optional[datetime] = None,
-        arrival_time: Optional[datetime] = None,
-        properties: Optional[List[Property]] = None,
-        travel_time: int = 3600,
-        range: Optional[FullRange] = None,
-    ) -> List[TimeFilterResult]:
-        return send_post(
-            TimeFilterResponse,
-            "time-filter",
-            self._headers(AcceptType.JSON),
-            create_time_filter(
-                locations,
-                search_ids,
-                transportation,
-                properties,
-                departure_time,
-                arrival_time,
-                travel_time,
-                range,
-            ),
-            self._sdk_params,
-        ).results
-
     async def map_info_async(self) -> List[Map]:
         res = await send_get_async(
             MapInfoResponse,
             "map-info",
             self._headers(AcceptType.JSON),
             self._sdk_params,
         )
         return res.maps
 
-    def map_info(self) -> List[Map]:
-        return send_get(
-            MapInfoResponse,
-            "map-info",
-            self._headers(AcceptType.JSON),
-            self._sdk_params,
-        ).maps
-
     async def geocoding_async(
         self,
         query: str,
         limit: Optional[int] = None,
         within_countries: Optional[List[str]] = None,
         format_name: Optional[bool] = None,
         format_exclude_country: Optional[bool] = None,
@@ -187,80 +147,36 @@
                 within_countries,
                 format_name,
                 format_exclude_country,
                 bounds,
             ),
         )
 
-    def geocoding(
-        self,
-        query: str,
-        limit: Optional[int] = None,
-        within_countries: Optional[List[str]] = None,
-        format_name: Optional[bool] = None,
-        format_exclude_country: Optional[bool] = None,
-        bounds: Optional[Rectangle] = None,
-    ) -> FeatureCollection:
-        return send_get(
-            FeatureCollection,
-            "geocoding/search",
-            self._headers(AcceptType.JSON),
-            self._sdk_params,
-            self._geocoding_params(
-                query,
-                limit,
-                within_countries,
-                format_name,
-                format_exclude_country,
-                bounds,
-            ),
-        )
-
     async def geocoding_reverse_async(
         self, lat: float, lng: float
     ) -> FeatureCollection:
         return await send_get_async(
             FeatureCollection,
             "geocoding/reverse",
             self._headers(AcceptType.JSON),
             self._sdk_params,
             self._geocoding_reverse_params(lat, lng),
         )
 
-    def geocoding_reverse(self, lat: float, lng: float) -> FeatureCollection:
-        return send_get(
-            FeatureCollection,
-            "geocoding/reverse",
-            self._headers(AcceptType.JSON),
-            self._sdk_params,
-            self._geocoding_reverse_params(lat, lng),
-        )
-
     async def supported_locations_async(
         self, locations: List[Location]
     ) -> SupportedLocationsResponse:
         return await send_post_async(
             SupportedLocationsResponse,
             "supported-locations",
             self._headers(AcceptType.JSON),
             SupportedLocationsRequest(locations=locations),
             self._sdk_params,
         )
 
-    def supported_locations(
-        self, locations: List[Location]
-    ) -> SupportedLocationsResponse:
-        return send_post(
-            SupportedLocationsResponse,
-            "supported-locations",
-            self._headers(AcceptType.JSON),
-            SupportedLocationsRequest(locations=locations),
-            self._sdk_params,
-        )
-
     async def time_filter_fast_async(
         self,
         locations: List[Location],
         search_ids: Dict[str, List[str]],
         transportation: Transportation,
         travel_time: int = 3600,
         properties: Optional[List[Property]] = None,
@@ -278,38 +194,14 @@
                 properties,
                 one_to_many,
             ),
             self._sdk_params,
         )
         return resp.results
 
-    def time_filter_fast(
-        self,
-        locations: List[Location],
-        search_ids: Dict[str, List[str]],
-        transportation: Transportation,
-        travel_time: int = 3600,
-        properties: Optional[List[Property]] = None,
-        one_to_many: bool = False,
-    ) -> List[TimeFilterFastResult]:
-        return send_post(
-            TimeFilterFastResponse,
-            "time-filter/fast",
-            self._headers(AcceptType.JSON),
-            create_time_filter_fast(
-                locations,
-                search_ids,
-                transportation,
-                travel_time,
-                properties,
-                one_to_many,
-            ),
-            self._sdk_params,
-        ).results
-
     async def postcodes_async(
         self,
         coordinates: List[Coordinates],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
         departure_time: Optional[datetime] = None,
@@ -331,42 +223,14 @@
                 properties,
                 range,
             ),
             self._sdk_params,
         )
         return resp.results
 
-    def postcodes(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        departure_time: Optional[datetime] = None,
-        arrival_time: Optional[datetime] = None,
-        travel_time: int = 1800,
-        properties: Optional[List[Property]] = None,
-        range: Optional[FullRange] = None,
-    ) -> List[PostcodesResult]:
-        return send_post(
-            PostcodesResponse,
-            "time-filter/postcodes",
-            self._headers(AcceptType.JSON),
-            create_postcodes(
-                coordinates,
-                departure_time,
-                arrival_time,
-                transportation,
-                travel_time,
-                properties,
-                range,
-            ),
-            self._sdk_params,
-        ).results
-
     async def postcodes_districts_async(
         self,
         coordinates: List[Coordinates],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
         travel_time: int = 1800,
@@ -390,44 +254,14 @@
                 properties,
                 range,
             ),
             self._sdk_params,
         )
         return res.results
 
-    def postcode_districts(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        travel_time: int = 1800,
-        departure_time: Optional[datetime] = None,
-        arrival_time: Optional[datetime] = None,
-        reachable_postcodes_threshold=0.1,
-        properties: Optional[List[ZonesProperty]] = None,
-        range: Optional[FullRange] = None,
-    ) -> List[PostcodesDistrictsResult]:
-        return send_post(
-            PostcodesDistrictsResponse,
-            "time-filter/postcode-districts",
-            self._headers(AcceptType.JSON),
-            create_districts(
-                coordinates,
-                transportation,
-                travel_time,
-                departure_time,
-                arrival_time,
-                reachable_postcodes_threshold,
-                properties,
-                range,
-            ),
-            self._sdk_params,
-        ).results
-
     async def postcodes_sectors_async(
         self,
         coordinates: List[Coordinates],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
         travel_time: int = 1800,
@@ -451,72 +285,14 @@
                 properties,
                 range,
             ),
             self._sdk_params,
         )
         return resp.results
 
-    def postcode_sectors(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        travel_time: int = 1800,
-        departure_time: Optional[datetime] = None,
-        arrival_time: Optional[datetime] = None,
-        reachable_postcodes_threshold=0.1,
-        properties: Optional[List[ZonesProperty]] = None,
-        range: Optional[FullRange] = None,
-    ) -> List[PostcodesSectorsResult]:
-        return send_post(
-            PostcodesSectorsResponse,
-            "time-filter/postcode-sectors",
-            self._headers(AcceptType.JSON),
-            create_sectors(
-                coordinates,
-                transportation,
-                travel_time,
-                departure_time,
-                arrival_time,
-                reachable_postcodes_threshold,
-                properties,
-                range,
-            ),
-            self._sdk_params,
-        ).results
-
-    def routes(
-        self,
-        locations: List[Location],
-        search_ids: Dict[str, List[str]],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        departure_time: Optional[datetime] = None,
-        arrival_time: Optional[datetime] = None,
-        properties: Optional[List[Property]] = None,
-        range: Optional[FullRange] = None,
-    ) -> List[RoutesResult]:
-        return send_post(
-            RoutesResponse,
-            "routes",
-            self._headers(AcceptType.JSON),
-            create_routes(
-                locations,
-                search_ids,
-                transportation,
-                departure_time,
-                arrival_time,
-                properties,
-                range,
-            ),
-            self._sdk_params,
-        ).results
-
     async def routes_async(
         self,
         locations: List[Location],
         search_ids: Dict[str, List[str]],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
@@ -571,66 +347,14 @@
             self._proto_headers(),
             create_proto_request(origin, destinations, transportation, travel_time),
             self._app_id,
             self._api_key,
         )
         return resp.travel_times
 
-    def time_map(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        arrival_time: Optional[datetime] = None,
-        departure_time: Optional[datetime] = None,
-        travel_time: int = 3600,
-        search_range: Optional[Range] = None,
-    ) -> List[TimeMapResult]:
-        return send_post(
-            TimeMapResponse,
-            "time-map",
-            self._headers(AcceptType.JSON),
-            create_time_map(
-                coordinates,
-                transportation,
-                travel_time,
-                arrival_time,
-                departure_time,
-                search_range,
-            ),
-            self._sdk_params,
-        ).results
-
-    def intersection(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        arrival_time: Optional[datetime] = None,
-        departure_time: Optional[datetime] = None,
-        travel_time: int = 3600,
-        search_range: Optional[Range] = None,
-    ) -> TimeMapResult:
-        return send_post(
-            TimeMapResponse,
-            "time-map",
-            self._headers(AcceptType.JSON),
-            create_intersection(
-                coordinates,
-                transportation,
-                travel_time,
-                arrival_time,
-                departure_time,
-                search_range,
-            ),
-            self._sdk_params,
-        ).results[0]
-
     async def intersection_async(
         self,
         coordinates: List[Coordinates],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
         arrival_time: Optional[datetime] = None,
@@ -650,40 +374,14 @@
                 departure_time,
                 search_range,
             ),
             self._sdk_params,
         )
         return resp.results[0]
 
-    def union(
-        self,
-        coordinates: List[Coordinates],
-        transportation: Union[
-            PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
-        ],
-        arrival_time: Optional[datetime] = None,
-        departure_time: Optional[datetime] = None,
-        travel_time: int = 3600,
-        search_range: Optional[Range] = None,
-    ) -> TimeMapResult:
-        return send_post(
-            TimeMapResponse,
-            "time-map",
-            self._headers(AcceptType.JSON),
-            create_union(
-                coordinates,
-                transportation,
-                travel_time,
-                arrival_time,
-                departure_time,
-                search_range,
-            ),
-            self._sdk_params,
-        ).results[0]
-
     async def union_async(
         self,
         coordinates: List[Coordinates],
         transportation: Union[
             PublicTransport, Driving, Ferry, Walking, Cycling, DrivingTrain
         ],
         arrival_time: Optional[datetime] = None,
```

### Comparing `traveltimepy-3.3.0b1/traveltimepy.egg-info/PKG-INFO` & `traveltimepy-3.4.0/traveltimepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.3.0b1
+Version: 3.4.0
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,34 +61,14 @@
 
 ```python
 from traveltimepy import TravelTimeSdk
 
 sdk = TravelTimeSdk(app_id="YOUR_APP_ID", api_key="YOUR_APP_KEY")
 ```
 
-### Synchronous calls
-
-Each method below has its own synchronous version.
-
-#### Example:
-
-```python
-from datetime import datetime
-
-from traveltimepy import Driving, Coordinates, TravelTimeSdk
-
-sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
-
-res = sdk.time_map(
-    coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
-    arrival_time=datetime.now(),
-    transportation=Driving()
-)
-```
-
 ### [Isochrones (Time Map)](https://docs.traveltime.com/api/reference/isochrones)
 
 Given origin coordinates, find shapes of zones reachable within corresponding travel time.
 
 #### Takes:
 
 * coordinates: List[Coordinates] - Isochrones coordinates.
```

### Comparing `traveltimepy-3.3.0b1/traveltimepy.egg-info/SOURCES.txt` & `traveltimepy-3.4.0/traveltimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

