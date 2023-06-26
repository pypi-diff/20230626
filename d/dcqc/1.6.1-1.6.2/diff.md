# Comparing `tmp/dcqc-1.6.1.tar.gz` & `tmp/dcqc-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcqc-1.6.1.tar", last modified: Fri Jun 23 17:26:36 2023, max compression
+gzip compressed data, was "dcqc-1.6.2.tar", last modified: Mon Jun 26 15:42:17 2023, max compression
```

## Comparing `dcqc-1.6.1.tar` & `dcqc-1.6.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.203589 dcqc-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-23 17:25:32.000000 dcqc-1.6.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.187588 dcqc-1.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.191588 dcqc-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-23 17:25:32.000000 dcqc-1.6.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-23 17:25:32.000000 dcqc-1.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 17:25:32.000000 dcqc-1.6.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-23 17:25:32.000000 dcqc-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-23 17:25:32.000000 dcqc-1.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 17:25:32.000000 dcqc-1.6.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 17:25:32.000000 dcqc-1.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-23 17:25:32.000000 dcqc-1.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 17:25:32.000000 dcqc-1.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-23 17:26:36.203589 dcqc-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 17:25:32.000000 dcqc-1.6.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-06-23 17:25:32.000000 dcqc-1.6.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-23 17:25:32.000000 dcqc-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.191588 dcqc-1.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.191588 dcqc-1.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 17:25:32.000000 dcqc-1.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-23 17:25:32.000000 dcqc-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-23 17:26:36.203589 dcqc-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-23 17:25:32.000000 dcqc-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.187588 dcqc-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.195588 dcqc-1.6.1/src/dcqc/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.195588 dcqc-1.6.1/src/dcqc/suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/suites/suite_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/suites/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.195588 dcqc-1.6.1/src/dcqc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/bioformats_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/file_extension_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/grep_date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/json_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/jsonld_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/libtiff_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/md5_checksum_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/ome_xml_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/paired_fastq_parity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/tests/tiff_tag_306_date_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/dcqc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.195588 dcqc-1.6.1/src/dcqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:26:35.000000 dcqc-1.6.1/src/dcqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 17:26:36.000000 dcqc-1.6.1/src/dcqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.195588 dcqc-1.6.1/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 17:25:32.000000 dcqc-1.6.1/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.199589 dcqc-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.203589 dcqc-1.6.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/circuit.tif
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/empty_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/example.bam
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/example.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/example.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/example.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/example.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/fastq1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/fastq2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/files.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/small.csv
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/suite.json
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/suites.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.203589 dcqc-1.6.1/tests/data/suites_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/suites_files/suites_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/suites_files/suites_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/suites_files/suites_3.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/target.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test.computed.json
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test.external.json
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test.internal.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test_contains_word_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test_image_dirty_datetime.tif
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/test_output.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:26:36.203589 dcqc-1.6.1/tests/data/tiffinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/tiffinfo/exit_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/tiffinfo/std_err.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/data/tiffinfo/std_out.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-23 17:25:32.000000 dcqc-1.6.1/tests/test_updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-23 17:25:32.000000 dcqc-1.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 15:41:28.000000 dcqc-1.6.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-26 15:41:28.000000 dcqc-1.6.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 15:41:28.000000 dcqc-1.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 15:41:28.000000 dcqc-1.6.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-26 15:41:28.000000 dcqc-1.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 15:41:28.000000 dcqc-1.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 15:41:28.000000 dcqc-1.6.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 15:41:28.000000 dcqc-1.6.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-26 15:41:28.000000 dcqc-1.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 15:41:28.000000 dcqc-1.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 15:42:17.984117 dcqc-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 15:41:28.000000 dcqc-1.6.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-06-26 15:41:28.000000 dcqc-1.6.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-26 15:41:28.000000 dcqc-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 15:41:28.000000 dcqc-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-26 15:42:17.984117 dcqc-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 15:41:28.000000 dcqc-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc/suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/suite_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/src/dcqc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/bioformats_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/file_extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/grep_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/json_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/jsonld_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/libtiff_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/md5_checksum_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/ome_xml_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/paired_fastq_parity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/tiff_tag_306_date_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/circuit.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/empty_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/fastq1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/fastq2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/files.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/suites_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/target.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.computed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.external.json
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_contains_word_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_image_dirty_datetime.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_output.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/tiffinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/exit_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/std_err.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/std_out.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-26 15:41:28.000000 dcqc-1.6.2/tox.ini
```

### Comparing `dcqc-1.6.1/.coveragerc` & `dcqc-1.6.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/.github/workflows/ci.yml` & `dcqc-1.6.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/.gitignore` & `dcqc-1.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/.pre-commit-config.yaml` & `dcqc-1.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/CONTRIBUTING.md` & `dcqc-1.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/LICENSE.txt` & `dcqc-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/PKG-INFO` & `dcqc-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.6.1/Pipfile.lock` & `dcqc-1.6.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/README.md` & `dcqc-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/docs/Makefile` & `dcqc-1.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/docs/conf.py` & `dcqc-1.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/docs/index.md` & `dcqc-1.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/pyproject.toml` & `dcqc-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/setup.cfg` & `dcqc-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/setup.py` & `dcqc-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/__init__.py` & `dcqc-1.6.2/src/dcqc/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/file.py` & `dcqc-1.6.2/src/dcqc/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
         url: Local or remote location of a file.
         metadata: File metadata.
         relative_to: Used to update any local URLs if they
             are relative to a directory other than the
             current work directory (default).
     """
 
+    tmp_dir: ClassVar[str] = "dcqc-staged-"
+
     _serialized_properties = ["name", "local_path"]
 
     url: str
     metadata: dict[str, Any]
     type: str
 
     def __init__(
@@ -332,17 +334,15 @@
         Returns:
             The path of the local copy.
         """
         if not destination:
             if self._local_path is not None:
                 return self._local_path
             else:
-                # TODO: This prefix is used by nf-dcqc to easily find the staged file.
-                #       It might be worth using a DCQCTMPDIR to avoid hard-coding this.
-                destination_str = mkdtemp(prefix="dcqc-staged-")
+                destination_str = mkdtemp(prefix=self.tmp_dir)
                 destination = Path(destination_str)
 
         # By this point, destination is defined (not None)
         if destination.is_dir():
             destination = destination / self.name
 
         if not destination.parent.exists():
```

### Comparing `dcqc-1.6.1/src/dcqc/main.py` & `dcqc-1.6.2/src/dcqc/main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/mixins.py` & `dcqc-1.6.2/src/dcqc/mixins.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/parsers.py` & `dcqc-1.6.2/src/dcqc/parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/reports.py` & `dcqc-1.6.2/src/dcqc/reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/suites/suite_abc.py` & `dcqc-1.6.2/src/dcqc/suites/suite_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/suites/suites.py` & `dcqc-1.6.2/src/dcqc/suites/suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/target.py` & `dcqc-1.6.2/src/dcqc/target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/__init__.py` & `dcqc-1.6.2/src/dcqc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/base_test.py` & `dcqc-1.6.2/src/dcqc/tests/base_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -198,29 +198,14 @@
         exit_code = exit_code.strip()
         if exit_code == self.pass_code:
             status = TestStatus.PASS
         else:
             status = TestStatus.FAIL
         return status
 
-    # TODO: make changes to this package or the nextflow
-    # workflow so that file mounting is handled cleaner
-    @staticmethod
-    def _short_string_path(path: Path, substring: str) -> str:
-        # chech if substring is in path
-        if substring not in path.as_posix():
-            raise ValueError(f"{substring} not in {path}")
-        # get index where staged folder is
-        index = next(i for i, item in enumerate(path.parts) if substring in item)
-        # shorten path starting from staged folder
-        short_path = Path(*path.parts[index:])
-        # wrap path string in quotes
-        quote_path = str(short_path)
-        return f"'{quote_path}'"
-
     # TODO: Include process in serialized test dictionary
     # def to_dict(self):
     #     dictionary = super(ExternalTestMixin, self).to_dict()
     #     process = self.generate_process()
     #     dictionary["process"] = process.to_dict()
     #     return dictionary
```

### Comparing `dcqc-1.6.1/src/dcqc/tests/bioformats_info_test.py` & `dcqc-1.6.2/src/dcqc/tests/bioformats_info_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 class BioFormatsInfoTest(ExternalBaseTest):
     tier = 2
     pass_code = "0"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
-        string_path = self._short_string_path(path, "dcqc-staged-")
 
         command_args = [
             "/opt/bftools/showinf",
             "-nopix",
             "-novalid",
             "-nocore",
-            string_path,
+            f"'{path.name}'",
         ]
         process = Process(
             container="quay.io/sagebionetworks/bftools:latest",
             command_args=command_args,
         )
         return process
```

### Comparing `dcqc-1.6.1/src/dcqc/tests/file_extension_test.py` & `dcqc-1.6.2/src/dcqc/tests/file_extension_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/grep_date_test.py` & `dcqc-1.6.2/src/dcqc/tests/grep_date_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 class GrepDateTest(ExternalBaseTest):
     tier = 4
     pass_code = "1"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
-        string_path = self._short_string_path(path, "dcqc-staged-")
 
         command_args = [
             "grep",
             "-E",  # extended regular expression
             "-i",  # case insensitive
             "-a",  # treat input as text
             "-q",  # suppress output
             "'date|time'",  # match date or time
-            string_path,
+            f"'{path.name}'",
         ]
         process = Process(
             container="quay.io/biocontainers/coreutils:8.30--h14c3975_1000",
             command_args=command_args,
         )
         return process
```

### Comparing `dcqc-1.6.1/src/dcqc/tests/json_load_test.py` & `dcqc-1.6.2/src/dcqc/tests/json_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/jsonld_load_test.py` & `dcqc-1.6.2/src/dcqc/tests/jsonld_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/md5_checksum_test.py` & `dcqc-1.6.2/src/dcqc/tests/md5_checksum_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/ome_xml_schema_test.py` & `dcqc-1.6.2/src/dcqc/tests/tiff_tag_306_date_time_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from dcqc.target import SingleTarget
 from dcqc.tests.base_test import ExternalBaseTest, Process
 
 
-class OmeXmlSchemaTest(ExternalBaseTest):
-    tier = 2
-    pass_code = "0"
+class TiffTag306DateTimeTest(ExternalBaseTest):
+    tier = 4
+    pass_code = "1"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
-        string_path = self._short_string_path(path, "dcqc-staged-")
 
         command_args = [
-            "/opt/bftools/xmlvalid",
-            string_path,
+            "tifftools",
+            "dump",
+            f"'{path.name}'",
+            "|",
+            "grep",  # pipe the output
+            "-a",  # treat input as text
+            "-q",  # suppress output
+            "'DateTime 306 (0x132) ASCII'",  # match the DateTime 306 tag
         ]
         process = Process(
-            container="quay.io/sagebionetworks/bftools:latest",
+            container="ghcr.io/sage-bionetworks-workflows/tifftools:latest",
             command_args=command_args,
         )
         return process
```

### Comparing `dcqc-1.6.1/src/dcqc/tests/paired_fastq_parity_test.py` & `dcqc-1.6.2/src/dcqc/tests/paired_fastq_parity_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/tests/tiff_tag_306_date_time_test.py` & `dcqc-1.6.2/src/dcqc/tests/ome_xml_schema_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 from dcqc.target import SingleTarget
 from dcqc.tests.base_test import ExternalBaseTest, Process
 
 
-class TiffTag306DateTimeTest(ExternalBaseTest):
-    tier = 4
-    pass_code = "1"
+class OmeXmlSchemaTest(ExternalBaseTest):
+    tier = 2
+    pass_code = "0"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
-        string_path = self._short_string_path(path, "dcqc-staged-")
 
         command_args = [
-            "tifftools",
-            "dump",
-            string_path,
-            "|",
-            "grep",  # pipe the output
-            "-a",  # treat input as text
-            "-q",  # suppress output
-            "'DateTime 306 (0x132) ASCII'",  # match the DateTime 306 tag
+            "/opt/bftools/xmlvalid",
+            f"'{path.name}'",
         ]
         process = Process(
-            container="ghcr.io/sage-bionetworks-workflows/tifftools:latest",
+            container="quay.io/sagebionetworks/bftools:latest",
             command_args=command_args,
         )
         return process
```

### Comparing `dcqc-1.6.1/src/dcqc/updaters.py` & `dcqc-1.6.2/src/dcqc/updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc/utils.py` & `dcqc-1.6.2/src/dcqc/utils.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/src/dcqc.egg-info/PKG-INFO` & `dcqc-1.6.2/src/dcqc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.6.1/src/dcqc.egg-info/SOURCES.txt` & `dcqc-1.6.2/src/dcqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/conftest.py` & `dcqc-1.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/circuit.tif` & `dcqc-1.6.2/tests/data/circuit.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/example.jsonld` & `dcqc-1.6.2/tests/data/example.jsonld`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/files.csv` & `dcqc-1.6.2/tests/data/files.csv`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/generate.py` & `dcqc-1.6.2/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/suite.json` & `dcqc-1.6.2/tests/data/suite.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/suites.json` & `dcqc-1.6.2/tests/data/suites.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/suites_files/suites_1.json` & `dcqc-1.6.2/tests/data/suites_files/suites_1.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/suites_files/suites_2.json` & `dcqc-1.6.2/tests/data/suites_files/suites_2.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/suites_files/suites_3.json` & `dcqc-1.6.2/tests/data/suites_files/suites_3.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/test_image_dirty_datetime.tif` & `dcqc-1.6.2/tests/data/test_image_dirty_datetime.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/data/tests.json` & `dcqc-1.6.2/tests/data/tests.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_acceptance.py` & `dcqc-1.6.2/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_file.py` & `dcqc-1.6.2/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_main.py` & `dcqc-1.6.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_parsers.py` & `dcqc-1.6.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_reports.py` & `dcqc-1.6.2/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_suites.py` & `dcqc-1.6.2/tests/test_suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_target.py` & `dcqc-1.6.2/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tests/test_tests.py` & `dcqc-1.6.2/tests/test_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -320,22 +320,7 @@
     test_files,
 ):
     fastq2 = test_files["fastq2"]
     target = PairedTarget([fastq2, fastq2])
     test = tests.PairedFastqParityTest(target)
     test_status = test.get_status()
     assert test_status == TestStatus.PASS
-
-
-def test_that_short_string_path_correctly_shortens_file_paths():
-    substring = "test-substring"
-    long_path = f"path/needs/to/be/shortened/{substring}/file.txt"
-    expected_short_path = f"'{substring}/file.txt'"
-    short_path = ExternalTestMixin._short_string_path(Path(long_path), substring)
-    assert short_path == expected_short_path
-
-
-def test_that_short_string_path_raises_valueerror_if_substring_not_in_path():
-    substring = "test-substring"
-    long_path = "path/needs/to/be/shortened/fail/file.txt"
-    with pytest.raises(ValueError):
-        ExternalTestMixin._short_string_path(Path(long_path), substring)
```

### Comparing `dcqc-1.6.1/tests/test_updaters.py` & `dcqc-1.6.2/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.1/tox.ini` & `dcqc-1.6.2/tox.ini`

 * *Files identical despite different names*

