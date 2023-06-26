# Comparing `tmp/medkit_lib-0.6.0.tar.gz` & `tmp/medkit_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medkit_lib-0.6.0.tar", max compression
+gzip compressed data, was "medkit_lib-0.7.0.tar", max compression
```

## Comparing `medkit_lib-0.6.0.tar` & `medkit_lib-0.7.0.tar`

### file list

```diff
@@ -1,124 +1,128 @@
--rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.6.0/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-23 15:19:08.254089 medkit_lib-0.6.0/README.md
--rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.6.0/medkit/__init__.py
--rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/__init__.py
--rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.6.0/medkit/audio/preprocessing/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/preprocessing/downmixer.py
--rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/preprocessing/power_normalizer.py
--rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/preprocessing/resampler.py
--rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.6.0/medkit/audio/segmentation/__init__.py
--rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/segmentation/pa_speaker_detector.py
--rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/segmentation/webrtc_voice_detector.py
--rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.6.0/medkit/audio/transcription/__init__.py
--rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/transcription/doc_transcriber.py
--rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/audio/transcription/hf_transcriber_function.py
--rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/audio/transcription/sb_transcriber_function.py
--rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/audio/transcription/transcribed_document.py
--rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/__init__.py
--rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.6.0/medkit/core/_prov_graph.py
--rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/annotation.py
--rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.6.0/medkit/core/annotation_container.py
--rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/core/attribute.py
--rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.6.0/medkit/core/attribute_container.py
--rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/__init__.py
--rw-r--r--   0        0        0     3718 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/annotation.py
--rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/annotation_container.py
--rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/audio_buffer.py
--rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/document.py
--rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/operation.py
--rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/span.py
--rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/collection.py
--rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/conversion.py
--rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/data_item.py
--rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/dict_conv.py
--rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/doc_pipeline.py
--rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/document.py
--rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/id.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/operation.py
--rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/operation_desc.py
--rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/pipeline.py
--rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/prov_store.py
--rw-r--r--   0        0        0    10886 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/prov_tracer.py
--rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/store.py
--rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/__init__.py
--rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.6.0/medkit/core/text/annotation.py
--rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/annotation_container.py
--rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/document.py
--rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/entity_attribute_container.py
--rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/core/text/entity_norm_attribute.py
--rw-r--r--   0        0        0     6471 2023-05-22 15:41:00.683311 medkit_lib-0.6.0/medkit/core/text/operation.py
--rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/span.py
--rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/span_utils.py
--rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/utils.py
--rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/utils.py
--rw-r--r--   0        0        0      401 2023-04-04 06:31:49.484372 medkit_lib-0.6.0/medkit/io/__init__.py
--rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/_brat_utils.py
--rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/io/brat.py
--rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/_common.py
--rw-r--r--   0        0        0     5506 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/audio.py
--rw-r--r--   0        0        0     5496 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/text.py
--rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/rttm.py
--rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/io/spacy.py
--rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/__init__.py
--rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/context/__init__.py
--rw-r--r--   0        0        0     9128 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/family_detector.py
--rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/context/family_detector_default_rules.yml
--rw-r--r--   0        0        0    14243 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector.py
--rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_rules.yml
--rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_verbs.yml
--rw-r--r--   0        0        0     9134 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/negation_detector.py
--rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/negation_detector_default_rules.yml
--rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/metrics/__init__.py
--rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/metrics/ner.py
--rw-r--r--   0        0        0     1320 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/__init__.py
--rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/adicap_norm_attribute.py
--rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/date_attribute.py
--rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/ner/duckling_matcher.py
--rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher.py
--rw-r--r--   0        0        0     8175 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher_trainable.py
--rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/ner/hf_tokenization_utils.py
--rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.6.0/medkit/text/ner/iamsystem_matcher.py
--rw-r--r--   0        0        0    13006 2023-05-05 09:01:47.817716 medkit_lib-0.6.0/medkit/text/ner/quick_umls_matcher.py
--rw-r--r--   0        0        0    12788 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/ner/regexp_matcher.py
--rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/regexp_matcher_default_rules.yml
--rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/tnm_attribute.py
--rw-r--r--   0        0        0    17079 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/ner/umls_coder_normalizer.py
--rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/umls_norm_attribute.py
--rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/umls_semgroups_v04.txt
--rw-r--r--   0        0        0     4365 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/umls_utils.py
--rw-r--r--   0        0        0       89 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/postprocessing/__init__.py
--rw-r--r--   0        0        0     3302 2023-05-23 14:37:42.938717 medkit_lib-0.6.0/medkit/text/postprocessing/attribute_duplicator.py
--rw-r--r--   0        0        0     2953 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/__init__.py
--rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/eds_cleaner.py
--rw-r--r--   0        0        0     3157 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/normalizer.py
--rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.6.0/medkit/text/relations/__init__.py
--rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/relations/syntactic_relation_extractor.py
--rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.6.0/medkit/text/segmentation/__init__.py
--rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/segmentation/default_section_definition.yml
--rw-r--r--   0        0        0      629 2023-05-05 09:23:06.369871 medkit_lib-0.6.0/medkit/text/segmentation/default_syntagma_definition.yml
--rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer.py
--rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
--rw-r--r--   0        0        0     8836 2023-05-15 07:18:23.883719 medkit_lib-0.6.0/medkit/text/segmentation/section_tokenizer.py
--rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.6.0/medkit/text/segmentation/sentence_tokenizer.py
--rw-r--r--   0        0        0     5798 2023-05-15 07:18:23.883719 medkit_lib-0.6.0/medkit/text/segmentation/syntagma_tokenizer.py
--rw-r--r--   0        0        0     1821 2023-05-05 09:23:06.377871 medkit_lib-0.6.0/medkit/text/segmentation/tokenizer_utils.py
--rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/spacy/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/spacy/displacy_utils.py
--rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/doc_pipeline.py
--rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/edsnlp.py
--rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/pipeline.py
--rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/spacy_utils.py
--rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.6.0/medkit/text/translation/__init__.py
--rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/translation/hf_translator.py
--rw-r--r--   0        0        0      204 2023-04-04 06:31:49.552376 medkit_lib-0.6.0/medkit/tools/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/tools/hf_utils.py
--rw-r--r--   0        0        0     5443 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/tools/save_prov_to_dot.py
--rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/training/__init__.py
--rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/callbacks.py
--rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.6.0/medkit/training/trainable_component.py
--rw-r--r--   0        0        0    11628 2023-05-23 14:37:42.938717 medkit_lib-0.6.0/medkit/training/trainer.py
--rw-r--r--   0        0        0      755 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/trainer_config.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/utils.py
--rw-r--r--   0        0        0     3875 2023-05-24 10:16:38.055392 medkit_lib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 medkit_lib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1087 2023-06-19 15:44:01.756861 medkit_lib-0.7.0/README.md
+-rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.7.0/medkit/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.7.0/medkit/audio/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/preprocessing/downmixer.py
+-rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/preprocessing/power_normalizer.py
+-rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/preprocessing/resampler.py
+-rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.7.0/medkit/audio/segmentation/__init__.py
+-rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/segmentation/pa_speaker_detector.py
+-rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/segmentation/webrtc_voice_detector.py
+-rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.7.0/medkit/audio/transcription/__init__.py
+-rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/transcription/doc_transcriber.py
+-rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/audio/transcription/hf_transcriber_function.py
+-rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/audio/transcription/sb_transcriber_function.py
+-rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/audio/transcription/transcribed_document.py
+-rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/__init__.py
+-rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.7.0/medkit/core/_prov_graph.py
+-rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/annotation.py
+-rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.7.0/medkit/core/annotation_container.py
+-rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/core/attribute.py
+-rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.7.0/medkit/core/attribute_container.py
+-rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/__init__.py
+-rw-r--r--   0        0        0     3712 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/core/audio/annotation.py
+-rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/annotation_container.py
+-rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/audio_buffer.py
+-rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/document.py
+-rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/operation.py
+-rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/span.py
+-rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/collection.py
+-rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/conversion.py
+-rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/data_item.py
+-rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/dict_conv.py
+-rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/doc_pipeline.py
+-rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/document.py
+-rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/id.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/operation.py
+-rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/operation_desc.py
+-rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/pipeline.py
+-rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/prov_store.py
+-rw-r--r--   0        0        0    10886 2023-06-23 09:52:38.445241 medkit_lib-0.7.0/medkit/core/prov_tracer.py
+-rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/store.py
+-rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/__init__.py
+-rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.7.0/medkit/core/text/annotation.py
+-rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/annotation_container.py
+-rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/document.py
+-rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/entity_attribute_container.py
+-rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/core/text/entity_norm_attribute.py
+-rw-r--r--   0        0        0     6471 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/core/text/operation.py
+-rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/span.py
+-rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/span_utils.py
+-rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/utils.py
+-rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/utils.py
+-rw-r--r--   0        0        0      401 2023-06-23 09:29:59.689283 medkit_lib-0.7.0/medkit/io/__init__.py
+-rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/_brat_utils.py
+-rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/io/brat.py
+-rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/medkit_json/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/medkit_json/_common.py
+-rw-r--r--   0        0        0     6302 2023-06-22 10:48:53.614279 medkit_lib-0.7.0/medkit/io/medkit_json/audio.py
+-rw-r--r--   0        0        0     6292 2023-06-22 10:48:53.614279 medkit_lib-0.7.0/medkit/io/medkit_json/text.py
+-rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/rttm.py
+-rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/io/spacy.py
+-rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/context/__init__.py
+-rw-r--r--   0        0        0     9607 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/family_detector.py
+-rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/context/family_detector_default_rules.yml
+-rw-r--r--   0        0        0    14243 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector.py
+-rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_rules.yml
+-rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_verbs.yml
+-rw-r--r--   0        0        0     9134 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/negation_detector.py
+-rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/negation_detector_default_rules.yml
+-rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/metrics/__init__.py
+-rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/metrics/ner.py
+-rw-r--r--   0        0        0     1320 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/adicap_norm_attribute.py
+-rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/date_attribute.py
+-rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.7.0/medkit/text/ner/duckling_matcher.py
+-rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher.py
+-rw-r--r--   0        0        0     8175 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher_trainable.py
+-rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/ner/hf_tokenization_utils.py
+-rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.7.0/medkit/text/ner/iamsystem_matcher.py
+-rw-r--r--   0        0        0    13006 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/quick_umls_matcher.py
+-rw-r--r--   0        0        0    12788 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/ner/regexp_matcher.py
+-rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/ner/regexp_matcher_default_rules.yml
+-rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/tnm_attribute.py
+-rw-r--r--   0        0        0    17079 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/umls_coder_normalizer.py
+-rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/umls_norm_attribute.py
+-rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/ner/umls_semgroups_v04.txt
+-rw-r--r--   0        0        0     4365 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/umls_utils.py
+-rw-r--r--   0        0        0      169 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/alignment_utils.py
+-rw-r--r--   0        0        0     2212 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/attribute_duplicator.py
+-rw-r--r--   0        0        0      639 2023-06-19 16:04:31.641932 medkit_lib-0.7.0/medkit/text/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/char_replacer.py
+-rw-r--r--   0        0        0     2374 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/char_rules.py
+-rw-r--r--   0        0        0    13519 2023-06-19 16:04:31.641932 medkit_lib-0.7.0/medkit/text/preprocessing/duplicate_finder.py
+-rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/preprocessing/eds_cleaner.py
+-rw-r--r--   0        0        0     3199 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/normalizer.py
+-rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.7.0/medkit/text/relations/__init__.py
+-rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/relations/syntactic_relation_extractor.py
+-rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.7.0/medkit/text/segmentation/__init__.py
+-rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/segmentation/default_section_definition.yml
+-rw-r--r--   0        0        0      629 2023-05-05 09:23:06.369871 medkit_lib-0.7.0/medkit/text/segmentation/default_syntagma_definition.yml
+-rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer.py
+-rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
+-rw-r--r--   0        0        0     8836 2023-05-15 07:18:23.883719 medkit_lib-0.7.0/medkit/text/segmentation/section_tokenizer.py
+-rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.7.0/medkit/text/segmentation/sentence_tokenizer.py
+-rw-r--r--   0        0        0     5798 2023-05-15 07:18:23.883719 medkit_lib-0.7.0/medkit/text/segmentation/syntagma_tokenizer.py
+-rw-r--r--   0        0        0     1821 2023-05-05 09:23:06.377871 medkit_lib-0.7.0/medkit/text/segmentation/tokenizer_utils.py
+-rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/spacy/__init__.py
+-rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/spacy/displacy_utils.py
+-rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/doc_pipeline.py
+-rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/edsnlp.py
+-rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/pipeline.py
+-rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/spacy_utils.py
+-rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.7.0/medkit/text/translation/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/translation/hf_translator.py
+-rw-r--r--   0        0        0      205 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/tools/__init__.py
+-rw-r--r--   0        0        0     5450 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/tools/_save_prov_to_dot.py
+-rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/tools/hf_utils.py
+-rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/training/__init__.py
+-rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.7.0/medkit/training/callbacks.py
+-rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.7.0/medkit/training/trainable_component.py
+-rw-r--r--   0        0        0    11628 2023-05-23 14:37:42.938717 medkit_lib-0.7.0/medkit/training/trainer.py
+-rw-r--r--   0        0        0     1998 2023-06-02 09:06:36.988920 medkit_lib-0.7.0/medkit/training/trainer_config.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.7.0/medkit/training/utils.py
+-rw-r--r--   0        0        0     3895 2023-06-26 15:42:53.840424 medkit_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 medkit_lib-0.7.0/PKG-INFO
```

### Comparing `medkit_lib-0.6.0/LICENSE` & `medkit_lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/README.md` & `medkit_lib-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This python library aims at:
 * (1) facilitating the manipulation of healthcare data of various modalities (e.g., structured, text, audio data) for the extraction of relevant features and
 * (2) developing supervised models from these various modalities for decision support in healthcare. 
 
 ## Getting started
 
-To get started with medkit, follow the installation instructions described in our [documentation website](https://heka.gitlabpages.inria.fr/medkit/index.html).
+To get started with medkit, follow the installation instructions described in our [documentation website](https://medkit.readthedocs.io/en/latest/).
 This website also contains tutorials and examples that you can use for starting with medkit. 
 
 ## Contributing
 
 We're still working for stabilizing source code and completing documentation, so that we'll be able to open it soon 
 
 However, we would already be happy to get your inputs !
```

### Comparing `medkit_lib-0.6.0/medkit/audio/preprocessing/downmixer.py` & `medkit_lib-0.7.0/medkit/audio/preprocessing/downmixer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/preprocessing/power_normalizer.py` & `medkit_lib-0.7.0/medkit/audio/preprocessing/power_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/preprocessing/resampler.py` & `medkit_lib-0.7.0/medkit/audio/preprocessing/resampler.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/segmentation/pa_speaker_detector.py` & `medkit_lib-0.7.0/medkit/audio/segmentation/pa_speaker_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/segmentation/webrtc_voice_detector.py` & `medkit_lib-0.7.0/medkit/audio/segmentation/webrtc_voice_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/transcription/__init__.py` & `medkit_lib-0.7.0/medkit/audio/transcription/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/transcription/doc_transcriber.py` & `medkit_lib-0.7.0/medkit/audio/transcription/doc_transcriber.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/transcription/hf_transcriber_function.py` & `medkit_lib-0.7.0/medkit/audio/transcription/hf_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/transcription/sb_transcriber_function.py` & `medkit_lib-0.7.0/medkit/audio/transcription/sb_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/audio/transcription/transcribed_document.py` & `medkit_lib-0.7.0/medkit/audio/transcription/transcribed_document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/__init__.py` & `medkit_lib-0.7.0/medkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/_prov_graph.py` & `medkit_lib-0.7.0/medkit/core/_prov_graph.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/annotation.py` & `medkit_lib-0.7.0/medkit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/annotation_container.py` & `medkit_lib-0.7.0/medkit/core/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/attribute.py` & `medkit_lib-0.7.0/medkit/core/attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/attribute_container.py` & `medkit_lib-0.7.0/medkit/core/attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/__init__.py` & `medkit_lib-0.7.0/medkit/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/annotation.py` & `medkit_lib-0.7.0/medkit/core/audio/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     PlaceholderAudioBuffer,
 )
 from medkit.core.id import generate_id
 
 
 @dataclasses.dataclass(init=False)
 class Segment(dict_conv.SubclassMapping):
-    """Audio segment referencing part of an {class}`~medkit.core.audio.AudioDocument`.
+    """Audio segment referencing part of an :class:`~.core.audio.AudioDocument`.
 
     Attributes
     ----------
     uid:
         Unique identifier of the segment.
     label:
         Label of the segment.
```

### Comparing `medkit_lib-0.6.0/medkit/core/audio/annotation_container.py` & `medkit_lib-0.7.0/medkit/core/audio/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/audio_buffer.py` & `medkit_lib-0.7.0/medkit/core/audio/audio_buffer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/document.py` & `medkit_lib-0.7.0/medkit/core/audio/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/operation.py` & `medkit_lib-0.7.0/medkit/core/audio/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/audio/span.py` & `medkit_lib-0.7.0/medkit/core/audio/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/collection.py` & `medkit_lib-0.7.0/medkit/core/collection.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/conversion.py` & `medkit_lib-0.7.0/medkit/core/conversion.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/dict_conv.py` & `medkit_lib-0.7.0/medkit/core/dict_conv.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/doc_pipeline.py` & `medkit_lib-0.7.0/medkit/core/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/document.py` & `medkit_lib-0.7.0/medkit/core/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/operation.py` & `medkit_lib-0.7.0/medkit/core/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/operation_desc.py` & `medkit_lib-0.7.0/medkit/core/operation_desc.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/pipeline.py` & `medkit_lib-0.7.0/medkit/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/prov_store.py` & `medkit_lib-0.7.0/medkit/core/prov_store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/prov_tracer.py` & `medkit_lib-0.7.0/medkit/core/prov_tracer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/store.py` & `medkit_lib-0.7.0/medkit/core/store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/__init__.py` & `medkit_lib-0.7.0/medkit/core/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/annotation.py` & `medkit_lib-0.7.0/medkit/core/text/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/annotation_container.py` & `medkit_lib-0.7.0/medkit/core/text/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/document.py` & `medkit_lib-0.7.0/medkit/core/text/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/entity_attribute_container.py` & `medkit_lib-0.7.0/medkit/core/text/entity_attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/entity_norm_attribute.py` & `medkit_lib-0.7.0/medkit/core/text/entity_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/operation.py` & `medkit_lib-0.7.0/medkit/core/text/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/span.py` & `medkit_lib-0.7.0/medkit/core/text/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/span_utils.py` & `medkit_lib-0.7.0/medkit/core/text/span_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/text/utils.py` & `medkit_lib-0.7.0/medkit/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/core/utils.py` & `medkit_lib-0.7.0/medkit/core/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/_brat_utils.py` & `medkit_lib-0.7.0/medkit/io/_brat_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/brat.py` & `medkit_lib-0.7.0/medkit/io/brat.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/medkit_json/__init__.py` & `medkit_lib-0.7.0/medkit/io/medkit_json/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/medkit_json/_common.py` & `medkit_lib-0.7.0/medkit/io/medkit_json/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/medkit_json/text.py` & `medkit_lib-0.7.0/medkit/io/medkit_json/audio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,227 @@
 __all__ = [
-    "load_text_document",
-    "load_text_documents",
-    "load_text_anns",
-    "save_text_document",
-    "save_text_documents",
-    "save_text_anns",
+    "load_audio_document",
+    "load_audio_documents",
+    "load_audio_anns",
+    "save_audio_document",
+    "save_audio_documents",
+    "save_audio_anns",
 ]
 
 import json
 from pathlib import Path
 from typing import Iterable, Iterator, Optional, Union
 import warnings
 
-from medkit.core.text import TextDocument, TextAnnotation
+from medkit.core.audio import AudioDocument, Segment
 from medkit.io.medkit_json._common import ContentType, build_header, check_header
 
 
 _DOC_ANNS_SUFFIX = "_anns.jsonl"
 
 
-def load_text_document(
+def load_audio_document(
     input_file: Union[str, Path],
     anns_input_file: Optional[Union[str, Path]] = None,
-) -> TextDocument:
+    encoding: Optional[str] = "utf-8",
+) -> AudioDocument:
     """
-    Load a text document from a medkit-json file generated with
-    :func:`~medkit.io.medkit_json.save_text_document`.
+    Load an audio document from a medkit-json file generated with
+    :func:`~medkit.io.medkit_json.save_audio_document`
 
     Parameters
     ----------
     input_file:
         Path to the medkit-json file containing the document
     anns_input_file:
         Optional medkit-json file containing separate annotations of the
         document.
+    encoding:
+        Optional encoding of `input_file` and `anns_input_file`
 
     Returns
     -------
-    TextDocument
-        The text document in the file
+    AudioDocument
+        The audio document in the file
     """
 
     input_file = Path(input_file)
 
-    with open(input_file) as fp:
+    with open(input_file, encoding=encoding) as fp:
         data = json.load(fp)
-    check_header(data, ContentType.TEXT_DOCUMENT)
-    doc = TextDocument.from_dict(data["content"])
+    check_header(data, ContentType.AUDIO_DOCUMENT)
+    doc = AudioDocument.from_dict(data["content"])
 
     if anns_input_file is not None:
-        for ann in load_text_anns(anns_input_file):
+        for ann in load_audio_anns(anns_input_file, encoding=encoding):
             doc.anns.add(ann)
 
     return doc
 
 
-def load_text_documents(input_file: Union[str, Path]) -> Iterator[TextDocument]:
+def load_audio_documents(
+    input_file: Union[str, Path], encoding: Optional[str] = "utf-8"
+) -> Iterator[AudioDocument]:
     """
-    Load text documents from a medkit-json file generated with
-    :func:`~medkit.io.medkit_json.save_text_documents`
+    Load audio documents from a medkit-json file generated with
+    :func:`~medkit.io.medkit_json.save_audio_documents`
 
     Parameters
     ----------
     input_file:
         Path to the medkit-json file containing the documents
+    encoding:
+        Optional encoding of `input_file`
 
     Returns
     -------
-    Iterator[TextDocument]
-        An iterator to the text documents in the file
+    Iterator[AudioDocument]
+        An iterator to the audio documents in the file
     """
 
     input_file = Path(input_file)
 
-    with open(input_file) as fp:
+    with open(input_file, encoding=encoding) as fp:
         line = fp.readline()
         data = json.loads(line)
-        check_header(data, ContentType.TEXT_DOCUMENT_LIST)
+        check_header(data, ContentType.AUDIO_DOCUMENT_LIST)
 
         for line in fp:
             doc_data = json.loads(line)
-            doc = TextDocument.from_dict(doc_data)
+            doc = AudioDocument.from_dict(doc_data)
             yield doc
 
 
-def load_text_anns(input_file: Union[str, Path]) -> Iterator[TextAnnotation]:
+def load_audio_anns(
+    input_file: Union[str, Path], encoding: Optional[str] = "utf-8"
+) -> Iterator[Segment]:
     """
-    Load text annotations from a medkit-json file generated with
+    Load audio annotations from a medkit-json file generated with
     :func:`~medkit.io.medkit_json.save_audio_anns`
 
     Parameters
     ----------
     input_file:
         Path to the medkit-json file containing the annotations
+    encoding:
+        Optional encoding of `input_file`
 
     Returns
     -------
-    Iterator[TextAnnotation]
-        An iterator to the text annotations in the file
+    Iterator[Segment]
+        An iterator to the audio annotations in the file
     """
 
     input_file = Path(input_file)
 
-    with open(input_file) as fp:
+    with open(input_file, encoding=encoding) as fp:
         line = fp.readline()
         data = json.loads(line)
-        check_header(data, ContentType.TEXT_ANNOTATION_LIST)
+        check_header(data, ContentType.AUDIO_ANNOTATION_LIST)
 
         for line in fp:
             ann_data = json.loads(line)
-            ann = TextAnnotation.from_dict(ann_data)
+            ann = Segment.from_dict(ann_data)
             yield ann
 
 
-def save_text_document(
-    doc: TextDocument,
+def save_audio_document(
+    doc: AudioDocument,
     output_file: Union[str, Path],
     split_anns: bool = False,
     anns_output_file: Optional[Union[str, Path]] = None,
+    encoding: Optional[str] = "utf-8",
 ):
     """
-    Save a text document into a medkit-json file.
+    Save an audio document into a medkit-json file.
 
     Parameters
     ----------
     doc:
-        The text document to save
+        The audio document to save
     output_file:
         Path of the generated medkit-json file
     split_anns:
         If True, the annotations will be saved in a separate medkit-json file
         instead of being included in the main document file
     anns_output_file:
         Path of the medkit-json file storing the annotations if `split_anns` is True.
         If not provided, `output_file` will be used with an extra "_anns" suffix.
+    encoding:
+        Optional encoding of `output_file` and `anns_output_file`
     """
 
     output_file = Path(output_file)
     anns_output_file = Path(anns_output_file) if anns_output_file is not None else None
 
     if not split_anns and anns_output_file is not None:
         warnings.warn(
             "anns_output_file provided but split_anns is False so it will not be used"
         )
 
-    data = build_header(content_type=ContentType.TEXT_DOCUMENT)
+    data = build_header(content_type=ContentType.AUDIO_DOCUMENT)
     data["content"] = doc.to_dict(with_anns=not split_anns)
-    with open(output_file, mode="w") as fp:
+    with open(output_file, mode="w", encoding=encoding) as fp:
         json.dump(data, fp, indent=4)
 
     if split_anns:
         if anns_output_file is None:
             anns_output_file = output_file.with_suffix(_DOC_ANNS_SUFFIX)
-        save_text_anns(doc.anns, anns_output_file)
+        save_audio_anns(doc.anns, anns_output_file, encoding=encoding)
 
 
-def save_text_documents(docs: Iterable[TextDocument], output_file: Union[str, Path]):
+def save_audio_documents(
+    docs: Iterable[AudioDocument],
+    output_file: Union[str, Path],
+    encoding: Optional[str] = "utf-8",
+):
     """
-    Save text documents into a medkit-json file.
+    Save audio documents into a medkit-json file.
 
     Parameters
     ----------
     docs:
-        The text documents to save
+        The audio documents to save
     output_file:
         Path of the generated medkit-json file
+    encoding:
+        Optional encoding of `output_file`
     """
 
     output_file = Path(output_file)
 
-    header = build_header(content_type=ContentType.TEXT_DOCUMENT_LIST)
-    with open(output_file, mode="w") as fp:
+    header = build_header(content_type=ContentType.AUDIO_DOCUMENT_LIST)
+    with open(output_file, mode="w", encoding=encoding) as fp:
         fp.write(json.dumps(header) + "\n")
 
         for doc in docs:
             doc_data = doc.to_dict()
             fp.write(json.dumps(doc_data) + "\n")
 
 
-def save_text_anns(anns: Iterable[TextAnnotation], output_file: Union[str, Path]):
+def save_audio_anns(
+    anns: Iterable[Segment],
+    output_file: Union[str, Path],
+    encoding: Optional[str] = "utf-8",
+):
     """
-    Save text annotations into a medkit-json file.
+    Save audio annotations into a medkit-json file.
 
     Parameters
     ----------
     docs:
-        The text annotations to save
+        The audio annotations to save
     output_file:
         Path of the generated medkit-json file
+    encoding:
+        Optional encoding of `output_file`
     """
 
     output_file = Path(output_file)
 
-    header = build_header(content_type=ContentType.TEXT_ANNOTATION_LIST)
-    with open(output_file, mode="w") as fp:
+    header = build_header(content_type=ContentType.AUDIO_ANNOTATION_LIST)
+    with open(output_file, mode="w", encoding=encoding) as fp:
         fp.write(json.dumps(header) + "\n")
 
         for ann in anns:
             ann_data = ann.to_dict()
             fp.write(json.dumps(ann_data) + "\n")
```

### Comparing `medkit_lib-0.6.0/medkit/io/rttm.py` & `medkit_lib-0.7.0/medkit/io/rttm.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/io/spacy.py` & `medkit_lib-0.7.0/medkit/io/spacy.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/__init__.py` & `medkit_lib-0.7.0/medkit/text/context/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/family_detector.py` & `medkit_lib-0.7.0/medkit/text/context/family_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,23 @@
 
     For detecting family references, the module uses rules that may be sensitive to unicode or
     not. When the rule is not sensitive to unicode, we try to convert unicode chars to
     the closest ascii chars. However, some characters need to be pre-processed before
     (e.g., `n°` -> `number`). So, if the text lengths are different, we fall back on
     initial unicode text for detection even if rule is not unicode-sensitive.
     In this case, a warning is logged for recommending to pre-process data.
+
+    Note that for better results, family detection should be run at the sentence
+    level (ie on sentence segments) rather than at the syntagma level [1].
+
+    [1] N. Garcelon, A. Neuraz, V. Benoit, R. Salomon, A. Burgun, "Improving a
+    full-text search engine: the importance of negation detection and family
+    history context to identify cases in a biomedical data warehouse", Journal
+    of the American Medical Informatics Association, Volume 24, Issue 3, May
+    2017
     """
 
     def __init__(
         self,
         output_label: str,
         rules: Optional[List[FamilyDetectorRule]] = None,
         uid: Optional[str] = None,
```

### Comparing `medkit_lib-0.6.0/medkit/text/context/family_detector_default_rules.yml` & `medkit_lib-0.7.0/medkit/text/context/family_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector.py` & `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_rules.yml` & `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_verbs.yml` & `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_verbs.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/negation_detector.py` & `medkit_lib-0.7.0/medkit/text/context/negation_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/context/negation_detector_default_rules.yml` & `medkit_lib-0.7.0/medkit/text/context/negation_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/metrics/ner.py` & `medkit_lib-0.7.0/medkit/text/metrics/ner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/__init__.py` & `medkit_lib-0.7.0/medkit/text/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/adicap_norm_attribute.py` & `medkit_lib-0.7.0/medkit/text/ner/adicap_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/date_attribute.py` & `medkit_lib-0.7.0/medkit/text/ner/date_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/duckling_matcher.py` & `medkit_lib-0.7.0/medkit/text/ner/duckling_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher.py` & `medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher_trainable.py` & `medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher_trainable.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/hf_tokenization_utils.py` & `medkit_lib-0.7.0/medkit/text/ner/hf_tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/iamsystem_matcher.py` & `medkit_lib-0.7.0/medkit/text/ner/iamsystem_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/quick_umls_matcher.py` & `medkit_lib-0.7.0/medkit/text/ner/quick_umls_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/regexp_matcher.py` & `medkit_lib-0.7.0/medkit/text/ner/regexp_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/regexp_matcher_default_rules.yml` & `medkit_lib-0.7.0/medkit/text/ner/regexp_matcher_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/tnm_attribute.py` & `medkit_lib-0.7.0/medkit/text/ner/tnm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/umls_coder_normalizer.py` & `medkit_lib-0.7.0/medkit/text/ner/umls_coder_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/umls_norm_attribute.py` & `medkit_lib-0.7.0/medkit/text/ner/umls_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/umls_semgroups_v04.txt` & `medkit_lib-0.7.0/medkit/text/ner/umls_semgroups_v04.txt`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/ner/umls_utils.py` & `medkit_lib-0.7.0/medkit/text/ner/umls_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/postprocessing/attribute_duplicator.py` & `medkit_lib-0.7.0/medkit/text/postprocessing/attribute_duplicator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __all__ = ["AttributeDuplicator"]
 
-from typing import List, Optional, Tuple
-from intervaltree import IntervalTree
+from typing import List, Optional
 from medkit.core import Attribute, Operation
-from medkit.core.text import Segment, span_utils
+from medkit.core.text import Segment
+
+from medkit.text.postprocessing import alignment_utils
 
 
 class AttributeDuplicator(Operation):
     """Annotator to copy attributes from a source segment to its nested segments.
     For each attribute to be duplicated, a new attribute is created in the nested segment
     """
 
@@ -38,60 +39,30 @@
         Parameters
         ----------
         source_segments:
             List of segments with attributes to copy
         target_segments:
             List of segments target
         """
-        nested = self._compute_nested_segments(source_segments, target_segments)
+        nested = alignment_utils.compute_nested_segments(
+            source_segments, target_segments
+        )
 
         for parent, children in nested:
             attrs_to_copy = [
                 attr
                 for label in self.attr_labels
                 for attr in parent.attrs.get(label=label)
             ]
 
             # create a new attr in target from the source attr
             for attr in attrs_to_copy:
                 for child in children:
                     self._duplicate_attr(attr=attr, target=child)
 
-    def _compute_nested_segments(
-        self, source_segments: List[Segment], target_segments: List[Segment]
-    ) -> List[Tuple[Segment, List[Segment]]]:
-        tree = IntervalTree()
-        for segment in target_segments:
-            normalized_spans = span_utils.normalize_spans(segment.spans)
-
-            if not normalized_spans:
-                continue
-
-            tree.addi(
-                normalized_spans[0].start,
-                normalized_spans[-1].end,
-                data=segment,
-            )
-        return self._find_nested(tree, source_segments)
-
-    def _find_nested(
-        self, tree: IntervalTree, source_segments: List[Segment]
-    ) -> List[Tuple[Segment, List[Segment]]]:
-        nested = []
-        for parent in source_segments:
-            normalized_spans = span_utils.normalize_spans(parent.spans)
-
-            if not normalized_spans:
-                continue
-
-            start, end = normalized_spans[0].start, normalized_spans[-1].end
-            children = [child.data for child in tree.overlap(start, end)]
-            nested.append((parent, children))
-        return nested
-
     def _duplicate_attr(self, attr: Attribute, target: Segment):
         target_attr = attr.copy()
         target.attrs.add(target_attr)
 
         if self._prov_tracer is not None:
             self._prov_tracer.add_prov(
                 target_attr, self.description, source_data_items=[attr]
```

### Comparing `medkit_lib-0.6.0/medkit/text/preprocessing/__init__.py` & `medkit_lib-0.7.0/medkit/text/preprocessing/char_rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,108 @@
 __all__ = [
-    "Normalizer",
-    "NormalizerRule",
+    "ALL_CHAR_RULES",
     "LIGATURE_RULES",
     "FRACTION_RULES",
     "SIGN_RULES",
     "SPACE_RULES",
-    "EDSCleaner",
+    "DOT_RULES",
+    "QUOTATION_RULES",
 ]
 
-from .normalizer import Normalizer, NormalizerRule
-from .eds_cleaner import EDSCleaner
-
-#: Normalizer rules for ligatures
+#: Rules for ligatures
 LIGATURE_RULES = [
-    NormalizerRule(*rule)
-    for rule in [
-        ("\u00c6", "AE"),
-        ("\u00E6", "ae"),
-        ("\u0152", "OE"),
-        ("\u0153", "oe"),
-    ]
+    ("\u00c6", "AE"),
+    ("\u00E6", "ae"),
+    ("\u0152", "OE"),
+    ("\u0153", "oe"),
 ]
-#: Normalizer rules for fraction characters
+#: Rules for fraction characters
 FRACTION_RULES = [
-    NormalizerRule(*rule)
-    for rule in [
-        ("\u00BC", "1/4"),
-        ("\u00BD", "1/2"),
-        ("\u00BE", "3/4"),
-        ("\u2150", "1/7"),
-        ("\u2151", "1/9"),
-        ("\u2152", "1/10"),
-        ("\u2153", "1/3"),
-        ("\u2154", "2/3"),
-        ("\u2155", "1/5"),
-        ("\u2156", "2/5"),
-        ("\u2157", "3/5"),
-        ("\u2158", "4/5"),
-        ("\u2159", "1/6"),
-        ("\u215A", "5/6"),
-        ("\u215B", "1/8"),
-        ("\u215C", "3/8"),
-        ("\u215D", "5/8"),
-        ("\u215E", "7/8"),
-        ("\u2189", "0/3"),
-    ]
+    ("\u00BC", "1/4"),
+    ("\u00BD", "1/2"),
+    ("\u00BE", "3/4"),
+    ("\u2150", "1/7"),
+    ("\u2151", "1/9"),
+    ("\u2152", "1/10"),
+    ("\u2153", "1/3"),
+    ("\u2154", "2/3"),
+    ("\u2155", "1/5"),
+    ("\u2156", "2/5"),
+    ("\u2157", "3/5"),
+    ("\u2158", "4/5"),
+    ("\u2159", "1/6"),
+    ("\u215A", "5/6"),
+    ("\u215B", "1/8"),
+    ("\u215C", "3/8"),
+    ("\u215D", "5/8"),
+    ("\u215E", "7/8"),
+    ("\u2189", "0/3"),
 ]
-#: Normalizer rules for non-standard spaces
+#: Rules for non-standard spaces
 SPACE_RULES = [
-    NormalizerRule(*rule)
-    for rule in [
-        ("\u00A0", " "),
-        ("\u1680", " "),
-        ("\u2002", " "),
-        ("\u2003", " "),
-        ("\u2004", " "),
-        ("\u2005", " "),
-        ("\u2006", " "),
-        ("\u2007", " "),
-        ("\u2008", " "),
-        ("\u2009", " "),
-        ("\u200A", " "),
-        ("\u200B", " "),
-        ("\u202F", " "),
-        ("\u205F", " "),
-        ("\u2420", " "),
-        ("\u3000", " "),
-        ("\u303F", " "),
-        ("\uFEFF", " "),
-        ("\u1DA7F", " "),
-        ("\u1DA80", " "),
-        ("\uE0020", " "),
-    ]
+    ("\u00A0", " "),
+    ("\u1680", " "),
+    ("\u2002", " "),
+    ("\u2003", " "),
+    ("\u2004", " "),
+    ("\u2005", " "),
+    ("\u2006", " "),
+    ("\u2007", " "),
+    ("\u2008", " "),
+    ("\u2009", " "),
+    ("\u200A", " "),
+    ("\u200B", " "),
+    ("\u202F", " "),
+    ("\u205F", " "),
+    ("\u2420", " "),
+    ("\u3000", " "),
+    ("\u303F", " "),
+    ("\uFEFF", " "),
 ]
 
-#: Normalizer rules for sign chars
+#: Rules for sign chars
 SIGN_RULES = [
-    NormalizerRule(*rule)
-    for rule in [
-        ("\u00A9", ""),  # copyright
-        ("\u00AE", ""),  # registered
-        ("\u2122", ""),  # trade
-    ]
+    ("\u00A9", ""),  # copyright
+    ("\u00AE", ""),  # registered
+    ("\u2122", ""),  # trade
 ]
 
-#: Normalizer rules for dot chars
+#: Rules for dot chars
 DOT_RULES = [
-    NormalizerRule(*rule)
-    for rule in [("\u2026", "..."), ("\u22EF", "...")]  # horizontal ellipsis
+    # horizontal ellipsis
+    ("\u2026", "..."),
+    ("\u22EF", "..."),
 ]
 
-#: Normalizer quotation marks
-# replace double and single quotation marks
+#: Normalizer quotation marks: replace double and single quotation marks
 QUOTATION_RULES = [
-    NormalizerRule(*rule)
-    for rule in [
-        ("»", '"'),  # normalize double quotation marks
-        ("«", '"'),  # replace double quotation marks
-        ("\u201C", '"'),
-        ("\u201D", '"'),
-        ("\u201E", '"'),
-        ("\u201F", '"'),
-        ("\u2039", '"'),
-        ("\u203A", '"'),
-        ("\u02F5", '"'),
-        ("\u02F6", '"'),
-        ("\u02DD", '"'),
-        ("\uFF02", '"'),
-        ("\u201A", ""),  # single low quotation (remove)
-        ("\u2018", "'"),  # left side single quotation
-        ("\u2019", "'"),  # right side single quotation
-        ("\u201B", "'"),  # single high reverse quotation
-        ("\u02CA", "'"),  # grave accent
-        ("\u0060", "'"),
-        ("\u02CB", "'"),  # acute accent
-        ("\u00B4", "'"),
-    ]
+    ("»", '"'),  # normalize double quotation marks
+    ("«", '"'),  # replace double quotation marks
+    ("\u201C", '"'),
+    ("\u201D", '"'),
+    ("\u201E", '"'),
+    ("\u201F", '"'),
+    ("\u2039", '"'),
+    ("\u203A", '"'),
+    ("\u02F5", '"'),
+    ("\u02F6", '"'),
+    ("\u02DD", '"'),
+    ("\uFF02", '"'),
+    ("\u201A", ""),  # single low quotation (remove)
+    ("\u2018", "'"),  # left side single quotation
+    ("\u2019", "'"),  # right side single quotation
+    ("\u201B", "'"),  # single high reverse quotation
+    ("\u02CA", "'"),  # grave accent
+    ("\u0060", "'"),
+    ("\u02CB", "'"),  # acute accent
+    ("\u00B4", "'"),
 ]
+
+#: All pre-defined rules for CharReplacer
+ALL_CHAR_RULES = (
+    DOT_RULES
+    + FRACTION_RULES
+    + LIGATURE_RULES
+    + QUOTATION_RULES
+    + SIGN_RULES
+    + SPACE_RULES
+)
```

### Comparing `medkit_lib-0.6.0/medkit/text/preprocessing/eds_cleaner.py` & `medkit_lib-0.7.0/medkit/text/preprocessing/eds_cleaner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/preprocessing/normalizer.py` & `medkit_lib-0.7.0/medkit/text/preprocessing/normalizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __all__ = ["Normalizer", "NormalizerRule"]
 
 import re
-from typing import List, NamedTuple, Optional
+from typing import List, NamedTuple, Optional, Tuple
 
 from medkit.core.operation import Operation
 from medkit.core.text import Segment, span_utils
 
 
 class NormalizerRule(NamedTuple):
     pattern_to_replace: str
@@ -23,39 +23,39 @@
     It respects the span modification by creating a new text-bound annotation containing
     the span modification information from input text.
     """
 
     def __init__(
         self,
         output_label: str,
-        rules: List[NormalizerRule] = None,
+        rules: List[Tuple[str, str]] = None,
         name: Optional[str] = None,
         uid: Optional[str] = None,
     ):
         """
         Parameters
         ----------
         output_label
             The output label of the created annotations
         rules
-            The list of normalization rules
+            The list of replacement rules
         name:
             Name describing the pre-processing module (defaults to the class name)
         uid
             Identifier of the pre-processing module
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
 
         self.output_label = output_label
         if rules is None:
             rules = []
-        self.rules = rules
+        self.rules = [NormalizerRule(*rule) for rule in rules]
 
         regex_rules = ["(" + rule.pattern_to_replace + ")" for rule in self.rules]
         regex_rule = r"|".join(regex_rules)
 
         self._pattern = re.compile(regex_rule)
 
     def run(self, segments: List[Segment]) -> List[Segment]:
```

### Comparing `medkit_lib-0.6.0/medkit/text/relations/syntactic_relation_extractor.py` & `medkit_lib-0.7.0/medkit/text/relations/syntactic_relation_extractor.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/default_section_definition.yml` & `medkit_lib-0.7.0/medkit/text/segmentation/default_section_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/default_syntagma_definition.yml` & `medkit_lib-0.7.0/medkit/text/segmentation/default_syntagma_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer.py` & `medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv` & `medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/section_tokenizer.py` & `medkit_lib-0.7.0/medkit/text/segmentation/section_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/sentence_tokenizer.py` & `medkit_lib-0.7.0/medkit/text/segmentation/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/syntagma_tokenizer.py` & `medkit_lib-0.7.0/medkit/text/segmentation/syntagma_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/segmentation/tokenizer_utils.py` & `medkit_lib-0.7.0/medkit/text/segmentation/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/__init__.py` & `medkit_lib-0.7.0/medkit/text/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/displacy_utils.py` & `medkit_lib-0.7.0/medkit/text/spacy/displacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/doc_pipeline.py` & `medkit_lib-0.7.0/medkit/text/spacy/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/edsnlp.py` & `medkit_lib-0.7.0/medkit/text/spacy/edsnlp.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/pipeline.py` & `medkit_lib-0.7.0/medkit/text/spacy/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/spacy/spacy_utils.py` & `medkit_lib-0.7.0/medkit/text/spacy/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/text/translation/hf_translator.py` & `medkit_lib-0.7.0/medkit/text/translation/hf_translator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/tools/hf_utils.py` & `medkit_lib-0.7.0/medkit/tools/hf_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/tools/save_prov_to_dot.py` & `medkit_lib-0.7.0/medkit/tools/_save_prov_to_dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     prov_tracer: ProvTracer,
     file: Union[str, Path],
     data_item_formatters: Optional[Dict[Type, Callable[[Any], str]]] = None,
     op_formatter: Optional[Callable[[OperationDescription], str]] = None,
     max_sub_prov_depth: Optional[int] = None,
     show_attr_links: bool = True,
 ):
-    """Generate a graphviz-compatible .dot file from a `~medkit.core.ProvTracer`
-    for visualization.
+    """Generate a graphviz-compatible .dot file from a
+    :class:`~medkit.core.ProvTracer` for visualization.
 
     Parameters
     ----------
     prov_tracer:
         Provenance tracer holding the provenance information to save.
     file:
         Path to the .dot file.
```

### Comparing `medkit_lib-0.6.0/medkit/training/__init__.py` & `medkit_lib-0.7.0/medkit/training/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/training/callbacks.py` & `medkit_lib-0.7.0/medkit/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/training/trainable_component.py` & `medkit_lib-0.7.0/medkit/training/trainable_component.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/training/trainer.py` & `medkit_lib-0.7.0/medkit/training/trainer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/medkit/training/utils.py` & `medkit_lib-0.7.0/medkit/training/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.6.0/pyproject.toml` & `medkit_lib-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medkit-lib"
-version = "0.6.0"
+version = "0.7.0"
 description = "A Python library for a learning health system"
 readme = "README.md"
 repository = "https://gitlab.inria.fr/heka/medkit/"
 documentation = "https://heka.gitlabpages.inria.fr/medkit/"
 authors = ["HeKA Research Team"]
 maintainers = [
     "medkit-maintainers <medkit-maintainers@inria.fr>"
@@ -21,14 +21,15 @@
 ]
 packages = [
   { include = "medkit" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <4.0"
+duptextfinder = "*"
 flashtext = "*"
 numpy = "*"
 pyaml = "*"
 requests = "*"
 smart-open = "*"
 soundfile = "*"
 tqdm = "*"
```

### Comparing `medkit_lib-0.6.0/PKG-INFO` & `medkit_lib-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medkit-lib
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for a learning health system
 Home-page: https://gitlab.inria.fr/heka/medkit/
 License: MIT
 Author: HeKA Research Team
 Maintainer: medkit-maintainers
 Maintainer-email: medkit-maintainers@inria.fr
 Requires-Python: >=3.7.1,<4.0
@@ -34,14 +34,15 @@
 Provides-Extra: spacy
 Provides-Extra: syntactic-relation-extractor
 Provides-Extra: training
 Provides-Extra: umls-coder-normalizer
 Provides-Extra: webrtc-voice-detector
 Requires-Dist: PyRuSH (>=1.0,<2.0) ; extra == "rush-sentence-tokenizer" or extra == "optional"
 Requires-Dist: Unidecode
+Requires-Dist: duptextfinder
 Requires-Dist: edsnlp (>=0.7,<0.8) ; extra == "edsnlp"
 Requires-Dist: feather-format (>=0.4,<0.5) ; extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: flashtext
 Requires-Dist: iamsystem (>=0.3)
 Requires-Dist: intervaltree
 Requires-Dist: numpy
 Requires-Dist: packaging ; extra == "quick-umls" or extra == "optional"
@@ -76,15 +77,15 @@
 
 This python library aims at:
 * (1) facilitating the manipulation of healthcare data of various modalities (e.g., structured, text, audio data) for the extraction of relevant features and
 * (2) developing supervised models from these various modalities for decision support in healthcare. 
 
 ## Getting started
 
-To get started with medkit, follow the installation instructions described in our [documentation website](https://heka.gitlabpages.inria.fr/medkit/index.html).
+To get started with medkit, follow the installation instructions described in our [documentation website](https://medkit.readthedocs.io/en/latest/).
 This website also contains tutorials and examples that you can use for starting with medkit. 
 
 ## Contributing
 
 We're still working for stabilizing source code and completing documentation, so that we'll be able to open it soon 
 
 However, we would already be happy to get your inputs !
```

