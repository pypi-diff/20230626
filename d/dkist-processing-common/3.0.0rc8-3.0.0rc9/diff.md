# Comparing `tmp/dkist-processing-common-3.0.0rc8.tar.gz` & `tmp/dkist-processing-common-3.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-3.0.0rc8.tar", last modified: Mon Jun 26 16:13:19 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc9.tar", last modified: Mon Jun 26 19:45:16 2023, max compression
```

## Comparing `dkist-processing-common-3.0.0rc8.tar` & `dkist-processing-common-3.0.0rc9.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/139.feature.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/139.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/changelog/140.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.268681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.264681 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4798 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 16:13:19.000000 dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-26 16:13:19.272681 dkist-processing-common-3.0.0rc8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-26 16:13:13.000000 dkist-processing-common-3.0.0rc8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/changelog/138.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.270571 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.270571 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.270571 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.270571 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.266571 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-26 19:45:16.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4824 2023-06-26 19:45:16.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 19:45:16.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-26 19:45:16.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 19:45:16.000000 dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 19:45:16.274571 dkist-processing-common-3.0.0rc9/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-26 19:45:16.278571 dkist-processing-common-3.0.0rc9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-26 19:45:08.000000 dkist-processing-common-3.0.0rc9/setup.py
```

### Comparing `dkist-processing-common-3.0.0rc8/.gitignore` & `dkist-processing-common-3.0.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/PKG-INFO` & `dkist-processing-common-3.0.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc8
+Version: 3.0.0rc9
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc8/README.rst` & `dkist-processing-common-3.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc9/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/json.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/codecs/str.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     modstate = "MODSTATE"
     dsps_repeat = "DSPS_REPEAT"
     calibrated = "CALIBRATED"  # A flag to indicate the data has been calibrated but not yet output
     quality = "QUALITY"
     exposure_time = "EXP_TIME"
     quality_task = "QUALITY_TASK"
     parameter = "PARAMETER"
+    workflow_task = "WORKFLOW_TASK"
     debug = "DEBUG"
 
 
 class Tag:
     """Controlled methods for creating tags from stems + optional suffixes."""
 
     @staticmethod
@@ -307,7 +308,24 @@
             path e.g. For object_key 'parameters/abc123.fits' the object name is 'abc123.fits'
 
         Returns
         -------
         A parameter file tag for the given object_name
         """
         return cls.format_tag(StemName.parameter, object_name)
+
+    @classmethod
+    def workflow_task(cls, class_name: str) -> str:
+        """
+        Return a unique workflow task tag.
+
+        Parameters
+        ----------
+        class_name
+            The unique value identifying the workflow task class that wrote the file.
+            e.g. TaskClass().__class__.__name__  # TaskClass
+
+        Returns
+        -------
+        A workflow task class tag for the given class_name
+        """
+        return cls.format_tag(StemName.workflow_task, class_name)
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from dkist_processing_common._util.config import get_config
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.codecs.bytes import bytes_encoder
 from dkist_processing_common.codecs.path import path_decoder
 from dkist_processing_common.models.constants import ConstantsBase
 from dkist_processing_common.models.tags import StemName
+from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 
 __all__ = ["WorkflowTaskBase", "tag_type_hint"]
 
 logger = logging.getLogger(__name__)
 
 tag_type_hint = Iterable[str] | str
@@ -204,14 +205,16 @@
 
         Returns
         -------
         The path for the written file
         """
         file_obj = encoder(data, **encoder_kwargs)
         tags = self._parse_tags(tags)
+        tags.append(Tag.workflow_task(self.__class__.__name__))
+
         relative_path = relative_path or self._build_generic_tag_filename(tags)
         relative_path = Path(relative_path)
         self.scratch.write(
             file_obj=file_obj, relative_path=relative_path, tags=tags, overwrite=overwrite
         )
         return relative_path
 
@@ -224,14 +227,15 @@
         """
         return [
             StemName.debug.value,
             StemName.input.value,
             StemName.intermediate.value,
             StemName.calibrated.value,
             StemName.output.value,
+            StemName.workflow_task.value,
             StemName.task.value,
             StemName.dsps_repeat.value,
             StemName.cs_step.value,
             StemName.modstate.value,
         ]
 
     def _build_generic_tag_filename(self, tags: Iterable[str]) -> str:
@@ -328,15 +332,15 @@
 
     def remove_tags(self, path: Path | str, tags: tag_type_hint) -> None:
         """Remove the association between the given tag(s) and the given path."""
         tags = self._parse_tags(tags)
         self.scratch.remove_tags(path, tags)
 
     @staticmethod
-    def _parse_tags(tags: tag_type_hint) -> Iterable[str]:
+    def _parse_tags(tags: tag_type_hint) -> list[str]:
         result = []
         if isinstance(tags, str):
             tags = [tags]
         for tag in tags:
             if not isinstance(tag, str):
                 raise TypeError(f"Tags must be strings. Got {type(tag)} instead.")
             result.append(tag)
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,24 +35,26 @@
         Tag.frame(),
         Tag.calibrated(),
         Tag.debug(),
         Tag.task("FOO"),
         Tag.dsps_repeat(2),
         Tag.cs_step(4),
         Tag.modstate(5),
+        Tag.workflow_task("BAR"),
         Tag.movie(),
         "ZZZ",
     ]
     shuffle(tags)
     expected_base_name = (
         f"{StemName.debug.value}_"
         f"{StemName.input.value}_"
         f"{StemName.intermediate.value}_"
         f"{StemName.calibrated.value}_"
         f"{StemName.output.value}_"
+        f"{StemName.workflow_task.value.replace('_', '-')}-BAR_"
         f"{StemName.task.value}-FOO_"
         f"{StemName.dsps_repeat.value.replace('_', '-')}-2_"
         f"{StemName.cs_step.value.replace('_', '-')}-4_"
         f"{StemName.modstate.value}-5_"
         f"{StemName.movie.value}_"
         f"ZZZ"
     )
@@ -101,7 +103,31 @@
     Then: The correct filename is returned
     """
     tags, expected_name = tags_and_expected_generic_name
 
     built_name = base_task._build_generic_tag_filename(tags)
     assert built_name.startswith(expected_name)
     assert built_name.endswith(".dat")
+
+
+@pytest.mark.parametrize(
+    "other_tags",
+    [
+        pytest.param("A", id="single"),
+        pytest.param(["A", "B"], id="list"),
+    ],
+)
+def test_write_workflow_task_tag(base_task, other_tags: str | list[str]):
+    """
+    :Given: A WorkflowTaskBase task and tags to write with
+    :When: Writing a file with given tags
+    :Then: Written file is tagged with a workflow task class tag in addition to given tags
+    """
+    # When
+    path = base_task.write(
+        data=b"123",
+        tags=other_tags,
+    )
+    path = base_task.scratch.workflow_base_path / path
+    # Then
+    tags = base_task.tags(path)
+    assert Tag.workflow_task(base_task.__class__.__name__) in tags
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,19 @@
     When: Tagging files with group information
     Then: All files are correctly tagged
     """
     tag_pot, _ = parse_inputs_task.make_flower_pots()
     parse_inputs_task.tag_petals(tag_pot)
     num_mod = parse_inputs_task._num_mod
     files_per_mod = parse_inputs_task._num_files_per_mod
-    expected_tag_set = {Tag.input(), Tag.frame()}
+    expected_tag_set = {
+        Tag.input(),
+        Tag.frame(),
+        Tag.workflow_task(parse_inputs_task.__class__.__name__),
+    }
     for m in range(num_mod):
         expected_tag_set.add(Tag.modstate(m))
         expected_mod_files = [
             parse_inputs_task.scratch.absolute_path(f"input/input_{i}.fits")
             for i in range(num_mod * files_per_mod)[m::num_mod]
         ]
         assert sorted(list(parse_inputs_task.read(tags=Tag.modstate(m)))) == expected_mod_files
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc9/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc8
+Version: 3.0.0rc9
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/138.feature.rst
 changelog/139.feature.2.rst
 changelog/139.feature.rst
 changelog/140.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
```

### Comparing `dkist-processing-common-3.0.0rc8/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc9/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/docs/Makefile` & `dkist-processing-common-3.0.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/docs/conf.py` & `dkist-processing-common-3.0.0rc9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/docs/make.bat` & `dkist-processing-common-3.0.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/pyproject.toml` & `dkist-processing-common-3.0.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc8/setup.cfg` & `dkist-processing-common-3.0.0rc9/setup.cfg`

 * *Files identical despite different names*

