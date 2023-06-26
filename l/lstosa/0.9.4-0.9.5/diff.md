# Comparing `tmp/lstosa-0.9.4.tar.gz` & `tmp/lstosa-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lstosa-0.9.4.tar", last modified: Fri May 20 15:50:17 2022, max compression
+gzip compressed data, was "lstosa-0.9.5.tar", last modified: Sat Oct 29 09:20:13 2022, max compression
```

## Comparing `lstosa-0.9.4.tar` & `lstosa-0.9.5.tar`

### file list

```diff
@@ -1,159 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.587761 lstosa-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-20 15:50:04.000000 lstosa-0.9.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-20 15:50:04.000000 lstosa-0.9.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-05-20 15:50:04.000000 lstosa-0.9.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-05-20 15:50:04.000000 lstosa-0.9.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-05-20 15:50:04.000000 lstosa-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-05-20 15:50:04.000000 lstosa-0.9.4/.mailmap
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-20 15:50:04.000000 lstosa-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    18371 2022-05-20 15:50:04.000000 lstosa-0.9.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-05-20 15:50:04.000000 lstosa-0.9.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-05-20 15:50:04.000000 lstosa-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-05-20 15:50:17.587761 lstosa-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-05-20 15:50:04.000000 lstosa-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/dev/
--rw-r--r--   0 runner    (1001) docker     (121)    10038 2022-05-20 15:50:04.000000 lstosa-0.9.4/dev/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/docs/components/
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/contribute.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/docs/documents/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/documents/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (121)     9801 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.575761 lstosa-0.9.4/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/introduction/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)   134003 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/introduction/reduction_steps_lstchain.png
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (121)   915577 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/logo_lstosa.png
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/nightsummary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/reports.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/scripts/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/docs/troubleshooting/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/troubleshooting/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/veto.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/docs/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)    17837 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/workflow/LSTOSA_flow.png
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-05-20 15:50:04.000000 lstosa-0.9.4/docs/workflow/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-05-20 15:50:04.000000 lstosa-0.9.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/extra/
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/example_sequencer.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/extra/history_files/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/history_files/sequence_LST1_04183.history
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/history_files/sequence_LST1_04183_failed.history
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/history_files/sequence_LST1_04183_oneline.history
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/history_files/sequence_LST1_04185.0010.history
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/sacct_output.csv
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-05-20 15:50:04.000000 lstosa-0.9.4/extra/squeue_output.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/lstosa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-05-20 15:50:16.000000 lstosa-0.9.4/lstosa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-05-20 15:50:17.000000 lstosa-0.9.4/lstosa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 15:50:17.000000 lstosa-0.9.4/lstosa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-05-20 15:50:17.000000 lstosa-0.9.4/lstosa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 15:50:16.000000 lstosa-0.9.4/lstosa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-20 15:50:17.000000 lstosa-0.9.4/lstosa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-05-20 15:50:17.000000 lstosa-0.9.4/lstosa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/_dev_version/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/_dev_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-20 15:50:16.000000 lstosa-0.9.4/osa/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/configs/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/configs/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/configs/sequencer.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    14777 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/high_level/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/high_level/selection_cuts.toml
--rw-r--r--   0 runner    (1001) docker     (121)     9300 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/high_level/significance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/high_level/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/high_level/tests/test_significance.py
--rw-r--r--   0 runner    (1001) docker     (121)    27043 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.579761 lstosa-0.9.4/osa/nightsummary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    16883 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/nightsummary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/set_source_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/nightsummary/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/tests/test_nightsummary.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/nightsummary/tests/test_source_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     8618 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/provenance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22462 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/capture.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/provenance/config/
--rw-r--r--   0 runner    (1001) docker     (121)    20534 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/config/definition.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/config/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/config/logger.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9547 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/provenance/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/raw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14813 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/autocloser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/calibration_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    14164 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/closer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/copy_datacheck.py
--rw-r--r--   0 runner    (1001) docker     (121)    10047 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/datasequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/gain_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)    18562 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/provprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/reprocess_longterm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/reprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12998 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/sequencer_webmaker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/show_run_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     7118 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/simulate_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12321 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/scripts/tests/test_osa_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15948 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_osa.py
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/tests/test_veto.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.583761 lstosa-0.9.4/osa/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14039 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/cliopts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/iofile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/mail.py
--rw-r--r--   0 runner    (1001) docker     (121)     5909 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/register.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.587761 lstosa-0.9.4/osa/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/tests/test_iofile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9227 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/veto.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.587761 lstosa-0.9.4/osa/webserver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/webserver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.587761 lstosa-0.9.4/osa/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10166 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/workflow/dl3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 15:50:17.587761 lstosa-0.9.4/osa/workflow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-05-20 15:50:04.000000 lstosa-0.9.4/osa/workflow/tests/test_dl3.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-05-20 15:50:04.000000 lstosa-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-05-20 15:50:17.587761 lstosa-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 15:50:04.000000 lstosa-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.937789 lstosa-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-29 09:20:03.000000 lstosa-0.9.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.897789 lstosa-0.9.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-29 09:20:03.000000 lstosa-0.9.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.901789 lstosa-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-29 09:20:03.000000 lstosa-0.9.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-29 09:20:03.000000 lstosa-0.9.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-29 09:20:03.000000 lstosa-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-10-29 09:20:03.000000 lstosa-0.9.5/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-10-29 09:20:03.000000 lstosa-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    18388 2022-10-29 09:20:03.000000 lstosa-0.9.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-29 09:20:03.000000 lstosa-0.9.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-10-29 09:20:03.000000 lstosa-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-10-29 09:20:13.937789 lstosa-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-10-29 09:20:03.000000 lstosa-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-10-29 09:20:03.000000 lstosa-0.9.5/codemeta.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.901789 lstosa-0.9.5/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)    10038 2022-10-29 09:20:03.000000 lstosa-0.9.5/dev/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.905789 lstosa-0.9.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.905789 lstosa-0.9.5/docs/components/
+-rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/contribute.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.905789 lstosa-0.9.5/docs/documents/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/documents/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.905789 lstosa-0.9.5/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (121)     9801 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.905789 lstosa-0.9.5/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   134003 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/introduction/reduction_steps_lstchain.png
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   915577 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/logo_lstosa.png
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/nightsummary.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/reports.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.909789 lstosa-0.9.5/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/scripts/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.909789 lstosa-0.9.5/docs/troubleshooting/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/troubleshooting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/veto.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.909789 lstosa-0.9.5/docs/workflow/
+-rw-r--r--   0 runner    (1001) docker     (121)    17837 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/workflow/LSTOSA_flow.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-10-29 09:20:03.000000 lstosa-0.9.5/docs/workflow/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-10-29 09:20:03.000000 lstosa-0.9.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.909789 lstosa-0.9.5/extra/
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/example_sequencer.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.909789 lstosa-0.9.5/extra/history_files/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/history_files/sequence_LST1_04183.history
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/history_files/sequence_LST1_04183_failed.history
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/history_files/sequence_LST1_04183_oneline.history
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/history_files/sequence_LST1_04185.0010.history
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/sacct_output.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-29 09:20:03.000000 lstosa-0.9.5/extra/squeue_output.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.913789 lstosa-0.9.5/lstosa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3286 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-29 09:20:13.000000 lstosa-0.9.5/lstosa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.917789 lstosa-0.9.5/osa/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.917789 lstosa-0.9.5/osa/_dev_version/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/_dev_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-29 09:20:13.000000 lstosa-0.9.5/osa/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.917789 lstosa-0.9.5/osa/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/configs/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/configs/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/configs/sequencer.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    15566 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.917789 lstosa-0.9.5/osa/high_level/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/high_level/selection_cuts.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     9039 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/high_level/significance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.921789 lstosa-0.9.5/osa/high_level/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/high_level/tests/test_significance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25376 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/job.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.921789 lstosa-0.9.5/osa/nightsummary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8746 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/nightsummary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/set_source_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.921789 lstosa-0.9.5/osa/nightsummary/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/tests/test_nightsummary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/nightsummary/tests/test_source_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/osadb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9488 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.925789 lstosa-0.9.5/osa/provenance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22348 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.925789 lstosa-0.9.5/osa/provenance/config/
+-rw-r--r--   0 runner    (1001) docker     (121)    20534 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/config/definition.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/config/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/config/logger.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9471 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10131 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/provenance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.929789 lstosa-0.9.5/osa/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14492 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/autocloser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/calibration_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14870 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/closer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/copy_datacheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9260 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/datasequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6111 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/gain_selection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18480 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/provprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/reprocess_longterm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/reprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8098 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4640 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/sequencer_webmaker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5197 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/show_run_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6941 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/simulate_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.929789 lstosa-0.9.5/osa/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12244 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/scripts/tests/test_osa_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.933789 lstosa-0.9.5/osa/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15340 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_osa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_osadb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/tests/test_veto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.933789 lstosa-0.9.5/osa/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13716 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/cliopts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/iofile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/mail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5818 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/register.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.937789 lstosa-0.9.5/osa/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/tests/test_iofile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/veto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.937789 lstosa-0.9.5/osa/webserver/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/webserver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.937789 lstosa-0.9.5/osa/workflow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9921 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/workflow/dl3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5330 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/workflow/stages.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 09:20:13.937789 lstosa-0.9.5/osa/workflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/workflow/tests/test_dl3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3944 2022-10-29 09:20:03.000000 lstosa-0.9.5/osa/workflow/tests/test_stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-29 09:20:03.000000 lstosa-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-10-29 09:20:13.941789 lstosa-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 09:20:03.000000 lstosa-0.9.5/setup.py
```

### Comparing `lstosa-0.9.4/.github/workflows/ci.yml` & `lstosa-0.9.5/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 jobs:
   pyflakes:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
 
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python 3.8
         uses: actions/setup-python@v2
         with:
           python-version: 3.8
 
       - name: pyflakes
         run: |
           pip install pyflakes
@@ -32,18 +32,14 @@
     needs: pyflakes
     runs-on: ubuntu-latest
 
     defaults:
       run:
         shell: bash -l {0}
 
-    strategy:
-      matrix:
-        python-version: [3.7, 3.8]
-
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Setup Miniconda
         uses: conda-incubator/setup-miniconda@v2.1.1
@@ -51,21 +47,21 @@
           mamba-version: "*"
           auto-update-conda: true
           activate-environment: "osa-ci"
           environment-file: environment.yml
 
       - name: Install dependencies
         env:
-          PYTHON_VERSION: ${{ matrix.python-version }}
+          PYTHON_VERSION: 3.8
 
         run: |
           python --version
           echo "Installing additional pip packages"
-          echo "pip install ."
-          pip install .
+          echo "pip install .[test]"
+          pip install .[test]
 
       - name: Tests
         env:
           COVERAGE_PROCESS_START: .coveragerc
           PYTHONPATH: .
 
         run: |
```

### Comparing `lstosa-0.9.4/.github/workflows/deploy.yml` & `lstosa-0.9.5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/.gitignore` & `lstosa-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/.mailmap` & `lstosa-0.9.5/.mailmap`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/.pylintrc` & `lstosa-0.9.5/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,16 @@
         W1203,
         C0103,
         B603,
         E1101,
         B404,
         D203,
         D212,
-        D205
+        D205,
+        C0330
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=c-extension-no-member
 
@@ -333,15 +334,15 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=90
+max-line-length=100
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
@@ -598,8 +599,8 @@
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "BaseException, Exception".
 overgeneral-exceptions=BaseException,
-                       Exception
+                       Exception
```

### Comparing `lstosa-0.9.4/LICENSE` & `lstosa-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/PKG-INFO` & `lstosa-0.9.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: lstosa
-Version: 0.9.4
+Version: 0.9.5
 Summary: Onsite analysis pipeline for the CTA LST-1
 Home-page: https://github.com/cta-observatory/lstosa
 Author: lstosa developers, CTA-LST project
 Author-email: dmorcuen@ucm.es
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cta-observatory/lstosa/issues
 Project-URL: Documentation, https://lstosa.readthedocs.io/
 Project-URL: Source Code, https://github.com/cta-observatory/lstosa
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # lstosa
 
   [![ci](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml)
   [![Documentation Status](https://readthedocs.org/projects/lstosa/badge/?version=latest)](https://lstosa.readthedocs.io/en/latest/?badge=latest)
   [![coverage](https://codecov.io/gh/cta-observatory/lstosa/branch/main/graph/badge.svg?token=Zjk1U1ytaG)](https://codecov.io/gh/cta-observatory/lstosa)
   [![quality](https://app.codacy.com/project/badge/Grade/a8743a706e7c45fc989d5ebc4d61d54f)](https://www.codacy.com/gh/cta-observatory/lstosa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/lstosa&amp;utm_campaign=Badge_Grade)
   [![pypi](https://img.shields.io/pypi/v/lstosa)](https://pypi.org/project/lstosa/)
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6567234.svg)](https://doi.org/10.5281/zenodo.6567234)
+
 
 Prototype onsite processing pipeline for the Large Size Telescope prototype (LST-1) of [CTA](https://www.cta-observatory.org/) (Cherenkov Telescope Array) based on [cta-lstchain](https://github.com/cta-observatory/cta-lstchain) running on the LST-1 IT onsite center at ORM (La Palma, Spain). It automatically carries out the next-day analysis of observed data using cron jobs, parallelizing the processing using the job scheduler SLURM. It provides data quality monitoring and tracking of analysis products' provenance.
 Moreover, it also massively reprocesses the entire LST-1 dataset with each cta-lstchain major release:
  - Code: <https://github.com/cta-observatory/lstosa>
  - Docs: <https://lstosa.readthedocs.io/>
  - License: [BSD-3-Clause](https://github.com/cta-observatory/lstosa/blob/main/LICENSE)
 
@@ -58,14 +60,16 @@
 
 To update the environment (provided dependencies get updated), use:
 
 ```bash
 conda env update -n osa -f environment.yml
 ```
 
+> **Note** to developers: to enforce a unique code convention, please install pre-commit (pre-commit install) after cloning the repository and creating the conda environment. This will black the committed files automatically.
+
 ## Workflow management
 `lstosa` workflow is handled daily by the `sequencer` script, which identifies which observations are to be processed, generates the analysis workflow, and submits the jobs. A first calibration job produces the daily calibration coefficients. Subsequently, data reconstruction jobs are scheduled on a subrun-wise basis (1 job corresponds to around 10 seconds of observed data, and its processing up to DL2 takes about 30-40 mins).
 
 ```mermaid
 
 flowchart LR
 
@@ -127,15 +131,15 @@
     D2 --> C1
     D3 --> C2
 
     subgraph Calibration
     C1[DRS4 baseline correction]
     C2[Calibration charge coeffitiens]
     C1 --> C2
-    end    
+    end
 
     subgraph lstMCpipe
     M1[gamma DL2 MC]
     M2[RF models]
     end
 
     subgraph Sky-data reconstruction
@@ -161,8 +165,8 @@
     DL4
     DL5
     S6 --> DL4
     DL4 --> DL5 --> ...
     end
 ```
 
-*Note:* Standard production of DL3 data and higher-level results is still under development.
+> **Warning**: standard production of DL3 data and higher-level results is still under development.
```

### Comparing `lstosa-0.9.4/README.md` & `lstosa-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # lstosa
 
   [![ci](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml)
   [![Documentation Status](https://readthedocs.org/projects/lstosa/badge/?version=latest)](https://lstosa.readthedocs.io/en/latest/?badge=latest)
   [![coverage](https://codecov.io/gh/cta-observatory/lstosa/branch/main/graph/badge.svg?token=Zjk1U1ytaG)](https://codecov.io/gh/cta-observatory/lstosa)
   [![quality](https://app.codacy.com/project/badge/Grade/a8743a706e7c45fc989d5ebc4d61d54f)](https://www.codacy.com/gh/cta-observatory/lstosa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/lstosa&amp;utm_campaign=Badge_Grade)
   [![pypi](https://img.shields.io/pypi/v/lstosa)](https://pypi.org/project/lstosa/)
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6567234.svg)](https://doi.org/10.5281/zenodo.6567234)
+
 
 Prototype onsite processing pipeline for the Large Size Telescope prototype (LST-1) of [CTA](https://www.cta-observatory.org/) (Cherenkov Telescope Array) based on [cta-lstchain](https://github.com/cta-observatory/cta-lstchain) running on the LST-1 IT onsite center at ORM (La Palma, Spain). It automatically carries out the next-day analysis of observed data using cron jobs, parallelizing the processing using the job scheduler SLURM. It provides data quality monitoring and tracking of analysis products' provenance.
 Moreover, it also massively reprocesses the entire LST-1 dataset with each cta-lstchain major release:
  - Code: <https://github.com/cta-observatory/lstosa>
  - Docs: <https://lstosa.readthedocs.io/>
  - License: [BSD-3-Clause](https://github.com/cta-observatory/lstosa/blob/main/LICENSE)
 
@@ -34,14 +36,16 @@
 
 To update the environment (provided dependencies get updated), use:
 
 ```bash
 conda env update -n osa -f environment.yml
 ```
 
+> **Note** to developers: to enforce a unique code convention, please install pre-commit (pre-commit install) after cloning the repository and creating the conda environment. This will black the committed files automatically.
+
 ## Workflow management
 `lstosa` workflow is handled daily by the `sequencer` script, which identifies which observations are to be processed, generates the analysis workflow, and submits the jobs. A first calibration job produces the daily calibration coefficients. Subsequently, data reconstruction jobs are scheduled on a subrun-wise basis (1 job corresponds to around 10 seconds of observed data, and its processing up to DL2 takes about 30-40 mins).
 
 ```mermaid
 
 flowchart LR
 
@@ -103,15 +107,15 @@
     D2 --> C1
     D3 --> C2
 
     subgraph Calibration
     C1[DRS4 baseline correction]
     C2[Calibration charge coeffitiens]
     C1 --> C2
-    end    
+    end
 
     subgraph lstMCpipe
     M1[gamma DL2 MC]
     M2[RF models]
     end
 
     subgraph Sky-data reconstruction
@@ -137,8 +141,8 @@
     DL4
     DL5
     S6 --> DL4
     DL4 --> DL5 --> ...
     end
 ```
 
-*Note:* Standard production of DL3 data and higher-level results is still under development.
+> **Warning**: standard production of DL3 data and higher-level results is still under development.
```

### Comparing `lstosa-0.9.4/dev/mysql.py` & `lstosa-0.9.5/dev/mysql.py`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/Makefile` & `lstosa-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/authors.rst` & `lstosa-0.9.5/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/components/index.rst` & `lstosa-0.9.5/docs/components/index.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/conf.py` & `lstosa-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/configuration.rst` & `lstosa-0.9.5/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/contribute.rst` & `lstosa-0.9.5/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/howto/index.rst` & `lstosa-0.9.5/docs/howto/index.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/index.rst` & `lstosa-0.9.5/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ``lstosa`` is the on-site processing pipeline of the CTA Large Size Telescope prototype (LST-1)
 making use of the `cta-lstchain`_ analysis library.
 
 * Code: https://github.com/cta-observatory/lstosa
 * Docs: https://lstosa.readthedocs.io/
 * License: BSD-3
-* Python 3.7, 3.8
+* Python 3.8+
 * Authors: Daniel Morcuende, Lab Saha, José Enrique Ruiz, José Luis Contreras, Andrés Baquero, María Lainez
 
 .. _`cta-lstchain`: https://github.com/cta-observatory/cta-lstchain
 
 .. _lstosa_guide:
 
 .. toctree::
```

### Comparing `lstosa-0.9.4/docs/introduction/index.rst` & `lstosa-0.9.5/docs/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/introduction/reduction_steps_lstchain.png` & `lstosa-0.9.5/docs/introduction/reduction_steps_lstchain.png`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/logo_lstosa.png` & `lstosa-0.9.5/docs/logo_lstosa.png`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/make.bat` & `lstosa-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/scripts/index.rst` & `lstosa-0.9.5/docs/scripts/index.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/utils.rst` & `lstosa-0.9.5/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/workflow/LSTOSA_flow.png` & `lstosa-0.9.5/docs/workflow/LSTOSA_flow.png`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/docs/workflow/index.rst` & `lstosa-0.9.5/docs/workflow/index.rst`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/environment.yml` & `lstosa-0.9.5/environment.yml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   - psutil
   - gammapy=0.19
   - h5py
   - joblib
   - click
   - pymongo
   - scikit-learn=1.0
+  - protobuf=3.20
   # dev dependencies
   - pre-commit
   - pytest
   - pytest-cov
   - coverage=6.2
   - black
   - isort
```

### Comparing `lstosa-0.9.4/extra/example_sequencer.txt` & `lstosa-0.9.5/extra/example_sequencer.txt`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/extra/history_files/sequence_LST1_04183_failed.history` & `lstosa-0.9.5/extra/history_files/sequence_LST1_04183_failed.history`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/extra/sacct_output.csv` & `lstosa-0.9.5/extra/sacct_output.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-12925480,LST1_01805,00:59:56,3596,00:59:56,58:55.330,,FAILED,1:0
+12925480,LST1_01809,00:59:56,3596,00:59:56,58:55.330,,FAILED,1:0
 12925480.batch,batch,00:59:56,3596,00:59:56,58:55.330,3.01G,FAILED,1:0
-12927823,LST1_01805,01:23:10,4990,01:23:10,01:21:54,,COMPLETED,0:0
+12927823,LST1_01809,01:23:10,4990,01:23:10,01:21:54,,COMPLETED,0:0
 12927823.batch,batch,01:23:10,4990,01:23:10,01:21:54,3.05G,COMPLETED,0:0
 12927824_0,LST1_01807,00:30:55,1855,00:30:55,30:30.367,,COMPLETED,0:0
 12927824_0.batch,batch,00:30:55,1855,00:30:55,30:30.367,2.38G,COMPLETED,0:0
 12927824_1,LST1_01807,00:30:43,1843,00:30:43,30:21.756,,FAILED,1:0
 12927824_1.batch,batch,00:30:43,1843,00:30:43,30:21.756,4.70G,FAILED,1:0
 12927824_2,LST1_01807,00:30:25,1825,00:30:25,29:45.289,,FAILED,1:0
 12927824_2.batch,batch,00:30:25,1825,00:30:25,29:45.289,2.01G,FAILED,1:0
 12927824_3,LST1_01807,00:31:03,1863,00:31:03,30:30.598,,FAILED,1:0
 12927824_3.batch,batch,00:31:03,1863,00:31:03,30:30.598,5.32G,FAILED,1:0
 12927824_4,LST1_01807,00:31:26,1886,00:31:26,30:41.448,,FAILED,1:0
 12927824_4.batch,batch,00:31:26,1886,00:31:26,30:41.448,2.60G,FAILED,1:0
-12929215,LST1_01805,00:22:49,1369,00:22:49,22:00.665,,FAILED,1:0
-12951086,LST1_01805,00:36:00,1369,00:36:00,00:36:00,,RUNNING,0:0
+12929215,LST1_01809,00:22:49,1369,00:22:49,22:00.665,,FAILED,1:0
+12951086,LST1_01809,00:36:00,1369,00:36:00,00:36:00,,RUNNING,0:0
```

### Comparing `lstosa-0.9.4/lstosa.egg-info/PKG-INFO` & `lstosa-0.9.5/lstosa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: lstosa
-Version: 0.9.4
+Version: 0.9.5
 Summary: Onsite analysis pipeline for the CTA LST-1
 Home-page: https://github.com/cta-observatory/lstosa
 Author: lstosa developers, CTA-LST project
 Author-email: dmorcuen@ucm.es
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cta-observatory/lstosa/issues
 Project-URL: Documentation, https://lstosa.readthedocs.io/
 Project-URL: Source Code, https://github.com/cta-observatory/lstosa
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # lstosa
 
   [![ci](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/lstosa/actions/workflows/ci.yml)
   [![Documentation Status](https://readthedocs.org/projects/lstosa/badge/?version=latest)](https://lstosa.readthedocs.io/en/latest/?badge=latest)
   [![coverage](https://codecov.io/gh/cta-observatory/lstosa/branch/main/graph/badge.svg?token=Zjk1U1ytaG)](https://codecov.io/gh/cta-observatory/lstosa)
   [![quality](https://app.codacy.com/project/badge/Grade/a8743a706e7c45fc989d5ebc4d61d54f)](https://www.codacy.com/gh/cta-observatory/lstosa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/lstosa&amp;utm_campaign=Badge_Grade)
   [![pypi](https://img.shields.io/pypi/v/lstosa)](https://pypi.org/project/lstosa/)
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6567234.svg)](https://doi.org/10.5281/zenodo.6567234)
+
 
 Prototype onsite processing pipeline for the Large Size Telescope prototype (LST-1) of [CTA](https://www.cta-observatory.org/) (Cherenkov Telescope Array) based on [cta-lstchain](https://github.com/cta-observatory/cta-lstchain) running on the LST-1 IT onsite center at ORM (La Palma, Spain). It automatically carries out the next-day analysis of observed data using cron jobs, parallelizing the processing using the job scheduler SLURM. It provides data quality monitoring and tracking of analysis products' provenance.
 Moreover, it also massively reprocesses the entire LST-1 dataset with each cta-lstchain major release:
  - Code: <https://github.com/cta-observatory/lstosa>
  - Docs: <https://lstosa.readthedocs.io/>
  - License: [BSD-3-Clause](https://github.com/cta-observatory/lstosa/blob/main/LICENSE)
 
@@ -58,14 +60,16 @@
 
 To update the environment (provided dependencies get updated), use:
 
 ```bash
 conda env update -n osa -f environment.yml
 ```
 
+> **Note** to developers: to enforce a unique code convention, please install pre-commit (pre-commit install) after cloning the repository and creating the conda environment. This will black the committed files automatically.
+
 ## Workflow management
 `lstosa` workflow is handled daily by the `sequencer` script, which identifies which observations are to be processed, generates the analysis workflow, and submits the jobs. A first calibration job produces the daily calibration coefficients. Subsequently, data reconstruction jobs are scheduled on a subrun-wise basis (1 job corresponds to around 10 seconds of observed data, and its processing up to DL2 takes about 30-40 mins).
 
 ```mermaid
 
 flowchart LR
 
@@ -127,15 +131,15 @@
     D2 --> C1
     D3 --> C2
 
     subgraph Calibration
     C1[DRS4 baseline correction]
     C2[Calibration charge coeffitiens]
     C1 --> C2
-    end    
+    end
 
     subgraph lstMCpipe
     M1[gamma DL2 MC]
     M2[RF models]
     end
 
     subgraph Sky-data reconstruction
@@ -161,8 +165,8 @@
     DL4
     DL5
     S6 --> DL4
     DL4 --> DL5 --> ...
     end
 ```
 
-*Note:* Standard production of DL3 data and higher-level results is still under development.
+> **Warning**: standard production of DL3 data and higher-level results is still under development.
```

### Comparing `lstosa-0.9.4/lstosa.egg-info/SOURCES.txt` & `lstosa-0.9.5/lstosa.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitignore
 .mailmap
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
 LICENSE
 README.md
+codemeta.json
 environment.yml
 pyproject.toml
 setup.cfg
 setup.py
 .github/release-drafter.yml
 .github/workflows/ci.yml
 .github/workflows/deploy.yml
@@ -52,14 +53,15 @@
 lstosa.egg-info/not-zip-safe
 lstosa.egg-info/requires.txt
 lstosa.egg-info/top_level.txt
 osa/__init__.py
 osa/_version.py
 osa/conftest.py
 osa/job.py
+osa/osadb.py
 osa/paths.py
 osa/raw.py
 osa/report.py
 osa/version.py
 osa/veto.py
 osa/_dev_version/__init__.py
 osa/configs/__init__.py
@@ -102,14 +104,15 @@
 osa/scripts/show_run_summary.py
 osa/scripts/simulate_processing.py
 osa/scripts/tests/__init__.py
 osa/scripts/tests/test_osa_scripts.py
 osa/tests/__init__.py
 osa/tests/test_jobs.py
 osa/tests/test_osa.py
+osa/tests/test_osadb.py
 osa/tests/test_paths.py
 osa/tests/test_raw.py
 osa/tests/test_report.py
 osa/tests/test_veto.py
 osa/utils/__init__.py
 osa/utils/cliopts.py
 osa/utils/iofile.py
@@ -119,8 +122,10 @@
 osa/utils/utils.py
 osa/utils/tests/test_iofile.py
 osa/utils/tests/test_utils.py
 osa/webserver/__init__.py
 osa/webserver/utils.py
 osa/workflow/__init__.py
 osa/workflow/dl3.py
-osa/workflow/tests/test_dl3.py
+osa/workflow/stages.py
+osa/workflow/tests/test_dl3.py
+osa/workflow/tests/test_stages.py
```

### Comparing `lstosa-0.9.4/lstosa.egg-info/entry_points.txt` & `lstosa-0.9.5/lstosa.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/osa/configs/config.py` & `lstosa-0.9.5/osa/configs/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from importlib_resources import files
 
 from osa.configs import options
 from osa.utils.logging import myLogger
 
 log = myLogger(logging.getLogger(__name__))
 
-__all__ = ['read_config', 'cfg', 'DEFAULT_CFG']
+__all__ = ["read_config", "cfg", "DEFAULT_CFG"]
 
 
 DEFAULT_CFG = files("osa").joinpath("configs/sequencer.cfg")
 
 
 def read_config():
     """
```

### Comparing `lstosa-0.9.4/osa/configs/datamodel.py` & `lstosa-0.9.5/osa/configs/datamodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,32 @@
-class Period(object):
-    def __init__(self):
-        self.period = None
-
+"""Definition of classes containing run and sequence information"""
 
-class Night(Period):
-    def __init__(self):
-        super(Night, self).__init__()
-        self.night = None
+from dataclasses import dataclass
 
 
-class Telescope(Night):
-    def __init__(self):
-        super(Telescope, self).__init__()
-        self.telescope = None
-
-
-class Source(Telescope):
-    def __init__(self):
-        super(Source, self).__init__()
-        self.source_name = None
-        self.source_ra = None
-        self.source_dec = None
-
-
-class Wobble(Source):
-    def __init__(self):
-        super(Wobble, self).__init__()
-        self.sourcewobble = None
-        self.wobble = None
-
-
-class RunObj(Wobble):
-    def __init__(self):
-        super(RunObj, self).__init__()
-        self.run_str = None
-        self.run = None
-        self.type = None
-        self.subrun_list = []
-        self.subruns = None
-
-
-class SubrunObj(RunObj):
-    def __init__(self):
-        super(SubrunObj, self).__init__()
-        self.runobj = None
-        self.subrun = None
-        self.kind = None
-        self.timestamp = None
-        self.time = None
-        self.date = None
-        self.ucts_timestamp = None
-        self.dragon_reference_time = None
-        self.dragon_reference_module_id = None
-        self.dragon_reference_module_index = None
-        self.dragon_reference_counter = None
-        self.dragon_reference_source = None
+@dataclass
+class RunObj:
+    run_str: str = None
+    run: int = None
+    type: str = None
+    subruns: int = None
+    source_name: str = None
+    source_ra: float = None
+    source_dec: float = None
+    telescope: str = "LST1"
+    night: str = None
 
 
 class Sequence(RunObj):
     def __init__(self):
         super(Sequence, self).__init__()
         self.seq = None
-        self.parent_list = []
+        self.pedcal_run = None
+        self.drs4_run = None
         self.parent = None
-        self.parentjobid = None
         self.previousrun = None
         self.script = None
         self.veto = None
         self.closed = None
         self.history = None
         self.queue = None
         self.jobname = None
@@ -86,24 +45,29 @@
 
 
 class SequenceCalibration(Sequence):
     def __init__(self, r):
         super(SequenceCalibration, self).__init__()
         super(SequenceCalibration, self).associate(r)
         self.calibstatus = None
+        self.seq = 1
+        self.parent = None
+        self.drs4_run = None
 
 
 class SequenceData(Sequence):
     def __init__(self, r):
         super(SequenceData, self).__init__()
         super(SequenceData, self).associate(r)
-        self.calibration = None
-        self.pedestal = None
+        self.parent = 1
+        self.time_calibration_run = None
         self.drive = None
-        self.time_calibration = None
-        self.systematic_correction = None
+        self.drs4_file = None
+        self.calibration_file = None
+        self.time_calibration_file = None
+        self.systematic_correction_file = None
         self.dl1status = None
         self.dl1abstatus = None
         self.muonstatus = None
         self.datacheckstatus = None
         self.dl2status = None
         self.dl3status = None
```

### Comparing `lstosa-0.9.4/osa/configs/options.py` & `lstosa-0.9.5/osa/configs/options.py`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/osa/configs/sequencer.cfg` & `lstosa-0.9.5/osa/configs/sequencer.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 dl1a_config: /software/lstchain/data/lstchain_standard_config.json
 store_image_dl1ab: True
 merge_dl1_datacheck: True
 dl1b_config: /software/lstchain/data/lstchain_standard_config.json
 dl2_config: /software/lstchain/data/lstchain_standard_config.json
 rf_models: /data/models/prod5/zenith_20deg/20201023_v0.6.3
 dl3_config: /software/lstchain/data/dl3_std_config.json
+max_tries: 3
 
 [MC]
 IRF_file: /path/to/irf.fits
 gamma: /path/to/DL2/gamma_mc_testing.h5
 proton: /path/to/DL2/proton_mc_testing.h5
 electron: /path/to/DL2/electron_mc_testing.h5
 
@@ -84,24 +85,17 @@
 [CACHE]
 # Sometimes when working with clusters and job schedulers, cache
 # directories need to be specified by the user. Otherwise leave them empty.
 CTAPIPE_CACHE: /fefs/aswg/lstanalyzer/.ctapipe/ctapipe_cache
 CTAPIPE_SVC_PATH: /fefs/aswg/lstanalyzer/.ctapipe/service
 MPLCONFIGDIR: /fefs/aswg/lstanalyzer/.cache/matplotlib
 
-[MYSQL]
-# Currently in development
-SERVER: hostname
-USER: username
-DATABASE: LST
-DAQTABLE: DAQ
-SEQUENCETABLE: SEQUENCE
-ANALYSISTABLE: ANALYSIS
-SUMMARYTABLE: SUMMARY
-STORAGETABLE: STORAGE
+[database]
+path: test_osa/test_files0/OSA/osa.db
+CaCo_db: mongodb://10.200.10.101:27017/
 
 [mail]
 recipient: your@email.com
 
 # From here on, users should not need to change anything.
 [PATTERN]
 # Prefixes
```

### Comparing `lstosa-0.9.4/osa/conftest.py` & `lstosa-0.9.5/osa/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from textwrap import dedent
 
 import pytest
 
 from osa.configs import options
 from osa.configs.config import cfg
-from osa.nightsummary.extract import extractruns, extractsubruns, extractsequences
+from osa.nightsummary.extract import extract_runs, extract_sequences
 from osa.nightsummary.nightsummary import run_summary_table
 from osa.scripts.tests.test_osa_scripts import run_program
 from osa.utils.utils import date_to_dir
 from datetime import datetime
 
 date = datetime.fromisoformat("2020-01-17")
 nightdir = date_to_dir(date)
@@ -159,15 +159,15 @@
     directory.mkdir(parents=True, exist_ok=True)
     return directory
 
 
 @pytest.fixture(scope="session")
 def calibration_file(calibration_dir):
     """Mock calibration files for testing."""
-    calib_file = calibration_dir / "calibration_filters_52.Run01805.0000.h5"
+    calib_file = calibration_dir / "calibration_filters_52.Run01809.0000.h5"
     calib_file.touch()
     return calib_file
 
 
 @pytest.fixture(scope="session")
 def drs4_baseline_file(drs4_baseline_dir):
     """Mock calibration files for testing."""
@@ -201,15 +201,16 @@
 
     return file_1, file_2
 
 
 @pytest.fixture(scope="session")
 def run_summary_file(run_summary_dir):
 
-    summary_content = dedent("""\
+    summary_content = dedent(
+        """\
     # %ECSV 0.9
     # ---
     # datatype:
     # - {name: run_id, datatype: int64}
     # - {name: n_subruns, datatype: int64}
     # - {name: run_type, datatype: string}
     # - {name: ucts_timestamp, datatype: int64}
@@ -221,30 +222,34 @@
     # - {name: dragon_reference_source, datatype: string}
     # delimiter: ','
     # meta: !!omap
     # - {date: '2020-01-17'}
     # - {lstchain_version: 0.7.0}
     # schema: astropy-2.0
     run_id,n_subruns,run_type,ucts_timestamp,run_start,dragon_reference_time,dragon_reference_module_id,dragon_reference_module_index,dragon_reference_counter,dragon_reference_source
+    1803,6,DRS4,1579289727863850890,1579289712000000000,1579289727863850890,90,0,5863850400,ucts
     1804,6,DRS4,1579289727863850890,1579289712000000000,1579289727863850890,90,0,5863850400,ucts
     1805,5,PEDCALIB,1579291426030146503,1579291413000000000,1579291426030146503,90,0,2030146000,ucts
     1806,5,PEDCALIB,1579291932080485703,1579291917000000000,1579291932080485703,90,0,5080485200,ucts
     1807,11,DATA,1579292477145904430,1579292461000000000,1579292477145904430,90,0,6145904000,ucts
-    1808,9,DATA,1579292985532016507,1579292975000000000,1579292985532016507,90,0,2532016000,ucts""")
+    1808,9,DATA,1579292985532016507,1579292975000000000,1579292985532016507,90,0,2532016000,ucts
+    1809,5,PEDCALIB,1579291932080485703,1579291917000000000,1579291932080485703,90,0,5080485200,ucts"""
+    )
 
-    summary_file = run_summary_dir / 'RunSummary_20200117.ecsv'
+    summary_file = run_summary_dir / "RunSummary_20200117.ecsv"
     summary_file.touch()
     summary_file.write_text(summary_content)
     return summary_file
 
 
 @pytest.fixture(scope="session")
 def merged_run_summary(base_test_dir):
     """Mock merged run summary file for testing."""
-    summary_content = dedent("""\
+    summary_content = dedent(
+        """\
     # %ECSV 1.0
     # ---
     # datatype:
     # - {name: date, datatype: string}
     # - {name: run_id, datatype: int64}
     # - {name: run_type, datatype: string}
     # - {name: n_subruns, datatype: int64}
@@ -269,20 +274,22 @@
     2019-11-23 1614 PEDCALIB 10 2019-11-23T23:33:59.000 4.6 2.1 1.1 4.5
     2019-11-23 1615 DATA 61 2019-11-23T23:41:13.000 8.1 45.1 1.5 4.6
     2019-11-23 1616 DATA 62 2019-11-24T00:11:52.000 3.2 4.2 0.9 1.6
     2020-01-17 1804 DRS4 35 2020-01-18T00:44:06.000 2.1 42.9 11.3 4.7
     2020-01-17 1805 PEDCALIB 62 2020-01-18T00:11:52.000 13.9 21.9 17.9 1.6
     2020-01-17 1806 PEDCALIB 35 2020-01-18T00:44:06.000 8.6 29.1 45.5 6.9
     2020-01-17 1807 DATA 35 2020-01-18T00:44:06.000 6.6 2.8 70.4 10.1
-    2020-01-17 1808 DATA 35 2020-01-18T00:44:06.000 8.6 9.2 60.8 3.2""")
+    2020-01-17 1808 DATA 35 2020-01-18T00:44:06.000 8.6 9.2 60.8 3.2
+    2020-01-17 1809 PEDCALIB 4 2020-01-18T00:44:06.000 6.9 4.2 16.8 11.2"""
+    )
 
     merged_summary_dir = base_test_dir / "OSA/Catalog"
     merged_summary_dir.mkdir(parents=True, exist_ok=True)
 
-    file = merged_summary_dir / 'merged_RunSummary.ecsv'
+    file = merged_summary_dir / "merged_RunSummary.ecsv"
     file.touch()
     file.write_text(summary_content)
     return file
 
 
 @pytest.fixture(scope="session")
 def run_summary(run_summary_file):
@@ -299,21 +306,21 @@
     file = pedestal_ids_dir / "pedestal_ids_Run01808.0000.h5"
     file.touch()
     return file
 
 
 @pytest.fixture(scope="session")
 def sequence_list(
-        running_analysis_dir,
-        run_summary,
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        r0_data,
-        pedestal_ids_file,
-        merged_run_summary
+    running_analysis_dir,
+    run_summary,
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    r0_data,
+    pedestal_ids_file,
+    merged_run_summary,
 ):
     """Creates a sequence list from a run summary file."""
     options.directory = running_analysis_dir
     options.simulate = True
     options.test = True
 
     for file in drs4_time_calibration_files:
@@ -324,55 +331,56 @@
 
     for file in r0_data:
         assert file.exists()
 
     assert pedestal_ids_file.exists()
     assert merged_run_summary.exists()
 
-    subrun_list = extractsubruns(run_summary)
-    run_list = extractruns(subrun_list)
+    run_list = extract_runs(run_summary)
     options.test = False
-    return extractsequences(run_list)
+    return extract_sequences(options.date, run_list)
 
 
 @pytest.fixture(scope="session")
 def sequence_file_list(
-        running_analysis_dir,
-        run_summary_file,
-        run_catalog,
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        r0_data
+    running_analysis_dir,
+    run_summary_file,
+    run_catalog,
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    r0_data,
 ):
     for r0_file in r0_data:
         assert r0_file.exists()
 
     for file in drs4_time_calibration_files:
         assert file.exists()
 
     for file in systematic_correction_files:
         assert file.exists()
 
     assert run_summary_file.exists()
     assert run_catalog.exists()
 
     run_program("sequencer", "-d", "2020-01-17", "--no-submit", "-t", "LST1")
+    # First sequence in the list corresponds to the calibration run 1809
     return [
-        running_analysis_dir / "sequence_LST1_01805.py",
+        running_analysis_dir / "sequence_LST1_01809.py",
         running_analysis_dir / "sequence_LST1_01807.py",
         running_analysis_dir / "sequence_LST1_01808.py",
     ]
 
 
 @pytest.fixture(scope="session")
 def txt_file_test(running_analysis_dir):
     from osa.utils.iofile import write_to_file
+
     options.simulate = False
     file = running_analysis_dir / "test.txt"
-    write_to_file(file, 'This is a test')
+    write_to_file(file, "This is a test")
     options.simulate = True
     return file
 
 
 @pytest.fixture(scope="session")
 def datacheck_dl1_files(base_test_dir):
     dl1b_dir = base_test_dir / "DL1" / "20200117" / "v0.1.0" / "tailcut84"
@@ -402,15 +410,15 @@
     return html_file, h5_file, log_file
 
 
 @pytest.fixture(scope="session")
 def calibration_check_plot(calibration_dir):
     calibration_dir_log = calibration_dir / "log"
     calibration_dir_log.mkdir(parents=True, exist_ok=True)
-    file = calibration_dir_log / "calibration_filters_52.Run01805.0000.pdf"
+    file = calibration_dir_log / "calibration_filters_52.Run01809.0000.pdf"
     file.touch()
     return file
 
 
 @pytest.fixture(scope="session")
 def drs4_check_plot(drs4_baseline_dir):
     drs4_baseline_dir_log = drs4_baseline_dir / "log"
@@ -418,25 +426,44 @@
     file = drs4_baseline_dir_log / "drs4_pedestal.Run01804.0000.pdf"
     file.touch()
     return file
 
 
 @pytest.fixture(scope="session")
 def run_catalog(run_catalog_dir):
-    source_information = dedent("""\
+    source_information = dedent(
+        """\
     # %ECSV 1.0
     # ---
     # datatype:
     # - {name: run_id, datatype: int32}
     # - {name: source_name, datatype: string}
     # - {name: source_ra, datatype: float64}
     # - {name: source_dec, datatype: float64}
     # delimiter: ','
     # schema: astropy-2.0
     run_id,source_name,source_ra,source_dec
     1807,Crab,83.543,22.08
-    1808,MadeUpSource,115.441,43.98""")
+    1808,MadeUpSource,115.441,43.98"""
+    )
 
-    catalog_file = run_catalog_dir / 'RunCatalog_20200117.ecsv'
+    catalog_file = run_catalog_dir / "RunCatalog_20200117.ecsv"
     catalog_file.touch()
     catalog_file.write_text(source_information)
     return catalog_file
+
+
+@pytest.fixture(scope="session")
+def database(base_test_dir):
+    import sqlite3
+
+    osa_dir = base_test_dir / "OSA"
+    osa_dir.mkdir(parents=True, exist_ok=True)
+    db_file = osa_dir / "osa.db"
+    with sqlite3.connect(db_file) as connection:
+        cursor = connection.cursor()
+        cursor.execute(
+            """CREATE TABLE IF NOT EXISTS processing
+            (telescope, date, prod_id, start, end, is_finished)"""
+        )
+        cursor.connection.commit()
+        yield cursor
```

### Comparing `lstosa-0.9.4/osa/high_level/significance.py` & `lstosa-0.9.5/osa/high_level/significance.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,39 +15,37 @@
 import click
 import numpy as np
 import pandas as pd
 import toml
 from ctapipe.containers import EventType
 from gammapy.stats import WStatCountsStatistic
 from lstchain.io.io import dl2_params_lstcam_key
-from lstchain.reco.utils import (
-    get_effective_time, extract_source_position, compute_theta2
-)
+from lstchain.reco.utils import get_effective_time, extract_source_position, compute_theta2
 from matplotlib import pyplot as plt
 
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.nightsummary.extract import get_source_list
 from osa.paths import DEFAULT_CFG, destination_dir, analysis_path
 from osa.utils.cliopts import get_prod_id, get_dl2_prod_id
 from osa.utils.logging import myLogger
 from osa.utils.utils import date_to_dir, YESTERDAY
 
 __all__ = [
-    'create_hist',
-    'lima_significance',
-    'event_selection',
-    'plot_theta2',
+    "create_hist",
+    "lima_significance",
+    "event_selection",
+    "plot_theta2",
 ]
 
 from osa.webserver.utils import directory_in_webserver
 
 log = myLogger(logging.getLogger(__name__))
 
-SELECTION_CUTS_FILE = Path(__file__).parent / 'selection_cuts.toml'
+SELECTION_CUTS_FILE = Path(__file__).parent / "selection_cuts.toml"
 
 mpl_linewidth = 1.6
 mpl_rc = {
     "figure.autolayout": True,
     "figure.dpi": 150,
     "font.size": 12,
     "lines.linewidth": mpl_linewidth,
@@ -82,20 +80,20 @@
     bin_width = bin_edges_on[1] - bin_edges_off[0]
     bin_center = bin_edges_on[:-1] + (bin_width / 2)
 
     return hist_on, hist_off, bin_edges_on, bin_edges_off, bin_center
 
 
 def lima_significance(
-        hist_on,
-        hist_off,
-        bin_edges_on,
-        bin_edges_off,
-        eff_time,
-        cuts: MutableMapping[str, Any],
+    hist_on,
+    hist_off,
+    bin_edges_on,
+    bin_edges_off,
+    eff_time,
+    cuts: MutableMapping[str, Any],
 ):
     """Return the text containing LiMa significance and statistics for plotting them."""
     N_on = np.sum(hist_on[bin_edges_on[1:] <= cuts["theta2_global_cut"]])
     N_off = np.sum(hist_off[bin_edges_off[1:] <= cuts["theta2_global_cut"]])
 
     idx_min = (np.abs(bin_edges_on - cuts["theta2_norm_range_min"])).argmin()
     idx_max = (np.abs(bin_edges_on - cuts["theta2_norm_range_max"])).argmin()
@@ -105,129 +103,121 @@
 
     alpha = Noff_norm / Non_norm
 
     stat = WStatCountsStatistic(n_on=N_on, n_off=N_off, alpha=alpha)
     significance_lima = stat.sqrt_ts
 
     text_statistics = (
-        f'N$_{{\\rm on}}$ = {N_on:.0f}\n'
-        f'N$_{{\\rm off}}$ = {N_off:.0f}\n'
-        f'Livetime = {eff_time.to(u.h):.1f}\n'
-        f'Li&Ma significance = {significance_lima:.1f} $\\sigma$'
+        f"N$_{{\\rm on}}$ = {N_on:.0f}\n"
+        f"N$_{{\\rm off}}$ = {N_off:.0f}\n"
+        f"Livetime = {eff_time.to(u.h):.1f}\n"
+        f"Li&Ma significance = {significance_lima:.1f} $\\sigma$"
     )
     log.info(text_statistics)
 
-    box_color = 'yellow' if significance_lima > 5 else 'white'
+    box_color = "yellow" if significance_lima > 5 else "white"
 
     return text_statistics, box_color
 
 
-def event_selection(
-        data: pd.DataFrame,
-        cuts: MutableMapping[str, Any]
-) -> pd.DataFrame:
+def event_selection(data: pd.DataFrame, cuts: MutableMapping[str, Any]) -> pd.DataFrame:
     """Return the dataframe with the selected events."""
     gammaness = np.array(data.gammaness)
     event_type = np.array(data.event_type)
 
     log.info(
         f'Gammaness global cut: {cuts["gammaness_global_cut"]}\n'
         f'Theta2 global cut: {cuts["theta2_global_cut"]}\n'
     )
     # Mask for event selection
     condition = (
-        (gammaness > cuts["gammaness_global_cut"]) &
-        (event_type != EventType.FLATFIELD.value) &
-        (event_type != EventType.SKY_PEDESTAL.value)
+        (gammaness > cuts["gammaness_global_cut"])
+        & (event_type != EventType.FLATFIELD.value)
+        & (event_type != EventType.SKY_PEDESTAL.value)
     )
     return data[condition]
 
 
 def plot_theta2(
-        bin_center,
-        hist_on,
-        hist_off,
-        legend_text,
-        box_color,
-        source_name,
-        date_obs,
-        runs,
-        highlevel_dir,
-        cuts: MutableMapping[str, Any],
+    bin_center,
+    hist_on,
+    hist_off,
+    legend_text,
+    box_color,
+    source_name,
+    date_obs,
+    runs,
+    highlevel_dir,
+    cuts: MutableMapping[str, Any],
 ):
     """Plot theta2 histogram and save the figure."""
     _, ax = plt.subplots()
 
     ax.errorbar(
         bin_center,
         hist_on,
         yerr=np.sqrt(hist_on),
-        fmt='o',
-        label='ON data',
+        fmt="o",
+        label="ON data",
     )
     ax.errorbar(
         bin_center,
         hist_off,
         yerr=np.sqrt(hist_off),
-        fmt='s',
-        label='Background',
+        fmt="s",
+        label="Background",
     )
     ax.set_xlim(0, 0.5)
-    ax.axvline(cuts["theta2_global_cut"], color='black', ls='--', alpha=0.75)
+    ax.axvline(cuts["theta2_global_cut"], color="black", ls="--", alpha=0.75)
     ax.set_xlabel("$\\theta^{2}$ [deg$^{2}$]")
     ax.set_ylabel("Counts")
-    ax.legend(
-        title=legend_text, facecolor=box_color, loc='upper right'
-    )._legend_box.align = 'left'
-    ax.set_title(
-        f"Source: {source_name}. Date: {date_obs.strftime('%Y-%m-%d')}\n Runs: {runs}"
-    )
-    plot_path = (
-        highlevel_dir / f"Theta2_{source_name}_{date_obs.strftime('%Y-%m-%d')}.png"
-    )
+    ax.legend(title=legend_text, facecolor=box_color, loc="upper right")._legend_box.align = "left"
+    ax.set_title(f"Source: {source_name}. Date: {date_obs.strftime('%Y-%m-%d')}\n Runs: {runs}")
+    plot_path = highlevel_dir / f"Theta2_{source_name}_{date_obs.strftime('%Y-%m-%d')}.png"
     plt.savefig(plot_path, dpi=300)
     return plot_path
 
 
 @click.command()
-@click.argument('telescope', type=click.Choice(['LST1']))
+@click.argument("telescope", type=click.Choice(["LST1"]))
 @click.option(
-    '-d',
-    '--date',
+    "-d",
+    "--date",
     type=click.DateTime(formats=["%Y-%m-%d"]),
-    default=YESTERDAY.strftime("%Y-%m-%d")
+    default=YESTERDAY.strftime("%Y-%m-%d"),
 )
 @click.option(
-    '-c', '--config',
+    "-c",
+    "--config",
     type=click.Path(dir_okay=False),
     default=DEFAULT_CFG,
-    help='Read option defaults from the specified cfg file',
+    help="Read option defaults from the specified cfg file",
 )
-@click.option('-s', '--simulate', is_flag=True)
+@click.option("-s", "--simulate", is_flag=True)
 def main(
-        date: datetime = YESTERDAY,
-        telescope: str = "LST1",
-        config: Path = DEFAULT_CFG,
-        simulate: bool = False,
+    date: datetime = YESTERDAY,
+    telescope: str = "LST1",
+    config: Path = DEFAULT_CFG,
+    simulate: bool = False,
 ):
     """Plot theta2 histograms for each source from a given date."""
     log.setLevel(logging.INFO)
 
     log.debug(f"Config: {config.resolve()}")
 
     # Initial setup of global parameters
     options.date = date
     flat_date = date_to_dir(date)
     options.tel_id = telescope
     options.prod_id = get_prod_id()
     options.dl2_prod_id = get_dl2_prod_id()
     options.directory = analysis_path(options.tel_id)
-    dl2_directory = Path(cfg.get('LST1', 'DL2_DIR'))
+    dl2_directory = Path(cfg.get("LST1", "DL2_DIR"))
     highlevel_directory = destination_dir("HIGH_LEVEL", create_dir=True)
-    host = cfg.get('WEBSERVER', 'HOST')
+    host = cfg.get("WEBSERVER", "HOST")
     cuts = toml.load(SELECTION_CUTS_FILE)
 
     sources = get_source_list(date)
     log.info(f"Sources: {sources}")
 
     for source in sources:
         df = pd.DataFrame()
@@ -235,66 +225,59 @@
         log.info(f"Source: {source}, runs: {runs}")
 
         if simulate:
             continue
 
         for run in runs:
             input_file = (
-                dl2_directory / flat_date / options.prod_id / options.dl2_prod_id /
-                f"dl2_LST-1.Run{run:05d}.h5"
-            )
-            df = pd.concat(
-                [df, pd.read_hdf(input_file, key=dl2_params_lstcam_key)]
+                dl2_directory
+                / flat_date
+                / options.prod_id
+                / options.dl2_prod_id
+                / f"dl2_LST-1.Run{run:05d}.h5"
             )
+            df = pd.concat([df, pd.read_hdf(input_file, key=dl2_params_lstcam_key)])
 
         selected_events = event_selection(data=df, cuts=cuts)
 
         try:
             true_source_position = extract_source_position(
-                data=selected_events,
-                observed_source_name=source
+                data=selected_events, observed_source_name=source
             )
             off_source_position = [element * -1 for element in true_source_position]
 
-            theta2_on = np.array(
-                compute_theta2(selected_events, true_source_position)
-            )
-            theta2_off = np.array(
-                compute_theta2(selected_events, off_source_position)
-            )
+            theta2_on = np.array(compute_theta2(selected_events, true_source_position))
+            theta2_off = np.array(compute_theta2(selected_events, off_source_position))
 
             hist_on, hist_off, bin_edges_on, bin_edges_off, bin_center = create_hist(
                 theta2_on, theta2_off, cuts
             )
             text, box_color = lima_significance(
                 hist_on=hist_on,
                 hist_off=hist_off,
                 bin_edges_on=bin_edges_on,
                 bin_edges_off=bin_edges_off,
                 eff_time=get_effective_time(df)[0],
-                cuts=cuts
+                cuts=cuts,
             )
             pdf_file = plot_theta2(
                 bin_center=bin_center,
                 hist_on=hist_on,
                 hist_off=hist_off,
                 legend_text=text,
                 box_color=box_color,
                 source_name=source,
                 date_obs=date,
                 runs=runs,
                 highlevel_dir=highlevel_directory,
-                cuts=cuts
+                cuts=cuts,
             )
             if not simulate:
                 dest_directory = directory_in_webserver(
-                    host=host,
-                    datacheck_type="HIGH_LEVEL",
-                    date=flat_date,
-                    prod_id=options.prod_id
+                    host=host, datacheck_type="HIGH_LEVEL", date=flat_date, prod_id=options.prod_id
                 )
                 cmd = ["scp", pdf_file, f"{host}:{dest_directory}/."]
                 subprocess.run(cmd, capture_output=True, check=True)
 
         except astropy.coordinates.name_resolve.NameResolveError:
             log.warning(f"Source {source} not found in the catalog. Skipping.")
             # TODO: get ra/dec from the TCU database instead
```

### Comparing `lstosa-0.9.4/osa/job.py` & `lstosa-0.9.5/osa/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,34 @@
 import logging
 import shutil
 import subprocess as sp
 import time
 from io import StringIO
 from pathlib import Path
 from textwrap import dedent
-from typing import List, Iterable, Optional
+from typing import Iterable
 
 import matplotlib.pyplot as plt
 import pandas as pd
 
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.paths import (
     pedestal_ids_file_exists,
     get_drive_file,
     get_summary_file,
-    get_pedestal_ids_file
+    get_pedestal_ids_file,
 )
-from osa.report import history
 from osa.utils.iofile import write_to_file
 from osa.utils.logging import myLogger
-from osa.utils.utils import (
-    date_to_dir,
-    time_to_seconds,
-    stringify, date_to_iso
-)
+from osa.utils.utils import date_to_dir, time_to_seconds, stringify, date_to_iso
 
 log = myLogger(logging.getLogger(__name__))
 
 __all__ = [
-    "run_program_with_history_logging",
     "are_all_jobs_correctly_finished",
     "historylevel",
     "prepare_jobs",
     "sequence_filenames",
     "set_queue_values",
     "job_header_template",
     "plot_job_statistics",
@@ -48,15 +42,15 @@
     "get_sacct_output",
     "get_squeue_output",
     "filter_jobs",
     "run_sacct",
     "run_squeue",
     "calibration_sequence_job_template",
     "data_sequence_job_template",
-    "save_job_information"
+    "save_job_information",
 ]
 
 TAB = "\t".expandtabs(4)
 FORMAT_SLURM = [
     "JobID",
     "JobName",
     "CPUTime",
@@ -105,26 +99,25 @@
             # looking for .../sequence_LST1_04180.history files
             # we need to check all the subrun wise history files
             # .../sequence_LST1_04180.XXXX.history
             out, _ = historylevel(history_file, sequence.type)
             if out == 0:
                 log.debug(f"Job {sequence.seq} ({sequence.type}) correctly finished")
                 continue
-            elif out == 1 and options.no_dl2:
+            if out == 1 and options.no_dl2:
                 log.debug(
                     f"Job {sequence.seq} ({sequence.type}) correctly "
                     f"finished up to DL1ab, but --no-dl2 option selected"
                 )
                 continue
-            else:
-                log.warning(
-                    f"Job {sequence.seq} (run {sequence.run}) not "
-                    f"correctly finished [level {out}]"
-                )
-                flag = False
+
+            log.warning(
+                f"Job {sequence.seq} (run {sequence.run}) not correctly finished [level {out}]"
+            )
+            flag = False
     return flag
 
 
 def check_history_level(history_file: Path, program_levels: dict):
     """
     Check the history of the calibration sequence.
 
@@ -146,18 +139,18 @@
     # Check the program exit_status (last string of the line), if it is 0, go
     # to the next level and check the next program. If exit_status is not 0, return the
     # actual level and the exit status. Stop the iteration when reaching the level 0.
     with open(history_file, "r") as file:
         for line in file:
             program = line.split()[1]
             exit_status = int(line.split()[-1])
-            if program in program_levels and exit_status != 0:
-                level = program_levels[program]
-                return level, exit_status
-            if program in program_levels and exit_status == 0:
+            if program in program_levels:
+                if exit_status != 0:
+                    level = program_levels[program]
+                    return level, exit_status
                 level = program_levels[program]
                 continue
 
         return level, exit_status
 
 
 def historylevel(history_file: Path, data_type: str):
@@ -206,39 +199,33 @@
     if history_file.exists():
         for line in history_file.read_text().splitlines():
             words = line.split()
             try:
                 program = words[1]
                 prod_id = words[2]
                 exit_status = int(words[-1])
-                log.debug(
-                    f"{program}, finished with error {exit_status} and prod ID {prod_id}"
-                )
+                log.debug(f"{program}, finished with error {exit_status} and prod ID {prod_id}")
             except (IndexError, ValueError) as err:
                 log.exception(f"Malformed history file {history_file}, {err}")
             else:
                 # Calibration sequence
                 if program == cfg.get("lstchain", "drs4_baseline"):
                     level = 1 if exit_status == 0 else 2
                 elif program == cfg.get("lstchain", "charge_calibration"):
                     level = 0 if exit_status == 0 else 1
                 # Data sequence
                 elif program == cfg.get("lstchain", "r0_to_dl1"):
                     level = 3 if exit_status == 0 else 4
                 elif program == cfg.get("lstchain", "dl1ab"):
                     if (exit_status == 0) and (prod_id == options.dl1_prod_id):
-                        log.debug(
-                            f"DL1ab prod ID: {options.dl1_prod_id} already produced"
-                        )
+                        log.debug(f"DL1ab prod ID: {options.dl1_prod_id} already produced")
                         level = 2
                     else:
                         level = 3
-                        log.debug(
-                            f"DL1ab prod ID: {options.dl1_prod_id} not produced yet"
-                        )
+                        log.debug(f"DL1ab prod ID: {options.dl1_prod_id} not produced yet")
                         break
                 elif program == cfg.get("lstchain", "check_dl1"):
                     level = 1 if exit_status == 0 else 2
                 elif program == cfg.get("lstchain", "dl1_to_dl2"):
                     if (exit_status == 0) and (prod_id == options.dl2_prod_id):
                         log.debug(f"DL2 prod ID: {options.dl2_prod_id} already produced")
                         level = 0
@@ -288,17 +275,15 @@
     sacct_output = run_sacct()
     jobs_df = get_sacct_output(sacct_output)
 
     # Fetch sacct output and prepare the data
     jobs_df_filtered = jobs_df.copy()
     jobs_df_filtered = jobs_df_filtered.dropna()
     # Remove the G from MaxRSS value and convert to float
-    jobs_df_filtered["MaxRSS"] = (
-        jobs_df_filtered["MaxRSS"].str.strip("G").astype(float)
-    )
+    jobs_df_filtered["MaxRSS"] = jobs_df_filtered["MaxRSS"].str.strip("G").astype(float)
 
     jobs_df_filtered.to_csv(file_path, index=False, sep=",")
 
 
 def plot_job_statistics(sacct_output: pd.DataFrame, directory: Path):
     """
     Get statistics of the jobs. Check elapsed time used,
@@ -316,17 +301,15 @@
     #  the jobs are done for a given production.
 
     # Plot a 2D histogram of the used memory (MaxRSS) as a function of the
     # elapsed time taking also into account the State of the job.
     sacct_output_filter = sacct_output.copy()
     sacct_output_filter = sacct_output_filter.dropna()
     # Remove the G from MaxRSS value and convert to float
-    sacct_output_filter["MaxRSS"] = (
-        sacct_output_filter["MaxRSS"].str.strip("G").astype(float)
-    )
+    sacct_output_filter["MaxRSS"] = sacct_output_filter["MaxRSS"].str.strip("G").astype(float)
 
     plt.figure()
     plt.hist2d(sacct_output_filter.MaxRSS, sacct_output_filter.CPUTimeRAW / 3600, bins=50)
     plt.xlabel("MaxRSS [GB]")
     plt.ylabel("Elapsed time [h]")
     directory.mkdir(exist_ok=True, parents=True)
     plot_path = directory / "job_statistics.pdf"
@@ -345,28 +328,24 @@
         f"--job-name={sequence.jobname}",
         f"--time={cfg.get('SLURM', 'WALLTIME')}",
         f"--chdir={options.directory}",
         f"--output=log/Run{sequence.run:05d}.%4a_jobid_%A.out",
         f"--error=log/Run{sequence.run:05d}.%4a_jobid_%A.err",
     ]
 
-    # Get the number of subruns. The number of subruns starts counting from 0.
-    subruns = int(sequence.subrun_list[-1].subrun) - 1
+    # Get the number of subruns counting from 0.
+    subruns = sequence.subruns - 1
 
     # Depending on the type of sequence, we need to set
     # different sbatch environment variables
     if sequence.type == "DATA":
         sbatch_parameters.append(f"--array=0-{subruns}")
 
-    sbatch_parameters.append(
-        f"--partition={cfg.get('SLURM', f'PARTITION_{sequence.type}')}"
-    )
-    sbatch_parameters.append(
-        f"--mem-per-cpu={cfg.get('SLURM', f'MEMSIZE_{sequence.type}')}"
-    )
+    sbatch_parameters.append(f"--partition={cfg.get('SLURM', f'PARTITION_{sequence.type}')}")
+    sbatch_parameters.append(f"--mem-per-cpu={cfg.get('SLURM', f'MEMSIZE_{sequence.type}')}")
 
     return ["#SBATCH " + line for line in sbatch_parameters]
 
 
 def job_header_template(sequence):
     """
     Returns a string with the job header template
@@ -438,27 +417,30 @@
     commandargs = ["datasequence"]
 
     if options.verbose:
         commandargs.append("-v")
     if options.simulate:
         commandargs.append("-s")
     if options.configfile:
-        commandargs.append("--config")
-        commandargs.append(f"{Path(options.configfile).resolve()}")
+        commandargs.extend(("--config", f"{Path(options.configfile).resolve()}"))
     if sequence.type == "DATA" and options.no_dl2:
         commandargs.append("--no-dl2")
 
-    commandargs.append(f"--date={date_to_iso(options.date)}")
-    commandargs.append(f"--prod-id={options.prod_id}")
-    commandargs.append(f"--drs4-pedestal-file={sequence.pedestal}")
-    commandargs.append(f"--time-calib-file={sequence.time_calibration}")
-    commandargs.append(f"--pedcal-file={sequence.calibration}")
-    commandargs.append(f"--systematic-correction-file={sequence.systematic_correction}")
-    commandargs.append(f"--drive-file={get_drive_file(flat_date)}")
-    commandargs.append(f"--run-summary={get_summary_file(flat_date)}")
+    commandargs.extend(
+        (
+            f"--date={date_to_iso(options.date)}",
+            f"--prod-id={options.prod_id}",
+            f"--drs4-pedestal-file={sequence.drs4_file}",
+            f"--time-calib-file={sequence.time_calibration_file}",
+            f"--pedcal-file={sequence.calibration_file}",
+            f"--systematic-correction-file={sequence.systematic_correction_file}",
+            f"--drive-file={get_drive_file(flat_date)}",
+            f"--run-summary={get_summary_file(flat_date)}",
+        )
+    )
 
     content = job_header + "\n" + PYTHON_IMPORTS
 
     if not options.test:
         content += set_cache_dirs()
         content += "\n"
         # Use the SLURM env variables
@@ -513,20 +495,22 @@
     commandargs = ["calibration_pipeline"]
 
     if options.verbose:
         commandargs.append("-v")
     if options.simulate:
         commandargs.append("-s")
     if options.configfile:
-        commandargs.append("--config")
-        commandargs.append(f"{Path(options.configfile).resolve()}")
-
-    commandargs.append(f"--date={date_to_iso(options.date)}")
-    commandargs.append(f"--drs4-pedestal-run={sequence.previousrun:05d}")
-    commandargs.append(f"--pedcal-run={sequence.run:05d}")
+        commandargs.extend(("--config", f"{Path(options.configfile).resolve()}"))
+    commandargs.extend(
+        (
+            f"--date={date_to_iso(options.date)}",
+            f"--drs4-pedestal-run={sequence.drs4_run:05d}",
+            f"--pedcal-run={sequence.run:05d}",
+        )
+    )
 
     content = job_header + "\n" + PYTHON_IMPORTS
 
     if not options.test:
         content += set_cache_dirs()
         content += "\n"
         # Use the SLURM env variables
@@ -593,28 +577,27 @@
 
             log.debug(stringify(commandargs))
 
         # Here sequence.jobid has not been redefined, so it keeps the one
         # from previous time sequencer was launched.
 
         # Add the job dependencies after calibration sequence
-        if sequence.parent_list and sequence.type == "DATA":
+        if sequence.type == "DATA":
             if not options.simulate and not options.no_calib and not options.test:
                 log.debug("Adding dependencies to job submission")
                 depend_string = f"--dependency=afterok:{parent_jobid}"
                 commandargs.append(depend_string)
 
             commandargs.append(sequence.script)
 
             if options.simulate:
                 log.debug("SIMULATE Launching scripts")
             elif options.test:
                 log.debug(
-                    "TEST launching datasequence scripts for "
-                    "first subrun without scheduler"
+                    "TEST launching datasequence scripts for " "first subrun without scheduler"
                 )
                 commandargs = ["python", sequence.script]
                 sp.check_output(commandargs, shell=False)
             else:
                 log.info("Submitting jobs to the cluster.")
                 try:
                     log.debug(f"Launching script {sequence.script}")
@@ -701,16 +684,16 @@
     -------
     queue_list: pd.DataFrame
     """
     sacct_output = pd.read_csv(sacct_output, names=FORMAT_SLURM)
 
     # Keep only the jobs corresponding to OSA sequences
     sacct_output = sacct_output[
-        (sacct_output['JobName'].str.contains("batch")) |
-        (sacct_output["JobName"].str.contains("LST1"))
+        (sacct_output["JobName"].str.contains("batch"))
+        | (sacct_output["JobName"].str.contains("LST1"))
     ]
 
     try:
         sacct_output["JobID"] = sacct_output["JobID"].apply(lambda x: x.split("_")[0])
         sacct_output["JobID"] = sacct_output["JobID"].str.strip(".batch").astype(int)
 
     except AttributeError:
@@ -723,17 +706,15 @@
     """Filter the job info list to get the values of the jobs in the current queue."""
     sequences_info = pd.DataFrame([vars(seq) for seq in sequence_list])
     # Keep the jobs in the sacct output that are present in the sequence list
     return job_info[job_info["JobName"].isin(sequences_info["jobname"])]
 
 
 def set_queue_values(
-        sacct_info: pd.DataFrame,
-        squeue_info: pd.DataFrame,
-        sequence_list: Iterable
+    sacct_info: pd.DataFrame, squeue_info: pd.DataFrame, sequence_list: Iterable
 ) -> None:
     """
     Extract job info from sacct output and
     fetch them into the table of sequences.
 
     Parameters
     ----------
@@ -792,55 +773,7 @@
         mask = ["CANCELLED" in job for job in filtered_job_info.State]
         sequence.exit = filtered_job_info[mask]["ExitCode"].iloc[0]
     elif any("TIMEOUT" in job for job in filtered_job_info.State):
         sequence.state = "TIMEOUT"
         sequence.exit = "0:15"
     elif any("RUNNING" in job for job in filtered_job_info.State):
         sequence.state = "RUNNING"
-
-
-def run_program_with_history_logging(
-        command_args: List[str],
-        history_file: Path,
-        run: str,
-        prod_id: str,
-        command: str,
-        input_file: Optional[str] = None,
-        config_file: Optional[str] = None,
-):
-    """
-    Run the program and log the output in the history file
-
-    Parameters
-    ----------
-    command_args: List[str]
-    history_file: pathlib.Path
-    run: str
-    prod_id: str
-    command: str
-    input_file: str, optional
-    config_file: str, optional
-
-    Returns
-    -------
-    rc: int
-        Return code of the program
-    """
-    log.info(f"Executing {stringify(command_args)}")
-
-    output = sp.run(command_args, stdout=sp.PIPE, stderr=sp.STDOUT, encoding='utf-8')
-    rc = output.returncode
-
-    history(
-        run=run,
-        prod_id=prod_id,
-        stage=command,
-        return_code=rc,
-        history_file=history_file,
-        input_file=input_file,
-        config_file=config_file
-    )
-
-    if rc != 0:
-        raise ValueError(f"{command_args[0]} failed with output: \n {output.stdout}")
-
-    return rc
```

### Comparing `lstosa-0.9.4/osa/nightsummary/database.py` & `lstosa-0.9.5/osa/nightsummary/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 
 from pymongo import MongoClient
 from pymongo.errors import ConnectionFailure
 
 from osa.utils.logging import myLogger
 
-__all__ = ['query', 'db_available']
+__all__ = ["query", "db_available"]
 
 
 log = myLogger(logging.getLogger(__name__))
 
 
 def db_available():
     """Check the connection to the TCU database."""
@@ -45,14 +45,18 @@
         Query result from database. It can be either the source name or its coordinates.
 
     Raises
     ------
     ConnectionFailure
     """
 
+    # Avoid problems with numpy int64 encoding in MongoDB
+    if not isinstance(obs_id, int):
+        obs_id = int(obs_id)
+
     caco_client = MongoClient("tcs01")
     tcu_client = MongoClient("tcs05")
 
     with caco_client, tcu_client:
         run_info = caco_client["CACO"]["RUN_INFORMATION"]
         run = run_info.find_one({"run_number": obs_id})
 
@@ -62,37 +66,30 @@
         except TypeError:
             return None
 
         bridges_monitoring = tcu_client["bridgesmonitoring"]
         property_collection = bridges_monitoring["properties"]
         chunk_collection = bridges_monitoring["chunks"]
         descriptors = property_collection.find(
-            {'property_name': property_name},
+            {"property_name": property_name},
         )
 
-        entries = {
-            'name': property_name,
-            'time': [],
-            'value': []
-        }
+        entries = {"name": property_name, "time": [], "value": []}
 
         for descriptor in descriptors:
-            query_property = {'pid': descriptor['_id']}
+            query_property = {"pid": descriptor["_id"]}
 
             if start is not None:
-                query_property.update({"begin": {"$gte": start}})
+                query_property["begin"] = {"$gte": start}
 
             if end is not None:
-                query_property.update({"end": {"$lte": end}})
+                query_property["end"] = {"$lte": end}
 
             chunks = chunk_collection.find(query_property)
 
             for chunk in chunks:
-                for value in chunk['values']:
-                    entries['time'].append(value['t'])
-                    entries['value'].append(value['val'])
+                for value in chunk["values"]:
+                    entries["time"].append(value["t"])
+                    entries["value"].append(value["val"])
 
                     source_name = entries["value"][0]
-                    if source_name != "":
-                        return source_name
-                    else:
-                        return None
+                    return source_name if source_name != "" else None
```

### Comparing `lstosa-0.9.4/osa/nightsummary/nightsummary.py` & `lstosa-0.9.5/osa/nightsummary/nightsummary.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     r0_dir = Path(cfg.get("LST1", "R0_DIR"))
     run_summary_dir = Path(cfg.get("LST1", "RUN_SUMMARY_DIR"))
 
     command = [
         "lstchain_create_run_summary",
         f"--date={nightdir}",
         f"--r0-path={r0_dir}",
-        f"--output-dir={run_summary_dir}"
+        f"--output-dir={run_summary_dir}",
     ]
 
     try:
         subprocess.run(command, check=True)
 
     except OSError as error:
         log.exception(f"Command {stringify(command)}, error: {error}")
```

### Comparing `lstosa-0.9.4/osa/nightsummary/set_source_coordinates.py` & `lstosa-0.9.5/osa/nightsummary/set_source_coordinates.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,46 +10,41 @@
 
 from osa.utils.logging import myLogger
 
 log = myLogger(logging.getLogger(__name__))
 
 
 @click.command()
-@click.argument('file', type=click.Path(exists=True))
-@click.option('--source', type=str)
-@click.option('--ra', type=float, help='Right Ascension in degrees')
-@click.option('--dec', type=float, help='Declination in degrees')
-def main(
-        file: Path = None,
-        source: str = None,
-        ra: float = np.nan,
-        dec: float = np.nan
-):
+@click.argument("file", type=click.Path(exists=True))
+@click.option("--source", type=str)
+@click.option("--ra", type=float, help="Right Ascension in degrees")
+@click.option("--dec", type=float, help="Declination in degrees")
+def main(file: Path = None, source: str = None, ra: float = np.nan, dec: float = np.nan):
     """Update the source coordinates in the RunCatalog ECSV files."""
     log.setLevel(logging.INFO)
 
     table = Table.read(file)
-    table.add_index('run_id')
+    table.add_index("run_id")
 
     for run in table:
-        source_name = run['source_name']
+        source_name = run["source_name"]
         try:
             coords = SkyCoord.from_name(source_name)
-            run['source_ra'] = coords.ra.deg
-            run['source_dec'] = coords.dec.deg
+            run["source_ra"] = coords.ra.deg
+            run["source_dec"] = coords.dec.deg
 
         except name_resolve.NameResolveError:
             if source is None:
                 log.warning(
-                    f'Could not resolve coordinates for {source_name}. '
-                    'Add coordinates through the command line.'
+                    f"Could not resolve coordinates for {source_name}. "
+                    "Add coordinates through the command line."
                 )
             if source_name == source:
-                run['source_ra'] = ra
-                run['source_dec'] = dec
+                run["source_ra"] = ra
+                run["source_dec"] = dec
 
-    log.info(f'Updated coordinates in {file}')
-    table.write(file, format='ascii.ecsv', overwrite=True, delimiter=',')
+    log.info(f"Updated coordinates in {file}")
+    table.write(file, format="ascii.ecsv", overwrite=True, delimiter=",")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `lstosa-0.9.4/osa/nightsummary/tests/test_extract.py` & `lstosa-0.9.5/osa/nightsummary/tests/test_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from datetime import datetime
 
 
-obs_date = datetime.fromisoformat('2020-01-17')
+obs_date = datetime.fromisoformat("2020-01-17")
 
 
 def test_source_list(
-        r0_data,
-        run_summary_file,
-        run_catalog,
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        pedestal_ids_file,
-        merged_run_summary,
+    r0_data,
+    run_summary_file,
+    run_catalog,
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    pedestal_ids_file,
+    merged_run_summary,
 ):
     """Test that the list of name of sources is correct."""
     from osa.nightsummary.extract import get_source_list
+
     sources = get_source_list(date=obs_date)
-    assert list(sources) == ['Crab', 'MadeUpSource']
-    assert sources == {'Crab': [1807], 'MadeUpSource': [1808]}
+    assert list(sources) == ["Crab", "MadeUpSource"]
+    assert sources == {"Crab": [1807], "MadeUpSource": [1808]}
 
 
 def test_build_sequences(sequence_list):
     """Test that building of sequences."""
     from osa.nightsummary.extract import build_sequences
+
     extracted_seq_list = build_sequences(date=obs_date)
     for sequence, extracted_seq in zip(sequence_list, extracted_seq_list):
         assert sequence.run == extracted_seq.run
```

### Comparing `lstosa-0.9.4/osa/nightsummary/tests/test_nightsummary.py` & `lstosa-0.9.5/osa/nightsummary/tests/test_nightsummary.py`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/osa/paths.py` & `lstosa-0.9.5/osa/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Handle the paths of the analysis products."""
 
 import logging
 from pathlib import Path
+from typing import List
+
 from astropy.table import Table
-from lstchain.onsite import (
-    find_systematics_correction_file, 
-    find_time_calibration_file
-)
+from lstchain.onsite import find_systematics_correction_file, find_time_calibration_file
+from lstchain.scripts.onsite.onsite_create_calibration_file import search_filter
 
 from osa.configs import options
+from osa.configs.config import DEFAULT_CFG
 from osa.configs.config import cfg
-from osa.utils.logging import myLogger
+from osa.configs.datamodel import Sequence
 from osa.utils import utils
-from osa.configs.config import DEFAULT_CFG
+from osa.utils.logging import myLogger
 
 log = myLogger(logging.getLogger(__name__))
 
 __all__ = [
     "get_calibration_file",
     "get_drs4_pedestal_file",
     "pedestal_ids_file_exists",
@@ -29,15 +30,15 @@
     "get_datacheck_files",
     "get_drive_file",
     "get_summary_file",
     "get_pedestal_ids_file",
     "DATACHECK_WEB_BASEDIR",
     "DEFAULT_CFG",
     "create_source_directories",
-    "analysis_path"
+    "analysis_path",
 ]
 
 
 DATACHECK_WEB_BASEDIR = Path(cfg.get("WEBSERVER", "DATACHECK"))
 
 
 def analysis_path(tel) -> Path:
@@ -93,20 +94,48 @@
     date = get_run_date(run_id)
     file = drs4_pedestal_dir / date / f"pro/drs4_pedestal.Run{run_id:05d}.0000.h5"
     return file.resolve()
 
 
 def get_calibration_file(run_id: int) -> Path:
     """
-    Return the drs4 pedestal file corresponding to a given run id
-    regardless of the date when the run was taken.
+    Return the calibration file corresponding to a given run_id.
+
+    Parameters
+    ----------
+    run_id : int
+        Run id of the calibration file to be built.
+
+    Notes
+    -----
+    The file path will be built regardless of the date when the run was taken.
+    We follow the naming convention of the calibration files produced by the lstchain script
+    which depends on the filter wheels position. Therefore, we need to try to fetch the filter
+    position from the CaCo database. If the filter position is not found, we assume the default
+    filter position 5-2. Filter information is not available in the database for runs taken before
+    mid 2021 approx.
     """
+
     calib_dir = Path(cfg.get("LST1", "CALIB_DIR"))
     date = get_run_date(run_id)
-    file = calib_dir / date / f"pro/calibration_filters_52.Run{run_id:05d}.0000.h5"
+
+    if options.test:  # Run tests avoiding the access to the database
+        filters = 52
+
+    else:
+        mongodb = cfg.get("database", "CaCo_db")
+        try:
+            # Cast run_id to int to avoid problems with numpy int64 encoding in MongoDB
+            filters = search_filter(int(run_id), mongodb)
+        except IOError:
+            log.warning("No filter information found in database. Assuming positions 52.")
+            filters = 52
+
+    file = calib_dir / date / f"pro/calibration_filters_{filters}.Run{run_id:05d}.0000.h5"
+
     return file.resolve()
 
 
 def pedestal_ids_file_exists(run_id: int) -> bool:
     """Look for the files with pedestal interleaved event identification."""
     pedestal_ids_dir = Path(cfg.get("LST1", "PEDESTAL_FINDER_DIR"))
     file_list = sorted(pedestal_ids_dir.rglob(f"pedestal_ids_Run{run_id:05d}.*.h5"))
@@ -144,33 +173,29 @@
     from a date in format YYYYMMDD.
     """
     pedestal_ids_dir = Path(cfg.get("LST1", "PEDESTAL_FINDER_DIR")) / date
     file = pedestal_ids_dir / f"pedestal_ids_Run{run_id:05d}.{{subruns:04d}}.h5"
     return file.resolve()
 
 
-def sequence_calibration_files(sequence_list):
+def sequence_calibration_files(sequence_list: List[Sequence]) -> None:
     """Build names of the calibration files for each sequence in the list."""
     flat_date = utils.date_to_dir(options.date)
     base_dir = Path(cfg.get("LST1", "BASE"))
 
     for sequence in sequence_list:
-
-        if not sequence.parent_list:
-            drs4_pedestal_run_id = sequence.previousrun
-            pedcal_run_id = sequence.run
-        else:
-            drs4_pedestal_run_id = sequence.parent_list[0].previousrun
-            pedcal_run_id = sequence.parent_list[0].run
-
         # Assign the calibration files to the sequence object
-        sequence.pedestal = get_drs4_pedestal_file(drs4_pedestal_run_id)
-        sequence.calibration = get_calibration_file(pedcal_run_id)
-        sequence.time_calibration = find_time_calibration_file("pro", pedcal_run_id, base_dir=base_dir)
-        sequence.systematic_correction = find_systematics_correction_file("pro", flat_date, base_dir=base_dir)
+        sequence.drs4_file = get_drs4_pedestal_file(sequence.drs4_run)
+        sequence.calibration_file = get_calibration_file(sequence.pedcal_run)
+        sequence.time_calibration_file = find_time_calibration_file(
+            "pro", sequence.pedcal_run, base_dir=base_dir
+        )
+        sequence.systematic_correction_file = find_systematics_correction_file(
+            "pro", flat_date, base_dir=base_dir
+        )
 
 
 def get_datacheck_files(pattern: str, directory: Path) -> list:
     """Return a list of files matching the pattern."""
     return sorted(directory.glob(pattern))
 
 
@@ -204,17 +229,15 @@
     -------
     path : pathlib.Path
         Path to the directory
     """
     nightdir = utils.date_to_dir(options.date)
 
     if concept == "MUON":
-        directory = (
-            Path(cfg.get(options.tel_id, concept + "_DIR")) / nightdir / options.prod_id
-        )
+        directory = Path(cfg.get(options.tel_id, concept + "_DIR")) / nightdir / options.prod_id
     elif concept in {"DL1AB", "DATACHECK"}:
         directory = (
             Path(cfg.get(options.tel_id, concept + "_DIR"))
             / nightdir
             / options.prod_id
             / options.dl1_prod_id
         )
@@ -223,24 +246,18 @@
             Path(cfg.get(options.tel_id, concept + "_DIR"))
             / nightdir
             / options.prod_id
             / options.dl2_prod_id
         )
     elif concept in {"PEDESTAL", "CALIB", "TIMECALIB"}:
         directory = (
-            Path(cfg.get(options.tel_id, concept + "_DIR"))
-            / nightdir
-            / options.calib_prod_id
+            Path(cfg.get(options.tel_id, concept + "_DIR")) / nightdir / options.calib_prod_id
         )
     elif concept == "HIGH_LEVEL":
-        directory = (
-            Path(cfg.get(options.tel_id, concept + "_DIR"))
-            / nightdir
-            / options.prod_id
-        )
+        directory = Path(cfg.get(options.tel_id, concept + "_DIR")) / nightdir / options.prod_id
     else:
         log.warning(f"Concept {concept} not known")
         directory = None
 
     if not options.simulate and create_dir:
         log.debug(f"Destination directory created for {concept}: {directory}")
         directory.mkdir(parents=True, exist_ok=True)
```

### Comparing `lstosa-0.9.4/osa/provenance/capture.py` & `lstosa-0.9.5/osa/provenance/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,15 @@
         # variables parsing
         global session_name, session_tag
         class_instance = parse_variables(class_instance)
         if class_instance.__name__ in REDUCTION_TASKS:
             session_tag = f"{activity}:{class_instance.ObservationRun}"
             session_name = f"{class_instance.ObservationRun}"
         else:
-            session_tag = (
-                f"{activity}:{class_instance.PedestalRun}-{class_instance.CalibrationRun}"
-            )
+            session_tag = f"{activity}:{class_instance.PedestalRun}-{class_instance.CalibrationRun}"
             session_name = f"{class_instance.PedestalRun}-{class_instance.CalibrationRun}"
         # OSA specific
         # variables parsing
 
         # provenance capture before execution
         derivation_records = get_derivation_records(class_instance, activity)
         parameter_records = get_parameters_records(class_instance, activity, activity_id)
@@ -369,23 +367,19 @@
         "startTime": start,
         "system": system,
         # OSA specific
         "observation_date": class_instance.ObservationDate,
         # OSA specific
         "software_version": class_instance.SoftwareVersion,
         "config_file": class_instance.ProcessingConfigFile,
-        "config_file_hash": get_file_hash(
-            class_instance.ProcessingConfigFile, buffer="path"
-        ),
+        "config_file_hash": get_file_hash(class_instance.ProcessingConfigFile, buffer="path"),
         "config_file_hash_type": get_hash_method(),
     }
     if class_instance.__name__ in REDUCTION_TASKS:
-        log_record[
-            "observation_run"
-        ] = class_instance.ObservationRun  # a session is run-wise
+        log_record["observation_run"] = class_instance.ObservationRun  # a session is run-wise
     else:
         log_record["pedestal_run"] = class_instance.PedestalRun
         log_record["calibration_run"] = class_instance.CalibrationRun
     log_prov_info(log_record)
     return session_id
 
 
@@ -416,17 +410,15 @@
         value = get_nested_value(class_instance, var)
         if value:
             new_id = get_entity_id(value, item)
             if new_id != entity_id:
                 log_record = {"entity_id": new_id, "progenitor_id": entity_id}
                 records.append(log_record)
                 traced_entities[var] = (new_id, item)
-                logger.warning(
-                    f"Derivation detected in {activity} for {var}. ID: {new_id}"
-                )
+                logger.warning(f"Derivation detected in {activity} for {var}. ID: {new_id}")
     return records
 
 
 def get_parameters_records(class_instance, activity, activity_id):
     """Get log records for parameters of the activity."""
     records = []
     parameter_list = definition["activities"][activity]["parameters"] or []
```

### Comparing `lstosa-0.9.4/osa/provenance/config/definition.yaml` & `lstosa-0.9.5/osa/provenance/config/definition.yaml`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/osa/provenance/io.py` & `lstosa-0.9.5/osa/provenance/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,18 @@
             # activity name
             if "name" in provdict:
                 act.add_attributes({"prov:label": provdict.pop("name")})
             if "script" in provdict:
                 act.add_attributes({"script": provdict.pop("script")})
             # activity start
             if "startTime" in provdict:
-                act.set_time(
-                    startTime=datetime.datetime.fromisoformat(provdict.pop("startTime"))
-                )
+                act.set_time(startTime=datetime.datetime.fromisoformat(provdict.pop("startTime")))
             # activity end
             if "endTime" in provdict:
-                act.set_time(
-                    endTime=datetime.datetime.fromisoformat(provdict.pop("endTime"))
-                )
+                act.set_time(endTime=datetime.datetime.fromisoformat(provdict.pop("endTime")))
             # in session?
             # if "in_session" in provdict:
             #     sess_id = DEFAULT_NS + ":" + str(provdict.pop("in_session"])
             #     pdoc.wasInfluencedBy(
             #         act_id, sess_id
             #     )  # , other_attributes={'prov:type': "Context"})
             # activity configuration
```

### Comparing `lstosa-0.9.4/osa/provenance/utils.py` & `lstosa-0.9.5/osa/provenance/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,26 +161,22 @@
         )
 
     if class_instance.__name__ == "dl1_to_dl2":
         # run_str       [0] 02006.0000
 
         class_instance.Analysisconfigfile_dl2 = configfile_dl2
         class_instance.ObservationRun = class_instance.args[0].split(".")[0]
-        class_instance.RFModelEnergyFile = os.path.realpath(
-            f"{rf_models_directory}/reg_energy.sav"
-        )
+        class_instance.RFModelEnergyFile = os.path.realpath(f"{rf_models_directory}/reg_energy.sav")
         class_instance.RFModelDispNormFile = os.path.realpath(
             f"{rf_models_directory}/reg_disp_norm.sav"
         )
         class_instance.RFModelDispSignFile = os.path.realpath(
             f"{rf_models_directory}/reg_disp_sign.sav"
         )
-        class_instance.RFModelGammanessFile = os.path.realpath(
-            f"{rf_models_directory}/cls_gh.sav"
-        )
+        class_instance.RFModelGammanessFile = os.path.realpath(f"{rf_models_directory}/cls_gh.sav")
         class_instance.DL1SubrunDataset = os.path.realpath(
             f"{outdir_dl1}/dl1_LST-1.Run{class_instance.args[0]}.h5"
         )
         class_instance.DL2SubrunDataset = os.path.realpath(
             f"{outdir_dl2}/dl2_LST-1.Run{class_instance.args[0]}.h5"
         )
         class_instance.DL2MergedFile = os.path.realpath(
```

### Comparing `lstosa-0.9.4/osa/raw.py` & `lstosa-0.9.5/osa/raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.utils.logging import myLogger
 from osa.utils.utils import date_to_dir
 
 log = myLogger(logging.getLogger(__name__))
 
-__all__ = [
-    "get_check_raw_dir",
-    "get_raw_dir",
-    "is_raw_data_available"
-]
+__all__ = ["get_check_raw_dir", "get_raw_dir", "is_raw_data_available"]
 
 
 def get_check_raw_dir(date: datetime) -> Path:
     """Get the raw directory and check if it contains raw files."""
     raw_dir = get_raw_dir(date)
     log.debug(f"Raw directory: {raw_dir}")
```

### Comparing `lstosa-0.9.4/osa/report.py` & `lstosa-0.9.5/osa/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from datetime import datetime
+from datetime import datetime, timezone
 from fnmatch import fnmatchcase
 from glob import glob
 from os.path import basename, getsize, join
 from pathlib import Path
 
 from osa.configs import config, options
 from osa.configs.config import cfg
@@ -15,15 +15,15 @@
 log = myLogger(logging.getLogger(__name__))
 
 __all__ = ["history", "start", "finished_assignments"]
 
 
 def start(parent_tag: str):
     """Print out the header of the script (e.g. sequencer, closer)."""
-    now = datetime.utcnow()
+    now = datetime.now(timezone.utc)
     simple_parent_tag = parent_tag.rsplit("(")[0]
     header(
         f"Starting {simple_parent_tag} at {now.strftime('%Y-%m-%d %H:%M')} "
         f"UTC for LST, Telescope: {options.tel_id}, "
         f"Date: {options.date.strftime('%Y-%m-%d')}"
     )
 
@@ -82,53 +82,52 @@
         disk_space_GB = int(round(disk_space_GB_f, 0))
 
     ana_files = glob(join(analysis_dir, "*" + cfg.get("PATTERN", "R0SUFFIX")))
     file_no = {}
     ana_set = set(ana_files)
 
     for concept in concept_set:
-        pattern = f"{cfg.get('PATTERN', concept + 'PREFIX')}*"
+        pattern = f"{cfg.get('PATTERN', f'{concept}PREFIX')}*"
         log.debug(f"Trying with {concept} and searching {pattern}")
         file_no[concept] = 0
         delete_set = set()
         for a in ana_set:
             ana_file = basename(a)
-            pattern_found = fnmatchcase(ana_file, pattern)
-            if pattern_found:
+            if pattern_found := fnmatchcase(ana_file, pattern):
                 log.debug(f"Was pattern {pattern} found in {ana_file}?: {pattern_found}")
                 file_no[concept] += 1
                 delete_set.add(a)
         ana_set -= delete_set
 
-    now_string = f"{datetime.utcnow().strftime('%Y-%m-%d %H:%M')}"
+    now_string = f"{datetime.now(timezone.utc).strftime('%Y-%m-%d %H:%M')}"
 
     dictionary = {
         "NIGHT": date_to_iso(options.date),
         "TELESCOPE": options.tel_id,
         "IS_CLOSED": 1,
         "SEQUENCES": len(sequence_list),
         "FILES_RAW": rawnum,
         "RAW_GB": disk_space_GB,
         "END": now_string,
     }
 
     for concept in concept_set:
-        dictionary["FILES_" + concept] = file_no[concept]
+        dictionary[f"FILES_{concept}"] = file_no[concept]
 
     return dictionary
 
 
 def history(
-        run: str,
-        prod_id: str,
-        stage: str,
-        return_code: int,
-        history_file: Path,
-        input_file=None,
-        config_file=None,
+    run: str,
+    prod_id: str,
+    stage: str,
+    return_code: int,
+    history_file: Path,
+    input_file=None,
+    config_file=None,
 ) -> None:
     """
     Appends a history line to the history file. A history line
     reports the outcome of the execution of a lstchain executable.
 
     Parameters
     ----------
@@ -145,11 +144,10 @@
     input_file : str, optional
         If needed, input file used for the lstchain executable
     config_file : str, optional
         Input card used for the lstchain executable.
     """
     date_string = datetime.utcnow().isoformat(sep=" ", timespec="minutes")
     string_to_write = (
-        f"{run} {stage} {prod_id} {date_string} "
-        f"{input_file} {config_file} {return_code}\n"
+        f"{run} {stage} {prod_id} {date_string} " f"{input_file} {config_file} {return_code}\n"
     )
     append_to_file(history_file, string_to_write)
```

### Comparing `lstosa-0.9.4/osa/scripts/autocloser.py` & `lstosa-0.9.5/osa/scripts/autocloser.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 from osa.utils.mail import send_warning_mail
 from osa.utils.utils import (
     night_finished_flag,
     is_day_closed,
     get_prod_id,
     is_night_time,
     cron_lock,
-    example_seq, date_to_iso
+    example_seq,
+    date_to_iso,
 )
 
 __all__ = ["Telescope", "Sequence"]
 
 log = myLogger(logging.getLogger())
 
 
 class Telescope:
     """Handle the telescope sequences, simulate and check them."""
 
     def __init__(
-            self,
-            telescope,
-            date,
-            config_file: Path,
-            ignore_cronlock: bool = False,
-            test: bool = False,
+        self,
+        telescope,
+        date,
+        config_file: Path,
+        ignore_cronlock: bool = False,
+        test: bool = False,
     ):
         """
         Parameters
         ----------
         telescope : str
             Options: LST1
         date : str
@@ -175,20 +176,20 @@
     def build_sequences(self):
         """Build the sequences and return True if there are any."""
         log.debug(f"Creating Sequence objects for {self.telescope}")
         self.sequences = [Sequence(self.keyLine, line) for line in self.data_lines]
         return bool(self.sequences)
 
     def close(
-            self,
-            date: str,
-            config: Path,
-            no_dl2: bool,
-            simulate: bool = False,
-            test: bool = False,
+        self,
+        date: str,
+        config: Path,
+        no_dl2: bool,
+        simulate: bool = False,
+        test: bool = False,
     ):
         """Launch the closer command."""
         log.info("Closing...")
 
         closer_cmd = [
             "closer",
             "-c",
@@ -211,17 +212,15 @@
 
         log.debug(f"Executing {' '.join(closer_cmd)}")
         closer = subprocess.Popen(
             closer_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=False
         )
         stdout, _ = closer.communicate()
         if closer.returncode != 0:
-            log.warning(
-                f"closer returned error code {closer.returncode}! See output: {stdout}"
-            )
+            log.warning(f"closer returned error code {closer.returncode}! See output: {stdout}")
             return False
         self.closed = True
         return True
 
 
 class Sequence:
     """
@@ -259,76 +258,70 @@
 
     def is_on_hold(self):
         return self.dict_sequence["State"] == "PENDING"
 
     def is_100(self, no_dl2: bool):
         """Check that all analysis products are 100% complete."""
         if (
-                no_dl2
-                and self.dict_sequence["Tel"] != "ST"
-                and self.dict_sequence["DL1%"] == "100"
-                and self.dict_sequence["DL1AB%"] == "100"
-                and self.dict_sequence["MUONS%"] == "100"
+            no_dl2
+            and self.dict_sequence["Tel"] != "ST"
+            and self.dict_sequence["DL1%"] == "100"
+            and self.dict_sequence["DL1AB%"] == "100"
+            and self.dict_sequence["MUONS%"] == "100"
         ):
             return True
 
         if (
-                self.dict_sequence["Tel"] != "ST"
-                and self.dict_sequence["DL1%"] == "100"
-                and self.dict_sequence["DL1AB%"] == "100"
-                and self.dict_sequence["MUONS%"] == "100"
-                and self.dict_sequence["DL2%"] == "100"
+            self.dict_sequence["Tel"] != "ST"
+            and self.dict_sequence["DL1%"] == "100"
+            and self.dict_sequence["DL1AB%"] == "100"
+            and self.dict_sequence["MUONS%"] == "100"
+            and self.dict_sequence["DL2%"] == "100"
         ):
             return True
 
         return False
 
     def is_flawless(self, no_dl2: bool):
         """Check that all jobs statuses are completed."""
         log.debug("Check if flawless")
         if (
-                self.dict_sequence["Type"] == "DATA"
-                and self.dict_sequence["Exit"] == "0:0"
-                and self.is_100(no_dl2=no_dl2)
-                and self.dict_sequence["State"] == "COMPLETED"
+            self.dict_sequence["Type"] == "DATA"
+            and self.dict_sequence["Exit"] == "0:0"
+            and self.is_100(no_dl2=no_dl2)
+            and self.dict_sequence["State"] == "COMPLETED"
         ):
             return True
         if (
-                self.dict_sequence["Type"] == "PEDCALIB"
-                and self.dict_sequence["Exit"] == "0:0"
-                and self.dict_sequence["State"] == "COMPLETED"
+            self.dict_sequence["Type"] == "PEDCALIB"
+            and self.dict_sequence["Exit"] == "0:0"
+            and self.dict_sequence["State"] == "COMPLETED"
         ):
             return True
 
         return False
 
     def has_all_subruns(self):
         """
         Check that all subruns are complete by checking the
         total number of subrun wise DL1 files.
         """
         if self.dict_sequence["Type"] == "PEDCALIB":
             log.debug("Cannot check for missing subruns for CALIBRATION sequence")
             return True
         search_str = (
-            f"{analysis_path(self.dict_sequence['Tel'])}/"
-            f"dl1*{self.dict_sequence['Run']}*.h5"
+            f"{analysis_path(self.dict_sequence['Tel'])}/" f"dl1*{self.dict_sequence['Run']}*.h5"
         )
         subrun_nrs = sorted(
             [int(os.path.basename(file).split(".")[2]) for file in glob.glob(search_str)]
         )
         return bool(subrun_nrs and len(subrun_nrs) == int(self.dict_sequence["Subruns"]))
 
     def close(
-            self,
-            date: str,
-            config: Path,
-            no_dl2: bool,
-            simulate: bool = False,
-            test: bool = False
+        self, date: str, config: Path, no_dl2: bool, simulate: bool = False, test: bool = False
     ):
         """Close the sequence by calling the 'closer' script for a given sequence."""
         log.info("Closing sequence...")
 
         closer_cmd = [
             "closer",
             "-c",
@@ -347,22 +340,18 @@
             closer_cmd.insert(1, "--no-dl2")
 
         if test:
             self.closed = True
             return True
 
         log.debug(f"Executing {' '.join(closer_cmd)}")
-        closer = subprocess.Popen(
-            closer_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
-        )
+        closer = subprocess.Popen(closer_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         stdout, _ = closer.communicate()
         if closer.returncode != 0:
-            log.warning(
-                f"closer returned error code {closer.returncode}! See output: {stdout}"
-            )
+            log.warning(f"closer returned error code {closer.returncode}! See output: {stdout}")
             return False
 
         self.closed = True
 
         return True
 
 
@@ -479,19 +468,15 @@
     # skip these checks if closing is forced
     if not args.force and not all(seq.readyToClose for seq in telescope):
         sys.exit(f"{args.tel_id} is NOT ready to close. Exiting.")
 
     log.info(f"Closing {args.tel_id}...")
 
     if not telescope.close(
-            date=date,
-            config=args.config,
-            no_dl2=args.no_dl2,
-            simulate=args.simulate,
-            test=args.test
+        date=date, config=args.config, no_dl2=args.no_dl2, simulate=args.simulate, test=args.test
     ):
         log.warning(f"Could not close the day for {args.tel_id}!")
         # Send email, if later than 18:00 UTC and telescope is not ready to close
         if hour > 18:
             send_warning_mail(date=date)
 
     log.info("Exit")
```

### Comparing `lstosa-0.9.4/osa/scripts/calibration_pipeline.py` & `lstosa-0.9.5/osa/scripts/calibration_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 import logging
 import sys
 from pathlib import Path
 
 from osa.configs import options
 from osa.configs.config import cfg
-from osa.job import historylevel, run_program_with_history_logging
+from osa.job import historylevel
+from osa.workflow.stages import DRS4PedestalStage, ChargeCalibrationStage
 from osa.paths import drs4_pedestal_exists, calibration_file_exists
 from osa.provenance.capture import trace
 from osa.utils.cliopts import calibration_pipeline_cliparsing
 from osa.utils.logging import myLogger
 
 __all__ = [
     "calibration_sequence",
@@ -32,18 +33,15 @@
 
 
 def is_calibration_produced(drs4_pedestal_run_id: int, pedcal_run_id: int) -> bool:
     """
     Check if both daily calibration (DRS4 baseline and
     charge calibration) files are already produced.
     """
-    return (
-        drs4_pedestal_exists(drs4_pedestal_run_id)
-        and calibration_file_exists(pedcal_run_id)
-    )
+    return drs4_pedestal_exists(drs4_pedestal_run_id) and calibration_file_exists(pedcal_run_id)
 
 
 def drs4_pedestal_command(drs4_pedestal_run_id: int) -> list:
     """Build the create_drs4_pedestal command."""
     base_dir = Path(cfg.get("LST1", "BASE")).resolve()
     return [
         "onsite_create_drs4_pedestal_file",
@@ -57,15 +55,14 @@
     """Build the create_calibration_file command."""
     base_dir = Path(cfg.get("LST1", "BASE")).resolve()
     return [
         "onsite_create_calibration_file",
         f"--pedestal_run={drs4_pedestal_run_id}",
         f"--run_number={pedcal_run_id}",
         f"--base_dir={base_dir}",
-        "--filters=52",
     ]
 
 
 def calibration_sequence(drs4_pedestal_run_id: int, pedcal_run_id: int) -> int:
     """
     Handle the two stages for creating the daily calibration products:
     DRS4 pedestal and charge calibration files.
@@ -77,127 +74,120 @@
 
     Returns
     -------
     rc : int
         Return code
     """
     analysis_dir = Path(options.directory)
-    history_file = analysis_dir / f"sequence_LST1_{pedcal_run_id}.history"
+    history_file = analysis_dir / f"sequence_LST1_{pedcal_run_id:05d}.history"
 
     level, rc = (2, 0) if options.simulate else historylevel(history_file, "PEDCALIB")
 
     log.info(f"Going to level {level}")
 
     if level == 2:
-        rc = drs4_pedestal(drs4_pedestal_run_id, pedcal_run_id, history_file)
+        rc = drs4_pedestal(drs4_pedestal_run_id, pedcal_run_id)
         level -= 1
         log.info(f"Going to level {level}")
     if level == 1:
-        rc = calibrate_charge(drs4_pedestal_run_id, pedcal_run_id, history_file)
+        rc = calibrate_charge(drs4_pedestal_run_id, pedcal_run_id)
         level -= 1
         log.info(f"Going to level {level}")
     if level == 0:
         log.info(f"Job for sequence {pedcal_run_id} finished without fatal errors")
 
     return rc
 
 
 @trace
 def drs4_pedestal(
-        drs4_pedestal_run_id: int,
-        pedcal_run_id: int,
-        history_file: Path
+    drs4_pedestal_run_id: int,
+    pedcal_run_id: int,
 ) -> int:
     """
     Create a DRS4 pedestal file for baseline correction.
 
     Parameters
     ----------
     drs4_pedestal_run_id : int
         DRS4 pedestal run number
     pedcal_run_id : int
         PEDCALIB run number
-    history_file : `pathlib.Path`
-        Path to the history file
 
     Returns
     -------
     rc : int
         Return code
     """
     if options.simulate or drs4_pedestal_exists(drs4_pedestal_run_id):
         return 0
 
     cmd = drs4_pedestal_command(drs4_pedestal_run_id)
 
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=f"{drs4_pedestal_run_id:05d}",
-        prod_id=options.calib_prod_id,
-        command=cmd[0],
+    analysis_step = DRS4PedestalStage(
+        run=f"{drs4_pedestal_run_id:05d}", run_pedcal=f"{pedcal_run_id:05d}", command_args=cmd
     )
+    analysis_step.execute()
+    return analysis_step.rc
 
 
 @trace
 def calibrate_charge(
-        drs4_pedestal_run_id: int,
-        pedcal_run_id: int,
-        history_file: Path
+    drs4_pedestal_run_id: int,
+    pedcal_run_id: int,
 ) -> int:
     """
     Create the calibration file to transform from ADC counts to photo-electrons
 
     Parameters
     ----------
     drs4_pedestal_run_id : int
         String with run number of the pedestal run
     pedcal_run_id : int
         String with run number of the pedcal run
-    history_file : `pathlib.Path`
-        Path to the history file
 
     Returns
     -------
     rc: int
         Return code
     """
     if options.simulate or calibration_file_exists(pedcal_run_id):
         return 0
 
     cmd = calibration_file_command(
-        drs4_pedestal_run_id=drs4_pedestal_run_id,
-        pedcal_run_id=pedcal_run_id
-    )
-
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=f"{pedcal_run_id:05d}",
-        prod_id=options.calib_prod_id,
-        command=cmd[0],
+        drs4_pedestal_run_id=drs4_pedestal_run_id, pedcal_run_id=pedcal_run_id
     )
+    
+    try:
+        analysis_step = ChargeCalibrationStage(run=f"{pedcal_run_id:05d}", command_args=cmd)
+        analysis_step.execute()
+        return analysis_step.rc
+
+    except:
+        log.info(f"Failed. Return code {analysis_step.rc}")
+        cmd.append("--filters=52")
+        log.info("Trying again by setting filters 52")
+        analysis_step = ChargeCalibrationStage(run=f"{pedcal_run_id:05d}", command_args=cmd)
+        analysis_step.execute()
+        return analysis_step.rc
 
 
 def main():
     """
     Performs the calibration steps (obtain the drs4 baseline correction
     and ADC to photo-electron coefficients)
     """
     drs4_pedestal_run, pedcal_run = calibration_pipeline_cliparsing()
 
     if options.verbose:
         log.setLevel(logging.DEBUG)
     else:
         log.setLevel(logging.INFO)
 
-    if is_calibration_produced(
-        drs4_pedestal_run_id=drs4_pedestal_run,
-        pedcal_run_id=pedcal_run
-    ):
+    if is_calibration_produced(drs4_pedestal_run_id=drs4_pedestal_run, pedcal_run_id=pedcal_run):
         log.info(
             f"Calibration files already produced from "
             f"runs {drs4_pedestal_run:05d} and {pedcal_run:05d}"
         )
         sys.exit(0)
 
     rc = calibration_sequence(drs4_pedestal_run, pedcal_run)
```

### Comparing `lstosa-0.9.4/osa/scripts/closer.py` & `lstosa-0.9.5/osa/scripts/closer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,52 +8,49 @@
 import shutil
 import subprocess
 import sys
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Tuple, Iterable, List
 
+from osa import osadb
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.job import are_all_jobs_correctly_finished, save_job_information
-from osa.nightsummary.extract import (
-    extractruns,
-    extractsequences,
-    extractsubruns,
-    sort_run_list
-)
+from osa.nightsummary.extract import extract_runs, extract_sequences
 from osa.nightsummary.nightsummary import run_summary_table
 from osa.paths import destination_dir
 from osa.raw import is_raw_data_available
 from osa.report import start
 from osa.utils.cliopts import closercliparsing
 from osa.utils.logging import myLogger
 from osa.utils.register import register_found_pattern
 from osa.utils.utils import (
     night_finished_flag,
     is_day_closed,
     stringify,
     date_to_dir,
     create_lock,
-    gettag, date_to_iso,
+    gettag,
+    date_to_iso,
 )
 
 __all__ = [
     "is_sequencer_successful",
     "ask_for_closing",
     "post_process",
     "post_process_files",
     "is_finished_check",
     "extract_provenance",
     "merge_dl1_datacheck",
     "set_closed_with_file",
     "merge_files",
     "daily_datacheck",
     "daily_longterm_cmd",
-    "observation_finished"
+    "observation_finished",
 ]
 
 log = myLogger(logging.getLogger())
 
 
 def main():
     """Main function in charge of closing the sequences."""
@@ -120,17 +117,14 @@
     if options.noninteractive:
         return
 
     answer_check = False
 
     while not answer_check:
         try:
-            if options.simulate:
-                question = "Close that day? (y/n): "
-                question += "[SIMULATE ongoing] "
             answer_user = "n"
         except KeyboardInterrupt:
             log.warning("Program exited by user.")
             sys.exit(1)
         except EOFError as error:
             log.exception(f"End of file not expected, {error}")
             sys.exit(2)
@@ -165,19 +159,23 @@
 
     # Extract the provenance info
     extract_provenance(seq_list)
 
     # Merge DL1b files run-wise
     merge_files(seq_list, data_level="DL1AB")
 
+    merge_muon_files(seq_list)
+
     # Merge DL2 files run-wise
     if not options.no_dl2:
         merge_files(seq_list, data_level="DL2")
 
     if options.seqtoclose is None:
+        osadb.end_processing(date_to_iso(options.date))
+        # Creating closing flag files will be deprecated in future versions
         return set_closed_with_file()
 
     return False
 
 
 def post_process_files(seq_list: list):
     """
@@ -189,15 +187,15 @@
     seq_list: list
         list of sequences
     """
 
     output_files_set = set(Path(options.directory).rglob("*Run*"))
 
     DL1AB_RE = re.compile(rf"{options.dl1_prod_id}/dl1.*.(?:h5|hdf5|hdf)")
-    DL2_RE = re.compile(f"{options.dl2_prod_id}" + r"/dl2.*.(?:h5|hdf5|hdf)")
+    DL2_RE = re.compile(f"{options.dl2_prod_id}/dl2.*.(?:h5|hdf5|hdf)")
     MUONS_RE = re.compile(r"muons.*.fits")
     DATACHECK_RE = re.compile(r"datacheck_dl1.*.(?:h5|hdf5|hdf)")
 
     pattern_files = dict(
         [
             ("DL1AB", DL1AB_RE),
             ("DL2", DL2_RE),
@@ -213,23 +211,20 @@
 
         log.debug(f"Checking if {concept} files need to be moved to {dst_path}")
 
         for file_path in output_files_set.copy():
 
             file = str(file_path)
             # If seqtoclose is set, we only want to close that sequence
-            if options.seqtoclose is not None and file.find(options.seqtoclose) == -1:
+            if options.seqtoclose is not None and options.seqtoclose not in file:
                 continue
 
-            pattern_found = pattern_re.search(file)
-            if pattern_found:
+            if pattern_found := pattern_re.search(file):
                 log.debug(f"Pattern {concept} found, {pattern_found} in {file}")
-                registered_file = register_found_pattern(
-                    file_path, seq_list, concept, dst_path
-                )
+                registered_file = register_found_pattern(file_path, seq_list, concept, dst_path)
                 output_files_set.remove(registered_file)
 
 
 def set_closed_with_file():
     """Write the analysis report to the closer file."""
     night_finished_file = night_finished_flag()
     is_closed = False
@@ -266,18 +261,16 @@
         True if all sequences are finished, False otherwise.
     seq_list: list
     """
 
     sequence_success = False
     if run_summary is not None:
         # building the sequences (the same way as the sequencer)
-        subrun_list = extractsubruns(run_summary)
-        run_list = extractruns(subrun_list)
-        sorted_run_list = sort_run_list(run_list)
-        sequence_list = extractsequences(sorted_run_list)
+        run_list = extract_runs(run_summary)
+        sequence_list = extract_sequences(options.date, run_list)
 
         if are_all_jobs_correctly_finished(sequence_list):
             sequence_success = True
         else:
             log.info("Jobs did not correctly/yet finish")
 
     else:
@@ -350,16 +343,16 @@
     """
     log.info("Extract provenance run wise")
 
     nightdir = date_to_dir(options.date)
 
     for sequence in seq_list:
         if sequence.type == "DATA":
-            drs4_pedestal_run_id = str(sequence.pedestal).split(".")[1].replace("Run", "")
-            pedcal_run_id = str(sequence.calibration).split(".")[1].replace("Run", "")
+            drs4_pedestal_run_id = str(sequence.drs4_run)
+            pedcal_run_id = str(sequence.pedcal_run)
             cmd = [
                 "sbatch",
                 "-D",
                 options.directory,
                 "-o",
                 f"log/provenance_{sequence.run:05d}_%j.log",
                 "provprocess",
@@ -367,28 +360,26 @@
                 options.configfile,
                 drs4_pedestal_run_id,
                 pedcal_run_id,
                 f"{sequence.run:05d}",
                 nightdir,
                 options.prod_id,
             ]
-            if (
-                    not options.simulate
-                    and not options.test
-                    and shutil.which('sbatch') is not None
-            ):
+            if not options.simulate and not options.test and shutil.which("sbatch") is not None:
                 subprocess.run(cmd, check=True)
             else:
                 log.debug("Simulate launching scripts")
 
 
 def get_pattern(data_level) -> Tuple[str, str]:
     """Return the subrun wise file pattern for the data level."""
     if data_level == "DL1AB":
         return "dl1_LST-1.Run?????.????.h5", "dl1"
+    if data_level == "MUON":
+        return "muons_LST-1.Run?????.????.fits", "muon"
     if data_level == "DL2":
         return "dl2_LST-1.Run?????.????.h5", "dl2"
 
     raise ValueError(f"Unknown data level {data_level}")
 
 
 def merge_files(sequence_list, data_level="DL2"):
@@ -415,24 +406,51 @@
                 "--no-progress",
                 f"--run-number={sequence.run}",
                 f"--pattern={pattern}",
             ]
 
             log.debug(f"Executing {stringify(cmd)}")
 
-            if (
-                    not options.simulate
-                    and not options.test
-                    and shutil.which('sbatch') is not None
-            ):
+            if not options.simulate and not options.test and shutil.which("sbatch") is not None:
                 subprocess.run(cmd, check=True)
             else:
                 log.debug("Simulate launching scripts")
 
 
+def merge_muon_files(sequence_list):
+    """Merge muon files run-wise."""
+    log.info("Looping over the sequences and merging the MUON files")
+
+    data_dir = destination_dir("MUON", create_dir=False)
+    pattern, prefix = get_pattern("MUON")
+
+    for sequence in sequence_list:
+        merged_file = Path(data_dir) / f"muons_LST-1.Run{sequence.run:05d}.fits"
+
+        cmd = [
+            "sbatch",
+            "-D",
+            options.directory,
+            "-o",
+            f"log/merge_{prefix}_{sequence.run:05d}_%j.log",
+            "lstchain_merge_muon_files",
+            f"--input-dir={data_dir}",
+            f"--output-file={merged_file}",
+            f"--run-number={sequence.run}",
+            f"--pattern={pattern}",
+        ]
+
+        log.debug(f"Executing {stringify(cmd)}")
+
+        if not options.simulate and not options.test and shutil.which("sbatch") is not None:
+            subprocess.run(cmd, check=True)
+        else:
+            log.debug("Simulate launching scripts")
+
+
 def daily_longterm_cmd(parent_job_ids: List[str]) -> List[str]:
     """Build the daily longterm command."""
     nightdir = date_to_dir(options.date)
     dl1_dir = destination_dir("DL1AB", create_dir=False)
     muons_dir = destination_dir("MUON", create_dir=False)
     longterm_dir = Path(cfg.get("LST1", "LONGTERM_DIR")) / options.prod_id / nightdir
     longterm_output_file = longterm_dir / f"DL1_datacheck_{nightdir}.h5"
@@ -444,24 +462,24 @@
         "-o",
         "log/longterm_daily_%j.log",
         f"--dependency=afterok:{','.join(parent_job_ids)}",
         "lstchain_longterm_dl1_check",
         f"--input-dir={dl1_dir}",
         f"--output-file={longterm_output_file}",
         f"--muons-dir={muons_dir}",
-        "--batch"
+        "--batch",
     ]
 
 
 def daily_datacheck(cmd: List[str]):
     """Run daily dl1 checks using longterm script."""
     log.info("Daily dl1 checks using longterm script.")
     log.debug(f"Executing {stringify(cmd)}")
 
-    if not options.simulate and not options.test and shutil.which('sbatch') is not None:
+    if not options.simulate and not options.test and shutil.which("sbatch") is not None:
         subprocess.run(cmd, check=True)
     else:
         log.debug("Simulate launching scripts")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lstosa-0.9.4/osa/scripts/copy_datacheck.py` & `lstosa-0.9.5/osa/scripts/copy_datacheck.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 """
 
 import logging
 
 from osa.configs import options
 from osa.paths import (
     datacheck_directory,
-    get_datacheck_files, destination_dir,
+    get_datacheck_files,
+    destination_dir,
 )
 from osa.utils.cliopts import copy_datacheck_parsing
 from osa.utils.logging import myLogger
 from osa.utils.utils import DATACHECK_FILE_PATTERNS, date_to_dir
 from osa.webserver.utils import copy_to_webserver
 
 log = myLogger(logging.getLogger())
@@ -23,27 +24,27 @@
     """Check if all files of a given data type are copied."""
     n_files = len(files)
 
     if n_files == 0:
         log.warning(f"No {data_type} files found.")
         return False
 
-    elif data_type == "PEDESTAL" and n_files != 1:
+    if data_type == "PEDESTAL" and n_files != 1:
         log.warning(f"Expected at least 1 PDF file, {n_files} found.")
         return False
 
-    elif data_type == "CALIB" and n_files != 1:
+    if data_type == "CALIB" and n_files != 1:
         log.warning(f"Expected at least 1 PDF file, {n_files} found.")
         return False
 
-    elif data_type == "DL1AB" and n_files != get_number_of_runs():
+    if data_type == "DL1AB" and n_files != get_number_of_runs():
         log.warning(f"Expected {get_number_of_runs()} PDF files, {n_files} found.")
         return False
 
-    elif data_type == "LONGTERM" and n_files != 3:
+    if data_type == "LONGTERM" and n_files != 3:
         log.warning(f"Expected 3 DL1 check files (HTML, h5 and log), {n_files} found.")
         return False
 
     return True
 
 
 def main():
```

### Comparing `lstosa-0.9.4/osa/scripts/datasequence.py` & `lstosa-0.9.5/osa/scripts/datasequence.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 import logging
 import sys
 from pathlib import Path
 
 from osa.configs import options
 from osa.configs.config import cfg
-from osa.job import historylevel, run_program_with_history_logging
+from osa.job import historylevel
+from osa.workflow.stages import AnalysisStage
 from osa.provenance.capture import trace
 from osa.utils.cliopts import data_sequence_cli_parsing
 from osa.utils.logging import myLogger
 from osa.utils.utils import date_to_dir
 
 __all__ = ["data_sequence", "r0_to_dl1", "dl1_to_dl2", "dl1ab", "dl1_datacheck"]
 
 log = myLogger(logging.getLogger())
 
 
 def data_sequence(
-        calibration_file: Path,
-        pedestal_file: Path,
-        time_calibration_file: Path,
-        systematic_correction_file: Path,
-        drive_file: Path,
-        run_summary: Path,
-        pedestal_ids_file: Path,
-        run_str: str
+    calibration_file: Path,
+    pedestal_file: Path,
+    time_calibration_file: Path,
+    systematic_correction_file: Path,
+    drive_file: Path,
+    run_summary: Path,
+    pedestal_ids_file: Path,
+    run_str: str,
 ):
     """
     Performs all the steps to process a whole run.
 
     Parameters
     ----------
     calibration_file: pathlib.Path
@@ -42,80 +43,78 @@
     run_str: str
 
     Returns
     -------
     rc: int
         Return code of the last executed command.
     """
-    history_file = (
-        Path(options.directory) / f"sequence_{options.tel_id}_{run_str}.history"
-    )
+    history_file = Path(options.directory) / f"sequence_{options.tel_id}_{run_str}.history"
+    # Set the starting level and corresponding return code from last analysis step
+    # registered in the history file.
     level, rc = (4, 0) if options.simulate else historylevel(history_file, "DATA")
     log.info(f"Going to level {level}")
 
     if level == 4:
         rc = r0_to_dl1(
             calibration_file,
             pedestal_file,
             time_calibration_file,
             systematic_correction_file,
             drive_file,
             run_summary,
             pedestal_ids_file,
             run_str,
-            history_file,
         )
         level -= 1
         log.info(f"Going to level {level}")
 
     if level == 3:
-        rc = dl1ab(run_str, history_file)
+        rc = dl1ab(run_str)
         if cfg.getboolean("lstchain", "store_image_dl1ab"):
             level -= 1
             log.info(f"Going to level {level}")
         else:
             level -= 2
             log.info(f"No images stored in dl1ab. Producing DL2. Going to level {level}")
 
     if level == 2:
-        rc = dl1_datacheck(run_str, history_file)
+        rc = dl1_datacheck(run_str)
         if options.no_dl2:
             level = 0
             log.info(f"No DL2 are going to be produced. Going to level {level}")
         else:
             level -= 1
             log.info(f"Going to level {level}")
 
     if level == 1:
         if options.no_dl2:
             level = 0
             log.info(f"No DL2 are going to be produced. Going to level {level}")
         else:
-            rc = dl1_to_dl2(run_str, history_file)
+            rc = dl1_to_dl2(run_str)
             level -= 1
             log.info(f"Going to level {level}")
 
     if level == 0:
         log.info(f"Job for sequence {run_str} finished without fatal errors")
 
     return rc
 
 
 @trace
 def r0_to_dl1(
-        calibration_file: Path,
-        pedestal_file: Path,
-        time_calibration_file: Path,
-        systematic_correction_file: Path,
-        drive_file: Path,
-        run_summary: Path,
-        pedestal_ids_file: Path,
-        run_str: str,
-        history_file: Path,
-):
+    calibration_file: Path,
+    pedestal_file: Path,
+    time_calibration_file: Path,
+    systematic_correction_file: Path,
+    drive_file: Path,
+    run_summary: Path,
+    pedestal_ids_file: Path,
+    run_str: str,
+) -> int:
     """
     Prepare and launch the actual lstchain script that is performing
     the low and high-level calibration to raw camera images.
     It also applies the image cleaning and obtains shower parameters.
 
     Parameters
     ----------
@@ -126,15 +125,14 @@
     drive_file: pathlib.Path
     run_summary: : pathlib.Path
         Path to the run summary file
     pedestal_ids_file: pathlib.Path
         Path to file containing the interleaved pedestal event ids
     run_str: str
         XXXXX.XXXX (run_number.subrun_number)
-    history_file: pathlib.Path
 
     Returns
     -------
     rc: int
         Return code of the executed command.
     """
     command = cfg.get("lstchain", "r0_to_dl1")
@@ -158,93 +156,78 @@
 
     if pedestal_ids_file is not None:
         cmd.append(f"--pedestal-ids-path={pedestal_ids_file}")
 
     if options.simulate:
         return 0
 
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=run_str,
-        prod_id=options.prod_id,
-        command=command,
-        input_file=calibration_file.name,
-        config_file=pedestal_file.name,
-    )
+    analysis_step = AnalysisStage(run=run_str, command_args=cmd, config_file=dl1a_config.name)
+    analysis_step.execute()
+    return analysis_step.rc
 
 
 @trace
-def dl1ab(run_str: str, history_file: Path):
+def dl1ab(run_str: str) -> int:
     """
     Prepare and launch the actual lstchain script that is performing
     the image cleaning considering the interleaved pedestal information
     and obtains shower parameters. It keeps the shower images.
 
     Parameters
     ----------
     run_str: str
-    history_file: pathlib.Path
 
     Returns
     -------
     rc: int
         Return code of the executed command.
     """
     # Create a new subdirectory for the dl1ab output
     dl1ab_subdirectory = Path(options.directory) / options.dl1_prod_id
     dl1ab_subdirectory.mkdir(parents=True, exist_ok=True)
-    dl1b_config_file = Path(cfg.get("lstchain", "dl1b_config"))
+    dl1b_config = Path(cfg.get("lstchain", "dl1b_config"))
     # DL1a input file from base running_analysis directory
     input_dl1_datafile = Path(options.directory) / f"dl1_LST-1.Run{run_str}.h5"
     # DL1b output file to be stored in the dl1ab subdirectory
     output_dl1_datafile = dl1ab_subdirectory / f"dl1_LST-1.Run{run_str}.h5"
 
     # Prepare and launch the actual lstchain script
     command = cfg.get("lstchain", "dl1ab")
     cmd = [
         command,
         f"--input-file={input_dl1_datafile}",
         f"--output-file={output_dl1_datafile}",
-        f"--config={dl1b_config_file}",
+        f"--config={dl1b_config}",
     ]
     if not cfg.getboolean("lstchain", "store_image_dl1ab"):
         cmd.append("--no-image=True")
 
     if options.simulate:
         return 0
 
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=run_str,
-        prod_id=options.dl1_prod_id,
-        command=command,
-        input_file=input_dl1_datafile.name,
-        config_file=dl1b_config_file.name,
-    )
+    analysis_step = AnalysisStage(run=run_str, command_args=cmd, config_file=dl1b_config.name)
+    analysis_step.execute()
+    return analysis_step.rc
 
 
 @trace
-def dl1_datacheck(run_str: str, history_file: Path):
+def dl1_datacheck(run_str: str) -> int:
     """
     Run datacheck script
 
     Parameters
     ----------
     run_str: str
-    history_file: pathlib.Path
 
     Returns
     -------
     rc: int
     """
     # Create a new subdirectory for the dl1ab output
     dl1ab_subdirectory = Path(options.directory) / options.dl1_prod_id
-    dl1b_config_file = Path(cfg.get("lstchain", "dl1b_config"))
     input_dl1_datafile = dl1ab_subdirectory / f"dl1_LST-1.Run{run_str}.h5"
     output_directory = Path(options.directory) / options.dl1_prod_id
     output_directory.mkdir(parents=True, exist_ok=True)
 
     # Prepare and launch the actual lstchain script
     command = cfg.get("lstchain", "check_dl1")
     cmd = [
@@ -255,68 +238,55 @@
         "--omit-pdf",
         "--batch",
     ]
 
     if options.simulate:
         return 0
 
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=run_str,
-        prod_id=options.dl1_prod_id,
-        command=command,
-        input_file=input_dl1_datafile.name,
-        config_file=dl1b_config_file.name,
-    )
+    analysis_step = AnalysisStage(run=run_str, command_args=cmd)
+    analysis_step.execute()
+    return analysis_step.rc
 
 
 @trace
-def dl1_to_dl2(run_str: str, history_file: Path):
+def dl1_to_dl2(run_str: str) -> int:
     """
     It prepares and execute the dl1 to dl2 lstchain scripts that applies
     the already trained RFs models to DL1 files. It identifies the
     primary particle, reconstructs its energy and direction.
 
     Parameters
     ----------
     run_str: str
-    history_file: pathlib.Path
 
     Returns
     -------
     rc: int
     """
     dl1ab_subdirectory = Path(options.directory) / options.dl1_prod_id
     dl2_subdirectory = Path(options.directory) / options.dl2_prod_id
-    dl2_config_file = Path(cfg.get("lstchain", "dl2_config"))
+    dl2_config = Path(cfg.get("lstchain", "dl2_config"))
     rf_models_directory = Path(cfg.get("lstchain", "RF_MODELS"))
     dl1_file = dl1ab_subdirectory / f"dl1_LST-1.Run{run_str}.h5"
 
     command = cfg.get("lstchain", "dl1_to_dl2")
     cmd = [
         command,
         f"--input-file={dl1_file}",
         f"--output-dir={dl2_subdirectory}",
         f"--path-models={rf_models_directory}",
-        f"--config={dl2_config_file}",
+        f"--config={dl2_config}",
     ]
 
     if options.simulate:
         return 0
 
-    return run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=run_str,
-        prod_id=options.dl2_prod_id,
-        command=command,
-        input_file=dl1_file.name,
-        config_file=dl2_config_file.name,
-    )
+    analysis_step = AnalysisStage(run=run_str, command_args=cmd, config_file=dl2_config.name)
+    analysis_step.execute()
+    return analysis_step.rc
 
 
 def main():
     """Performs the analysis steps to convert raw data into DL2 files."""
     (
         calibration_file,
         drs4_ped_file,
@@ -329,15 +299,15 @@
     ) = data_sequence_cli_parsing()
 
     if options.verbose:
         log.setLevel(logging.DEBUG)
     else:
         log.setLevel(logging.INFO)
 
-    # run the routine
+    # Run the routine piping all the analysis steps
     rc = data_sequence(
         calibration_file,
         drs4_ped_file,
         time_calibration_file,
         systematic_correction_file,
         drive_log_file,
         run_summary_file,
```

### Comparing `lstosa-0.9.4/osa/scripts/gain_selection.py` & `lstosa-0.9.5/osa/scripts/gain_selection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,187 @@
 """Script to run the gain selection over a list of dates."""
-import fileinput
 import logging
 import re
+import shutil
+import glob
 import subprocess as sp
 from pathlib import Path
 from textwrap import dedent
+from io import StringIO
 
 import click
 from astropy.table import Table
 from lstchain.paths import run_info_from_filename
 
 from osa.scripts.reprocessing import get_list_of_dates
 from osa.utils.logging import myLogger
+from osa.job import get_sacct_output, FORMAT_SLURM
 
 log = myLogger(logging.getLogger(__name__))
 
 PATH = "PATH=/fefs/aswg/software/gain_selection/bin:$PATH"
 
 
 def get_sbatch_script(
-        run_id,
-        subrun,
-        input_file,
-        output_dir,
-        log_dir,
-        ref_time,
-        ref_counter,
-        module,
-        ref_source
+    run_id, subrun, input_file, output_dir, log_dir, ref_time, ref_counter, module, ref_source
 ):
     """Build the sbatch job pilot script for running the gain selection."""
-    return dedent(f"""\
+    return dedent(
+        f"""\
     #!/bin/bash
 
     #SBATCH -D {log_dir}
     #SBATCH -o "gain_selection_{run_id:05d}_{subrun:04d}_%j.log"
     #SBATCH --job-name "gain_selection_{run_id:05d}"
     #SBATCH --export {PATH}
 
     lst_select_gain {input_file} {output_dir} {ref_time} {ref_counter} {module} {ref_source}
-    """)
+    """
+    )
 
 
 def apply_gain_selection(date: str, output_basedir: Path = None):
     """
     Submit the jobs to apply the gain selection to the data for a given date
     on a subrun-by-subrun basis.
     """
 
     run_summary_dir = Path("/fefs/aswg/data/real/monitoring/RunSummary")
     run_summary_file = run_summary_dir / f"RunSummary_{date}.ecsv"
     summary_table = Table.read(run_summary_file)
     # Apply gain selection only to DATA runs
-    summary_table = summary_table[summary_table['run_type'] == 'DATA']
+    data_runs = summary_table[summary_table["run_type"] == "DATA"]
 
     output_dir = output_basedir / date
-    log_dir = output_basedir / "log"
+    log_dir = output_basedir / "log" / date
     output_dir.mkdir(parents=True, exist_ok=True)
     log_dir.mkdir(parents=True, exist_ok=True)
+    r0_dir = Path(f"/fefs/aswg/data/real/R0/{date}")
 
-    for run in summary_table:
+    for run in data_runs:
         run_id = run["run_id"]
         ref_time = run["dragon_reference_time"]
         ref_counter = run["dragon_reference_counter"]
         module = run["dragon_reference_module_index"]
         ref_source = run["dragon_reference_source"].upper()
 
-        r0_dir = Path(f"/fefs/aswg/data/real/R0/{date}")
-        input_files = r0_dir.glob(f"LST-1.1.Run{run_id:05d}.????.fits.fz")
+        files = glob.glob(f"{r0_dir}/LST-1.?.Run{run_id:05d}.????.fits.fz")
+        subrun_numbers = [int(file[-12:-8]) for file in files]
+        input_files = []
+
+        if ref_source in ["UCTS", "TIB"]:
+
+            n_subruns = max(subrun_numbers)
+
+            for subrun in range(n_subruns + 1):
+                new_files = glob.glob(f"{r0_dir}/LST-1.?.Run{run_id:05d}.{subrun:04d}.fits.fz")
+
+                if len(new_files) != 4:
+                    for file in new_files:
+                        sp.run(["cp", file, output_dir])
+
+                else:
+                    new_files.sort()
+                    input_files.append(new_files[0])
+
+            for file in input_files:
+                run_info = run_info_from_filename(file)
+                job_file = log_dir / f"gain_selection_{run_info.run:05d}.{run_info.subrun:04d}.sh"
+                with open(job_file, "w") as f:
+                    f.write(
+                        get_sbatch_script(
+                            run_id,
+                            run_info.subrun,
+                            file,
+                            output_dir,
+                            log_dir,
+                            ref_time,
+                            ref_counter,
+                            module,
+                            ref_source,
+                        )
+                    )
+                sp.run(["sbatch", job_file], check=True)
+
+        else:
+
+            input_files = r0_dir.glob(f"LST-1.?.Run{run_id:05d}.????.fits.fz")
+
+            for file in input_files:
+                sp.run(["cp", file, output_dir])
+
+    calib_runs = summary_table[summary_table["run_type"] != "DATA"]
+
+    for run in calib_runs:
+        run_id = run["run_id"]
+        r0_files = r0_dir.glob(f"LST-1.?.Run{run_id:05d}.????.fits.fz")
 
-        for file in input_files:
-            run_info = run_info_from_filename(file)
-            job_file = log_dir / f"gain_selection_{run_info.run:05d}.{run_info.subrun:04d}.sh"
-            with open(job_file, "w") as f:
-                f.write(get_sbatch_script(
-                    run_id,
-                    run_info.subrun,
-                    file,
-                    output_dir,
-                    log_dir,
-                    ref_time,
-                    ref_counter,
-                    module,
-                    ref_source
-                ))
-            sp.run(["sbatch", job_file], check=True)
+        for file in r0_files:
+            sp.run(["cp", file, output_dir])
 
+def run_sacct_j(job) -> StringIO:
+    """Run sacct to obtain the job information."""
+    if shutil.which("sacct") is None:
+        log.warning("No job info available since sacct command is not available")
+        return StringIO()
+
+    sacct_cmd = [
+        "sacct",
+        "-n",
+        "--parsable2",
+        "--delimiter=,",
+        "--units=G",
+        "-o",
+        ",".join(FORMAT_SLURM),
+        "-j",
+        job,
+    ]
+    
+    return StringIO(sp.check_output(sacct_cmd).decode())
+    
 
-def check_failed_jobs(output_basedir: Path = None):
+def check_failed_jobs(date: str, output_basedir: Path = None):
     """Search for failed jobs in the log directory."""
     failed_jobs = []
-    log_dir = output_basedir / "log"
-    filenames = log_dir.glob('gain_selection*.log')
-
-    for line in fileinput.input(filenames):
-        if re.search('FAILED', line):
-            job_id = fileinput.filename()[-12:-4]
-            failed_jobs.append(job_id)
+    log_dir = output_basedir / "log" / date
+    filenames = glob.glob(f"{log_dir}/gain_selection*.log")
+    jobs = [re.search(r'(?<=_)(.[0-9.]+?)(?=.log)', i).group(0) for i in filenames]
+
+    for job in jobs: 
+        output = run_sacct_j(job)
+        df = get_sacct_output(output)
+        
+        if not df.iloc[0]["State"] == "COMPLETED":
+            log.warning(f"Job {job} did not finish successfully")
+            failed_jobs.append(job)
 
     if not failed_jobs:
-        log.info('All jobs finished successfully.')
+        log.info("All jobs finished successfully")
     else:
-        log.warning(f'The following jobs failed: {failed_jobs}')
+        log.warning("Some jobs did not finish successfully")
 
 
 @click.command()
-@click.option('--check', is_flag=True, default=False, help='Check for failed jobs.')
-@click.argument('dates-file', type=click.Path(exists=True, path_type=Path))
-@click.argument('output-basedir', type=click.Path(path_type=Path))
+@click.option("--check", is_flag=True, default=False, help="Check for failed jobs.")
+@click.argument("dates-file", type=click.Path(exists=True, path_type=Path))
+@click.argument("output-basedir", type=click.Path(path_type=Path))
 def main(dates_file: Path = None, output_basedir: Path = None, check: bool = False):
     """
     Loop over the dates listed in the input file and launch the gain selection
     script for each of them. The input file should list the dates in the format
     YYYYMMDD one date per line.
     """
     log.setLevel(logging.INFO)
 
+    list_of_dates = get_list_of_dates(dates_file)
+
     if check:
-        check_failed_jobs(output_basedir)
+        for date in list_of_dates:
+            check_failed_jobs(date, output_basedir)
     else:
-        list_of_dates = get_list_of_dates(dates_file)
-
         for date in list_of_dates:
             apply_gain_selection(date, output_basedir)
 
         log.info("Done! No more dates to process.")
 
 
 if __name__ == "__main__":
```

### Comparing `lstosa-0.9.4/osa/scripts/provprocess.py` & `lstosa-0.9.5/osa/scripts/provprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,15 @@
     }
     cuts["all"] = cuts["calibration"] + cuts["r0_to_dl1"] + cuts["dl1_to_dl2"]
 
     with open(LOG_FILENAME, "r") as f:
         for line in f.readlines():
             ll = line.split(PROV_PREFIX)
             if len(ll) != 3:
-                log.warning(
-                    f"format {PROV_PREFIX} mismatch in log file {LOG_FILENAME}\n{line}"
-                )
+                log.warning(f"format {PROV_PREFIX} mismatch in log file {LOG_FILENAME}\n{line}")
                 continue
             prov_str = ll.pop()
             prov_dict = yaml.safe_load(prov_str)
             keep = False
             session_tag = prov_dict.get("session_tag", "0:0")
             session_id = prov_dict.get("session_id", False)
             tag_activity, tag_run = session_tag.split(":")
@@ -400,17 +398,15 @@
 
     # TODO
     # create calibration prov files only if filtering
     if options.filter == "calibration":
         pass
 
     if options.filter == "r0_to_dl1" or not options.filter:
-        paths_r0_dl1 = define_paths(
-            "r0_to_dl1", PATH_DL1, options.dl1_prod_id, base_filename
-        )
+        paths_r0_dl1 = define_paths("r0_to_dl1", PATH_DL1, options.dl1_prod_id, base_filename)
         plines_r0 = parse_lines_run(
             "r0_to_dl1",
             read_prov(filename=session_log_filename),
             str(paths_r0_dl1["out_path"]),
         )
         plines_ab = parse_lines_run(
             "dl1ab",
@@ -420,17 +416,15 @@
         dl1_lines = plines_r0 + plines_ab[1:]
 
     # create r0_to_dl1 prov files only if filtering
     if options.filter == "r0_to_dl1":
         produce_provenance_files(plines_r0 + plines_ab[1:], paths_r0_dl1)
 
     if options.filter == "dl1_to_dl2" or not options.filter:
-        paths_dl1_dl2 = define_paths(
-            "dl1_to_dl2", PATH_DL2, options.dl2_prod_id, base_filename
-        )
+        paths_dl1_dl2 = define_paths("dl1_to_dl2", PATH_DL2, options.dl2_prod_id, base_filename)
         plines_check = parse_lines_run(
             "dl1_datacheck",
             read_prov(filename=session_log_filename),
             str(paths_dl1_dl2["out_path"]),
         )
         plines_dl2 = parse_lines_run(
             "dl1_to_dl2",
```

### Comparing `lstosa-0.9.4/osa/scripts/reprocess_longterm.py` & `lstosa-0.9.5/osa/scripts/reprocess_longterm.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import subprocess as sp
 from pathlib import Path
 
 import click
 
 from osa.utils.logging import myLogger
 
-ANALYSIS_PATH = Path('/fefs/aswg/data/real')
-LONGTERM_PATH = ANALYSIS_PATH / 'OSA/DL1DataCheck_LongTerm'
+ANALYSIS_PATH = Path("/fefs/aswg/data/real")
+LONGTERM_PATH = ANALYSIS_PATH / "OSA/DL1DataCheck_LongTerm"
 
 
 log = myLogger(logging.getLogger())
 
 
 def run_longterm(date: str, prod_id: str, new_prod_id: str, log_dir: Path):
     """
@@ -41,33 +41,33 @@
         "sbatch",
         "-o",
         str(log_file),
         "lstchain_longterm_dl1_check",
         f"--input-dir={dl1_dir}",
         f"--output-file={longterm_output_file}",
         f"--muons-dir={muons_dir}",
-        "--batch"
+        "--batch",
     ]
 
     sp.run(cmd)
     log.info(f"Executing {' '.join(cmd)}")
 
 
 @click.command()
-@click.option('--prod-id', help='Production ID to reprocess')
-@click.option('--new-prod-id', help='New production ID')
-@click.option('--log-dir', type=click.Path(path_type=Path), help='Path to log directory')
+@click.option("--prod-id", help="Production ID to reprocess")
+@click.option("--new-prod-id", help="New production ID")
+@click.option("--log-dir", type=click.Path(path_type=Path), help="Path to log directory")
 def main(prod_id: str = None, new_prod_id: str = None, log_dir: Path = None):
     """
     Reprocess the daily check files for all existing dates found on a given production.
     """
     log_dir.mkdir(exist_ok=True, parents=True)
     longterm_dir = LONGTERM_PATH / prod_id
 
-    list_of_processed_dates = longterm_dir.glob('20*')
+    list_of_processed_dates = longterm_dir.glob("20*")
 
     for date_directory in list_of_processed_dates:
         run_longterm(date_directory.name, prod_id, new_prod_id, log_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lstosa-0.9.4/osa/scripts/reprocessing.py` & `lstosa-0.9.5/osa/scripts/reprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,34 @@
 def number_of_pending_jobs():
     """Return the number of jobs in the slurm queue."""
     cmd = ["squeue", "-u", "lstanalyzer", "-h", "-t", "pending", "-r"]
     output = sp.check_output(cmd)
     return output.count(b"\n")
 
 
-def run_script(script: str, date, config: Path, no_dl2: bool, simulate: bool):
+def run_script(
+    script: str, date, config: Path, no_dl2: bool, no_calib: bool, simulate: bool, force: bool
+):
     """Run the sequencer for a given date."""
     osa_config = Path(config).resolve()
 
     cmd = [script, "--config", str(osa_config), "--date", date]
 
     if no_dl2:
         cmd.append("--no-dl2")
 
+    if no_calib:
+        cmd.append("--no-calib")
+
     if simulate:
         cmd.append("--simulate")
 
+    if force:
+        cmd.append("--force")
+
     # Append the telescope to the command in the last place
     cmd.append("LST1")
 
     log.info(f"\nRunning {' '.join(cmd)}")
     sp.run(cmd)
 
 
@@ -60,38 +68,37 @@
     """
     while time.localtime().tm_hour <= 6 or time.localtime().tm_hour >= 18:
         log.info("Waiting for sunrise to not interfere with the data-taking. Sleeping.")
         time.sleep(3600)
 
 
 @click.command()
+@click.option("--no-dl2", is_flag=True, help="Do not run the DL2 step.")
+@click.option("--no-calib", is_flag=True, help="Do not run the calibration step.")
+@click.option("-s", "--simulate", is_flag=True, help="Activate simulation mode.")
+@click.option("-f", "--force", is_flag=True, help="Force the autocloser to close the day.")
 @click.option(
-    "--no-dl2",
-    is_flag=True,
-    help="Do not run the DL2 step."
-)
-@click.option(
-    "-s", "--simulate",
-    is_flag=True,
-    help="Activate simulation mode."
-)
-@click.option(
-    '-c', '--config',
+    "-c",
+    "--config",
     type=click.Path(exists=True),
     default=DEFAULT_CFG,
-    help='Path to the OSA config file.',
+    help="Path to the OSA config file.",
+)
+@click.argument(
+    "script", type=click.Choice(["sequencer", "closer", "copy_datacheck", "autocloser"])
 )
-@click.argument('script', type=click.Choice(['sequencer', 'closer', 'copy_datacheck']))
-@click.argument('dates-file', type=click.Path(exists=True))
+@click.argument("dates-file", type=click.Path(exists=True))
 def main(
-        script: str = None,
-        dates_file: Path = None,
-        config: Path = DEFAULT_CFG,
-        no_dl2: bool = False,
-        simulate: bool = False
+    script: str = None,
+    dates_file: Path = None,
+    config: Path = DEFAULT_CFG,
+    no_dl2: bool = False,
+    no_calib: bool = False,
+    simulate: bool = False,
+    force: bool = False,
 ):
     """
     Loop over the dates listed in the input file and launch the script for each of them.
     The input file should list the dates in the format YYYY-MM-DD one date per line.
     """
     logging.basicConfig(level=logging.INFO)
 
@@ -100,15 +107,15 @@
     # Check slurm queue status
     check_job_status_and_wait()
 
     for date in list_of_dates:
         # Avoid running jobs while it is still night time
         wait_for_daytime()
 
-        run_script(script, date, config, no_dl2, simulate)
+        run_script(script, date, config, no_dl2, no_calib, simulate, force)
         log.info("Waiting 1 minute to launch the process for the next date...\n")
         time.sleep(60)
 
         # Check slurm queue status and sleep for a while to avoid overwhelming the queue
         check_job_status_and_wait()
 
     log.info("Done! No more dates to process.")
```

### Comparing `lstosa-0.9.4/osa/scripts/sequencer_webmaker.py` & `lstosa-0.9.5/osa/scripts/sequencer_webmaker.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,17 +82,15 @@
         options.tel_id,
     ]
 
     if test:
         commandargs.insert(-1, "-t")
 
     try:
-        output = sp.run(
-            commandargs, stdout=sp.PIPE, stderr=sp.STDOUT, encoding="utf-8", check=True
-        )
+        output = sp.run(commandargs, stdout=sp.PIPE, stderr=sp.STDOUT, encoding="utf-8", check=True)
     except sp.CalledProcessError as error:
         log.error(f"Command {commandargs} failed, {error.returncode}")
         sys.exit(1)
     else:
         # Strip newlines and fit it into a table:
         return output.stdout.splitlines()
```

### Comparing `lstosa-0.9.4/osa/scripts/show_run_summary.py` & `lstosa-0.9.5/osa/scripts/show_run_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,34 +72,30 @@
     Returns
     -------
     end_timestamp
     """
 
     last_subrun = num_files - 1  # first subrun is 0
     pattern_first_subrun = r0_path / f"LST-1.1.Run{run_number:05d}.0000.fits.fz"
-    pattern_last_subrun = (
-        r0_path / f"LST-1.1.Run{run_number:05d}.{last_subrun:04d}.fits.fz"
-    )
+    pattern_last_subrun = r0_path / f"LST-1.1.Run{run_number:05d}.{last_subrun:04d}.fits.fz"
     try:
         # Get start and end times from the creation and last modification timestamps
         # from the first and last file in the run
         run_start = Time(os.path.getctime(pattern_first_subrun), format="unix")
         run_end = Time(os.path.getmtime(pattern_last_subrun), format="unix")
         elapsed_time = run_end - run_start
 
         return dict(
             time_start=run_start.iso,
             time_end=run_end.iso,
             elapsed=np.round(elapsed_time.to_value("min"), decimals=1),
         )
 
     except Exception as err:
-        log.error(
-            f"Files {pattern_first_subrun} or {pattern_last_subrun} have error: {err}"
-        )
+        log.error(f"Files {pattern_first_subrun} or {pattern_last_subrun} have error: {err}")
 
         return dict(
             time_start=None,
             time_end=None,
             elapsed=0.0,
         )
 
@@ -169,17 +165,15 @@
 
     header = " Observation time per run type "
     print(f"{header.center(50, '*')}")
     total_obs_time.pprint_all()
     print("\n")
 
     run_summary["number_of_runs"] = 1
-    total_obs = run_summary["number_of_runs", "n_subruns", "elapsed"].groups.aggregate(
-        np.sum
-    )
+    total_obs = run_summary["number_of_runs", "n_subruns", "elapsed"].groups.aggregate(np.sum)
     total_obs["elapsed"].format = "7.1f"
     header = " Total observation time "
     print(f"{header.center(50, '*')}")
     total_obs.pprint_all()
 
 
 if __name__ == "__main__":
```

### Comparing `lstosa-0.9.4/osa/scripts/simulate_processing.py` & `lstosa-0.9.5/osa/scripts/simulate_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,20 +69,16 @@
     )
     CONFIG_FLAGS["TearSubDL1"] = (
         False if path_dl1sub.exists() or options.provenance else path_dl1sub
     )
     CONFIG_FLAGS["TearSubDL2"] = (
         False if path_dl2_sub.exists() or options.provenance else path_dl2_sub
     )
-    CONFIG_FLAGS["TearDL1"] = (
-        False if path_dl1.exists() or options.provenance else path_dl1
-    )
-    CONFIG_FLAGS["TearDL2"] = (
-        False if path_dl2.exists() or options.provenance else path_dl2
-    )
+    CONFIG_FLAGS["TearDL1"] = False if path_dl1.exists() or options.provenance else path_dl1
+    CONFIG_FLAGS["TearDL2"] = False if path_dl2.exists() or options.provenance else path_dl2
 
     if options.provenance and not options.force:
         if path_sub_analysis.exists():
             CONFIG_FLAGS["Go"] = False
             log.info(f"Folder {path_sub_analysis} already exist.")
         if path_dl1sub.exists():
             CONFIG_FLAGS["Go"] = False
@@ -151,35 +147,34 @@
     options.test = True
 
     sequence_list = build_sequences(options.date)
 
     # simulate data calibration and reduction
     for sequence in sequence_list:
         processed = False
-        for sub_list in sequence.subrun_list:
-            if sub_list.runobj.type == "PEDCALIB":
-                args_cal = parse_template(calibration_sequence_job_template(sequence), 0)
-                simulate_calibration(args_cal)
-            elif sub_list.runobj.type == "DATA":
-                with mp.Pool() as poolproc:
-                    args_proc = [
-                        parse_template(data_sequence_job_template(sequence), subrun_idx)
-                        for subrun_idx in range(sub_list.subrun)
-                    ]
-                    processed = poolproc.map(simulate_subrun_processing, args_proc)
-        drs4_pedestal_run_id = str(sequence.pedestal).split(".")[1].replace("Run", "")
-        pedcal_run_id = str(sequence.calibration).split(".")[1].replace("Run", "")
-
+        if sequence.type == "PEDCALIB":
+            args_cal = parse_template(calibration_sequence_job_template(sequence), 0)
+            simulate_calibration(args_cal)
+        elif sequence.type == "DATA":
+            with mp.Pool() as poolproc:
+                args_proc = [
+                    parse_template(data_sequence_job_template(sequence), subrun_idx)
+                    for subrun_idx in range(sequence.subruns)
+                ]
+                processed = poolproc.map(simulate_subrun_processing, args_proc)
         # produce prov if overwrite prov arg
         if processed and options.provenance:
             command = "provprocess"
+            drs4_pedestal_run_id = f"{sequence.drs4_run:05d}"
+            pedcal_run_id = f"{sequence.pedcal_run:05d}"
+
             args_pp = [
                 command,
                 "-c",
-                options.configfile,
+                f"{options.configfile}",
                 drs4_pedestal_run_id,
                 pedcal_run_id,
                 sequence.run_str,
                 options.directory,
                 options.prod_id,
             ]
             log.info(f"Processing provenance for run {sequence.run_str}")
```

### Comparing `lstosa-0.9.4/osa/scripts/tests/test_osa_scripts.py` & `lstosa-0.9.5/osa/scripts/tests/test_osa_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "calibration_pipeline",
     "show_run_summary",
     "provprocess",
     "simulate_processing",
     "dl3_stage",
     "theta2_significance",
     "source_coordinates",
-    "sequencer_webmaker"
+    "sequencer_webmaker",
 ]
 
 options.date = datetime.datetime.fromisoformat("2020-01-17")
 options.tel_id = "LST1"
 options.prod_id = "v0.1.0"
 options.dl1_prod_id = "tailcut84"
 options.directory = "test_osa/test_files0/running_analysis/20200117/v0.1.0/"
@@ -54,18 +54,19 @@
 @pytest.mark.parametrize("script", ALL_SCRIPTS)
 def test_all_help(script):
     """Test for all scripts if at least the help works."""
     run_program(script, "--help")
 
 
 def test_simulate_processing(
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        run_summary_file,
-        r0_data
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    run_summary_file,
+    r0_data,
+    merged_run_summary,
 ):
 
     for file in drs4_time_calibration_files:
         assert file.exists()
 
     for file in systematic_correction_files:
         assert file.exists()
@@ -112,46 +113,46 @@
 
     remove_provlog()
     rc = run_program("simulate_processing", "-p")
     assert rc.returncode == 0
 
 
 def test_simulated_sequencer(
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        run_summary_file,
-        run_catalog,
-        r0_data
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    run_summary_file,
+    run_catalog,
+    r0_data,
+    merged_run_summary,
 ):
     assert run_summary_file.exists()
     assert run_catalog.exists()
 
     for r0_file in r0_data:
         assert r0_file.exists()
 
     for file in drs4_time_calibration_files:
         assert file.exists()
 
     for file in systematic_correction_files:
         assert file.exists()
 
-    rc = run_program(
-        "sequencer", "-d", "2020-01-17", "-s", "-t", "LST1"
-    )
+    rc = run_program("sequencer", "-d", "2020-01-17", "-s", "-t", "LST1")
 
     assert rc.returncode == 0
-    now = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M")
+    now = datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d %H:%M")
     assert rc.stdout == dedent(
         f"""\
         =================================== Starting sequencer.py at {now} UTC for LST, Telescope: LST1, Date: 2020-01-17 ===================================
         Tel   Seq  Parent  Type      Run   Subruns  Source        Action  Tries  JobID  State  CPU_time  Exit  DL1%  MUONS%  DL1AB%  DATACHECK%  DL2%  
-        LST1    0  None    PEDCALIB  1805  5        None          None    None   None   None   None      None  None  None    None    None        None  
-        LST1    1       0  DATA      1807  11       Crab          None    None   None   None   None      None     0       0       0           0     0  
-        LST1    2       0  DATA      1808  9        MadeUpSource  None    None   None   None   None      None     0       0       0           0     0  
-        """)
+        LST1    1  None    PEDCALIB  1809  5        None          None    None   None   None   None      None  None  None    None    None        None  
+        LST1    2       1  DATA      1807  11       Crab          None    None   None   None   None      None     0       0       0           0     0  
+        LST1    3       1  DATA      1808  9        MadeUpSource  None    None   None   None   None      None     0       0       0           0     0  
+        """
+    )
 
 
 def test_sequencer(sequence_file_list):
     for sequence_file in sequence_file_list:
         assert sequence_file.exists()
 
 
@@ -164,21 +165,21 @@
         "LST1",
     )
     assert os.path.exists(running_analysis_dir)
     assert result.stdout.split()[-1] == "Exit"
 
 
 def test_closer(
-        r0_data,
-        running_analysis_dir,
-        test_observed_data,
-        run_summary_file,
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        merged_run_summary
+    r0_data,
+    running_analysis_dir,
+    test_observed_data,
+    run_summary_file,
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    merged_run_summary,
 ):
     # First assure that the end of night flag is not set and remove it otherwise
     night_finished_flag = Path(
         "./test_osa/test_files0/OSA/Closer/20200117/v0.1.0/NightFinished.txt"
     )
     if night_finished_flag.exists():
         night_finished_flag.unlink()
@@ -191,42 +192,37 @@
         assert file.exists()
     assert running_analysis_dir.exists()
     assert run_summary_file.exists()
     for obs_file in test_observed_data:
         assert obs_file.exists()
     assert merged_run_summary.exists()
 
-    run_program(
-        "closer", "-y", "-v", "-t", "-d", "2020-01-17", "LST1"
-    )
-    closed_seq_file = running_analysis_dir / "sequence_LST1_01805.closed"
+    run_program("closer", "-y", "-v", "-t", "-d", "2020-01-17", "LST1")
+    closed_seq_file = running_analysis_dir / "sequence_LST1_01809.closed"
 
     # Check that files have been moved to their final destinations
     assert os.path.exists(
         "./test_osa/test_files0/DL1/20200117/v0.1.0/muons_LST-1.Run01808.0011.fits"
     )
     assert os.path.exists(
         "./test_osa/test_files0/DL1/20200117/v0.1.0/tailcut84/dl1_LST-1.Run01808.0011.h5"
     )
     assert os.path.exists(
         "./test_osa/test_files0/DL1/20200117/v0.1.0/tailcut84/"
         "datacheck_dl1_LST-1.Run01808.0011.h5"
     )
     assert os.path.exists(
-        "./test_osa/test_files0/DL2/20200117/v0.1.0/model2/"
-        "dl2_LST-1.Run01808.0011.h5"
+        "./test_osa/test_files0/DL2/20200117/v0.1.0/model2/" "dl2_LST-1.Run01808.0011.h5"
     )
     # Assert that the link to dl1 and muons files have been created
     assert os.path.islink(
-        "./test_osa/test_files0/running_analysis/20200117/"
-        "v0.1.0/muons_LST-1.Run01808.0011.fits"
+        "./test_osa/test_files0/running_analysis/20200117/" "v0.1.0/muons_LST-1.Run01808.0011.fits"
     )
     assert os.path.islink(
-        "./test_osa/test_files0/running_analysis/20200117/"
-        "v0.1.0/dl1_LST-1.Run01808.0011.h5"
+        "./test_osa/test_files0/running_analysis/20200117/" "v0.1.0/dl1_LST-1.Run01808.0011.h5"
     )
 
     assert night_finished_flag.exists()
     assert closed_seq_file.exists()
 
 
 def test_datasequence(running_analysis_dir):
@@ -255,16 +251,16 @@
         "LST1",
     )
     assert output.returncode == 0
 
 
 def test_calibration_pipeline(running_analysis_dir):
     prod_id = "v0.1.0"
-    drs4_run_number = "01805"
-    pedcal_run_number = "01806"
+    drs4_run_number = "01804"
+    pedcal_run_number = "01805"
     options.directory = running_analysis_dir
 
     output = run_program(
         "calibration_pipeline",
         "--date=2020-01-17",
         "--simulate",
         f"--prod-id={prod_id}",
@@ -281,93 +277,95 @@
     seq_tuple = is_finished_check(run_summary)
     options.test = False
     assert is_sequencer_successful(seq_tuple) is True
 
 
 def test_drs4_pedestal_cmd(base_test_dir):
     from osa.scripts.calibration_pipeline import drs4_pedestal_command
+
     cmd = drs4_pedestal_command(drs4_pedestal_run_id="01804")
     expected_command = [
         "onsite_create_drs4_pedestal_file",
         "--run_number=01804",
         f"--base_dir={base_test_dir}",
         "--no-progress",
     ]
     assert cmd == expected_command
 
 
 def test_calibration_file_cmd(base_test_dir):
     from osa.scripts.calibration_pipeline import calibration_file_command
-    cmd = calibration_file_command(drs4_pedestal_run_id="01804", pedcal_run_id="01805")
+
+    cmd = calibration_file_command(drs4_pedestal_run_id="01804", pedcal_run_id="01809")
     expected_command = [
         "onsite_create_calibration_file",
         "--pedestal_run=01804",
-        "--run_number=01805",
+        "--run_number=01809",
         f"--base_dir={base_test_dir}",
-        "--filters=52"
     ]
     assert cmd == expected_command
 
 
 def test_daily_longterm_cmd():
     from osa.scripts.closer import daily_longterm_cmd
+
     job_ids = ["12345", "54321"]
     cmd = daily_longterm_cmd(parent_job_ids=job_ids)
 
     expected_cmd = [
         "sbatch",
         "-D",
         options.directory,
         "-o",
         "log/longterm_daily_%j.log",
         "--dependency=afterok:12345,54321",
         "lstchain_longterm_dl1_check",
         "--input-dir=test_osa/test_files0/DL1/20200117/v0.1.0/tailcut84",
         "--output-file=test_osa/test_files0/OSA/DL1DataCheck_LongTerm/v0.1.0/20200117/DL1_datacheck_20200117.h5",
         "--muons-dir=test_osa/test_files0/DL1/20200117/v0.1.0",
-        "--batch"
+        "--batch",
     ]
 
     assert cmd == expected_cmd
 
 
 def test_observation_finished():
     """Check if observation is finished for `options.date=2020-01-17`."""
     from osa.scripts.closer import observation_finished
+
     date1 = datetime.datetime(2020, 1, 21, 12, 0, 0)
     assert observation_finished(date=date1) is True
     date2 = datetime.datetime(2020, 1, 17, 5, 0, 0)
     assert observation_finished(date=date2) is False
 
 
 def test_no_runs_found():
     output = sp.run(
-        ["sequencer", "-s", "-d", "2015-01-01", "LST1"],
-        text=True,
-        stdout=sp.PIPE,
-        stderr=sp.PIPE
+        ["sequencer", "-s", "-d", "2015-01-01", "LST1"], text=True, stdout=sp.PIPE, stderr=sp.PIPE
     )
     assert output.returncode == 0
     assert "No runs found for this date. Nothing to do. Exiting." in output.stderr.splitlines()[-1]
 
 
 def test_sequencer_webmaker(
-        run_summary,
-        merged_run_summary,
-        drs4_time_calibration_files,
-        systematic_correction_files,
-        base_test_dir
+    run_summary,
+    merged_run_summary,
+    drs4_time_calibration_files,
+    systematic_correction_files,
+    base_test_dir,
 ):
     # Check if night finished flag is set
     night_finished = base_test_dir / "OSA/Closer/20200117/v0.1.0/NightFinished.txt"
 
     if night_finished.exists():
         output = sp.run(
             ["sequencer_webmaker", "--test", "-d", "2020-01-17"],
-            text=True, stdout=sp.PIPE, stderr=sp.PIPE
+            text=True,
+            stdout=sp.PIPE,
+            stderr=sp.PIPE,
         )
         assert output.returncode != 0
         assert output.stderr.splitlines()[-1] == "Date 2020-01-17 is already closed for LST1"
         night_finished.unlink()
 
     output = sp.run(["sequencer_webmaker", "--test", "-d", "2020-01-17"])
     assert output.returncode == 0
```

### Comparing `lstosa-0.9.4/osa/tests/test_jobs.py` & `lstosa-0.9.5/osa/tests/test_jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,16 @@
 
 import pytest
 
 from osa.configs import options
 from osa.configs.config import cfg
 
 extra_files = Path(os.getenv("OSA_TEST_DATA", "extra"))
-datasequence_history_file = (
-        extra_files / "history_files/sequence_LST1_04185.0010.history"
-)
-calibration_history_file = (
-        extra_files / "history_files/sequence_LST1_04183.history"
-)
+datasequence_history_file = extra_files / "history_files/sequence_LST1_04185.0010.history"
+calibration_history_file = extra_files / "history_files/sequence_LST1_04183.history"
 options.date = "2020-01-17"
 options.tel_id = "LST1"
 options.prod_id = "v0.1.0"
 
 
 def test_historylevel():
     from osa.job import historylevel
@@ -43,109 +39,115 @@
 
 def test_preparejobs(running_analysis_dir, sequence_list):
     from osa.job import prepare_jobs
 
     options.simulate = False
     options.directory = running_analysis_dir
     prepare_jobs(sequence_list)
-    expected_calib_script = os.path.join(running_analysis_dir, "sequence_LST1_01805.py")
+    expected_calib_script = os.path.join(running_analysis_dir, "sequence_LST1_01809.py")
     expected_data_script = os.path.join(running_analysis_dir, "sequence_LST1_01807.py")
     assert os.path.isfile(os.path.abspath(expected_calib_script))
     assert os.path.isfile(os.path.abspath(expected_data_script))
 
 
 def test_sequence_filenames(running_analysis_dir, sequence_list):
     from osa.job import sequence_filenames
 
     for sequence in sequence_list:
         sequence_filenames(sequence)
-        assert sequence.script == running_analysis_dir / \
-               f"sequence_LST1_{sequence.run:05d}.py"
+        assert sequence.script == running_analysis_dir / f"sequence_LST1_{sequence.run:05d}.py"
 
 
 def test_scheduler_env_variables(sequence_list, running_analysis_dir):
     from osa.job import scheduler_env_variables
+
     # Extract the first sequence
     first_sequence = sequence_list[0]
     env_variables = scheduler_env_variables(first_sequence)
     assert env_variables == [
-        '#SBATCH --job-name=LST1_01805',
-        '#SBATCH --time=1:15:00',
-        f'#SBATCH --chdir={running_analysis_dir}',
-        '#SBATCH --output=log/Run01805.%4a_jobid_%A.out',
-        '#SBATCH --error=log/Run01805.%4a_jobid_%A.err',
+        "#SBATCH --job-name=LST1_01809",
+        "#SBATCH --time=1:15:00",
+        f"#SBATCH --chdir={running_analysis_dir}",
+        "#SBATCH --output=log/Run01809.%4a_jobid_%A.out",
+        "#SBATCH --error=log/Run01809.%4a_jobid_%A.err",
         f'#SBATCH --partition={cfg.get("SLURM", "PARTITION_PEDCALIB")}',
-        '#SBATCH --mem-per-cpu=3GB'
+        "#SBATCH --mem-per-cpu=3GB",
     ]
     # Extract the second sequence
     second_sequence = sequence_list[1]
     env_variables = scheduler_env_variables(second_sequence)
     assert env_variables == [
-        '#SBATCH --job-name=LST1_01807',
-        '#SBATCH --time=1:15:00',
-        f'#SBATCH --chdir={running_analysis_dir}',
-        '#SBATCH --output=log/Run01807.%4a_jobid_%A.out',
-        '#SBATCH --error=log/Run01807.%4a_jobid_%A.err',
-        '#SBATCH --array=0-10',
+        "#SBATCH --job-name=LST1_01807",
+        "#SBATCH --time=1:15:00",
+        f"#SBATCH --chdir={running_analysis_dir}",
+        "#SBATCH --output=log/Run01807.%4a_jobid_%A.out",
+        "#SBATCH --error=log/Run01807.%4a_jobid_%A.err",
+        "#SBATCH --array=0-10",
         f'#SBATCH --partition={cfg.get("SLURM", "PARTITION_DATA")}',
-        '#SBATCH --mem-per-cpu=16GB'
+        "#SBATCH --mem-per-cpu=16GB",
     ]
 
 
 def test_job_header_template(sequence_list, running_analysis_dir):
     """Extract and check the header for the first two sequences."""
     from osa.job import job_header_template
+
     # Extract the first sequence
     first_sequence = sequence_list[0]
     header = job_header_template(first_sequence)
-    output_string1 = dedent(f"""\
+    output_string1 = dedent(
+        f"""\
     #!/bin/env python
 
-    #SBATCH --job-name=LST1_01805
+    #SBATCH --job-name=LST1_01809
     #SBATCH --time=1:15:00
     #SBATCH --chdir={running_analysis_dir}
-    #SBATCH --output=log/Run01805.%4a_jobid_%A.out
-    #SBATCH --error=log/Run01805.%4a_jobid_%A.err
+    #SBATCH --output=log/Run01809.%4a_jobid_%A.out
+    #SBATCH --error=log/Run01809.%4a_jobid_%A.err
     #SBATCH --partition={cfg.get('SLURM', 'PARTITION_PEDCALIB')}
-    #SBATCH --mem-per-cpu=3GB""")
+    #SBATCH --mem-per-cpu=3GB"""
+    )
     assert header == output_string1
 
     # Extract the second sequence
     second_sequence = sequence_list[1]
     header = job_header_template(second_sequence)
-    output_string2 = dedent(f"""\
+    output_string2 = dedent(
+        f"""\
     #!/bin/env python
-    
+
     #SBATCH --job-name=LST1_01807
     #SBATCH --time=1:15:00
     #SBATCH --chdir={running_analysis_dir}
     #SBATCH --output=log/Run01807.%4a_jobid_%A.out
     #SBATCH --error=log/Run01807.%4a_jobid_%A.err
     #SBATCH --array=0-10
     #SBATCH --partition={cfg.get('SLURM', 'PARTITION_DATA')}
-    #SBATCH --mem-per-cpu=16GB""")
+    #SBATCH --mem-per-cpu=16GB"""
+    )
     assert header == output_string2
 
 
 def test_create_job_template_scheduler(
-        sequence_list,
-        drs4_time_calibration_files,
-        drs4_baseline_file,
-        calibration_file,
-        run_summary_file,
-        pedestal_ids_file,
+    sequence_list,
+    drs4_time_calibration_files,
+    drs4_baseline_file,
+    calibration_file,
+    run_summary_file,
+    pedestal_ids_file,
 ):
     from osa.job import data_sequence_job_template
 
     assert pedestal_ids_file.exists()
 
     options.test = False
     options.simulate = False
     content1 = data_sequence_job_template(sequence_list[1])
-    expected_content1 = dedent(f"""\
+    expected_content1 = dedent(
+        f"""\
     #!/bin/env python
 
     #SBATCH --job-name=LST1_01807
     #SBATCH --time=1:15:00
     #SBATCH --chdir={Path.cwd()}/test_osa/test_files0/running_analysis/20200117/v0.1.0
     #SBATCH --output=log/Run01807.%4a_jobid_%A.out
     #SBATCH --error=log/Run01807.%4a_jobid_%A.err
@@ -177,18 +179,20 @@
             '--systematic-correction-file={Path.cwd()}/test_osa/test_files0/monitoring/PixelCalibration/Cat-A/ffactor_systematics/20200725/pro/ffactor_systematics_20200725.h5',
             '--drive-file={Path.cwd()}/test_osa/test_files0/monitoring/DrivePositioning/drive_log_20_01_17.txt',
             '--run-summary={run_summary_file}',
             f'01807.{{subruns:04d}}',
             'LST1'
         ])
 
-    sys.exit(proc.returncode)""")
+    sys.exit(proc.returncode)"""
+    )
 
     content2 = data_sequence_job_template(sequence_list[2])
-    expected_content2 = dedent(f"""\
+    expected_content2 = dedent(
+        f"""\
         #!/bin/env python
 
         #SBATCH --job-name=LST1_01808
         #SBATCH --time=1:15:00
         #SBATCH --chdir={Path.cwd()}/test_osa/test_files0/running_analysis/20200117/v0.1.0
         #SBATCH --output=log/Run01808.%4a_jobid_%A.out
         #SBATCH --error=log/Run01808.%4a_jobid_%A.err
@@ -221,30 +225,31 @@
                 '--drive-file={Path.cwd()}/test_osa/test_files0/monitoring/DrivePositioning/drive_log_20_01_17.txt',
                 '--run-summary={run_summary_file}',
                 f'--pedestal-ids-file={Path.cwd()}/test_osa/test_files0/auxiliary/PedestalFinder/20200117/pedestal_ids_Run01808.{{subruns:04d}}.h5',
                 f'01808.{{subruns:04d}}',
                 'LST1'
             ])
 
-        sys.exit(proc.returncode)""")
+        sys.exit(proc.returncode)"""
+    )
 
     options.simulate = True
     assert content1 == expected_content1
     assert content2 == expected_content2
 
 
 def test_create_job_template_local(
-        sequence_list,
-        drs4_time_calibration_files,
-        drs4_baseline_file,
-        calibration_file,
-        systematic_correction_files,
-        run_summary_file,
-        pedestal_ids_file,
-        r0_data
+    sequence_list,
+    drs4_time_calibration_files,
+    drs4_baseline_file,
+    calibration_file,
+    systematic_correction_files,
+    run_summary_file,
+    pedestal_ids_file,
+    r0_data,
 ):
     """Check the job file in local mode (assuming no scheduler)."""
     from osa.job import data_sequence_job_template
 
     for file in drs4_time_calibration_files:
         assert file.exists()
 
@@ -256,15 +261,16 @@
 
     assert pedestal_ids_file.exists()
 
     options.test = True
     options.simulate = False
 
     content1 = data_sequence_job_template(sequence_list[1])
-    expected_content1 = dedent(f"""\
+    expected_content1 = dedent(
+        f"""\
     #!/bin/env python
 
     import os
     import subprocess
     import sys
     import tempfile
 
@@ -284,18 +290,20 @@
             '--systematic-correction-file={Path.cwd()}/test_osa/test_files0/monitoring/PixelCalibration/Cat-A/ffactor_systematics/20200725/pro/ffactor_systematics_20200725.h5',
             '--drive-file={Path.cwd()}/test_osa/test_files0/monitoring/DrivePositioning/drive_log_20_01_17.txt',
             '--run-summary={run_summary_file}',
             f'01807.{{subruns:04d}}',
             'LST1'
         ])
 
-    sys.exit(proc.returncode)""")
+    sys.exit(proc.returncode)"""
+    )
 
     content2 = data_sequence_job_template(sequence_list[2])
-    expected_content2 = dedent(f"""\
+    expected_content2 = dedent(
+        f"""\
         #!/bin/env python
 
         import os
         import subprocess
         import sys
         import tempfile
 
@@ -316,29 +324,32 @@
                 '--drive-file={Path.cwd()}/test_osa/test_files0/monitoring/DrivePositioning/drive_log_20_01_17.txt',
                 '--run-summary={run_summary_file}',
                 f'--pedestal-ids-file={Path.cwd()}/test_osa/test_files0/auxiliary/PedestalFinder/20200117/pedestal_ids_Run01808.{{subruns:04d}}.h5',
                 f'01808.{{subruns:04d}}',
                 'LST1'
             ])
 
-        sys.exit(proc.returncode)""")
+        sys.exit(proc.returncode)"""
+    )
 
     options.simulate = True
 
     assert content1 == expected_content1
     assert content2 == expected_content2
 
 
 def test_create_job_scheduler_calibration(sequence_list):
     """Check the pilot job file for the calibration pipeline."""
     from osa.job import calibration_sequence_job_template
+
     options.test = True
     options.simulate = False
     content = calibration_sequence_job_template(sequence_list[0])
-    expected_content = dedent(f"""\
+    expected_content = dedent(
+        f"""\
     #!/bin/env python
 
     import os
     import subprocess
     import sys
     import tempfile
 
@@ -348,121 +359,97 @@
         os.environ['NUMBA_CACHE_DIR'] = tmpdirname
         proc = subprocess.run([
             'calibration_pipeline',
             '--config',
             '{Path.cwd()}/osa/configs/sequencer.cfg',
             '--date=2020-01-17',
             '--drs4-pedestal-run=01804',
-            '--pedcal-run=01805',
+            '--pedcal-run=01809',
             'LST1'
         ])
 
-    sys.exit(proc.returncode)""")
+    sys.exit(proc.returncode)"""
+    )
     options.simulate = True
     assert content == expected_content
 
 
 def test_set_cache_dirs():
     from osa.job import set_cache_dirs
 
     cache = set_cache_dirs()
-    cache_dirs = dedent(f"""\
+    cache_dirs = dedent(
+        f"""\
     os.environ['CTAPIPE_CACHE'] = '{cfg.get('CACHE', 'CTAPIPE_CACHE')}'
     os.environ['CTAPIPE_SVC_PATH'] = '{cfg.get('CACHE', 'CTAPIPE_SVC_PATH')}'
-    os.environ['MPLCONFIGDIR'] = '{cfg.get('CACHE', 'MPLCONFIGDIR')}'""")
+    os.environ['MPLCONFIGDIR'] = '{cfg.get('CACHE', 'MPLCONFIGDIR')}'"""
+    )
     assert cache_dirs == cache
 
 
 def test_calibration_history_level():
     from osa.job import check_history_level
-    levels = {
-        "onsite_create_drs4_pedestal_file": 1,
-        "onsite_create_calibration_file": 0
-    }
-    level, exit_status = check_history_level(
-        calibration_history_file, levels
-    )
+
+    levels = {"onsite_create_drs4_pedestal_file": 1, "onsite_create_calibration_file": 0}
+    level, exit_status = check_history_level(calibration_history_file, levels)
     assert level == 0
     assert exit_status == 0
 
 
 @pytest.fixture
 def mock_sacct_output():
     """Mock output of sacct to be able to use it in get_squeue_output function."""
-    return Path("./extra") / 'sacct_output.csv'
+    return Path("./extra") / "sacct_output.csv"
 
 
 @pytest.fixture
 def mock_squeue_output():
     """Mock output of squeue to be able to use it in get_squeue_output function."""
-    return Path("./extra") / 'squeue_output.csv'
+    return Path("./extra") / "squeue_output.csv"
 
 
 @pytest.fixture
 def sacct_output(mock_sacct_output):
     from osa.job import get_sacct_output
+
     return get_sacct_output(mock_sacct_output)
 
 
 @pytest.fixture
 def squeue_output(mock_squeue_output):
     from osa.job import get_squeue_output
+
     return get_squeue_output(mock_squeue_output)
 
 
-def test_set_queue_values(
-        sacct_output,
-        squeue_output,
-        sequence_list
-):
+def test_set_queue_values(sacct_output, squeue_output, sequence_list):
     from osa.job import set_queue_values
+
     set_queue_values(
         sacct_info=sacct_output,
         squeue_info=squeue_output,
         sequence_list=sequence_list,
     )
+    # Running calibration sequence
     assert sequence_list[0].state == "RUNNING"
     assert sequence_list[0].exit is None
     assert sequence_list[0].jobid == 12951086
     assert sequence_list[0].cputime == "00:36:00"
     assert sequence_list[0].tries == 4
+    # Pending DATA sequences
     assert sequence_list[1].state == "PENDING"
     assert sequence_list[1].tries == 2
     assert sequence_list[1].exit is None
     assert sequence_list[2].state == "PENDING"
     assert sequence_list[2].exit is None
     assert sequence_list[2].tries == 1
 
 
 def test_plot_job_statistics(sacct_output, running_analysis_dir):
     from osa.job import plot_job_statistics
+
     log_dir = running_analysis_dir / "log"
     log_dir.mkdir(parents=True, exist_ok=True)
     assert log_dir.exists()
     plot_job_statistics(sacct_output, log_dir)
     plot_file = log_dir / "job_statistics.pdf"
     assert plot_file.exists()
-
-
-def test_run_program_with_history_logging(running_analysis_dir):
-    from osa.job import run_program_with_history_logging
-
-    options.simulate = False
-
-    cmd = ["echo", "Testing"]
-    history_file = running_analysis_dir / "test.history"
-    run = "01140"
-    prod_id = "v0.2.0"
-    command = "echo"
-    config_file = "config_test.json"
-
-    rc = run_program_with_history_logging(
-        command_args=cmd,
-        history_file=history_file,
-        run=run,
-        prod_id=prod_id,
-        command=command,
-        config_file=config_file,
-    )
-    options.simulate = True
-    assert rc == 0
-    assert history_file.exists()
```

### Comparing `lstosa-0.9.4/osa/tests/test_paths.py` & `lstosa-0.9.5/osa/tests/test_paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,45 +3,50 @@
 
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.utils.utils import date_to_dir
 
 options.date = datetime.fromisoformat("2020-01-17")
 
+
 def test_get_calibration_file(r0_data, merged_run_summary):
     from osa.paths import get_calibration_file
+
     for file in r0_data:
         assert file.exists()
-    file = get_calibration_file(1805)
+    file = get_calibration_file(1809)
     file.exists()
 
 
 def test_get_drs4_pedestal_file(r0_data, merged_run_summary):
     from osa.paths import get_drs4_pedestal_file
+
     for file in r0_data:
         assert file.exists()
     file = get_drs4_pedestal_file(1804)
     file.exists()
 
 
 def test_pedestal_ids_file_exists(pedestal_ids_file):
     from osa.paths import pedestal_ids_file_exists
+
     pedestal_ids_file.exists()
     assert pedestal_ids_file_exists(1808) is True
 
 
 def test_get_datacheck_file(datacheck_dl1_files):
     from osa.paths import get_datacheck_files
+
     for file in datacheck_dl1_files:
         assert file.exists()
     dl1_path = Path("test_osa/test_files0/DL1/20200117/v0.1.0/tailcut84")
     files = get_datacheck_files(pattern="datacheck*.pdf", directory=dl1_path)
     expected_files = [
         dl1_path / "datacheck_dl1_LST-1.Run01808.pdf",
-        dl1_path / "datacheck_dl1_LST-1.Run01807.pdf"
+        dl1_path / "datacheck_dl1_LST-1.Run01807.pdf",
     ]
     assert set(files) == set(expected_files)
 
 
 def test_destination_dir():
     from osa.paths import destination_dir
```

### Comparing `lstosa-0.9.4/osa/tests/test_raw.py` & `lstosa-0.9.5/osa/tests/test_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 def test_get_raw_dir():
     options.date = datetime.fromisoformat("2020-01-17")
     night_dir = date_to_dir(options.date)
     r0_dir = Path(cfg.get("LST1", "R0_DIR")) / night_dir
     from osa.raw import get_raw_dir
+
     assert get_raw_dir(options.date) == r0_dir
 
 
 def test_get_check_raw_dir(r0_dir):
     options.date = datetime.fromisoformat("2020-01-18")
     from osa.raw import get_check_raw_dir
 
@@ -32,9 +33,7 @@
     from osa.raw import is_raw_data_available
 
     for file in r0_data:
         assert file.exists()
 
     options.date = datetime.fromisoformat("2020-01-17")
     assert is_raw_data_available(options.date) is True
-
-
```

### Comparing `lstosa-0.9.4/osa/tests/test_report.py` & `lstosa-0.9.5/osa/tests/test_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,18 @@
     history(
         run=run,
         prod_id=prod_id,
         stage=program,
         return_code=rc,
         history_file=history_file,
         input_file=input_file,
-        config_file=input_card
+        config_file=input_card,
     )
 
     options.simulate = True
 
-    logged_string = f"01800 r0_to_dl1 v1.0.0 {date_string} " \
-        "r0_to_dl1_01800.fits r0_dl1.config 0\n"
+    logged_string = (
+        f"01800 r0_to_dl1 v1.0.0 {date_string} " "r0_to_dl1_01800.fits r0_dl1.config 0\n"
+    )
 
     assert history_file.exists()
     assert history_file.read_text() == logged_string
```

### Comparing `lstosa-0.9.4/osa/tests/test_veto.py` & `lstosa-0.9.5/osa/tests/test_veto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from pathlib import Path
 
 
 def test_failed_history():
     from osa.veto import failed_history
-    good_history_file = Path(
-        './extra/history_files/sequence_LST1_04183.history'
-    )
-    bad_history_file = Path(
-        './extra/history_files/sequence_LST1_04183_failed.history'
-    )
-    one_line_history_file = Path(
-        './extra/history_files/sequence_LST1_04183_oneline.history'
-    )
+
+    good_history_file = Path("./extra/history_files/sequence_LST1_04183.history")
+    bad_history_file = Path("./extra/history_files/sequence_LST1_04183_failed.history")
+    one_line_history_file = Path("./extra/history_files/sequence_LST1_04183_oneline.history")
     one_line_history = failed_history(one_line_history_file)
     good_history_failed = failed_history(good_history_file)
     bad_history_failed = failed_history(bad_history_file)
 
     assert good_history_failed is False
     assert one_line_history is False
     assert bad_history_failed is True
 
 
 def test_get_veto_list(sequence_list):
     from osa.veto import get_veto_list
+
     veto_list = get_veto_list(sequence_list)
     assert not veto_list
 
 
 def test_get_closed_list(sequence_list):
     from osa.veto import get_closed_list
+
     closed_list = get_closed_list(sequence_list)
-    seq_list = ['LST1_01805', 'LST1_01807', 'LST1_01808']
+    seq_list = ["LST1_01807", "LST1_01808", "LST1_01809"]
     for sequence in seq_list:
         assert sequence in closed_list
```

### Comparing `lstosa-0.9.4/osa/utils/cliopts.py` & `lstosa-0.9.5/osa/utils/cliopts.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from osa.utils.utils import (
     get_calib_prod_id,
     get_dl1_prod_id,
     get_dl2_prod_id,
     get_prod_id,
     is_defined,
     set_prod_ids,
-    current_date
+    YESTERDAY,
 )
 
 __all__ = [
     "closer_argparser",
     "closercliparsing",
     "copy_datacheck_parsing",
     "data_sequence_cli_parsing",
@@ -35,15 +35,15 @@
     "get_prod_id",
     "get_dl1_prod_id",
     "get_dl2_prod_id",
     "get_calib_prod_id",
     "calibration_pipeline_cliparsing",
     "calibration_pipeline_argparser",
     "autocloser_cli_parser",
-    "common_parser"
+    "common_parser",
 ]
 
 log = myLogger(logging.getLogger(__name__))
 
 
 def valid_date(string):
     """Check if the string is a valid date and return a datetime object."""
@@ -141,24 +141,16 @@
     parser.add_argument(
         "--prod-id",
         action="store",
         type=str,
         dest="prod_id",
         help="Set the prod ID to define data directories",
     )
-    parser.add_argument(
-        "--drs4-pedestal-run",
-        type=int,
-        help="DRS4 pedestal run number"
-    )
-    parser.add_argument(
-        "--pedcal-run",
-        type=int,
-        help="Calibration run number"
-    )
+    parser.add_argument("--drs4-pedestal-run", type=int, help="DRS4 pedestal run number")
+    parser.add_argument("--pedcal-run", type=int, help="Calibration run number")
 
     parser.add_argument("tel_id", choices=["LST1"])
 
     return parser
 
 
 def calibration_pipeline_cliparsing():
@@ -198,38 +190,24 @@
     )
     parser.add_argument(
         "--no-dl2",
         action="store_true",
         default=False,
         help="Do not produce DL2 files (default False)",
     )
-    parser.add_argument(
-        "--pedcal-file",
-        type=Path,
-        help="Path of the calibration file"
-    )
-    parser.add_argument(
-        "--drs4-pedestal-file",
-        type=Path,
-        help="Path of the DRS4 pedestal file"
-    )
-    parser.add_argument(
-        "--time-calib-file",
-        type=Path,
-        help="Path of the time calibration file"
-    )
+    parser.add_argument("--pedcal-file", type=Path, help="Path of the calibration file")
+    parser.add_argument("--drs4-pedestal-file", type=Path, help="Path of the DRS4 pedestal file")
+    parser.add_argument("--time-calib-file", type=Path, help="Path of the time calibration file")
     parser.add_argument(
         "--systematic-correction-file",
         type=Path,
-        help="Path of the systematic correction factor file"
+        help="Path of the systematic correction factor file",
     )
     parser.add_argument(
-        "--drive-file",
-        type=Path,
-        help="Path of drive log file with pointing information"
+        "--drive-file", type=Path, help="Path of drive log file with pointing information"
     )
     parser.add_argument(
         "--run-summary",
         type=Path,
         help="Path of run summary file with time reference information",
     )
     parser.add_argument(
@@ -276,28 +254,28 @@
     )
 
 
 def sequencer_argparser():
     """Argument parser for sequencer script."""
     parser = ArgumentParser(
         description="Build the jobs for each run and process them for a given date",
-        parents=[common_parser]
+        parents=[common_parser],
     )
     parser.add_argument(
         "--no-submit",
         action="store_true",
         default=False,
         help="Produce job files but do not submit them",
     )
     parser.add_argument(
         "--no-calib",
         action="store_true",
         default=False,
         help="Skip calibration sequence. Run data sequences assuming "
-             "calibration products already produced (default False)",
+        "calibration products already produced (default False)",
     )
     parser.add_argument(
         "--no-dl2",
         action="store_true",
         default=False,
         help="Do not produce DL2 files (default False)",
     )
@@ -350,26 +328,19 @@
     parser.add_argument(
         "-q",
         action="store_true",
         dest="quit",
         help="use this flag to reset session and remove log file",
     )
     parser.add_argument(
-        "drs4_pedestal_run_id",
-        help="Number of the drs4_pedestal used in the calibration"
-    )
-    parser.add_argument(
-        "pedcal_run_id", help="Number of the used pedcal used in the calibration"
-    )
-    parser.add_argument(
-        "run", help="Number of the run whose provenance is to be extracted"
-    )
-    parser.add_argument(
-        "date", action="store", type=str, help="Observation starting date YYYYMMDD"
+        "drs4_pedestal_run_id", help="Number of the drs4_pedestal used in the calibration"
     )
+    parser.add_argument("pedcal_run_id", help="Number of the used pedcal used in the calibration")
+    parser.add_argument("run", help="Number of the run whose provenance is to be extracted")
+    parser.add_argument("date", action="store", type=str, help="Observation starting date YYYYMMDD")
     parser.add_argument("prod_id", action="store", type=str, help="Production ID")
 
     return parser
 
 
 def provprocessparsing():
 
@@ -461,29 +432,25 @@
         options.dl1_prod_id = get_dl1_prod_id()
     else:
         options.dl1_prod_id = options.prod_id
 
 
 def sequencer_webmaker_argparser():
     parser = ArgumentParser(
-        description="Script to make an xhtml from LSTOSA sequencer output",
-        parents=[common_parser]
+        description="Script to make an xhtml from LSTOSA sequencer output", parents=[common_parser]
     )
     options.tel_id = "LST1"
     options.prod_id = get_prod_id()
 
     return parser
 
 
 def set_default_date_if_needed():
     """Check if the date is set, if not set it to yesterday."""
-    if is_defined(options.date):
-        return options.date
-
-    return current_date()
+    return options.date if is_defined(options.date) else YESTERDAY
 
 
 def set_common_globals(opts):
     """Define common global variables using options module."""
     options.configfile = opts.config.resolve()
     options.date = opts.date
     options.simulate = opts.simulate
@@ -491,33 +458,23 @@
     options.verbose = opts.verbose
     options.tel_id = opts.tel_id
 
 
 def autocloser_cli_parser():
     """Define the command line parser for the autocloser."""
     parser = ArgumentParser(
-        description="Automatic job completion check and sequence closer.",
-        parents=[common_parser]
+        description="Automatic job completion check and sequence closer.", parents=[common_parser]
     )
+    parser.add_argument("--ignore-cronlock", action="store_true", help='Ignore "cron.lock"')
     parser.add_argument(
-        "--ignore-cronlock", action="store_true", help='Ignore "cron.lock"'
-    )
-    parser.add_argument(
-        "-f",
-        "--force",
-        action="store_true",
-        help="Force the autocloser to close the day"
+        "-f", "--force", action="store_true", help="Force the autocloser to close the day"
     )
     parser.add_argument(
         "--no-dl2",
         action="store_true",
         default=False,
         help="Disregard the production of DL2 files",
     )
-    parser.add_argument(
-        "-r", "--runwise", action="store_true", help="Close the day run-wise."
-    )
-    parser.add_argument(
-        "-l", "--log", type=Path, default=None, help="Write log to a file."
-    )
+    parser.add_argument("-r", "--runwise", action="store_true", help="Close the day run-wise.")
+    parser.add_argument("-l", "--log", type=Path, default=None, help="Write log to a file.")
     parser.add_argument("tel_id", type=str, choices=["LST1"])
     return parser
```

### Comparing `lstosa-0.9.4/osa/utils/iofile.py` & `lstosa-0.9.5/osa/utils/iofile.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,22 @@
     if file.exists() and file.is_file():
         if filecmp.cmp(file, file_temp):
             remove(file_temp)
             return False
 
         if options.simulate:
             remove(file_temp)
-            log.debug(
-                f"SIMULATE File {file_temp} would replace {file}."
-                f"Deleting {file_temp}"
-            )
+            log.debug(f"SIMULATE File {file_temp} would replace {file}." f"Deleting {file_temp}")
         else:
             try:
                 rename(file_temp, file)
             except (IOError, OSError) as e:
                 log.exception(f"{e.strerror} {e.filename}")
     elif options.simulate:
-        log.debug(
-            f"SIMULATE File {file_temp} would be written as {file}. Deleting {file_temp}"
-        )
+        log.debug(f"SIMULATE File {file_temp} would be written as {file}. Deleting {file_temp}")
     else:
         rename(file_temp, file)
     return True
 
 
 def append_to_file(file: pathlib.Path, content: str) -> None:
     """
```

### Comparing `lstosa-0.9.4/osa/utils/logging.py` & `lstosa-0.9.5/osa/utils/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 )
 
 __all__ = ["myLogger"]
 
 
 class MyFormatter(logging.Formatter):
     """Customize formatter of info logging level."""
+
     info_fmt = "%(message)s"
 
     def __init__(self):
         super().__init__(fmt=DEFAULT_LOGGING_FORMAT, datefmt=None, style="%")
 
     def format(self, record):
         """
```

### Comparing `lstosa-0.9.4/osa/utils/register.py` & `lstosa-0.9.5/osa/utils/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from osa.utils.logging import myLogger
 from osa.veto import set_closed_sequence
 
 __all__ = [
     "register_files",
     "register_run_concept_files",
     "register_found_pattern",
-    "register_non_existing_file"
+    "register_non_existing_file",
 ]
 
 log = myLogger(logging.getLogger(__name__))
 
 
 def register_files(run_str, analysis_dir, prefix, suffix, output_dir) -> None:
     """
@@ -61,18 +61,15 @@
     analysis_dir = Path(options.directory)
     dl1ab_dir = analysis_dir / options.dl1_prod_id
 
     if prefix == "dl1_LST-1" and suffix == ".h5":
         dl1_filepath_analysis_dir = analysis_dir / input_file.name
         dl1_filepath_dl1_dir = dl1ab_dir / input_file.name
         # Remove the original DL1 files pre DL1ab stage and keep only symlinks
-        if (
-                dl1_filepath_analysis_dir.is_file()
-                and not dl1_filepath_analysis_dir.is_symlink()
-        ):
+        if dl1_filepath_analysis_dir.is_file() and not dl1_filepath_analysis_dir.is_symlink():
             dl1_filepath_analysis_dir.unlink()
 
         if not dl1_filepath_analysis_dir.is_symlink():
             dl1_filepath_analysis_dir.symlink_to(output_file.resolve())
 
         # Also set the symlink in the DL1ab subdirectory
         if not dl1_filepath_dl1_dir.is_symlink():
@@ -98,33 +95,26 @@
     if concept == "DL2":
         initial_dir = initial_dir / options.dl2_prod_id
 
     elif concept in ["DL1AB", "DATACHECK"]:
         initial_dir = initial_dir / options.dl1_prod_id
 
     output_dir = destination_dir(concept, create_dir=False)
-    data_level = cfg.get("PATTERN", concept + "TYPE")
-    prefix = cfg.get("PATTERN", concept + "PREFIX")
-    suffix = cfg.get("PATTERN", concept + "SUFFIX")
+    data_level = cfg.get("PATTERN", f"{concept}TYPE")
+    prefix = cfg.get("PATTERN", f"{concept}PREFIX")
+    suffix = cfg.get("PATTERN", f"{concept}SUFFIX")
 
     log.debug(f"Registering {data_level} file for {prefix}*{run_string}*{suffix}")
-    if concept in [
-        "DL1AB", "DATACHECK", "PEDESTAL", "CALIB", "TIMECALIB", "MUON", "DL2"
-    ]:
+    if concept in ["DL1AB", "DATACHECK", "PEDESTAL", "CALIB", "TIMECALIB", "MUON", "DL2"]:
         register_files(run_string, initial_dir, prefix, suffix, output_dir)
     else:
         log.warning(f"Concept {concept} not known")
 
 
-def register_found_pattern(
-        file_path: Path,
-        seq_list: list,
-        concept: str,
-        destination_path: Path
-):
+def register_found_pattern(file_path: Path, seq_list: list, concept: str, destination_path: Path):
     """
 
     Parameters
     ----------
     file_path: pathlib.Path
     seq_list: list
     concept: str
```

### Comparing `lstosa-0.9.4/osa/utils/tests/test_utils.py` & `lstosa-0.9.5/osa/utils/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,90 @@
 import datetime
 
 import pytest
 
 from osa.configs import options
 from osa.configs.config import cfg
-from osa.utils.utils import date_to_iso
 
 options.date = datetime.datetime.fromisoformat("2020-01-17")
 options.tel_id = "LST1"
 options.prod_id = "v0.1.0"
 
 
-def test_get_current_date():
-    from osa.utils.utils import current_date
-
-    # Both having the same separator
-    now = datetime.datetime.utcnow()
-    if now.hour < 12:
-        # In our convention, date changes at 12:00 pm
-        yesterday_lst_date = now - datetime.timedelta(hours=12)
-        assert date_to_iso(current_date()) == date_to_iso(yesterday_lst_date)
-    else:
-        assert date_to_iso(current_date()) == date_to_iso(now)
-
-
 def test_analysis_path(running_analysis_dir):
     from osa.paths import analysis_path
 
     assert analysis_path("LST1").resolve() == running_analysis_dir
 
 
 def test_get_lstchain_version():
     from osa.utils.utils import get_lstchain_version
     from lstchain import __version__
 
-    assert get_lstchain_version() == "v" + __version__
+    assert get_lstchain_version() == f"v{__version__}"
 
 
 def test_get_prod_id():
     from osa.utils.utils import get_prod_id
 
     prod_id = cfg.get(options.tel_id, "PROD_ID")
     assert get_prod_id() == prod_id
 
 
 def test_get_calib_prod_id():
     from osa.utils.utils import get_calib_prod_id
+
     prod_id = cfg.get(options.tel_id, "CALIB_PROD_ID")
     assert get_calib_prod_id() == prod_id
 
 
 def test_date_in_yymmdd():
     from osa.utils.utils import date_in_yymmdd
 
     assert date_in_yymmdd("20200113") == "20_01_13"
 
 
 def test_date_to_dir():
     from osa.utils.utils import date_to_dir
+
     assert date_to_dir(options.date) == "20200117"
 
 
 def test_time_to_seconds():
     from osa.utils.utils import time_to_seconds
+
     seconds_with_day = time_to_seconds("2-02:27:15")
     assert seconds_with_day == 2 * 24 * 3600 + 2 * 3600 + 27 * 60 + 15
     seconds = time_to_seconds("02:27:15")
     assert seconds == 2 * 3600 + 27 * 60 + 15
     seconds = time_to_seconds("27:15")
     assert seconds == 27 * 60 + 15
     assert time_to_seconds(None) == 0
 
     with pytest.raises(ValueError):
         time_to_seconds("12.11.11")
 
 
 def test_stringify():
     from osa.utils.utils import stringify
+
     assert stringify(["command", "foo", "--bar"]) == "command foo --bar"
 
 
 def test_gettag():
     from osa.utils.utils import gettag
+
     assert gettag() == "test_utils.py(test_gettag)"
 
 
 def test_night_finished_flag(base_test_dir):
     from osa.utils.utils import night_finished_flag
+
     assert night_finished_flag() == base_test_dir / "OSA/Closer/20200117/v0.1.0/NightFinished.txt"
 
 
 def test_create_lock(base_test_dir):
     from osa.utils.utils import create_lock
+
     lock_path = base_test_dir / "test_lock.closed"
     is_closed = create_lock(lock_path)
     assert is_closed is False
```

### Comparing `lstosa-0.9.4/osa/utils/utils.py` & `lstosa-0.9.5/osa/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions to deal with dates and prod IDs."""
 
+
 import inspect
 import logging
 import os
 from datetime import datetime, timedelta
 from pathlib import Path
 from socket import gethostname
 
@@ -24,67 +25,48 @@
     "is_defined",
     "create_lock",
     "stringify",
     "gettag",
     "get_calib_prod_id",
     "get_dl1_prod_id",
     "get_dl2_prod_id",
-    "get_night_limit_timestamp",
     "time_to_seconds",
     "DATACHECK_FILE_PATTERNS",
     "YESTERDAY",
     "set_prod_ids",
     "is_night_time",
     "cron_lock",
     "example_seq",
-    "current_date"
 ]
 
 log = myLogger(logging.getLogger(__name__))
 
 DATACHECK_PRODUCTS = ["drs4", "enf_calibration", "dl1"]
 
 DATACHECK_FILE_PATTERNS = {
     "PEDESTAL": "drs4*.pdf",
     "CALIB": "calibration*.pdf",
     "DL1AB": "datacheck_dl1*.pdf",
-    "LONGTERM": "DL1_datacheck_*.*"
+    "LONGTERM": "DL1_datacheck_*.*",
 }
 
-YESTERDAY = datetime.today() - timedelta(days=1)
-
-
-def current_date() -> datetime:
-    """
-    Get current data following LST data-taking convention in which the date
-    changes at 12:00 pm instead of 00:00 or 12:00 am to cover a natural
-    data-taking night.
-
-    Returns
-    -------
-    date: datetime.datetime
-        Current date following LST data-taking convention.
-    """
-    return (
-        datetime.now() - timedelta(days=1)
-        if datetime.now().hour < 12
-        else datetime.now()
-    )
+YESTERDAY = datetime.now() - timedelta(days=1)
 
 
 def get_lstchain_version():
     """
     Get the lstchain version.
 
     Returns
     -------
     lstchain_version: string
     """
     from lstchain import __version__
-    return "v" + __version__
+
+    return f"v{__version__}"
 
 
 def get_prod_id():
     """
     Get production ID from the configuration file if it is defined.
     Otherwise, it takes the lstchain version used.
 
@@ -219,35 +201,14 @@
     try:
         variable
     except NameError:
         variable = None
     return variable is not None
 
 
-def get_night_limit_timestamp():
-    """Night limit timestamp for DB."""
-    from dev.mysql import select_db
-
-    night_limit = None
-    server = cfg.get("MYSQL", "server")
-    user = cfg.get("MYSQL", "user")
-    database = cfg.get("MYSQL", "database")
-    table = cfg.get("MYSQL", "nighttimes")
-    night = date_to_iso(options.date)
-    selections = ["END"]
-    conditions = {"NIGHT": night}
-    matrix = select_db(server, user, database, table, selections, conditions)
-    if len(matrix) > 0:
-        night_limit = matrix[0][0]
-    else:
-        log.warning("No night_limit found")
-    log.debug(f"Night limit is {night_limit}")
-    return night_limit
-
-
 def is_day_closed() -> bool:
     """Get the name and Check for the existence of the Closer flag file."""
     flag_file = night_finished_flag()
     return flag_file.exists()
 
 
 def date_in_yymmdd(date_string):
@@ -298,17 +259,15 @@
     """
     if timestring is None:
         timestring = "00:00:00"
     if "-" in timestring:
         # Day is also specified (D-)HH:MM:SS
         days, hhmmss = timestring.split("-")
         hours, minutes, seconds = hhmmss.split(":")
-        return (
-            int(days) * 24 * 3600 + int(hours) * 3600 + int(minutes) * 60 + int(seconds)
-        )
+        return int(days) * 24 * 3600 + int(hours) * 3600 + int(minutes) * 60 + int(seconds)
 
     split_time = timestring.split(":")
     if len(split_time) == 2:
         # MM:SS
         minutes, seconds = split_time
         hours = 0
     elif len(split_time) == 3:
```

### Comparing `lstosa-0.9.4/osa/version.py` & `lstosa-0.9.5/osa/version.py`

 * *Files identical despite different names*

### Comparing `lstosa-0.9.4/osa/veto.py` & `lstosa-0.9.5/osa/veto.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __all__ = [
     "failed_history",
     "get_veto_list",
     "get_closed_list",
     "set_veto_action",
     "set_closed_action",
     "update_vetoes",
-    "set_closed_sequence"
+    "set_closed_sequence",
 ]
 
 log = myLogger(logging.getLogger(__name__))
 
 
 def get_veto_list(sequence_list):
     """Get a list of vetoed sequences."""
@@ -42,17 +42,17 @@
             log.debug(f"Attributes of sequence {sequence.seq} updated")
 
 
 def update_vetoes(sequence_list):
     """Create a .veto file for a given sequence if reached maximum number of trials."""
     for sequence in sequence_list:
         if (
-                not os.path.exists(sequence.veto)
-                and os.path.exists(sequence.history)
-                and failed_history(sequence.history)
+            not os.path.exists(sequence.veto)
+            and os.path.exists(sequence.history)
+            and failed_history(sequence.history)
         ):
             Path(sequence.veto).touch()
             log.debug(f"Created veto file {sequence.veto}")
 
 
 def failed_history(history_file: Path) -> bool:
     """
@@ -65,18 +65,15 @@
 
     # Check if history file has at least two trials
     if len(history_lines) < 2:
         return False
 
     # Check if the last line of the history file is repeated twice
     # and the exit status is non-zero
-    return (
-        history_lines[-1] == history_lines[-2]
-        and history_lines[-1].split()[-1] != "0"
-    )
+    return history_lines[-1] == history_lines[-2] and history_lines[-1].split()[-1] != "0"
 
 
 def set_closed_sequence(sequence):
     """Creates a .closed lock file for a given sequence."""
     sequence.closed = Path(options.directory) / f"sequence_{sequence.jobname}.closed"
     sequence.closed.touch()
```

### Comparing `lstosa-0.9.4/osa/webserver/utils.py` & `lstosa-0.9.5/osa/webserver/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 from osa.utils.logging import myLogger
 
 __all__ = ["directory_in_webserver", "copy_to_webserver"]
 
 log = myLogger(logging.getLogger(__name__))
 
 
-def directory_in_webserver(
-        host: str,
-        datacheck_type: str,
-        date: str,
-        prod_id: str
-) -> Path:
+def directory_in_webserver(host: str, datacheck_type: str, date: str, prod_id: str) -> Path:
     """
     Create directories in the datacheck web server.
 
     Parameters
     ----------
     host : str
         Hostname of the server to which the datacheck products will be copied
@@ -51,20 +46,15 @@
 
     remote_mkdir = ["ssh", host, "mkdir", "-p", destination_dir]
     sp.run(remote_mkdir, check=True)
 
     return destination_dir
 
 
-def copy_to_webserver(
-        files: List[Path],
-        datacheck_type: str,
-        date: str,
-        prod_id: str
-) -> None:
+def copy_to_webserver(files: List[Path], datacheck_type: str, date: str, prod_id: str) -> None:
     """
     Copy files to the webserver in host.
 
     Parameters
     ----------
     files : List[Path]
         List of files to be copied
```

### Comparing `lstosa-0.9.4/osa/workflow/dl3.py` & `lstosa-0.9.5/osa/workflow/dl3.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 import click
 from astropy.utils import iers
 
 from osa.configs import options
 from osa.configs.config import cfg
 from osa.nightsummary.extract import build_sequences, get_source_list
-from osa.paths import (
-    destination_dir, DEFAULT_CFG, create_source_directories, analysis_path
-)
+from osa.paths import destination_dir, DEFAULT_CFG, create_source_directories, analysis_path
 from osa.utils.cliopts import get_prod_id, get_dl2_prod_id
 from osa.utils.logging import myLogger
 from osa.utils.utils import stringify, YESTERDAY
 
 iers.conf.auto_download = False
 
 __all__ = [
@@ -34,28 +32,21 @@
     "batch_cmd_create_dl3",
     "batch_cmd_create_index_dl3",
     "get_irf_file",
     "create_irf",
     "produce_dl3_files",
     "setup_global_options",
     "cuts_subdirectory",
-    "create_obs_index"
+    "create_obs_index",
 ]
 
 log = myLogger(logging.getLogger(__name__))
 
 
-def batch_cmd_create_irf(
-        cwd,
-        mc_gamma,
-        mc_proton,
-        mc_electron,
-        output_irf_file,
-        dl3_config
-):
+def batch_cmd_create_irf(cwd, mc_gamma, mc_proton, mc_electron, output_irf_file, dl3_config):
     """Create batch command to create IRF file with sbatch."""
     return [
         "sbatch",
         "--parsable",
         "--mem=6GB",
         "--job-name=irf",
         "-D",
@@ -70,23 +61,15 @@
         f"--output-irf-file={output_irf_file}",
         f"--config={dl3_config}",
         "--overwrite",
     ]
 
 
 def batch_cmd_create_dl3(
-        dl2_file,
-        dl3_dir,
-        run,
-        source_name,
-        source_ra,
-        source_dec,
-        irf,
-        dl3_config,
-        job_irf
+    dl2_file, dl3_dir, run, source_name, source_ra, source_dec, irf, dl3_config, job_irf
 ):
     """Create batch command to create DL3 files with sbatch."""
     log_dir = dl3_dir / "log"
     log_dir.mkdir(exist_ok=True, parents=True)
     log_file = log_dir / f"dl2_to_dl3_Run{run:05d}_{source_name}_%j.log"
     sbatch_cmd = [
         "sbatch",
@@ -185,21 +168,21 @@
         capture_output=True,
         text=True,
     )
     return irf_file, job_irf.stdout.strip()
 
 
 def produce_dl3_files(
-        sequence_list,
-        irf_file: Path,
-        dl2_dir: Path,
-        cuts_dir: Path,
-        dl3_config: Path,
-        job_id_irf: int,
-        simulate: bool = False
+    sequence_list,
+    irf_file: Path,
+    dl2_dir: Path,
+    cuts_dir: Path,
+    dl3_config: Path,
+    job_id_irf: int,
+    simulate: bool = False,
 ):
     """Produce the DL3 files for a given list of sequences."""
     list_of_job_id = []
 
     log.info("Looping over the runs to produce the DL3 files.")
     for sequence in sequence_list:
 
@@ -235,20 +218,15 @@
                 log.debug("Simulate launching scripts")
 
             log.debug(f"Executing {stringify(cmd2)}")
 
     return list_of_job_id
 
 
-def create_obs_index(
-        source_list: list,
-        cuts_dir: Path,
-        parent_jobs: list,
-        simulate: bool = False
-):
+def create_obs_index(source_list: list, cuts_dir: Path, parent_jobs: list, simulate: bool = False):
     """Creating observation index for each source."""
     log.info("Creating observation index for each source.")
 
     for source in source_list:
         dl3_subdir = cuts_dir / source
 
         cmd3 = batch_cmd_create_index_dl3(dl3_subdir, parent_jobs)
@@ -285,37 +263,33 @@
     std_cuts_dir.mkdir(parents=True, exist_ok=True)
     log_dir.mkdir(exist_ok=True)
     log.debug(f"DL3 directory: {dl3_dir}")
     return std_cuts_dir
 
 
 @click.command()
-@click.argument('telescope', type=click.Choice(['LST1', 'LST2']))
+@click.argument("telescope", type=click.Choice(["LST1", "LST2"]))
+@click.option("-d", "--date-obs", type=click.DateTime(formats=["%Y-%m-%d"]), default=YESTERDAY)
 @click.option(
-    '-d',
-    '--date-obs',
-    type=click.DateTime(formats=["%Y-%m-%d"]),
-    default=YESTERDAY
-)
-@click.option(
-    '-c', '--config',
+    "-c",
+    "--config",
     type=click.Path(dir_okay=False),
     default=DEFAULT_CFG,
-    help='Read option defaults from the specified cfg file',
+    help="Read option defaults from the specified cfg file",
 )
-@click.option('-v', '--verbose', is_flag=True)
-@click.option('--local', is_flag=True)
-@click.option('-s', '--simulate', is_flag=True)
+@click.option("-v", "--verbose", is_flag=True)
+@click.option("--local", is_flag=True)
+@click.option("-s", "--simulate", is_flag=True)
 def main(
-        date_obs: datetime = YESTERDAY,
-        telescope: str = "LST1",
-        verbose: bool = False,
-        simulate: bool = False,
-        local: bool = False,
-        config: Path = DEFAULT_CFG,
+    date_obs: datetime = YESTERDAY,
+    telescope: str = "LST1",
+    verbose: bool = False,
+    simulate: bool = False,
+    local: bool = False,
+    config: Path = DEFAULT_CFG,
 ):
     """Produce the IRF and DL3 files tool in a run basis."""
     log.setLevel(logging.INFO)
 
     if verbose:
         log.setLevel(logging.DEBUG)
 
@@ -343,18 +317,15 @@
     # Create a subdirectory inside the DL3 directory corresponding to the selection cuts
     std_cuts_dir = cuts_subdirectory()
 
     # Create a subdirectory for each source
     create_source_directories(source_list, std_cuts_dir)
 
     # Get IRF file
-    irf_file, dl3_config, job_id_irf = get_irf_file(
-        directory=std_cuts_dir,
-        simulate=simulate
-    )
+    irf_file, dl3_config, job_id_irf = get_irf_file(directory=std_cuts_dir, simulate=simulate)
 
     # Create the DL3 files
     list_of_job_id = produce_dl3_files(
         sequence_list=sequence_list,
         irf_file=irf_file,
         dl2_dir=dl2_dir,
         cuts_dir=std_cuts_dir,
@@ -364,13 +335,13 @@
     )
 
     # Creating an observation file index for each source
     create_obs_index(
         source_list=source_list,
         cuts_dir=std_cuts_dir,
         parent_jobs=list_of_job_id,
-        simulate=simulate
+        simulate=simulate,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lstosa-0.9.4/setup.cfg` & `lstosa-0.9.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 setup_requires = setuptools_scm
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	astropy~=4.2
 	lstchain==0.9.6
 	ctapipe~=0.12.0
 	matplotlib~=3.5
 	numpy<1.22.0a0
 	pandas
@@ -35,14 +35,16 @@
 	pydot
 	pydotplus
 	psutil
 	click
 	toml
 	pymongo
 	gammapy~=0.19.0
+	tenacity
+	protobuf~=3.20.0
 zip_safe = no
 include_package_data = True
 
 [options.packages.find]
 exclude = osa._dev_version
 
 [options.entry_points]
@@ -65,14 +67,15 @@
 	gain_selection = osa.scripts.gain_selection:main
 
 [options.extras_require]
 setup = setuptools_scm
 test = 
 	pytest
 	pytest-cov
+	freezegun
 docs = 
 	sphinx
 	sphinx_rtd_theme
 	sphinx_automodapi
 	sphinx_argparse
 	sphinx-autoapi
 	numpydoc
```

