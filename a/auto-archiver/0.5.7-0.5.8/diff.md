# Comparing `tmp/auto_archiver-0.5.7.tar.gz` & `tmp/auto_archiver-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.5.7.tar", last modified: Tue Apr 18 18:30:57 2023, max compression
+gzip compressed data, was "auto_archiver-0.5.8.tar", last modified: Tue May  2 13:32:57 2023, max compression
```

## Comparing `auto_archiver-0.5.7.tar` & `auto_archiver-0.5.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.402122 auto_archiver-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/youtubedl_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/auto_auto_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 13:32:57.396901 auto_archiver-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.380901 auto_archiver-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.384901 auto_archiver-0.5.8/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/youtubedl_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/auto_auto_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.384901 auto_archiver-0.5.8/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.5.7/LICENSE` & `auto_archiver-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/PKG-INFO` & `auto_archiver-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.5.7
+Version: 0.5.8
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.7/README.md` & `auto_archiver-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/setup.cfg` & `auto_archiver-0.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.5.8/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/auto_auto_archive.py` & `auto_archiver-0.5.8/src/auto_archiver/auto_auto_archive.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/config.py` & `auto_archiver-0.5.8/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/context.py` & `auto_archiver-0.5.8/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/media.py` & `auto_archiver-0.5.8/src/auto_archiver/core/media.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/metadata.py` & `auto_archiver-0.5.8/src/auto_archiver/core/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             return right.merge(self)
         return self
 
     def store(self: Metadata, override_storages: List = None):
         # calls .store for all contained media. storages [Storage]
         storages = override_storages or ArchivingContext.get("storages")
         for media in self.media:
-            media.store(override_storages=storages)
+            media.store(override_storages=storages, url=self.get_url())
 
     def set(self, key: str, val: Any) -> Metadata:
         self.metadata[key] = val
         return self
 
     def get(self, key: str, default: Any = None, create_if_missing=False) -> Union[Metadata, str]:
         # goes through metadata and returns the Metadata available
```

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.5.8/src/auto_archiver/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/core/step.py` & `auto_archiver-0.5.8/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.5.8/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.5.8/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/databases/database.py` & `auto_archiver-0.5.8/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.5.8/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.5.8/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.5.8/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.5.8/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.5.8/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.5.8/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.5.8/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.5.8/src/auto_archiver/formatters/templates/html_template.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.5.8/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/storages/gd.py` & `auto_archiver-0.5.8/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/storages/local.py` & `auto_archiver-0.5.8/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/storages/s3.py` & `auto_archiver-0.5.8/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/storages/storage.py` & `auto_archiver-0.5.8/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.5.8/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.5.8/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/utils/misc.py` & `auto_archiver-0.5.8/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/utils/url.py` & `auto_archiver-0.5.8/src/auto_archiver/utils/url.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.5.8/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.7/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.5.8/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.5.7
+Version: 0.5.8
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.7/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.5.8/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

