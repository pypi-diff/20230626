# Comparing `tmp/dkist-processing-common-3.0.0rc7.tar.gz` & `tmp/dkist-processing-common-3.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-3.0.0rc7.tar", last modified: Thu Jun 22 22:57:51 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc8.tar", last modified: Mon Jun 26 16:13:19 2023, max compression
```

## Comparing `dkist-processing-common-3.0.0rc7.tar` & `dkist-processing-common-3.0.0rc8.tar`

### file list

```diff
@@ -1,133 +1,131 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/139.feature.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/139.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/140.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6844 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/setup.py
```

### Comparing `dkist-processing-common-3.0.0rc7/.gitignore` & `dkist-processing-common-3.0.0rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc8/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/PKG-INFO` & `dkist-processing-common-3.0.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc7
+Version: 3.0.0rc8
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc7/README.rst` & `dkist-processing-common-3.0.0rc8/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc8/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/json.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/str.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/trial_output_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from abc import abstractmethod
 from functools import cached_property
 from pathlib import Path
 
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.globus import GlobusMixin
 from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
-from dkist_processing_common.tasks.output_data_base import OutputDataBase
 from dkist_processing_common.tasks.output_data_base import TransferDataBase
 
 logger = logging.getLogger(__name__)
 
 
 class TransferTrialDataBase(TransferDataBase, GlobusMixin, ABC):
     """
```

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc7
+Version: 3.0.0rc8
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 dkist_processing_common/tasks/parse_l0_input_data.py
 dkist_processing_common/tasks/quality_metrics.py
 dkist_processing_common/tasks/teardown.py
 dkist_processing_common/tasks/transfer_input_data.py
 dkist_processing_common/tasks/trial_output_data.py
 dkist_processing_common/tasks/write_l1.py
 dkist_processing_common/tasks/mixin/__init__.py
-dkist_processing_common/tasks/mixin/debug_frame.py
 dkist_processing_common/tasks/mixin/fits.py
 dkist_processing_common/tasks/mixin/globus.py
 dkist_processing_common/tasks/mixin/input_dataset.py
 dkist_processing_common/tasks/mixin/interservice_bus.py
 dkist_processing_common/tasks/mixin/metadata_store.py
 dkist_processing_common/tasks/mixin/object_store.py
 dkist_processing_common/tasks/mixin/quality/__init__.py
@@ -83,15 +82,14 @@
 dkist_processing_common/tests/__init__.py
 dkist_processing_common/tests/conftest.py
 dkist_processing_common/tests/test_assemble_movie.py
 dkist_processing_common/tests/test_base.py
 dkist_processing_common/tests/test_codecs.py
 dkist_processing_common/tests/test_constants.py
 dkist_processing_common/tests/test_cs_step.py
-dkist_processing_common/tests/test_debug_frame.py
 dkist_processing_common/tests/test_dkist_location.py
 dkist_processing_common/tests/test_fits.py
 dkist_processing_common/tests/test_fits_access.py
 dkist_processing_common/tests/test_fits_flowers.py
 dkist_processing_common/tests/test_flower_pot.py
 dkist_processing_common/tests/test_input_dataset.py
 dkist_processing_common/tests/test_output_data_base.py
```

### Comparing `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/docs/Makefile` & `dkist-processing-common-3.0.0rc8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/docs/conf.py` & `dkist-processing-common-3.0.0rc8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/docs/make.bat` & `dkist-processing-common-3.0.0rc8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc8/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/pyproject.toml` & `dkist-processing-common-3.0.0rc8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc7/setup.cfg` & `dkist-processing-common-3.0.0rc8/setup.cfg`

 * *Files identical despite different names*

