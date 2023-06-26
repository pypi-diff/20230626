# Comparing `tmp/elementpath-4.1.3.tar.gz` & `tmp/elementpath-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementpath-4.1.3.tar", last modified: Sat Jun 17 17:41:47 2023, max compression
+gzip compressed data, was "elementpath-4.1.4.tar", last modified: Mon Jun 26 14:00:36 2023, max compression
```

## Comparing `elementpath-4.1.3.tar` & `elementpath-4.1.4.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.490959 elementpath-4.1.3/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.3/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15969 2023-06-17 17:40:45.000000 elementpath-4.1.3/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.3/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.3/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-17 17:41:47.490959 elementpath-4.1.3/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:55:05.000000 elementpath-4.1.3/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.479959 elementpath-4.1.3/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.3/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.3/doc/advanced.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-06-17 17:40:45.000000 elementpath-4.1.3/doc/conf.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.3/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.3/doc/introduction.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.3/doc/make.bat
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.3/doc/pratt_api.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.3/doc/xpath_api.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.481959 elementpath-4.1.3/elementpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-06-17 17:40:45.000000 elementpath-4.1.3/elementpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.3/elementpath/collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.3/elementpath/compare.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.483959 elementpath-4.1.3/elementpath/datatypes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/datatypes/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.3/elementpath/datatypes/atomic_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/binary.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/datatypes/datetime.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/numeric.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/proxies.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/qname.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/string.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/untyped.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.3/elementpath/datatypes/uri.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.3/elementpath/protocols.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.3/elementpath/py.typed
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/regex/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.3/elementpath/regex/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.3/elementpath/regex/character_classes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.3/elementpath/regex/codepoints.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/regex/generate_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/regex/patterns.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.3/elementpath/regex/unicode_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/regex/unicode_subsets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17185 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35099 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/tdop.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    12572 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/tree_builders.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/validators/analyze-string.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/validators/schema-for-json.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/xpath1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.3/elementpath/xpath1/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_axes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28752 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/xpath1/xpath1_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.485959 elementpath-4.1.3/elementpath/xpath2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.3/elementpath/xpath2/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.486959 elementpath-4.1.3/elementpath/xpath30/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.3/elementpath/xpath30/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.3/elementpath/xpath30/_translation_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67943 2023-06-17 17:40:45.000000 elementpath-4.1.3/elementpath/xpath30/_xpath30_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath30/_xpath30_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/xpath30/xpath30_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath30/xpath30_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.486959 elementpath-4.1.3/elementpath/xpath31/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.3/elementpath/xpath31/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath31/_xpath31_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath31/_xpath31_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/xpath31/xpath31_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30076 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_tokens.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.482959 elementpath-4.1.3/elementpath.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3478 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/SOURCES.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/dependency_links.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/requires.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/top_level.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.3/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-04-28 13:30:35.000000 elementpath-4.1.3/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-06-17 17:41:47.490959 elementpath-4.1.3/setup.cfg
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2346 2023-06-17 17:40:45.000000 elementpath-4.1.3/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.489959 elementpath-4.1.3/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.3/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/execute_w3c_tests.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/memory_profiling.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.489959 elementpath-4.1.3/tests/mypy_tests/
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2023-05-05 12:45:43.000000 elementpath-4.1.3/tests/mypy_tests/selectors.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.490959 elementpath-4.1.3/tests/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.3/tests/resources/analyze-string.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.3/tests/resources/sample.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/resources/schema-for-json.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unused_external_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unused_unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_compare.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_datatypes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.3/tests/test_elementpath.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.3/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_regex.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_schema_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3793 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15434 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17460 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16558 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_tdop_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7919 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_tree_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1446 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_typing.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_validators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    84397 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_xpath1_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.3/tests/test_xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    60913 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_xpath30.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_xpath31.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/test_xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17766 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-04-26 14:25:47.000000 elementpath-4.1.3/tests/test_xpath_tokens.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    12175 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/xpath_test_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1592 2023-06-17 17:40:45.000000 elementpath-4.1.3/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.329744 elementpath-4.1.4/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.4/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16193 2023-06-26 13:59:50.000000 elementpath-4.1.4/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.4/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.4/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-26 14:00:36.329744 elementpath-4.1.4/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:55:05.000000 elementpath-4.1.4/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.299744 elementpath-4.1.4/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.4/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.4/doc/advanced.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-06-26 13:59:50.000000 elementpath-4.1.4/doc/conf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.4/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.4/doc/introduction.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.4/doc/make.bat
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.4/doc/pratt_api.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.4/doc/xpath_api.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.304744 elementpath-4.1.4/elementpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-06-26 13:59:50.000000 elementpath-4.1.4/elementpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.4/elementpath/collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.4/elementpath/compare.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.309744 elementpath-4.1.4/elementpath/datatypes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/datatypes/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.4/elementpath/datatypes/atomic_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6007 2023-06-26 13:59:50.000000 elementpath-4.1.4/elementpath/datatypes/binary.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/datatypes/datetime.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/datatypes/numeric.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/datatypes/proxies.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/datatypes/qname.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/datatypes/string.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/datatypes/untyped.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.4/elementpath/datatypes/uri.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.4/elementpath/protocols.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.4/elementpath/py.typed
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.310744 elementpath-4.1.4/elementpath/regex/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.4/elementpath/regex/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.4/elementpath/regex/character_classes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.4/elementpath/regex/codepoints.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/regex/generate_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/regex/patterns.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.4/elementpath/regex/unicode_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.4/elementpath/regex/unicode_subsets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17185 2023-04-28 14:38:26.000000 elementpath-4.1.4/elementpath/serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35099 2023-04-28 14:38:26.000000 elementpath-4.1.4/elementpath/tdop.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12572 2023-04-28 14:38:26.000000 elementpath-4.1.4/elementpath/tree_builders.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.311744 elementpath-4.1.4/elementpath/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.4/elementpath/validators/analyze-string.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.4/elementpath/validators/schema-for-json.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.314744 elementpath-4.1.4/elementpath/xpath1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.4/elementpath/xpath1/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath1/_xpath1_axes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath1/_xpath1_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28770 2023-06-26 13:59:50.000000 elementpath-4.1.4/elementpath/xpath1/_xpath1_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/xpath1/xpath1_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.316744 elementpath-4.1.4/elementpath/xpath2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.4/elementpath/xpath2/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath2/_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath2/_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath2/_xpath2_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-06-26 06:57:51.000000 elementpath-4.1.4/elementpath/xpath2/xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.4/elementpath/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.317744 elementpath-4.1.4/elementpath/xpath30/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.4/elementpath/xpath30/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.4/elementpath/xpath30/_translation_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67943 2023-06-17 17:40:45.000000 elementpath-4.1.4/elementpath/xpath30/_xpath30_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath30/_xpath30_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.4/elementpath/xpath30/xpath30_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath30/xpath30_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.318744 elementpath-4.1.4/elementpath/xpath31/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.4/elementpath/xpath31/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath31/_xpath31_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath31/_xpath31_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.4/elementpath/xpath31/xpath31_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30076 2023-04-28 14:38:26.000000 elementpath-4.1.4/elementpath/xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.4/elementpath/xpath_tokens.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.306744 elementpath-4.1.4/elementpath.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-26 14:00:36.000000 elementpath-4.1.4/elementpath.egg-info/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3478 2023-06-26 14:00:36.000000 elementpath-4.1.4/elementpath.egg-info/SOURCES.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-06-26 14:00:36.000000 elementpath-4.1.4/elementpath.egg-info/dependency_links.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-06-26 14:00:36.000000 elementpath-4.1.4/elementpath.egg-info/requires.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-06-26 14:00:36.000000 elementpath-4.1.4/elementpath.egg-info/top_level.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.4/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-04-28 13:30:35.000000 elementpath-4.1.4/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-06-26 14:00:36.329744 elementpath-4.1.4/setup.cfg
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2346 2023-06-26 13:59:50.000000 elementpath-4.1.4/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.326744 elementpath-4.1.4/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.4/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.4/tests/execute_w3c_tests.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/memory_profiling.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.327744 elementpath-4.1.4/tests/mypy_tests/
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2023-05-05 12:45:43.000000 elementpath-4.1.4/tests/mypy_tests/selectors.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-26 14:00:36.328744 elementpath-4.1.4/tests/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.4/tests/resources/analyze-string.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.4/tests/resources/sample.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/resources/schema-for-json.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/resources/unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/resources/unused_external_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/resources/unused_unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/test_collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.4/tests/test_compare.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86452 2023-06-26 13:59:50.000000 elementpath-4.1.4/tests/test_datatypes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.4/tests/test_elementpath.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.4/tests/test_etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.4/tests/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.4/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.4/tests/test_namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.4/tests/test_regex.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/test_schema_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/test_schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3793 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15434 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17460 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16558 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_tdop_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7919 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_tree_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1446 2023-06-17 17:40:45.000000 elementpath-4.1.4/tests/test_typing.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.4/tests/test_validators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    84397 2023-06-17 17:40:45.000000 elementpath-4.1.4/tests/test_xpath1_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34479 2023-06-26 13:59:50.000000 elementpath-4.1.4/tests/test_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.4/tests/test_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.4/tests/test_xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60913 2023-06-17 17:40:45.000000 elementpath-4.1.4/tests/test_xpath30.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.4/tests/test_xpath31.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.4/tests/test_xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17766 2023-04-28 14:38:26.000000 elementpath-4.1.4/tests/test_xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-04-26 14:25:47.000000 elementpath-4.1.4/tests/test_xpath_tokens.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12175 2023-06-17 17:40:45.000000 elementpath-4.1.4/tests/xpath_test_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1592 2023-06-26 13:59:50.000000 elementpath-4.1.4/tox.ini
```

### Comparing `elementpath-4.1.3/CHANGELOG.rst` & `elementpath-4.1.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v4.1.4`_ (2023-06-26)
+======================
+* Fix select of prefixed names (issue #68)
+* Fix zero length *xs:base64Binary* (pull request #69)
+
 `v4.1.3`_ (2023-06-17)
 ======================
 * Fix XP30+ fn:path (issue #67)
 * Fix weak tests (issues #64 and #66)
 
 `v4.1.2`_ (2023-04-28)
 ======================
@@ -420,7 +425,8 @@
 .. _v3.0.2: https://github.com/sissaschool/elementpath/compare/v3.0.1...v3.0.2
 .. _v4.0.0: https://github.com/sissaschool/elementpath/compare/v3.0.2...v4.0.0
 .. _v4.0.1: https://github.com/sissaschool/elementpath/compare/v4.0.0...v4.0.1
 .. _v4.1.0: https://github.com/sissaschool/elementpath/compare/v4.0.1...v4.1.0
 .. _v4.1.1: https://github.com/sissaschool/elementpath/compare/v4.1.0...v4.1.1
 .. _v4.1.2: https://github.com/sissaschool/elementpath/compare/v4.1.1...v4.1.2
 .. _v4.1.3: https://github.com/sissaschool/elementpath/compare/v4.1.2...v4.1.3
+.. _v4.1.4: https://github.com/sissaschool/elementpath/compare/v4.1.3...v4.1.4
```

### Comparing `elementpath-4.1.3/LICENSE` & `elementpath-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/PKG-INFO` & `elementpath-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.3
+Version: 4.1.4
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `elementpath-4.1.3/README.rst` & `elementpath-4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/doc/Makefile` & `elementpath-4.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/doc/advanced.rst` & `elementpath-4.1.4/doc/advanced.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/doc/conf.py` & `elementpath-4.1.4/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = 'elementpath'
 copyright = '2018-2023, SISSA (International School for Advanced Studies)'
 author = 'Davide Brunato'
 
 # The short X.Y version
 version = '4.1'
 # The full version, including alpha/beta/rc tags
-release = '4.1.3'
+release = '4.1.4'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `elementpath-4.1.3/doc/make.bat` & `elementpath-4.1.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/doc/pratt_api.rst` & `elementpath-4.1.4/doc/pratt_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/doc/xpath_api.rst` & `elementpath-4.1.4/doc/xpath_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/__init__.py` & `elementpath-4.1.4/elementpath/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-__version__ = '4.1.3'
+__version__ = '4.1.4'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2018-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 # Imports here are considered as stable API, other internal calls may change.
```

### Comparing `elementpath-4.1.3/elementpath/collations.py` & `elementpath-4.1.4/elementpath/collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/compare.py` & `elementpath-4.1.4/elementpath/compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/__init__.py` & `elementpath-4.1.4/elementpath/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/atomic_types.py` & `elementpath-4.1.4/elementpath/datatypes/atomic_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/binary.py` & `elementpath-4.1.4/elementpath/datatypes/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,22 @@
     def __str__(self) -> str:
         return self.value.decode('utf-8')
 
     def __hash__(self) -> int:
         return hash(self.value)
 
     def __len__(self) -> int:
-        if self.value[-2] == ord('='):
-            return len(self.value) // 4 * 3 - 2
+        length = len(self.value)
+        if length == 0:
+            return 0
+        elif self.value[-2] == ord('='):
+            return length // 4 * 3 - 2
         elif self.value[-1] == ord('='):
-            return len(self.value) // 4 * 3 - 1
-        return len(self.value) // 4 * 3
+            return length // 4 * 3 - 1
+        return length // 4 * 3
 
     @staticmethod
     def encoder(value: bytes) -> bytes:
         return codecs.encode(value, 'base64').rstrip(b'\n')
 
     def decode(self) -> bytes:
         return codecs.decode(self.value, 'base64')
```

### Comparing `elementpath-4.1.3/elementpath/datatypes/datetime.py` & `elementpath-4.1.4/elementpath/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/numeric.py` & `elementpath-4.1.4/elementpath/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/proxies.py` & `elementpath-4.1.4/elementpath/datatypes/proxies.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/qname.py` & `elementpath-4.1.4/elementpath/datatypes/qname.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/string.py` & `elementpath-4.1.4/elementpath/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/untyped.py` & `elementpath-4.1.4/elementpath/datatypes/untyped.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/datatypes/uri.py` & `elementpath-4.1.4/elementpath/datatypes/uri.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/etree.py` & `elementpath-4.1.4/elementpath/etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/exceptions.py` & `elementpath-4.1.4/elementpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/helpers.py` & `elementpath-4.1.4/elementpath/helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/namespaces.py` & `elementpath-4.1.4/elementpath/namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/protocols.py` & `elementpath-4.1.4/elementpath/protocols.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/__init__.py` & `elementpath-4.1.4/elementpath/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/character_classes.py` & `elementpath-4.1.4/elementpath/regex/character_classes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/codepoints.py` & `elementpath-4.1.4/elementpath/regex/codepoints.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/generate_categories.py` & `elementpath-4.1.4/elementpath/regex/generate_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/patterns.py` & `elementpath-4.1.4/elementpath/regex/patterns.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/unicode_categories.py` & `elementpath-4.1.4/elementpath/regex/unicode_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/regex/unicode_subsets.py` & `elementpath-4.1.4/elementpath/regex/unicode_subsets.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/schema_proxy.py` & `elementpath-4.1.4/elementpath/schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/sequence_types.py` & `elementpath-4.1.4/elementpath/sequence_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/serialization.py` & `elementpath-4.1.4/elementpath/serialization.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/tdop.py` & `elementpath-4.1.4/elementpath/tdop.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/tree_builders.py` & `elementpath-4.1.4/elementpath/tree_builders.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/validators/__init__.py` & `elementpath-4.1.4/elementpath/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/validators/analyze-string.xsd` & `elementpath-4.1.4/elementpath/validators/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/validators/schema-for-json.xsd` & `elementpath-4.1.4/elementpath/validators/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath1/_xpath1_axes.py` & `elementpath-4.1.4/elementpath/xpath1/_xpath1_axes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath1/_xpath1_functions.py` & `elementpath-4.1.4/elementpath/xpath1/_xpath1_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath1/_xpath1_operators.py` & `elementpath-4.1.4/elementpath/xpath1/_xpath1_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
         if self[0].value == '*':
             name = '*:%s' % self[1].value
         else:
             name = '{%s}%s' % (self.get_namespace(self[0].value), self[1].value)
 
         if context is None:
-            yield name
+            raise self.missing_context()
         elif isinstance(context, XPathSchemaContext):
             yield from self.select_xsd_nodes(context, name)
 
         elif self.xsd_types is self.parser.schema:
             for item in context.iter_children_or_self():
                 if item.match_name(name):
                     yield item
```

### Comparing `elementpath-4.1.3/elementpath/xpath1/xpath1_parser.py` & `elementpath-4.1.4/elementpath/xpath1/xpath1_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath2/__init__.py` & `elementpath-4.1.4/elementpath/xpath2/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath2/_xpath2_constructors.py` & `elementpath-4.1.4/elementpath/xpath2/_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath2/_xpath2_functions.py` & `elementpath-4.1.4/elementpath/xpath2/_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath2/_xpath2_operators.py` & `elementpath-4.1.4/elementpath/xpath2/_xpath2_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath2/xpath2_parser.py` & `elementpath-4.1.4/elementpath/xpath2/xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/__init__.py` & `elementpath-4.1.4/elementpath/xpath30/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/_translation_maps.py` & `elementpath-4.1.4/elementpath/xpath30/_translation_maps.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/_xpath30_functions.py` & `elementpath-4.1.4/elementpath/xpath30/_xpath30_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/_xpath30_operators.py` & `elementpath-4.1.4/elementpath/xpath30/_xpath30_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/xpath30_helpers.py` & `elementpath-4.1.4/elementpath/xpath30/xpath30_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath30/xpath30_parser.py` & `elementpath-4.1.4/elementpath/xpath30/xpath30_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath31/__init__.py` & `elementpath-4.1.4/elementpath/xpath31/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath31/_xpath31_functions.py` & `elementpath-4.1.4/elementpath/xpath31/_xpath31_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath31/_xpath31_operators.py` & `elementpath-4.1.4/elementpath/xpath31/_xpath31_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath31/xpath31_parser.py` & `elementpath-4.1.4/elementpath/xpath31/xpath31_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath_context.py` & `elementpath-4.1.4/elementpath/xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath_nodes.py` & `elementpath-4.1.4/elementpath/xpath_nodes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath_selectors.py` & `elementpath-4.1.4/elementpath/xpath_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath/xpath_tokens.py` & `elementpath-4.1.4/elementpath/xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/elementpath.egg-info/PKG-INFO` & `elementpath-4.1.4/elementpath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.3
+Version: 4.1.4
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `elementpath-4.1.3/elementpath.egg-info/SOURCES.txt` & `elementpath-4.1.4/elementpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/setup.py` & `elementpath-4.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='elementpath',
-    version='4.1.3',
+    version='4.1.4',
     packages=find_packages(include=['elementpath', 'elementpath.*']),
     package_data={
         'elementpath': ['py.typed'],
         'elementpath.validators': ['analyze-string.xsd', 'schema-for-json.xsd'],
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
```

### Comparing `elementpath-4.1.3/tests/execute_w3c_tests.py` & `elementpath-4.1.4/tests/execute_w3c_tests.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/memory_profiling.py` & `elementpath-4.1.4/tests/memory_profiling.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/resources/analyze-string.xsd` & `elementpath-4.1.4/tests/resources/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/resources/schema-for-json.xsd` & `elementpath-4.1.4/tests/resources/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_collations.py` & `elementpath-4.1.4/tests/test_collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_compare.py` & `elementpath-4.1.4/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_datatypes.py` & `elementpath-4.1.4/tests/test_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1436,15 +1436,16 @@
         self.assertEqual(str(HexBinary(b'F859')), 'F859')
 
     def test_hash_value(self):
         self.assertEqual(hash(Base64Binary(b'YWxwaGE=')), hash(b'YWxwaGE='))
         self.assertEqual(hash(HexBinary(b'F859')), hash(b'F859'))
 
     def test_length(self):
-        self.assertEqual(len(Base64Binary(b'ZQ==')), 1)
+        self.assertEqual(len(Base64Binary(b'')), 0)
+        self.assertEqual(len(Base64Binary(b'ZQ==')), 1),
         self.assertEqual(len(Base64Binary(b'YWxwaGE=')), 5)
         self.assertEqual(len(Base64Binary(b'bGNlbmdnamh4eXBy')), 12)
         self.assertEqual(len(HexBinary(b'F859')), 2)
 
     def test_equality(self):
         self.assertEqual(HexBinary(b'8A7F'), HexBinary(b'8A7F'))
         self.assertEqual(HexBinary(b'8a7f'), HexBinary(b'8a7f'))
```

### Comparing `elementpath-4.1.3/tests/test_elementpath.py` & `elementpath-4.1.4/tests/test_elementpath.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_etree.py` & `elementpath-4.1.4/tests/test_etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_exceptions.py` & `elementpath-4.1.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_helpers.py` & `elementpath-4.1.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_namespaces.py` & `elementpath-4.1.4/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_package.py` & `elementpath-4.1.4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_regex.py` & `elementpath-4.1.4/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_schema_context.py` & `elementpath-4.1.4/tests/test_schema_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_schema_proxy.py` & `elementpath-4.1.4/tests/test_schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_selectors.py` & `elementpath-4.1.4/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_sequence_types.py` & `elementpath-4.1.4/tests/test_sequence_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_serialization.py` & `elementpath-4.1.4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_tdop_parser.py` & `elementpath-4.1.4/tests/test_tdop_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_tree_builders.py` & `elementpath-4.1.4/tests/test_tree_builders.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_typing.py` & `elementpath-4.1.4/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_validators.py` & `elementpath-4.1.4/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath1_parser.py` & `elementpath-4.1.4/tests/test_xpath1_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath2_constructors.py` & `elementpath-4.1.4/tests/test_xpath2_constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from decimal import Decimal
 
 try:
     import lxml.etree as lxml_etree
 except ImportError:
     lxml_etree = None
 
-from elementpath import XPathContext, AttributeNode
+from elementpath import XPathContext, AttributeNode, select
 from elementpath.datatypes import Timezone, DateTime10, DateTime, DateTimeStamp, \
     GregorianDay, GregorianMonth, GregorianMonthDay, GregorianYear10, GregorianYearMonth10, \
     Duration, YearMonthDuration, DayTimeDuration, Date10, Time, QName, UntypedAtomic, \
     Base64Binary, HexBinary
 from elementpath.namespaces import XSD_NAMESPACE
 from elementpath.xpath_tokens import XPathConstructor
 
@@ -698,14 +698,33 @@
     def test_notation_constructor(self):
         self.wrong_type('xs:NOTATION()', 'XPST0017')
         self.wrong_type('xs:NOTATION(()', 'XPST0017')
         self.wrong_type('xs:NOTATION(())', 'XPST0017',
                         'no constructor function exists for xs:NOTATION')
         self.wrong_name('"A120" castable as xs:NOTATION', 'XPST0080')
 
+    def test_missing_context_on_namespaced_name__issue_068(self):
+        namespaces = {
+            'test': "urn:example:names:common-test-names"
+        }
+
+        root = self.etree.XML("""
+        <A xmlns:test="urn:example:names:common-test-names">
+            <B>
+                <test:number>1</test:number>
+            </B>
+        </A>
+        """)
+
+        context_node = select(root, "B", namespaces=namespaces)[0]
+        result = select(root, "xs:decimal(./test:number)", namespaces, item=context_node)
+        self.assertEqual(result, 1)
+        result = select(root, "xs:decimal(test:number)", namespaces, item=context_node)
+        self.assertEqual(result, 1)
+
 
 @unittest.skipIf(lxml_etree is None, "The lxml library is not installed")
 class LxmlXPath2ConstructorsTest(XPath2ConstructorsTest):
     etree = lxml_etree
 
 
 if __name__ == '__main__':
```

### Comparing `elementpath-4.1.3/tests/test_xpath2_functions.py` & `elementpath-4.1.4/tests/test_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath2_parser.py` & `elementpath-4.1.4/tests/test_xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath30.py` & `elementpath-4.1.4/tests/test_xpath30.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath31.py` & `elementpath-4.1.4/tests/test_xpath31.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath_context.py` & `elementpath-4.1.4/tests/test_xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath_nodes.py` & `elementpath-4.1.4/tests/test_xpath_nodes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/test_xpath_tokens.py` & `elementpath-4.1.4/tests/test_xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tests/xpath_test_class.py` & `elementpath-4.1.4/tests/xpath_test_class.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.3/tox.ini` & `elementpath-4.1.4/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     flake8
 commands =
     flake8 elementpath
     flake8 tests
 
 [testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.3.0
+    mypy==1.4.1
     xmlschema
     lxml-stubs
 commands =
     mypy --strict elementpath
     python tests/test_typing.py
 
 [testenv:coverage]
```

