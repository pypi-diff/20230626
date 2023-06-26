# Comparing `tmp/ocdskit-1.1.7.tar.gz` & `tmp/ocdskit-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdskit-1.1.7.tar", last modified: Tue Jun 13 19:23:57 2023, max compression
+gzip compressed data, was "ocdskit-1.1.8.tar", last modified: Mon Jun 26 20:40:52 2023, max compression
```

## Comparing `ocdskit-1.1.7.tar` & `ocdskit-1.1.8.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.398697 ocdskit-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-13 19:23:48.000000 ocdskit-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-13 19:23:48.000000 ocdskit-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-13 19:23:57.398697 ocdskit-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 19:23:48.000000 ocdskit-1.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.362697 ocdskit-1.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.366697 ocdskit-1.1.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/combine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/mapping_sheet.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/packager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/upgrade.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.366697 ocdskit-1.1.7/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/cli/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/cli/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/cli/ocds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/cli/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 19:23:48.000000 ocdskit-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.366697 ocdskit-1.1.7/ocdskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.370697 ocdskit-1.1.7/ocdskit/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/combine_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/combine_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/package_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/package_releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/schema_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/schema_strict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/set_closed_codelist_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/split_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/split_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-06-13 19:23:48.000000 ocdskit-1.1.7/ocdskit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.366697 ocdskit-1.1.7/ocdskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 19:23:57.000000 ocdskit-1.1.7/ocdskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 19:23:48.000000 ocdskit-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 19:23:57.398697 ocdskit-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.370697 ocdskit-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.374697 ocdskit-1.1.7/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)   109677 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/cassettes/test_combine-test_merge_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  3538926 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/cassettes/test_combine-test_merge_with_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81406 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/cassettes/test_packager-test_output_package_no_streaming.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.378697 ocdskit-1.1.7/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.382697 ocdskit-1.1.7/tests/commands/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)   108359 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)   110211 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_combine_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_combine_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_package_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_package_releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_schema_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_schema_strict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_set_closed_codelist_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_split_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_split_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/commands/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.394697 ocdskit-1.1.7/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.394697 ocdskit-1.1.7/tests/fixtures/bods/
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/bods/components.json
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/bods/person-statement.json
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/combine-record-packages_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/combine-release-packages_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/compile_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/compile_no-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/compile_warning.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_false.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_mixed.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_number.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_true.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/detect-format_whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/encoding_ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/encoding_utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_bods.csv
--rw-r--r--   0 runner    (1001) docker     (123)   165693 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_codelist.csv
--rw-r--r--   0 runner    (1001) docker     (123)   164755 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension-field.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173802 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension.csv
--rw-r--r--   0 runner    (1001) docker     (123)   174656 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170180 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_array.csv
--rw-r--r--   0 runner    (1001) docker     (123)   177039 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_language.csv
--rw-r--r--   0 runner    (1001) docker     (123)   177811 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_location.csv
--rw-r--r--   0 runner    (1001) docker     (123)   174640 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv
--rw-r--r--   0 runner    (1001) docker     (123)    95829 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_no-deprecated.csv
--rw-r--r--   0 runner    (1001) docker     (123)    67545 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_oc4ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_order-by.csv
--rw-r--r--   0 runner    (1001) docker     (123)    67509 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/mapping-sheet_sedl.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/ocds-sample-data.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)    56591 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/project-schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:23:57.398697 ocdskit-1.1.7/tests/fixtures/realdata/
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/compile_encoding_encoding.json
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/compiled-release-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/compiled-release-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_linked-releases.json
--rw-r--r--   0 runner    (1001) docker     (123)    54140 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_package.json
--rw-r--r--   0 runner    (1001) docker     (123)    55971 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_package_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_record-package.json
--rw-r--r--   0 runner    (1001) docker     (123)    54149 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_split.json
--rw-r--r--   0 runner    (1001) docker     (123)   111387 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/record-package_versioned.json
--rw-r--r--   0 runner    (1001) docker     (123)    36724 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.0-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.0-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.1-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_encoding-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_record-package.json
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/release-package_split.json
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/versioned-release-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/realdata/versioned-release-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_maximal.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_minimal-1-2-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_minimal-1-2-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_minimal-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_minimal-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record-package_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record_minimal-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record_minimal-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/record_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_additional-contact-points.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_maximal.json
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_minimal-1-2-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_minimal-1-2-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_minimal-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_minimal-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_unknown-version.json
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_url-error.json
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_url-timeout.json
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_urls.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-package_warning.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-packages.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-packages.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    88734 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_minimal-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_minimal-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/release_minimal_pretty.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/schema-strict.json
--rw-r--r--   0 runner    (1001) docker     (123)    62362 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/sedl-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/fixtures/test-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/test_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-13 19:23:48.000000 ocdskit-1.1.7/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.717928 ocdskit-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 20:40:43.000000 ocdskit-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 20:40:43.000000 ocdskit-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-26 20:40:52.717928 ocdskit-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-26 20:40:43.000000 ocdskit-1.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/combine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/mapping_sheet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/packager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/ocds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/ocdskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/ocdskit/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/combine_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/combine_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/package_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/package_releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/schema_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/schema_strict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/set_closed_codelist_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/split_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/split_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/ocdskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 20:40:43.000000 ocdskit-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 20:40:52.717928 ocdskit-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.693928 ocdskit-1.1.8/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)   109677 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  3538926 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_with_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81406 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_packager-test_output_package_no_streaming.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.697928 ocdskit-1.1.8/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.701928 ocdskit-1.1.8/tests/commands/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   108359 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   110211 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_combine_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_combine_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_package_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_package_releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_schema_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_schema_strict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_set_closed_codelist_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_split_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_split_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.713928 ocdskit-1.1.8/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.713928 ocdskit-1.1.8/tests/fixtures/bods/
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/bods/components.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/bods/person-statement.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_no-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_warning.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_false.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_mixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_number.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_true.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/encoding_ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/encoding_utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_bods.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   165693 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   164755 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension-field.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   173802 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   174656 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170180 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_array.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   177039 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_language.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   177811 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_location.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   174640 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    95829 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_no-deprecated.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    67545 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_oc4ids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_order-by.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    67509 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_sedl.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/ocds-sample-data.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    56591 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/project-schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.717928 ocdskit-1.1.8/tests/fixtures/realdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compile_encoding_encoding.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_linked-releases.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54140 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55971 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_package_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_record-package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54149 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_split.json
+-rw-r--r--   0 runner    (1001) docker     (123)   111387 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_versioned.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36724 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_record-package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_split.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_maximal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_additional-contact-points.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_maximal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_unknown-version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_url-error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_url-timeout.json
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_urls.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_warning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-packages.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    88734 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal_pretty.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/schema-strict.json
+-rw-r--r--   0 runner    (1001) docker     (123)    62362 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/sedl-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/test-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_util.py
```

### Comparing `ocdskit-1.1.7/LICENSE` & `ocdskit-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/PKG-INFO` & `ocdskit-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdskit
-Version: 1.1.7
+Version: 1.1.8
 Summary: A suite of command-line tools for working with OCDS data
 Home-page: https://github.com/open-contracting/ocdskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdskit-1.1.7/README.rst` & `ocdskit-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/Makefile` & `ocdskit-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/changelog.rst` & `ocdskit-1.1.8/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.1.8 (2023-06-26)
+------------------
+
+Changed
+~~~~~~~
+
+-  :ref:`schema-strict`: Add ``minItems`` last, to match existing schema.
+
 1.1.7 (2023-06-13)
 ------------------
 
 Changed
 ~~~~~~~
 
 -  :ref:`compile`: Prefix the ``ocid`` to a warning.
```

### Comparing `ocdskit-1.1.7/docs/cli/examples.rst` & `ocdskit-1.1.8/docs/cli/examples.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/cli/ocds.rst` & `ocdskit-1.1.8/docs/cli/ocds.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/cli/schema.rst` & `ocdskit-1.1.8/docs/cli/schema.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/cli.rst` & `ocdskit-1.1.8/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/conf.py` & `ocdskit-1.1.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Kit"
 copyright = "2017, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "1.1.7"
+version = "1.1.8"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdskit-1.1.7/docs/contributing.rst` & `ocdskit-1.1.8/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/index.rst` & `ocdskit-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/docs/library.rst` & `ocdskit-1.1.8/docs/library.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/__main__.py` & `ocdskit-1.1.8/ocdskit/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/combine.py` & `ocdskit-1.1.8/ocdskit/combine.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/base.py` & `ocdskit-1.1.8/ocdskit/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/combine_record_packages.py` & `ocdskit-1.1.8/ocdskit/commands/combine_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/combine_release_packages.py` & `ocdskit-1.1.8/ocdskit/commands/combine_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/compile.py` & `ocdskit-1.1.8/ocdskit/commands/compile.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/detect_format.py` & `ocdskit-1.1.8/ocdskit/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/indent.py` & `ocdskit-1.1.8/ocdskit/commands/indent.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/mapping_sheet.py` & `ocdskit-1.1.8/ocdskit/commands/mapping_sheet.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/package_records.py` & `ocdskit-1.1.8/ocdskit/commands/package_records.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/package_releases.py` & `ocdskit-1.1.8/ocdskit/commands/package_releases.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/schema_report.py` & `ocdskit-1.1.8/ocdskit/commands/schema_report.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/schema_strict.py` & `ocdskit-1.1.8/ocdskit/commands/schema_strict.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/set_closed_codelist_enums.py` & `ocdskit-1.1.8/ocdskit/commands/set_closed_codelist_enums.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/split_record_packages.py` & `ocdskit-1.1.8/ocdskit/commands/split_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/split_release_packages.py` & `ocdskit-1.1.8/ocdskit/commands/split_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/commands/upgrade.py` & `ocdskit-1.1.8/ocdskit/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/exceptions.py` & `ocdskit-1.1.8/ocdskit/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/mapping_sheet.py` & `ocdskit-1.1.8/ocdskit/mapping_sheet.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/packager.py` & `ocdskit-1.1.8/ocdskit/packager.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/schema.py` & `ocdskit-1.1.8/ocdskit/schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -206,19 +206,19 @@
                 and 'format' not in schema
                 # The pattern is assumed to not match zero-length strings.
                 and 'pattern' not in schema
             ):
                 schema.setdefault('minLength', 1)
 
             if 'array' in schema['type']:
-                schema.setdefault('minItems', 1)
                 # Allow non-unique items for coordinates fields (e.g. closed polygons).
                 if sorted(schema.get('items', {}).get('type', [])) == ['array', 'number']:
                     coordinates = True
                 if unique_items and not coordinates:
                     schema.setdefault('uniqueItems', True)
+                schema.setdefault('minItems', 1)
 
             if 'object' in schema['type']:
                 schema.setdefault('minProperties', 1)
 
         for value in schema.values():
             add_validation_properties(value, unique_items=unique_items, coordinates=coordinates)
```

### Comparing `ocdskit-1.1.7/ocdskit/upgrade.py` & `ocdskit-1.1.8/ocdskit/upgrade.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit/util.py` & `ocdskit-1.1.8/ocdskit/util.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/ocdskit.egg-info/PKG-INFO` & `ocdskit-1.1.8/ocdskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdskit
-Version: 1.1.7
+Version: 1.1.8
 Summary: A suite of command-line tools for working with OCDS data
 Home-page: https://github.com/open-contracting/ocdskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdskit-1.1.7/ocdskit.egg-info/SOURCES.txt` & `ocdskit-1.1.8/ocdskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/setup.cfg` & `ocdskit-1.1.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdskit
-version = 1.1.7
+version = 1.1.8
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = A suite of command-line tools for working with OCDS data
 url = https://github.com/open-contracting/ocdskit
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdskit-1.1.7/tests/__init__.py` & `ocdskit-1.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/cassettes/test_combine-test_merge_empty.yaml` & `ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_empty.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/cassettes/test_combine-test_merge_with_schema.yaml` & `ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_with_schema.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/cassettes/test_packager-test_output_package_no_streaming.yaml` & `ocdskit-1.1.8/tests/cassettes/test_packager-test_output_package_no_streaming.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml` & `ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_combine_record_packages.py` & `ocdskit-1.1.8/tests/commands/test_combine_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_combine_release_packages.py` & `ocdskit-1.1.8/tests/commands/test_combine_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_compile.py` & `ocdskit-1.1.8/tests/commands/test_compile.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_detect_format.py` & `ocdskit-1.1.8/tests/commands/test_detect_format.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_echo.py` & `ocdskit-1.1.8/tests/commands/test_echo.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_indent.py` & `ocdskit-1.1.8/tests/commands/test_indent.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_mapping_sheet.py` & `ocdskit-1.1.8/tests/commands/test_mapping_sheet.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_package_records.py` & `ocdskit-1.1.8/tests/commands/test_package_records.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_package_releases.py` & `ocdskit-1.1.8/tests/commands/test_package_releases.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_schema_report.py` & `ocdskit-1.1.8/tests/commands/test_schema_report.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_schema_strict.py` & `ocdskit-1.1.8/tests/commands/test_schema_strict.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     "enumString",
     "formatString",
     "patternString"
   ],
   "properties": {
     "optionalArray": {
       "type": "array",
-      "minItems": 1,
-      "uniqueItems": true
+      "uniqueItems": true,
+      "minItems": 1
     },
     "array": {
       "type": "array",
-      "minItems": 1,
-      "uniqueItems": true
+      "uniqueItems": true,
+      "minItems": 1
     },
     "minItemsArray": {
       "type": "array",
       "minItems": 2,
       "uniqueItems": true
     },
     "optionalObject": {
```

### Comparing `ocdskit-1.1.7/tests/commands/test_set_closed_codelist_enums.py` & `ocdskit-1.1.8/tests/commands/test_set_closed_codelist_enums.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/commands/test_upgrade.py` & `ocdskit-1.1.8/tests/commands/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/bods/components.json` & `ocdskit-1.1.8/tests/fixtures/bods/components.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/bods/person-statement.json` & `ocdskit-1.1.8/tests/fixtures/bods/person-statement.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json` & `ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json` & `ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_bods.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_bods.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_codelist.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_codelist.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension-field.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension-field.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_array.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_array.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_language.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_language.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_location.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_location.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_no-deprecated.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_no-deprecated.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_oc4ids.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_oc4ids.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_order-by.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_order-by.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/mapping-sheet_sedl.csv` & `ocdskit-1.1.8/tests/fixtures/mapping-sheet_sedl.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/ocds-sample-data.json.gz` & `ocdskit-1.1.8/tests/fixtures/ocds-sample-data.json.gz`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/project-schema.json` & `ocdskit-1.1.8/tests/fixtures/project-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/compile_encoding_encoding.json` & `ocdskit-1.1.8/tests/fixtures/realdata/compile_encoding_encoding.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/compiled-release-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/compiled-release-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package-1-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package-1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_1.0.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.0.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_1.1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_linked-releases.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_linked-releases.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_package.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_package_1.1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_package_1.1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_record-package.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_record-package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_split.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_split.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/record-package_versioned.json` & `ocdskit-1.1.8/tests/fixtures/realdata/record-package_versioned.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package-1-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package-1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.0-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.0-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.1-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_1.1-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_encoding-utf-8.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-utf-8.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_record-package.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_record-package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/release-package_split.json` & `ocdskit-1.1.8/tests/fixtures/realdata/release-package_split.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/versioned-release-1.json` & `ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/realdata/versioned-release-2.json` & `ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/release-package-schema.json` & `ocdskit-1.1.8/tests/fixtures/release-package-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/release-package_additional-contact-points.json` & `ocdskit-1.1.8/tests/fixtures/release-package_additional-contact-points.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/release-packages.jsonl` & `ocdskit-1.1.8/tests/fixtures/release-packages.jsonl`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/release-schema.json` & `ocdskit-1.1.8/tests/fixtures/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/schema-strict.json` & `ocdskit-1.1.8/tests/fixtures/schema-strict.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/sedl-schema.json` & `ocdskit-1.1.8/tests/fixtures/sedl-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/fixtures/test-schema.json` & `ocdskit-1.1.8/tests/fixtures/test-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/test_combine.py` & `ocdskit-1.1.8/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/test_packager.py` & `ocdskit-1.1.8/tests/test_packager.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.7/tests/test_util.py` & `ocdskit-1.1.8/tests/test_util.py`

 * *Files identical despite different names*

