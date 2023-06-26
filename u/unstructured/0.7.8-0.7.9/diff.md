# Comparing `tmp/unstructured-0.7.8.tar.gz` & `tmp/unstructured-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.8.tar", last modified: Fri Jun 23 02:24:47 2023, max compression
+gzip compressed data, was "unstructured-0.7.9.tar", last modified: Mon Jun 26 21:56:55 2023, max compression
```

## Comparing `unstructured-0.7.8.tar` & `unstructured-0.7.9.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-23 02:24:36.000000 unstructured-0.7.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 02:24:36.000000 unstructured-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-23 02:24:47.132688 unstructured-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-23 02:24:36.000000 unstructured-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-23 02:24:47.132688 unstructured-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-23 02:24:36.000000 unstructured-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25924 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-23 02:24:47.000000 unstructured-0.7.8/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-26 21:56:47.000000 unstructured-0.7.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-26 21:56:47.000000 unstructured-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-06-26 21:56:55.377841 unstructured-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-06-26 21:56:47.000000 unstructured-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.361840 unstructured-0.7.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-26 21:56:55.377841 unstructured-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-26 21:56:47.000000 unstructured-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.361840 unstructured-0.7.9/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26315 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.373841 unstructured-0.7.9/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.8/LICENSE.md` & `unstructured-0.7.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/PKG-INFO` & `unstructured-0.7.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.8
+Version: 0.7.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -34,14 +34,24 @@
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
         <h3 align="center">
+          <p>API Announcement!</p>
+        </h3>
+        
+        <p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
+          
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+        We'd love to hear your feedback, let us know how it goes in our
+          community slack. And stay tuned for improvements to both quality and performance!</p>
+        
+        <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
         users the building blocks they need to build pipelines targeted at the documents they care
         about. Bricks in the library fall into three categories:
@@ -99,14 +109,15 @@
         | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
         | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
         | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
+        | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -15,14 +15,21 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          **** API Announcement! ****
+While access to the hosted Unstructured API will remain free, API Keys will
+soon be required to make requests. To prevent any disruption, get yours here
+now and start using it today!
+Checkout the readme here to get started making API calls. We'd love to hear
+your feedback, let us know how it goes in our community slack. And stay tuned
+for improvements to both quality and performance!
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -60,15 +67,16 @@
 | None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
 (`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
+Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
```

### Comparing `unstructured-0.7.8/README.md` & `unstructured-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,24 @@
   </a>
   <a href="https://www.linkedin.com/company/unstructuredio/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </div>
 
 <h3 align="center">
+  <p>API Announcement!</p>
+</h3>
+
+<p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
+  
+<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+We'd love to hear your feedback, let us know how it goes in our
+  community slack. And stay tuned for improvements to both quality and performance!</p>
+
+<h3 align="center">
   <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
 </h3>
 
 The `unstructured` library provides open-source components for pre-processing text documents
 such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
 users the building blocks they need to build pipelines targeted at the documents they care
 about. Bricks in the library fall into three categories:
@@ -91,14 +101,15 @@
 | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
 | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
 | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
 | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
 | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
 | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
+| Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
 | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
 | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
 | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
 | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
```

#### html2text {}

```diff
@@ -11,14 +11,21 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          **** API Announcement! ****
+While access to the hosted Unstructured API will remain free, API Keys will
+soon be required to make requests. To prevent any disruption, get yours here
+now and start using it today!
+Checkout the readme here to get started making API calls. We'd love to hear
+your feedback, let us know how it goes in our community slack. And stay tuned
+for improvements to both quality and performance!
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -56,15 +63,16 @@
 | None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
 (`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
+Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
```

### Comparing `unstructured-0.7.8/setup.py` & `unstructured-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.9/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.9/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/test_unstructured/test_utils.py` & `unstructured-0.7.9/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/cleaners/core.py` & `unstructured-0.7.9/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/cleaners/extract.py` & `unstructured-0.7.9/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/cleaners/translate.py` & `unstructured-0.7.9/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/base.py` & `unstructured-0.7.9/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/coordinates.py` & `unstructured-0.7.9/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/elements.py` & `unstructured-0.7.9/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/email_elements.py` & `unstructured-0.7.9/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/html.py` & `unstructured-0.7.9/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/documents/xml.py` & `unstructured-0.7.9/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/file_utils/encoding.py` & `unstructured-0.7.9/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/file_utils/exploration.py` & `unstructured-0.7.9/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.9/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/file_utils/filetype.py` & `unstructured-0.7.9/unstructured/file_utils/filetype.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
     # Markup Types
     HTML = 50
     XML = 51
     MD = 52
     EPUB = 53
     RST = 54
+    ORG = 55
 
     # Compressed Types
     ZIP = 60
 
     # Open Office Types
     ODT = 70
 
@@ -113,14 +114,15 @@
     "application/x-csv": FileType.CSV,
     "text/comma-separated-values": FileType.CSV,
     "text/x-comma-separated-values": FileType.CSV,
     "text/csv": FileType.CSV,
     "text/tsv": FileType.TSV,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
+    "text/org": FileType.ORG,
     "text/x-rst": FileType.RST,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "application/json": FileType.JSON,
     "application/rtf": FileType.RTF,
     "text/rtf": FileType.RTF,
     "text/html": FileType.HTML,
@@ -157,14 +159,15 @@
     ".text": FileType.TXT,
     ".log": FileType.TXT,
     ".eml": FileType.EML,
     ".xml": FileType.XML,
     ".htm": FileType.HTML,
     ".html": FileType.HTML,
     ".md": FileType.MD,
+    ".org": FileType.ORG,
     ".rst": FileType.RST,
     ".xlsx": FileType.XLSX,
     ".pptx": FileType.PPTX,
     ".png": FileType.PNG,
     ".doc": FileType.DOC,
     ".zip": FileType.ZIP,
     ".xls": FileType.XLS,
@@ -285,15 +288,15 @@
 
         if _is_text_file_a_csv(file=file, filename=filename, encoding=encoding):
             return FileType.CSV
 
         if file and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
 
-        if extension in [".eml", ".md", ".rtf", ".html", ".rst", ".tsv", ".json"]:
+        if extension in [".eml", ".md", ".rtf", ".html", ".rst", ".org", ".tsv", ".json"]:
             return EXT_TO_FILETYPE.get(extension)
 
         # Safety catch
         if mime_type in STR_TO_FILETYPE:
             return STR_TO_FILETYPE[mime_type]
 
         return FileType.TXT
```

### Comparing `unstructured-0.7.8/unstructured/file_utils/metadata.py` & `unstructured-0.7.9/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/azure.py` & `unstructured-0.7.9/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.9/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/discord.py` & `unstructured-0.7.9/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.9/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/gcs.py` & `unstructured-0.7.9/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/git.py` & `unstructured-0.7.9/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/github.py` & `unstructured-0.7.9/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.9/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.9/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/local.py` & `unstructured-0.7.9/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.9/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/s3.py` & `unstructured-0.7.9/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/slack.py` & `unstructured-0.7.9/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.9/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.9/unstructured/ingest/doc_processor/generalized.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def initialize():
     """Download default model (avoids subprocesses all doing the same)"""
 
     get_model()
 
 
 def process_document(doc: "IngestDoc", **partition_kwargs) -> Optional[List[Dict[str, Any]]]:
-    """Process any IngestDoc-like class of document with choosen Unstructured's partition logic.
+    """Process any IngestDoc-like class of document with chosen Unstructured's partition logic.
 
     Parameters
     ----------
     partition_kwargs
         ultimately the parameters passed to partition()
     """
     isd_elems_no_filename = None
```

### Comparing `unstructured-0.7.8/unstructured/ingest/interfaces.py` & `unstructured-0.7.9/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/ingest/main.py` & `unstructured-0.7.9/unstructured/ingest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,22 @@
 @click.option(
     "--partition-strategy",
     default="auto",
     help="The method that will be used to process the documents. "
     "Default: auto. Other strategies include `fast` and `hi_res`.",
 )
 @click.option(
+    "--partition-ocr-languages",
+    default="eng",
+    help="A list of language packs to specify which languages to use for OCR, separated by '+' "
+    "e.g. 'eng+deu' to use the English and German language packs. The appropriate Tesseract "
+    "language pack needs to be installed."
+    "Default: eng",
+)
+@click.option(
     "--api-key",
     default="",
     help="API Key for partition endpoint.",
 )
 @click.option(
     "--local-input-path",
     default=None,
@@ -466,14 +474,15 @@
     metadata_exclude,
     fields_include,
     flatten_metadata,
     max_docs,
     partition_by_api,
     partition_endpoint,
     partition_strategy,
+    partition_ocr_languages,
     api_key,
     local_input_path,
     local_file_glob,
     download_only,
 ):
     default_values = collections.Counter([option.default for option in ctx.command.params])
     passed_values = collections.Counter(ctx.params.values())
@@ -777,22 +786,23 @@
     # Check for other connector-specific options here and define the doc_connector object
     # e.g. "elif azure_container:  ..."
 
     else:
         logger.error("No connector-specific option was specified!")
         sys.exit(1)
 
-    process_document_with_partition_strategy = partial(
+    process_document_with_partition_args = partial(
         process_document,
         strategy=partition_strategy,
+        ocr_languages=partition_ocr_languages,
     )
 
     MainProcess(
         doc_connector=doc_connector,
-        doc_processor_fn=process_document_with_partition_strategy,
+        doc_processor_fn=process_document_with_partition_args,
         num_processes=num_processes,
         reprocess=reprocess,
         verbose=verbose,
         max_docs=max_docs,
     ).run()
```

### Comparing `unstructured-0.7.8/unstructured/nlp/english-words.txt` & `unstructured-0.7.9/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/nlp/english_words.py` & `unstructured-0.7.9/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/nlp/patterns.py` & `unstructured-0.7.9/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/nlp/tokenize.py` & `unstructured-0.7.9/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/__init__.py` & `unstructured-0.7.9/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/api.py` & `unstructured-0.7.9/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/auto.py` & `unstructured-0.7.9/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from unstructured.partition.epub import partition_epub
 from unstructured.partition.html import partition_html
 from unstructured.partition.image import partition_image
 from unstructured.partition.json import partition_json
 from unstructured.partition.md import partition_md
 from unstructured.partition.msg import partition_msg
 from unstructured.partition.odt import partition_odt
+from unstructured.partition.org import partition_org
 from unstructured.partition.pdf import partition_pdf
 from unstructured.partition.ppt import partition_ppt
 from unstructured.partition.pptx import partition_pptx
 from unstructured.partition.rst import partition_rst
 from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
 from unstructured.partition.tsv import partition_tsv
@@ -150,14 +151,21 @@
     elif filetype == FileType.EPUB:
         elements = partition_epub(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
             **kwargs,
         )
+    elif filetype == FileType.ORG:
+        elements = partition_org(
+            filename=filename,
+            file=file,
+            include_page_breaks=include_page_breaks,
+            **kwargs,
+        )
     elif filetype == FileType.RST:
         elements = partition_rst(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
             **kwargs,
         )
```

### Comparing `unstructured-0.7.8/unstructured/partition/common.py` & `unstructured-0.7.9/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/csv.py` & `unstructured-0.7.9/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/doc.py` & `unstructured-0.7.9/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/docx.py` & `unstructured-0.7.9/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/email.py` & `unstructured-0.7.9/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/epub.py` & `unstructured-0.7.9/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/html.py` & `unstructured-0.7.9/unstructured/partition/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     html_assemble_articles: bool = False,
     **kwargs,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
-     filename
+    filename
         A string defining the target filename path.
     file
         A file-like object using "r" mode --> open(filename, "r").
     text
         The string representation of the HTML document.
     url
         The URL of a webpage to parse. Only for URLs that return an HTML document.
```

### Comparing `unstructured-0.7.8/unstructured/partition/image.py` & `unstructured-0.7.9/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/json.py` & `unstructured-0.7.9/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/md.py` & `unstructured-0.7.9/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/msg.py` & `unstructured-0.7.9/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/odt.py` & `unstructured-0.7.9/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/pdf.py` & `unstructured-0.7.9/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/ppt.py` & `unstructured-0.7.9/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/pptx.py` & `unstructured-0.7.9/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/rst.py` & `unstructured-0.7.9/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/rtf.py` & `unstructured-0.7.9/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/strategies.py` & `unstructured-0.7.9/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/text.py` & `unstructured-0.7.9/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/text_type.py` & `unstructured-0.7.9/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/tsv.py` & `unstructured-0.7.9/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/xlsx.py` & `unstructured-0.7.9/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/partition/xml.py` & `unstructured-0.7.9/unstructured/partition/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from unstructured.partition.text import partition_text
 
 
 def is_leaf(elem):
     return not bool(elem)
 
 
+def is_string(elem):
+    return isinstance(elem, str) or (hasattr(elem, "text") and isinstance(elem.text, str))
+
+
 def get_leaf_elements(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     xml_path: str = ".",
 ):
     if filename:
         _, raw_text = read_txt_file(filename=filename)
@@ -29,15 +33,15 @@
         raise ValueError("Either 'filename' or 'file' must be provided.")
 
     root = ET.fromstring(raw_text)
     leaf_elements = []
 
     for elem in root.findall(xml_path):
         for subelem in elem.iter():
-            if is_leaf(subelem):
+            if is_leaf(subelem) and is_string(subelem.text):
                 leaf_elements.append(subelem.text)
 
     return "\n".join(leaf_elements)  # type: ignore
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.XML)
```

### Comparing `unstructured-0.7.8/unstructured/staging/argilla.py` & `unstructured-0.7.9/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/base.py` & `unstructured-0.7.9/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/baseplate.py` & `unstructured-0.7.9/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/datasaur.py` & `unstructured-0.7.9/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/huggingface.py` & `unstructured-0.7.9/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/label_box.py` & `unstructured-0.7.9/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/label_studio.py` & `unstructured-0.7.9/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/prodigy.py` & `unstructured-0.7.9/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/staging/weaviate.py` & `unstructured-0.7.9/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured/utils.py` & `unstructured-0.7.9/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.8/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.9/unstructured.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.8
+Version: 0.7.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -34,14 +34,24 @@
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
         <h3 align="center">
+          <p>API Announcement!</p>
+        </h3>
+        
+        <p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
+          
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+        We'd love to hear your feedback, let us know how it goes in our
+          community slack. And stay tuned for improvements to both quality and performance!</p>
+        
+        <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
         users the building blocks they need to build pipelines targeted at the documents they care
         about. Bricks in the library fall into three categories:
@@ -99,14 +109,15 @@
         | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
         | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
         | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
+        | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -15,14 +15,21 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          **** API Announcement! ****
+While access to the hosted Unstructured API will remain free, API Keys will
+soon be required to make requests. To prevent any disruption, get yours here
+now and start using it today!
+Checkout the readme here to get started making API calls. We'd love to hear
+your feedback, let us know how it goes in our community slack. And stay tuned
+for improvements to both quality and performance!
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -60,15 +67,16 @@
 | None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
 (`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
+Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
```

### Comparing `unstructured-0.7.8/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.9/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 unstructured/partition/epub.py
 unstructured/partition/html.py
 unstructured/partition/image.py
 unstructured/partition/json.py
 unstructured/partition/md.py
 unstructured/partition/msg.py
 unstructured/partition/odt.py
+unstructured/partition/org.py
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
 unstructured/partition/rst.py
 unstructured/partition/rtf.py
 unstructured/partition/strategies.py
 unstructured/partition/text.py
```

### Comparing `unstructured-0.7.8/unstructured.egg-info/requires.txt` & `unstructured-0.7.9/unstructured.egg-info/requires.txt`

 * *Files identical despite different names*

