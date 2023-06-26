# Comparing `tmp/MTGProxyPrinter-0.23.0.tar.gz` & `tmp/MTGProxyPrinter-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.23.0.tar", last modified: Thu Jun  8 16:39:38 2023, max compression
+gzip compressed data, was "MTGProxyPrinter-0.24.0.tar", last modified: Mon Jun 26 12:25:24 2023, max compression
```

## Comparing `MTGProxyPrinter-0.23.0.tar` & `MTGProxyPrinter-0.24.0.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.23.0/LICENSE.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.23.0/MANIFEST.in
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.762258 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9892 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13399 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-06-08 16:39:38.000000 MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9892 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8436 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-06-08 13:24:21.000000 MTGProxyPrinter-0.23.0/ThirdPartyLicenses.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.762258 MTGProxyPrinter-0.23.0/doc/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    41844 2023-06-08 16:20:15.000000 MTGProxyPrinter-0.23.0/doc/changelog.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.766258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3255 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/__main__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1491 2023-06-05 09:41:25.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/app_dirs.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/application.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/argument_parser.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-06-08 15:23:14.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/card_info_downloader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_downloader.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.766258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/re_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.766258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/_interface.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11368 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/card_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/compact_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/edit_document_settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/import_deck_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/load_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/move_cards.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/new_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/page_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/replace_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/shuffle_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/downloader_base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/http_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-06-08 16:20:15.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/meta_data.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/metered_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/missing_images_manager.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.770258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11186 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/card_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    42104 2023-06-08 15:48:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7526 2023-06-05 08:21:15.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30725 2023-06-05 08:41:09.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb_migrations.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v2.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v3.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v4.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v5.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v6.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23886 2023-06-08 16:11:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26006 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document_loader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1650 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    18911 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/imagedb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/string_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/natsort.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/print.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-05-24 09:56:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/progress_meter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.770258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.742257 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.770258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.742257 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.770258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      490 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.774258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      441 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.962258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-05-24 12:10:19.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-05-24 12:09:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-05-24 11:50:42.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      475 2023-05-24 11:50:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.962258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/index.theme
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.742257 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.962258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.962258 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-05-24 12:15:01.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/resources.qrc
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/about_dialog.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4226 2023-05-24 13:03:39.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4081 2023-05-24 13:04:02.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3703 2023-05-24 13:04:26.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/main_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.966259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10340 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17043 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-05 16:19:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/sqlite_helpers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/stop_thread.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/add_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21267 2023-06-08 13:21:37.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11610 2023-06-05 16:19:35.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/central_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/deck_import_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11517 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/dialogs.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/about_dialog.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5497 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5224 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4125 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/page_config_dialog.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/page_config_widget.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13804 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-06-08 16:39:27.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3670 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/item_delegates.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23416 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/page_renderer.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5903 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/printing_filter_widgets.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17242 2023-05-23 17:35:26.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3878 2023-06-08 13:58:06.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/units_and_sizes.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/mtg_proxy_printer/update_checker.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5565 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.23.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-06-08 16:39:38.970259 MTGProxyPrinter-0.23.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.23.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/LICENSE.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.24.0/MANIFEST.in
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13399 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-06-26 12:25:24.000000 MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8781 2023-06-26 12:16:57.000000 MTGProxyPrinter-0.24.0/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-06-08 13:24:21.000000 MTGProxyPrinter-0.24.0/ThirdPartyLicenses.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/doc/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    43567 2023-06-26 12:18:31.000000 MTGProxyPrinter-0.24.0/doc/changelog.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3255 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/__main__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1437 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/app_dirs.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/application.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/argument_parser.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-06-08 15:23:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/card_info_downloader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_downloader.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/re_parsers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/_interface.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11404 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/card_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/compact_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/edit_document_settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/import_deck_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/load_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/move_cards.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/new_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/page_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/replace_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/shuffle_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/downloader_base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/http_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-06-26 12:19:05.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/meta_data.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/metered_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/missing_images_manager.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11186 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/card_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    46173 2023-06-25 19:44:33.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8066 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    32805 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb_migrations.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v2.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v3.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v4.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v5.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v6.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24082 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26031 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_loader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1685 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    19124 2023-06-24 23:03:11.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/imagedb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/string_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/natsort.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/print.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-05-24 09:56:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/progress_meter.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.306116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.310116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      490 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.310116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      441 2023-05-06 09:19:50.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-05-24 12:10:19.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-05-24 12:09:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-05-24 11:50:42.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      475 2023-05-24 11:50:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/index.theme
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.302116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-05-24 12:15:01.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/resources.qrc
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/about_dialog.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4226 2023-05-24 13:03:39.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4081 2023-05-24 13:04:02.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3703 2023-05-24 13:04:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/main_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.314116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10340 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17043 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-05 16:19:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/sqlite_helpers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/stop_thread.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/add_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21267 2023-06-08 13:21:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14318 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/central_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/deck_import_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11677 2023-06-26 08:34:03.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/dialogs.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/about_dialog.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5497 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5224 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4125 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_dialog.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_widget.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13804 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-06-26 12:25:14.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3670 2023-06-08 16:06:37.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/item_delegates.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26406 2023-06-26 11:18:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_renderer.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5903 2023-05-23 14:01:56.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/printing_filter_widgets.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17242 2023-05-23 17:35:26.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3913 2023-06-26 08:32:35.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/units_and_sizes.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/mtg_proxy_printer/update_checker.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5835 2023-06-26 11:58:49.000000 MTGProxyPrinter-0.24.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-06-26 12:25:24.318116 MTGProxyPrinter-0.24.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-04-27 09:06:29.000000 MTGProxyPrinter-0.24.0/setup.py
```

### Comparing `MTGProxyPrinter-0.23.0/LICENSE.md` & `MTGProxyPrinter-0.24.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/PKG-INFO` & `MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.23.0
+Version: 0.24.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -35,37 +35,39 @@
 - Create, save and load documents
 - Multi-level undo & redo
 - Export documents as PDFs
   - Optional, automatic splitting into configurable chunks to accommodate file size limits present in various printers.
 - Direct printing using your operating system’s printing support. Can use any available and suitable printer
 - Obtains high-quality images from Scryfall (where available)
   - Images are cached locally for faster loading times when printing the same cards again
+- Basic support for printing custom cards. Drop images onto the main window to add them as custom regular-size cards.
 - Import deck lists in various formats, like Magic Arena deck lists and XMage deck files (see below for a list of supported formats)
   - Automatic download of deck lists from various deck list database websites (see below for a list)
   - One-click removal of basic lands (optionally also including Wastes and Snow-covered basic lands)
   - Optional, automatic deck list translation. Translate all cards in the deck list to your preferred language. (Depending on image availability.)
   - Manually override chosen card printings, if you dislike the printing choices made in the deck list
   - When importing a deck list that contains excluded printings (see below), MTGProxyPrinter tries to replace them with suitable surrogates, where possible
 - Supports double-faced cards and split cards
   - Both front and back are searchable by all names printed on the card
   - Automatic handling of opposing card faces: MTGProxyPrinter automatically adds the same number of copies of the other face. (This feature can be disabled)
+  - Optional generation of check cards for double-faced cards. Those combine both sides on a single side
 - Hide cards using various card and printing filters. Hidden cards are treated as though they do not exist.
   - Bans in various formats supported by Scryfall
   - Border color (white-bordered, gold-bordered)
   - Funny cards (Silver-bordered and other black-bordered promotional cards, like the “Heroes of the Realm” cards. Also cards from Un-sets with acorn-shaped security stamp.)
   - Image availability (for non-English cards)
   - Being oversized
   - Digital printings (includes both Magic Online promotional card versions, MTG Arena digital-only cards and other digital printings)
 - Supports cards in all languages supported by Scryfall
 - Supports the official tokens (As offered by Scryfall, which is currently English only. If Scryfall starts to offer localized tokens, these will be become available, too.)
 - Adjustable paper size, page margins, image spacing
 - Optional printing of cut helper lines to aid machine-cutting printed sheets
 - Full support for oversized cards, like Archenemy Scheme cards or Planechase Planes. 
   - Regular-size cards and oversized cards are kept on separate pages to ensure consistent image spacing and proper rendering of cut helper lines.
-
+- Ability to add “related cards” of cards added to the document. These are cards referenced by name or tokens created.
 
 ### Supported deck list formats
 
 - Magic Arena
 - Magic Online (MTGO)
 - [XMage](http://xmage.de)
 - [Tappedout.net](https://tappedout.net) deck lists (choose CSV export)
```

### Comparing `MTGProxyPrinter-0.23.0/MTGProxyPrinter.egg-info/SOURCES.txt` & `MTGProxyPrinter-0.24.0/MTGProxyPrinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/PKG-INFO` & `MTGProxyPrinter-0.24.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.23.0
+Version: 0.24.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -35,37 +35,39 @@
 - Create, save and load documents
 - Multi-level undo & redo
 - Export documents as PDFs
   - Optional, automatic splitting into configurable chunks to accommodate file size limits present in various printers.
 - Direct printing using your operating system’s printing support. Can use any available and suitable printer
 - Obtains high-quality images from Scryfall (where available)
   - Images are cached locally for faster loading times when printing the same cards again
+- Basic support for printing custom cards. Drop images onto the main window to add them as custom regular-size cards.
 - Import deck lists in various formats, like Magic Arena deck lists and XMage deck files (see below for a list of supported formats)
   - Automatic download of deck lists from various deck list database websites (see below for a list)
   - One-click removal of basic lands (optionally also including Wastes and Snow-covered basic lands)
   - Optional, automatic deck list translation. Translate all cards in the deck list to your preferred language. (Depending on image availability.)
   - Manually override chosen card printings, if you dislike the printing choices made in the deck list
   - When importing a deck list that contains excluded printings (see below), MTGProxyPrinter tries to replace them with suitable surrogates, where possible
 - Supports double-faced cards and split cards
   - Both front and back are searchable by all names printed on the card
   - Automatic handling of opposing card faces: MTGProxyPrinter automatically adds the same number of copies of the other face. (This feature can be disabled)
+  - Optional generation of check cards for double-faced cards. Those combine both sides on a single side
 - Hide cards using various card and printing filters. Hidden cards are treated as though they do not exist.
   - Bans in various formats supported by Scryfall
   - Border color (white-bordered, gold-bordered)
   - Funny cards (Silver-bordered and other black-bordered promotional cards, like the “Heroes of the Realm” cards. Also cards from Un-sets with acorn-shaped security stamp.)
   - Image availability (for non-English cards)
   - Being oversized
   - Digital printings (includes both Magic Online promotional card versions, MTG Arena digital-only cards and other digital printings)
 - Supports cards in all languages supported by Scryfall
 - Supports the official tokens (As offered by Scryfall, which is currently English only. If Scryfall starts to offer localized tokens, these will be become available, too.)
 - Adjustable paper size, page margins, image spacing
 - Optional printing of cut helper lines to aid machine-cutting printed sheets
 - Full support for oversized cards, like Archenemy Scheme cards or Planechase Planes. 
   - Regular-size cards and oversized cards are kept on separate pages to ensure consistent image spacing and proper rendering of cut helper lines.
-
+- Ability to add “related cards” of cards added to the document. These are cards referenced by name or tokens created.
 
 ### Supported deck list formats
 
 - Magic Arena
 - Magic Online (MTGO)
 - [XMage](http://xmage.de)
 - [Tappedout.net](https://tappedout.net) deck lists (choose CSV export)
```

### Comparing `MTGProxyPrinter-0.23.0/README.md` & `MTGProxyPrinter-0.24.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 - Create, save and load documents
 - Multi-level undo & redo
 - Export documents as PDFs
   - Optional, automatic splitting into configurable chunks to accommodate file size limits present in various printers.
 - Direct printing using your operating system’s printing support. Can use any available and suitable printer
 - Obtains high-quality images from Scryfall (where available)
   - Images are cached locally for faster loading times when printing the same cards again
+- Basic support for printing custom cards. Drop images onto the main window to add them as custom regular-size cards.
 - Import deck lists in various formats, like Magic Arena deck lists and XMage deck files (see below for a list of supported formats)
   - Automatic download of deck lists from various deck list database websites (see below for a list)
   - One-click removal of basic lands (optionally also including Wastes and Snow-covered basic lands)
   - Optional, automatic deck list translation. Translate all cards in the deck list to your preferred language. (Depending on image availability.)
   - Manually override chosen card printings, if you dislike the printing choices made in the deck list
   - When importing a deck list that contains excluded printings (see below), MTGProxyPrinter tries to replace them with suitable surrogates, where possible
 - Supports double-faced cards and split cards
   - Both front and back are searchable by all names printed on the card
   - Automatic handling of opposing card faces: MTGProxyPrinter automatically adds the same number of copies of the other face. (This feature can be disabled)
+  - Optional generation of check cards for double-faced cards. Those combine both sides on a single side
 - Hide cards using various card and printing filters. Hidden cards are treated as though they do not exist.
   - Bans in various formats supported by Scryfall
   - Border color (white-bordered, gold-bordered)
   - Funny cards (Silver-bordered and other black-bordered promotional cards, like the “Heroes of the Realm” cards. Also cards from Un-sets with acorn-shaped security stamp.)
   - Image availability (for non-English cards)
   - Being oversized
   - Digital printings (includes both Magic Online promotional card versions, MTG Arena digital-only cards and other digital printings)
 - Supports cards in all languages supported by Scryfall
 - Supports the official tokens (As offered by Scryfall, which is currently English only. If Scryfall starts to offer localized tokens, these will be become available, too.)
 - Adjustable paper size, page margins, image spacing
 - Optional printing of cut helper lines to aid machine-cutting printed sheets
 - Full support for oversized cards, like Archenemy Scheme cards or Planechase Planes. 
   - Regular-size cards and oversized cards are kept on separate pages to ensure consistent image spacing and proper rendering of cut helper lines.
-
+- Ability to add “related cards” of cards added to the document. These are cards referenced by name or tokens created.
 
 ### Supported deck list formats
 
 - Magic Arena
 - Magic Online (MTGO)
 - [XMage](http://xmage.de)
 - [Tappedout.net](https://tappedout.net) deck lists (choose CSV export)
```

### Comparing `MTGProxyPrinter-0.23.0/ThirdPartyLicenses.md` & `MTGProxyPrinter-0.24.0/ThirdPartyLicenses.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/doc/changelog.md` & `MTGProxyPrinter-0.24.0/doc/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,78 @@
 # Changelog
 
+# Version 0.24.0 (2023-06-26)  <a name="v0_24_0"></a>
+
+## New features
+
+- Added basic support for printing custom cards. You can drag & drop image files onto the application window,
+  which are then added to the document as regular-sized cards
+    - Importing most common image formats is supported
+    - For best results, use images with size 745px×1040px, others will be scaled to that size
+    - As of now, there are a few limitations, which may be lifted in future updates:
+        - Custom cards cannot be saved. They are removed from saved documents
+        - Only regular-sized cards are supported. You can not add custom over-sized cards, i.e. no custom Planes or Schemes
+        - You cannot set the card name
+        - They cannot be defined as being double-faced, thus you cannot generate check cards for them (see point below)
+- Generation of check cards for double faced cards. Check cards render both sides of a double-faced card next to each
+  other on a single card side, like a split card. They can be used to represent double-faced cards in the library or
+  hand, in case you prefer playing DFCs with fully transparent sleeves.
+    - Check cards can be added by right-clicking any side of a DFC card. Additional ways may be added in the future.
+- Export of individual card images as files, including generated check cards. Right-click a card and select the export
+  option to save the image file to a location of your choice.
+- Loading documents via drag & drop. The application now supports loading saved documents
+  (with `.mtgproxies` file extension) dropped onto the main window. 
+
 # Version 0.23.0 (2023-06-08)  <a name="v0_23_0"></a>
 
 ## New features
 
 - Added context menu to the table that shows the cards on the current page. You can now:
-  - Right-click a card to add additional copies of that card to the document
-  - Right-click a card to add specific or all related cards, like cards referenced by name or created tokens.
-    For example, right-click a Swan Song to add the 2/2 Bird token created by that spell.
+    - Right-click a card to add additional copies of that card to the document
+    - Right-click a card to add specific or all related cards, like cards referenced by name or created tokens.
+      For example, right-click a Swan Song to add the 2/2 Bird token created by that spell.
 - Added additional card filters to hide potentially unwanted printings in the settings.
-  - Borderless cards, i.e. cards without a defined, solid border.
+    - Borderless cards, i.e. cards without a defined, solid border.
     [Scryfall search](https://scryfall.com/search?q=border%3Aborderless)
-  - Reversible cards. Some Secret Lair double-sided printings of otherwise single-sided cards.
+    - Reversible cards. Some Secret Lair double-sided printings of otherwise single-sided cards.
     [Scryfall search](https://scryfall.com/search?q=is%3Areversible)
 
 The new card filters and adding related cards via the new context menu require re-downloading the card data 
 from Scryfall once to start working, as previous versions did not store the required information in the local
 card database.
 
 ## Changed features
 
 - Redesigned the document save file format. Older versions will not be able to load documents saved with this version,
   and it is not possible to save documents in the old format.
-  - Loading older documents (internal format versions 2 to 5) is still supported.
-    Older documents will be automatically converted to version 6 when saved over.
+    - Loading older documents (internal format versions 2 to 5) is still supported.
+      Older documents will be automatically converted to version 6 when saved over.
 - Improved display of hidden printings hidden in the downloaded image cleanup wizard.
-  - It now shows full information for hidden printings, instead of identifying them as "unknown garbage".
+    - It now shows full information for hidden printings, instead of identifying them as "unknown garbage".
 
 ## Fixed issues
 
 - Handle the back sides of Secret Lair reversible cards when switching card printings. The application no longer offers
   alternative printings for the back sides of those cards and then silently fails to switch the printing. 
 - Subsequent card data download attempts no longer always fail, if the first attempt 
   failed due to receiving invalid data from the Scryfall API.
-  - This also prevents entering an invalid state with partially imported card data. 
+    - This also prevents entering an invalid state with partially imported card data. 
 - Restored displaying the download progress when using the “Download card data as file” option in the Debug settings.
 
 # Version 0.22.0 (2023-04-18)  <a name="v0_22_0"></a>
 
 ## New features
 
 - Added support for importing Magic Workstation Deck Data (`.mwDeck`) deck lists
 - Support for direct downloads from additional card list database websites:
-  - MTG Arena Zone ([mtgazone.com](https://mtgazone.com))
-  - MTGTop8 ([mtgtop8.com](http://mtgtop8.com))
-  - MTGDecks ([mtgdecks.net](https://mtgdecks.net/))
-  - Archidekt ([archidekt.com](https://archidekt.com/))
-  - TCGPlayer Infinite ([infinite.tcgplayer.com](https://infinite.tcgplayer.com/magic-the-gathering))
+    - MTG Arena Zone ([mtgazone.com](https://mtgazone.com))
+    - MTGTop8 ([mtgtop8.com](http://mtgtop8.com))
+    - MTGDecks ([mtgdecks.net](https://mtgdecks.net/))
+    - Archidekt ([archidekt.com](https://archidekt.com/))
+    - TCGPlayer Infinite ([infinite.tcgplayer.com](https://infinite.tcgplayer.com/magic-the-gathering))
 
 ## Changed features
 
 - Drawing sharp card corners is no longer always enabled,
   when loading documents created with MTGProxyPrinter version 0.18.0 or older.
   The option now follows the global application settings.
 - The "funny cards" card filter no longer hides tournament-legal cards from Un-sets like Unfinity.
@@ -60,38 +82,38 @@
 - Fixed crash that occurred when compacting the document moved cards from other pages onto the currently shown page.
 
 # Version 0.21.0 (2023-02-08)  <a name="v0_21_0"></a>
 
 ## New features
 
 - Added Undo and Redo actions. It is now possible to undo changes to the document, and also redo undone changes.
-  - The undo and redo button tooltip shows a short description
-    of the change that is performed when the button is clicked.
+    - The undo and redo button tooltip shows a short description
+      of the change that is performed when the button is clicked.
 
 ## Changed features
 
 - Temporarily disable automatic dark mode rendering on Windows 10, if dark mode rendering for applications is active,
   because of rendering issues in the deck import wizard and card image cleanup wizard.
   The feature will return with better rendering at some point in the future.
-  - Linux is unaffected by this change, as following the system color scheme generally just works there.
+    - Linux is unaffected by this change, as following the system color scheme generally just works there.
 
 ## Fixed issues
 
 - Fixed crash in the settings validation logic, introduced in version 0.19.0, that may occur when
   manually fiddling with the app configuration file creates an invalid document page size.
 - Fixed crash when shuffling a document that contains both regular-sized and over-sized cards.
   Individual cards of the same size will be shuffled around across pages, but regular and over-sized card pages
   will stay in their relative order and position.
 - After completing a card data update, properly hide cards which got banned in a format
   for which hiding banned cards is enabled in the settings. This prevents potential crashes when trying to add
   these cards to the document. (Cards already added to the document are unaffected by such a card data update)
 - Optimized the document renderer and improved rendering quality
-  - Fixed location of horizontal cut helper lines for over-sized cards, which were off by one pixel
-  - Fixed a sub-pixel overlap of card images when image spacing is set to zero (the default).
-  - Images are now always placed on full pixels, avoiding aliasing artifacts.
+    - Fixed location of horizontal cut helper lines for over-sized cards, which were off by one pixel
+    - Fixed a sub-pixel overlap of card images when image spacing is set to zero (the default).
+    - Images are now always placed on full pixels, avoiding aliasing artifacts.
 
 # Version 0.20.1 (2022-10-27)  <a name="v0_20_1"></a>
 
 - Fixed crash in the card data importer: The importer now handles double faced cards with missing back face images.
   These cards are skipped during the import.
 
 ## Other
@@ -100,15 +122,15 @@
 
 # Version 0.20.0 (2022-10-09)  <a name="v0_20_0"></a>
 
 ## New features
 
 - Automatic deck list downloads. The deck list import wizard now has an input field that accepts
   links to deck lists on various deck list database websites. 
-  - Currently supported are [Scryfall](https://scryfall.com),
+    - Currently supported are [Scryfall](https://scryfall.com),
     [MTGGoldfish](https://www.mtggoldfish.com/),
     [mtg.wtf](https://mtg.wtf/), [TappedOut](https://tappedout.net/),
     [Moxfield](https://www.moxfield.com/) and
     [Deckstats](https://deckstats.net/)
 
 ## Changed features
 
@@ -133,18 +155,18 @@
 
 # Version 0.18.0 (2022-07-09)  <a name="v0_18_0"></a>
 
 ## New features
 
 - Proper, full support for oversized cards, like Archenemy schemes or Planechase plane cards. Regular cards and larger
   cards are always kept on separate pages to ensure that drawn cut marker lines (if enabled) are always 100% accurate.
-  - Note: Some cards, like the Legacy Championship winner rewards, are tagged as being oversized, but are then served
-    with regular-size images by Scryfall.
-    When the image is downloaded, it will be treated as a regular card, even if the deck import wizard warns
-    about it being potentially oversized.
+    - Note: Some cards, like the Legacy Championship winner rewards, are tagged as being oversized, but are then served
+      with regular-size images by Scryfall.
+      When the image is downloaded, it will be treated as a regular card, even if the deck import wizard warns
+      about it being potentially oversized.
 
 ## Fixed issues
 
 - Significantly optimized card database size and import speed.
   (The database now takes roughly 25% less time to update on fast internet connections
   and uses about 30% less disk space)
 - Fixed the “Remove selected” cards button in the deck list importer unexpectedly staying active
@@ -162,18 +184,18 @@
   shuffling effort required after putting the printed deck in sleeves. Beware: The shuffling currently separates front 
   and back faces of double faced cards. This may be improved in future versions.
 
 ## Changed features
 
 - The “New” document button will now ask for confirmation, before replacing the currently edited document with a new one.
 - Improved the advanced deck list parser that allows defining a custom regular expression to parse the deck list:
-  - Added buttons that insert preset regular expression building blocks. This reduces typing effort required to build
-    a working RE.
-  - The wizard only accepts the input regular expression, if it deems it being able to extract sufficient information
-    for card identification.
+    - Added buttons that insert preset regular expression building blocks. This reduces typing effort required to build
+      a working RE.
+    - The wizard only accepts the input regular expression, if it deems it being able to extract sufficient information
+      for card identification.
 
 ## Fixed issues
 
 - Fixed broken file type filters when loading deck lists. The file selection dialog now properly filters for deck
   list files instead of showing nothing.
 - Fixed potential crash when exiting the application while a card image download runs
 
@@ -208,17 +230,17 @@
 - Added short descriptions when the progress bar is shown at the bottom of the main window.
 - In the settings window, the card filters check boxes now have buttons next to them that open a web browser showing
   the Scryfall query highlighting the cards affected by the corresponding filter.
 
 ## Changed features
 
 - Card download filters are now filters used to hide printings.
-  - Updating the settings no longer requires re-downloading the data from Scryfall.
-  - Inverted the display: Instead of specifying which cards or printings are included,
-    the settings now state which printings are hidden. (Settings saved with previous versions are migrated.)
+    - Updating the settings no longer requires re-downloading the data from Scryfall.
+    - Inverted the display: Instead of specifying which cards or printings are included,
+      the settings now state which printings are hidden. (Settings saved with previous versions are migrated.)
 - The deck list import wizard now shows only matching files when browsing the file system for a deck list to load.
   The filtering can be disabled by switching to the “All files” filter.
 - When the deck list import wizard has the freedom of printing choice, it will now prefer the newest, regular,
   tournament-legal printings over others like oversized cards or art series cards,
   even if those are not hidden in the settings. You can still access them, but these printings won’t be automatically
   chosen.
 - The document and PDF save path now defaults to the local Documents directory.
@@ -227,19 +249,19 @@
   context information is used to obtain a correct translation, if available. Otherwise, a majority vote is performed
   to guess the most likely meaning of a given card name.
 
 ## Fixed issues
 
 - Added potentially missing icons to buttons in the document settings dialog.
 - Fixed the incomplete Magic Arena deck list parser.
-  - Added support for the simple and more common card list format that does not specify the exact printing.
+    - Added support for the simple and more common card list format that does not specify the exact printing.
     (I.e. the parser now accept valid entries like `5 Island` instead of only accepting `5 Island (SNC) 265`)
-  - Also recognizes the segment headers that may be present in the deck list, 
-    that are “Deck”, “Commander”, “Companion” and “Sideboard”,
-    and will no longer complain that these are unidentified cards.
+    - Also recognizes the segment headers that may be present in the deck list, 
+      that are “Deck”, “Commander”, “Companion” and “Sideboard”,
+      and will no longer complain that these are unidentified cards.
 - Mitigate crashes when using the wrong CSV deck list parser with a given CSV file. An error message is now shown in
   this case.
 
 # Version 0.15.1 (2022-04-13) <a name="v0_15_1"></a>
 
 ## Changed features
 
@@ -264,16 +286,16 @@
 
 # Version 0.15.0 (2022-04-03) <a name="v0_15_0"></a>
 
 ## Implemented features
 
 - Document settings, like paper size, margins, spacings are now stored in saved documents. When loading a document,
   the stored settings overwrite the default values set in the application settings.
-  - The Edit menu in the main window has a new option to edit these document settings for the current document only.
-  - Older save files do not contain the relevant data and have to be saved explicitly to perform a save file migration.
+    - The Edit menu in the main window has a new option to edit these document settings for the current document only.
+    - Older save files do not contain the relevant data and have to be saved explicitly to perform a save file migration.
 - Added new card download filter that allows excluding digital cards.
   The new filter matches both digital “reprints” of existing cards
   (for example Magic Online-exclusive promotional card versions)
   and digital-only cards that aren’t available as physical cards at all (like the Magic Arena Alchemy cards).
 - Added a new user interface layout that uses tabs to only show one part of the main window at a time.
   This is mainly useful for small and high-DPI monitors in portrait mode, i.e. when using 
   a monitor with an aspect ratio of 9:16.
@@ -425,33 +447,33 @@
 # Version 0.11.0 (2021-05-12) <a name="v0_11_0"></a>
 
 ## Implemented features
 
 - Suggest a PDF document file name based on the loaded document’s file name, if the current document was saved to
   or loaded from disk.
 - Added optional, automatic update checks, both for MTGProxyPrinter itself and the card data from Scryfall.
-  - The application asks for consent for both when starting the application for the first time or
-    when updating from prior versions
-  - For now, the application update check only notifies about updates, and does not perform any automatic update.
+    - The application asks for consent for both when starting the application for the first time or
+      when updating from prior versions
+    - For now, the application update check only notifies about updates, and does not perform any automatic update.
 - Integrated the changelog into the application, as a new tab in the About dialog.
-  - Automatically show the changelog once after each application update.
+    - Automatically show the changelog once after each application update.
 
 ## Changed Features
 
 - Use cx_Freeze instead of PyInstaller for stand-alone distributions. This yields cleaner, but larger builds,
   and an actual installer for Windows. The application can now be installed and uninstalled using standard OS
   features on Windows.
 
 ## Fixed issues
 
 - The application now handles offline operation and network outages during download processes.
-  - Shows a message box whenever a download fails
-  - The card database will revert to the last state, if downloading fresh card data fails.
-  - When downloading card images fails, the card will be added to the document using a blank placeholder.
-    The user can save the document and load it the next time network access is available to fetch the missing images.
+    - Shows a message box whenever a download fails
+    - The card database will revert to the last state, if downloading fresh card data fails.
+    - When downloading card images fails, the card will be added to the document using a blank placeholder.
+      The user can save the document and load it the next time network access is available to fetch the missing images.
 
 # Version 0.10.0 (2021-04-21) <a name="v0_10_0"></a>
 
 ## Implemented features
 
 - Added a "New document" entry to the File menu and the toolbar.
   It closes the currently edited document and creates a new one.
@@ -541,16 +563,16 @@
 
 ## Implemented features
 
 - Added direct printing support. The user can now directly print documents using a physical printer attached to the
   computer. It uses the systems native printing support, where available.
 - Added command line arguments: The application now accepts a document path as a positional argument.
   This allows opening documents when starting the application.
-  - On Windows, this can be used to drag&drop saved documents onto the EXE and load the file, and it can be used
-    to associate the file type with the program and then automatically open saved documents by clicking on them.
+    - On Windows, this can be used to drag&drop saved documents onto the EXE and load the file, and it can be used
+      to associate the file type with the program and then automatically open saved documents by clicking on them.
 - When changing download filter settings, ask the user if they want to re-download the card data. The user can do so
   when asked or any time later.
 - Implemented a way to trim down the locally stored images: Added a wizard to the Settings menu that allows deletion
   of unused or seldom used card images based on configurable criteria.
   If the user wishes, they can exactly select which images to delete.
 
 ## Changed Features
@@ -606,22 +628,22 @@
 ## Changed features
 
 - Re-written the card search to use a hierarchical search, focussing primarily on the card name.
   The card search now shows a list of suggestions that can be filtered using a search term,
   including basic wildcard support. When a card name is selected from the suggestion list,
   a specific printing can be selected. The search selects a random printing as a suggestion by default 
   to speed up the process,  if the user doesn’t care about the specific printing used.
-  - The new search displays sets using their human-readable English name.
-  - The search does not reset itself anymore, when adding a card.
+    - The new search displays sets using their human-readable English name.
+    - The search does not reset itself anymore, when adding a card.
 - Added a setting to choose between a horizontal search area layout above the currently edited page and a
   vertical search area that sits between the page list and the currently edited page.
-  - The horizontal layout resembles a traditional search bar, as used in other programs, looking more familiar
-  - The vertical layout makes better use of the available screen space, requires less mouse movement
-    and works better on widescreen monitors
-  - Switching the layout requires an application restart.
+    - The horizontal layout resembles a traditional search bar, as used in other programs, looking more familiar
+    - The vertical layout makes better use of the available screen space, requires less mouse movement
+      and works better on widescreen monitors
+    - Switching the layout requires an application restart.
 - The overview table showing the cards of the current page now shows the full, 
   human-readable English set name plus the short, three(-or-more)-letter set code,
   instead of showing only the cryptic set code.
 
 ## Fixed issues
 
 - Vastly improved accuracy of all download progress bars, especially for the card data download.
@@ -640,19 +662,19 @@
 
 
 # Version 0.7.0 (2012-02-18) <a name="v0_7_0"></a>
 
 ## Implemented features
 
 - Implemented automatic deck list imports
-  - Implemented as a multi-page wizard that guides the user through the process.
-    Accessible via an entry in the File menu.
-  - Supports Magic Online, MTG Arena and XMage deck files (And Websites that export compatible files)
-  - Appends the imported list to the currently edited document or optionally completely replaces it.
-  - Current limitation: Cards have to be matched exactly. Cards that do not specify a unique printing are not imported.
+    - Implemented as a multi-page wizard that guides the user through the process.
+      Accessible via an entry in the File menu.
+    - Supports Magic Online, MTG Arena and XMage deck files (And Websites that export compatible files)
+    - Appends the imported list to the currently edited document or optionally completely replaces it.
+    - Current limitation: Cards have to be matched exactly. Cards that do not specify a unique printing are not imported.
   
 ## Fixed issues
 
 - Fixed that when the current page overflows, each card batch got added to a completely new page,
   even if the next pages had free slots. Now, free slots on pages after the currently viewed page are used up,
   before adding new pages.
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/__init__.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/__main__.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/__main__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/app_dirs.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/app_dirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 data_directories = platformdirs.PlatformDirs(PROGRAMNAME)
 
 
 def migrate_from_old_appdirs():
     # Skip migration, if not applicable
     old_logs = data_directories.user_cache_path / "log"
-    if sys.platform != "linux" or platformdirs.version.__version_tuple__ < (2, 6, 0) or not old_logs.exists():
+    if sys.platform != "linux" or not old_logs.exists():
         return
     import shutil
     data_directories.user_log_path.mkdir(parents=True, exist_ok=True)
     new_log_path = data_directories.user_log_path
     for item in old_logs.glob("*"):
         if (new_log_path/item).exists():
             item.unlink()  # New location already exists, cannot migrate. Simply prune the old log file
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/application.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/application.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/argument_parser.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/argument_parser.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/card_info_downloader.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/card_info_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_downloader.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/common.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/csv_parsers.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/csv_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/decklist_parser/re_parsers.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/decklist_parser/re_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/_interface.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/_interface.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/card_actions.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/card_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import functools
 import itertools
 import math
 import typing
 
-from mtg_proxy_printer.model.carddb import Card
+from mtg_proxy_printer.model.carddb import Card, CheckCard
 if typing.TYPE_CHECKING:
     from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.model.document_page import CardContainer
 from ._interface import DocumentAction, IllegalStateError, Self
 from .page_actions import ActionNewPage, ActionRemovePage
 from mtg_proxy_printer.logger import get_logger
 
@@ -38,15 +38,15 @@
     """
     Add an amount of copies of a card to a document page. If the count exceeds the available space on that page,
     distribute the remainder across free spots on later pages or append new pages to the document end.
     """
 
     COMPARISON_ATTRIBUTES = ["card", "count", "added_new_pages", "added_cards_to_existing_pages"]
 
-    def __init__(self, card: Card, count: int = 1):
+    def __init__(self, card: typing.Union[Card, CheckCard], count: int = 1):
         self.card = card
         self.count = count
         self.added_new_pages: int = 0
         self.first_added_page: int = 0
         self.added_cards_to_existing_pages: typing.List[typing.Tuple[int, int]] = []
 
     def apply(self, document: "Document") -> Self:
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/compact_document.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/compact_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/edit_document_settings.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/edit_document_settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/import_deck_list.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/import_deck_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/load_document.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/load_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/move_cards.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/move_cards.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/new_document.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/new_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/page_actions.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/page_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/replace_card.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/replace_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/document_controller/shuffle_document.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/document_controller/shuffle_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/downloader_base.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/downloader_base.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/http_file.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/http_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/logger.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/logger.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/meta_data.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/meta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 PROGRAMNAME = "MTGProxyPrinter"
-__version__ = "0.23.0"
+__version__ = "0.24.0"
 COPYRIGHT = "(C) 2019-2023 Thomas Hess"
 HOME_PAGE = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter"
 
 DOWNLOAD_WEB_PAGE = f"{HOME_PAGE}/uv/download.html"
 USER_AGENT = f"{PROGRAMNAME}/{__version__} ({HOME_PAGE})"
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/metered_file.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/metered_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/missing_images_manager.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/missing_images_manager.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/card_list.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/card_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import enum
 import itertools
 import functools
 import pathlib
 import textwrap
 import typing
 
-from PyQt5.QtGui import QPixmap, QColor
-from PyQt5.QtCore import Qt, QPoint, QRect, QSize, QObject, pyqtSignal as Signal
+from PyQt5.QtGui import QPixmap, QColor, QTransform, QPainter, QColorConstants
+from PyQt5.QtCore import Qt, QPoint, QRect, QSize, QPointF, QObject, pyqtSignal as Signal
 import delegateto
 
 if typing.TYPE_CHECKING:
     from mtg_proxy_printer.model.imagedb import CacheContent
 import mtg_proxy_printer.app_dirs
 from mtg_proxy_printer.model.carddb_migrations import migrate_card_database
 from mtg_proxy_printer.natsort import natural_sorted
@@ -50,14 +50,15 @@
 # The card data is mostly stable, Scryfall recommends fetching the card bulk data only in larger intervals, like
 # once per month or so.
 MINIMUM_REFRESH_DELAY = datetime.timedelta(days=14)
 
 __all__ = [
     "CardIdentificationData",
     "MTGSet",
+    "CheckCard",
     "Card",
     "CardCorner",
     "CardDatabase",
     "cached_dedent",
     "CardList",
     "OLD_DATABASE_LOCATION",
     "DEFAULT_DATABASE_LOCATION",
@@ -116,14 +117,15 @@
     scryfall_id: str = dataclasses.field(compare=True)
     is_front: bool = dataclasses.field(compare=True)
     oracle_id: str = dataclasses.field(compare=True)
     image_uri: str = dataclasses.field(compare=False)
     highres_image: bool = dataclasses.field(compare=False)
     is_oversized: bool = dataclasses.field(compare=False)
     face_number: int = dataclasses.field(compare=False)
+    is_dfc: bool = dataclasses.field(compare=False)
     image_file: typing.Optional[QPixmap] = dataclasses.field(default=None, compare=False)
 
     def set_image_file(self, image: QPixmap):
         self.image_file = image
         self.corner_color.cache_clear()
 
     def requested_page_type(self) -> PageType:
@@ -134,28 +136,137 @@
             return PageType.OVERSIZED
         return PageType.REGULAR
 
     @functools.lru_cache(maxsize=len(CardCorner))
     def corner_color(self, corner: CardCorner) -> QColor:
         """Returns the color of the card at the given corner. """
         if self.image_file is None:
-            return QColor.fromRgb(255, 255, 255, 0)  # fully transparent white
+            return QColorConstants.Transparent
         sample_area = self.image_file.copy(QRect(
             QPoint(
                 round(self.image_file.width() * corner.value[0]),
                 round(self.image_file.height() * corner.value[1])),
             QSize(10, 10)
         ))
         average_color = sample_area.scaled(1, 1, transformMode=Qt.SmoothTransformation).toImage().pixelColor(0, 0)
         return average_color
 
     def display_string(self):
         return f'"{self.name}" [{self.set.code.upper()}:{self.collector_number}]'
 
 
+@dataclasses.dataclass(unsafe_hash=True)
+class CheckCard:
+    front: Card
+    back: Card
+
+    @property
+    def name(self) -> str:
+        return f"{self.front.name} // {self.back.name}"
+
+    @property
+    def set(self) -> MTGSet:
+        return self.front.set
+
+    @property
+    def collector_number(self) -> str:
+        return self.front.collector_number
+
+    @property
+    def language(self) -> str:
+        return self.front.language
+
+    @property
+    def scryfall_id(self) -> str:
+        return self.front.scryfall_id
+
+    @property
+    def is_front(self) -> bool:
+        return True
+
+    @property
+    def oracle_id(self) -> str:
+        return self.front.oracle_id
+
+    @property
+    def image_uri(self) -> str:
+        return ""
+
+    @property
+    def highres_image(self) -> bool:
+        return self.front.highres_image and self.back.highres_image
+
+    @property
+    def is_oversized(self):
+        return self.front.is_oversized
+
+    @property
+    def face_number(self) -> int:
+        return 0
+
+    @property
+    def is_dfc(self) -> bool:
+        return False
+
+    @property
+    def image_file(self) -> typing.Optional[QPixmap]:
+        if self.front.image_file is None or self.back.image_file is None:
+            return None
+        card_size = self.front.image_file.size()
+        # Unlike metric paper sizes, the MTG card aspect ratio does not follow the golden ratio.
+        # Cards thus can’t be scaled using a singular factor of sqrt(2) on both axis.
+        # The scaled cards get a bit compressed horizontally.
+        vertical_scaling_factor = card_size.width() / card_size.height()
+        horizontal_scaling_factor = card_size.height()/(card_size.width()*2)
+        combined_image = QPixmap(card_size)
+        combined_image.fill(QColor.fromRgb(255, 255, 255, 0))  # Fill with fully transparent white
+        painter = QPainter(combined_image)
+        painter.setRenderHints(QPainter.SmoothPixmapTransform | QPainter.HighQualityAntialiasing)
+        transformation = QTransform()
+        transformation.rotate(90)
+        transformation.scale(horizontal_scaling_factor, vertical_scaling_factor)
+        painter.setTransform(transformation)
+        painter.drawPixmap(QPointF(card_size.width(), -card_size.height()), self.back.image_file)
+        painter.drawPixmap(QPointF(0, -card_size.height()), self.front.image_file)
+
+        return combined_image
+
+    def requested_page_type(self) -> PageType:
+        if self.front.image_file is None or self.back.image_file is None:
+            return PageType.OVERSIZED if self.is_oversized else PageType.REGULAR
+        size = self.front.image_file.size()
+        if (size.width(), size.height()) == (1040, 1490):
+            return PageType.OVERSIZED
+        return PageType.REGULAR
+
+    @functools.lru_cache(maxsize=len(CardCorner))
+    def corner_color(self, corner: CardCorner) -> QColor:
+        """Returns the color of the card at the given corner. """
+        if self.front.image_file is None or self.back.image_file is None:
+            return QColorConstants.Transparent
+        if corner == CardCorner.TOP_LEFT:
+            self.front.corner_color(CardCorner.BOTTOM_LEFT)
+        elif corner == CardCorner.TOP_RIGHT:
+            self.front.corner_color(CardCorner.TOP_LEFT)
+        elif corner == CardCorner.BOTTOM_LEFT:
+            self.back.corner_color(CardCorner.BOTTOM_RIGHT)
+        elif corner == CardCorner.BOTTOM_RIGHT:
+            self.back.corner_color(CardCorner.TOP_RIGHT)
+        return QColorConstants.Transparent
+
+    def display_string(self):
+        return f'"{self.name}" [{self.set.code.upper()}:{self.collector_number}]'
+
+
+class ImageDatabaseCards(typing.NamedTuple):
+    visible: typing.List[typing.Tuple[Card, "CacheContent"]] = []
+    hidden: typing.List[typing.Tuple[Card, "CacheContent"]] = []
+    unknown: typing.List["CacheContent"] = []
+
+
 OptionalCard = typing.Optional[Card]
 CardList = typing.List[Card]
 
 
 @functools.lru_cache(None)
 def cached_dedent(text: str):
     """Wraps textwrap.dedent() in an LRU cache."""
@@ -174,26 +285,25 @@
     def __init__(self, db_path: typing.Union[str, pathlib.Path] = DEFAULT_DATABASE_LOCATION, parent: QObject = None):
         """
         :param db_path: Path to the database file. May be “:memory:” to create an in-memory database for testing
             purposes.
         """
         super().__init__(parent)
         logger.info(f"Creating {self.__class__.__name__} instance.")
-        db = mtg_proxy_printer.sqlite_helpers.open_database(
+        self.db = db = mtg_proxy_printer.sqlite_helpers.open_database(
             db_path, SCHEMA_NAME, self.MIN_SUPPORTED_SQLITE_VERSION, False)
         migrate_card_database(db)
         logger.debug("Validating schema of the opened database")
         try:
             mtg_proxy_printer.sqlite_helpers.validate_database_schema(
                 db, 0, SCHEMA_NAME, self.MIN_SUPPORTED_SQLITE_VERSION, "Card database has unknown application id.")
         except AssertionError:
             logger.exception("Card database schema validation failed. Trying to continue, but expect crashes")
         else:
             logger.debug("Card database schema valid")
-        self.db = db
         self._exit_hook = None
         if db_path != ":memory:":
             self._register_exit_hook()
         self.store_current_printing_filters()
 
     def _register_exit_hook(self):
         logger.debug("Registering cleanup hooks that close the database on exit.")
@@ -326,25 +436,20 @@
         Returns an empty list, if the given data does not match any known card.
 
          :param card: card identification data container that contains values to find cards
          :param order_by_print_count: Enable sorting the result list by the recorded print count. Defaults to False
         """
         query = cached_dedent('''\
         SELECT card_name, set_code, set_name, collector_number, png_image_uri, scryfall_id, is_front,
-                oracle_id, highres_image, is_oversized, face_number, language -- get_cards_from_data()
-            FROM CardFace
-            JOIN Printing USING (printing_id)
-            JOIN FaceName USING (face_name_id)
-            JOIN PrintLanguage USING (language_id)
-            JOIN MTGSet USING (set_id)
-            JOIN Card USING (card_id)
+                oracle_id, highres_image, is_oversized, face_number, language, is_dfc -- get_cards_from_data()
+            FROM VisiblePrintings
         ''')
         if order_by_print_count:
             query += '    LEFT OUTER JOIN LastImageUseTimestamps USING (scryfall_id, is_front)\n'
-        where_clause = ['    WHERE Printing.is_hidden IS FALSE']
+        where_clause = ['    WHERE TRUE']
         where_parameters = []
         if card.language:
             where_clause.append(f'AND "language" = ?')
             where_parameters.append(card.language)
         if card.name:
             where_clause.append(f'AND card_name = ?')
             where_parameters.append(card.name)
@@ -364,27 +469,28 @@
             where_clause.append(f'AND oracle_id = ?')
             where_parameters.append(card.oracle_id)
         where_clause.append("")  # Insert final newline after joining
         query += "\n    ".join(where_clause)
         order_by_terms = []
         if order_by_print_count:
             order_by_terms.append("LastImageUseTimestamps.usage_count DESC NULLS LAST")
-        order_by_terms.append("MTGSet.wackiness_score ASC")
-        order_by_terms.append("MTGSet.release_date DESC")
+        order_by_terms.append("wackiness_score ASC")
+        order_by_terms.append("release_date DESC")
         query += "ORDER BY " + "\n    ,".join(order_by_terms)
         result = self._get_cards_from_data(query, where_parameters)
         return result
 
     def get_replacement_card_for_unknown_printing(
             self, card: CardIdentificationData, /, *, order_by_print_count: bool = False) -> CardList:
         preferred_language = mtg_proxy_printer.settings.settings["images"]["preferred-language"]
         query = cached_dedent('''\
+        -- get_replacement_card_for_unknown_printing()
         SELECT card_name, set_code, set_name, collector_number, png_image_uri,
                VisiblePrintings.scryfall_id, is_front, oracle_id, highres_image,
-               is_oversized, face_number, VisiblePrintings.language -- get_replacement_card_for_unknown_printing()
+               is_oversized, face_number, VisiblePrintings.language, is_dfc
             FROM RemovedPrintings
             JOIN VisiblePrintings USING (oracle_id)
             LEFT OUTER JOIN LastImageUseTimestamps USING (scryfall_id, is_front)
             WHERE RemovedPrintings.scryfall_id = ?
             AND is_front = ?
             ORDER BY 
                 -- Match with original language first, fall back to preferred language, then fall back to English
@@ -402,62 +508,66 @@
 
     def _get_cards_from_data(self, query, parameters) -> CardList:
         cursor = self.db.execute(query, parameters)
         result = [
             Card(
                 name, MTGSet(set_code, set_name), collector_number,
                 language, scryfall_id, bool(is_front), oracle_id, image_uri,
-                bool(highres_image), bool(is_oversized), face_number,
+                bool(highres_image), bool(is_oversized), face_number, bool(is_dfc),
             )
             for name, set_code, set_name, collector_number, image_uri, scryfall_id, is_front, oracle_id, highres_image,
-                is_oversized, face_number, language in cursor
+                is_oversized, face_number, language, is_dfc in cursor
         ]
         return result
 
     def find_related_cards(self, card: Card) -> CardList:
         """
-        Recursively finds all cards related to the given card.
-        This may be cards referenced by name in either direction, or token cards created
+        Recursively finds all cards related to the given non-token card.
+        This may be cards referenced by name in either direction, or token cards created.
+        Tokens cannot have outgoing related cards, as that would create potentially huge graphs
+        due to evergreen tokens like Treasures, Food, Clues, 2/2 Zombies, etc.
         """
         query = cached_dedent("""\
         WITH RECURSIVE 
           source_oracle_id (card_id) AS (
             SELECT card_id
             FROM Card
             WHERE oracle_id = ?),
           related_oracle_ids(related_id) AS (
             SELECT related_id
               FROM RelatedPrintings
               JOIN source_oracle_id USING (card_id)
-            UNION
+            UNION  -- Deduplicate to break infinite recursion on cross-referenced cards
             SELECT RelatedPrintings.related_id
               FROM RelatedPrintings
               JOIN related_oracle_ids ON RelatedPrintings.card_id = related_oracle_ids.related_id
+              -- Do not include the initial input card in the output dataset
               WHERE RelatedPrintings.related_id NOT IN (SELECT source_oracle_id.card_id FROM source_oracle_id)
         )
         SELECT oracle_id
           FROM Card
           JOIN related_oracle_ids ON Card.card_id = related_oracle_ids.related_id
         """)
         related_card_ids = self.db.execute(query, (card.oracle_id,)).fetchall()
         cards = []
         for related_oracle_id, in related_card_ids:
             # Prefer same set over other sets, which is important for multi-component cards like Meld cards. If it
             # isn't available, take from any other set. As a last-ditch fallback, resort to English printings.
             # The last case is most likely hit with non-English token-producing cards,
             # as long as Scryfall does not provide localized tokens.
-            related_cards = self.get_cards_from_data(
-                CardIdentificationData(card.language, set_code=card.set.code, oracle_id=related_oracle_id),
-                order_by_print_count=True) or \
-            self.get_cards_from_data(
-                CardIdentificationData(card.language, oracle_id=related_oracle_id),
-                order_by_print_count=True) or \
-            self.get_cards_from_data(
-                CardIdentificationData("en", oracle_id=related_oracle_id),
-                order_by_print_count=True)
+            related_cards = \
+                self.get_cards_from_data(
+                    CardIdentificationData(card.language, set_code=card.set.code, oracle_id=related_oracle_id),
+                    order_by_print_count=True) or \
+                self.get_cards_from_data(
+                    CardIdentificationData(card.language, oracle_id=related_oracle_id),
+                    order_by_print_count=True) or \
+                self.get_cards_from_data(
+                    CardIdentificationData("en", oracle_id=related_oracle_id),
+                    order_by_print_count=True)
             if related_cards:
                 cards.append(related_cards[0])
         return cards
 
     def find_collector_numbers_matching(self, card_name: str, set_abbr: str, language: str) -> StringList:
         """
         Finds all collector numbers matching the given filter. The result contains multiple elements, if the card
@@ -519,66 +629,64 @@
 
         query += '    ORDER BY set_name ASC\n'
         return list(itertools.starmap(MTGSet, self.db.execute(query, parameters)))
 
     def get_card_with_scryfall_id(self, scryfall_id: str, is_front: bool) -> OptionalCard:
         query = cached_dedent('''\
         SELECT card_name, set_code, set_name, collector_number, "language", png_image_uri, oracle_id,
-            highres_image, is_oversized, face_number -- get_card_with_scryfall_id()
+            highres_image, is_oversized, face_number, is_dfc -- get_card_with_scryfall_id()
             FROM VisiblePrintings
             WHERE scryfall_id = ? AND is_front = ?
         ''')
         result = self.db.execute(query, (scryfall_id, is_front)).fetchone()
         if result is None:
             return None
         else:
             name, set_abbr, set_name, collector_number, language, image_uri, oracle_id, highres_image,\
-                is_oversized, face_number = result
+                is_oversized, face_number, is_dfc = result
             return Card(
                 name, MTGSet(set_abbr, set_name), collector_number,
                 language, scryfall_id, bool(is_front), oracle_id, image_uri,
-                bool(highres_image), bool(is_oversized), face_number
+                bool(highres_image), bool(is_oversized), face_number, bool(is_dfc),
             )
 
-    def get_all_cards_from_image_cache(self, cache_content: typing.List["CacheContent"]):
+    def get_all_cards_from_image_cache(self, cache_content: typing.List["CacheContent"]) -> ImageDatabaseCards:
         """
         Partitions the content of the ImageDatabase disk cache into three lists:
         - All visible card printings
         - All hidden card printings
         - All unknown images
 
         Visible and invisible printings are returned as lists containing tuples (Card, CacheContent),
         unknown images are returned as a list with plain CacheContent instances.
         """
         query = cached_dedent('''\
         SELECT card_name, set_code, set_name, collector_number, "language", png_image_uri, oracle_id,
-            highres_image, is_oversized, face_number, is_hidden -- get_all_cards_from_image_cache()
+            highres_image, is_oversized, face_number, is_dfc, is_hidden -- get_all_cards_from_image_cache()
             FROM AllPrintings
             WHERE scryfall_id = ? AND is_front = ?
         ''')
-        visible: typing.List[typing.Tuple[Card, "CacheContent"]] = []
-        hidden: typing.List[typing.Tuple[Card, "CacheContent"]] = []
-        unknown: typing.List["CacheContent"] = []
+        cards = ImageDatabaseCards([], [], [])
         for cache_item in cache_content:
             result = self.db.execute(query, (cache_item.scryfall_id, cache_item.is_front)).fetchone()
             if result is None:
-                unknown.append(cache_item)
+                cards.unknown.append(cache_item)
                 continue
             name, set_abbr, set_name, collector_number, language, image_uri, oracle_id, highres_image, \
-                    is_oversized, face_number, is_hidden = result
+                    is_oversized, face_number, is_dfc, is_hidden = result
             card = Card(
                 name, MTGSet(set_abbr, set_name), collector_number,
                 language, cache_item.scryfall_id, cache_item.is_front, oracle_id, image_uri,
-                bool(highres_image), bool(is_oversized), face_number
+                bool(highres_image), bool(is_oversized), face_number, is_dfc
             )
             if is_hidden:
-                hidden.append((card, cache_item))
+                cards.hidden.append((card, cache_item))
             else:
-                visible.append((card, cache_item))
-        return visible, hidden, unknown
+                cards.visible.append((card, cache_item))
+        return cards
 
     def get_opposing_face(self, card) -> OptionalCard:
         """
         Returns the opposing face for double faced cards, or None for single-faced cards.
         """
         return self.get_card_with_scryfall_id(card.scryfall_id, not card.is_front)
 
@@ -757,31 +865,31 @@
         # computed similarity is equal to the maximum similarity encountered. This avoids creating a B-Tree required
         # for the alternative, appending a clause like "ORDER BY similarity DESC LIMIT 1"
         # This was chosen as a performance optimization,
         # because card translation can take considerable time during a deck list import.
         query = cached_dedent("""\
         SELECT card_name, set_code, set_name, collector_number, -- _translate_card()
                scryfall_id, png_image_uri, highres_image,
-               is_oversized, face_number,
+               is_oversized, face_number, is_dfc,
                MAX((set_code = ?) + (collector_number = ?)) AS similarity
             FROM VisiblePrintings
             WHERE oracle_id = ? AND language = ? AND is_front = ?
         """)
         parameters = [card.set.code, card.collector_number, card.oracle_id, language_override, card.is_front]
         # Because of the aggregate function used, no hit will result in a single row consisting of only NULL values.
         result = self.db.execute(query, parameters).fetchone()
         name, set_code, set_name, collector_number, scryfall_id, image_uri, highres_image, \
-            is_oversized, face_number, similarity = result
+            is_oversized, face_number, is_dfc, similarity = result
         if similarity is None:
             logger.debug(f"Found no translations to {language_override} for card '{card.name}'.")
             return None
         return Card(
             name, MTGSet(set_code, set_name), collector_number,
             language_override, scryfall_id, card.is_front, card.oracle_id, image_uri,
-            bool(highres_image), bool(is_oversized), face_number
+            bool(highres_image), bool(is_oversized), face_number, bool(is_dfc),
         )
 
     def store_current_printing_filters(
             self, use_transaction: bool = True, *,
             force_update_hidden_column: bool = False, progress_signal: typing.Callable[[], None] = None):
         if progress_signal is None:
             progress_signal = (lambda: None)
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb.sql`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 -- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 -- GNU General Public License for more details.
 
 -- You should have received a copy of the GNU General Public License
 -- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
-PRAGMA user_version = 0000030;
+PRAGMA user_version = 0000031;
 PRAGMA foreign_keys = on;
 BEGIN TRANSACTION;
 
 
 CREATE TABLE PrintLanguage (
   language_id INTEGER PRIMARY KEY NOT NULL,
   "language" TEXT NOT NULL UNIQUE
@@ -147,31 +147,43 @@
 );
 
 CREATE INDEX FaceName_for_translation ON FaceName(language_id, card_name DESC);
 CREATE INDEX CardFace_for_translation ON CardFace(face_name_id, face_number, printing_id);
 
 
 CREATE VIEW VisiblePrintings AS
+WITH double_faced_printings(printing_id, is_dfc) AS (
+	SELECT DISTINCT printing_id, TRUE as is_dfc
+	    FROM CardFace
+	    WHERE is_front IS FALSE)
   SELECT card_name, set_code, set_name, "language", collector_number, scryfall_id, highres_image, face_number,
-         is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, release_date
+         is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, release_date,
+		 coalesce(double_faced_printings.is_dfc, FALSE) as is_dfc
   FROM Card
   JOIN Printing USING (card_id)
   JOIN MTGSet   USING (set_id)
   JOIN CardFace USING (printing_id)
   JOIN FaceName USING (face_name_id)
   JOIN PrintLanguage USING (language_id)
+  LEFT OUTER JOIN double_faced_printings USING (printing_id)
   WHERE Printing.is_hidden IS FALSE
     AND FaceName.is_hidden IS FALSE
 ;
 
 CREATE VIEW AllPrintings AS
+WITH double_faced_printings(printing_id, is_dfc) AS (
+	SELECT DISTINCT printing_id, TRUE as is_dfc
+	    FROM CardFace
+	    WHERE is_front IS FALSE)
   SELECT card_name, set_code, set_name, "language", collector_number, scryfall_id, highres_image, face_number,
-         is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, Printing.is_hidden
+         is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, Printing.is_hidden,
+		 coalesce(double_faced_printings.is_dfc, FALSE) as is_dfc
   FROM Card
   JOIN Printing USING (card_id)
   JOIN MTGSet   USING (set_id)
   JOIN CardFace USING (printing_id)
   JOIN FaceName USING (face_name_id)
   JOIN PrintLanguage USING (language_id)
+  LEFT OUTER JOIN double_faced_printings USING (printing_id)
 ;
 
 COMMIT;
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/carddb_migrations.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/carddb_migrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -614,14 +614,58 @@
     CREATE TABLE RelatedPrintings (
       card_id INTEGER NOT NULL REFERENCES Card(card_id) ON UPDATE CASCADE ON DELETE CASCADE,
       related_id INTEGER NOT NULL REFERENCES Card(card_id) ON UPDATE CASCADE ON DELETE CASCADE,
       PRIMARY KEY (card_id, related_id),
       CONSTRAINT 'No self-reference' CHECK (card_id <> related_id)
     ) WITHOUT ROWID;
     """))
+    
+    
+def _migrate_30_to_31(db: sqlite3.Connection):
+    for statement in [
+        "DROP VIEW VisiblePrintings\n",
+        "DROP VIEW AllPrintings\n",
+        textwrap.dedent("""\
+        CREATE VIEW VisiblePrintings AS
+        WITH double_faced_printings(printing_id, is_dfc) AS (
+            SELECT DISTINCT printing_id, TRUE as is_dfc
+                FROM CardFace
+                WHERE is_front IS FALSE)
+          SELECT card_name, set_code, set_name, "language", collector_number, scryfall_id, highres_image, face_number,
+                 is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, release_date,
+                 coalesce(double_faced_printings.is_dfc, FALSE) as is_dfc
+          FROM Card
+          JOIN Printing USING (card_id)
+          JOIN MTGSet   USING (set_id)
+          JOIN CardFace USING (printing_id)
+          JOIN FaceName USING (face_name_id)
+          JOIN PrintLanguage USING (language_id)
+          LEFT OUTER JOIN double_faced_printings USING (printing_id)
+          WHERE Printing.is_hidden IS FALSE
+            AND FaceName.is_hidden IS FALSE
+        ;"""),
+        textwrap.dedent("""\
+        CREATE VIEW AllPrintings AS
+        WITH double_faced_printings(printing_id, is_dfc) AS (
+            SELECT DISTINCT printing_id, TRUE as is_dfc
+                FROM CardFace
+                WHERE is_front IS FALSE)
+          SELECT card_name, set_code, set_name, "language", collector_number, scryfall_id, highres_image, face_number,
+                 is_front, is_oversized, png_image_uri, oracle_id, release_date, wackiness_score, Printing.is_hidden,
+                 coalesce(double_faced_printings.is_dfc, FALSE) as is_dfc
+          FROM Card
+          JOIN Printing USING (card_id)
+          JOIN MTGSet   USING (set_id)
+          JOIN CardFace USING (printing_id)
+          JOIN FaceName USING (face_name_id)
+          JOIN PrintLanguage USING (language_id)
+          LEFT OUTER JOIN double_faced_printings USING (printing_id)
+        ;"""),
+    ]:
+        db.execute(statement)
 
 
 MIGRATION_SCRIPTS: MigrationScriptListing = (
     # First component of each tuple contains the source schema version, second contains the migration script function.
     # These MUST be ordered by source schema version, otherwise the migration logic breaks. In other words: APPEND only.
     (9, _migrate_9_to_10),
     (10, _migrate_10_to_11),
@@ -640,14 +684,15 @@
     (23, _migrate_23_to_24),
     (24, _migrate_24_to_25),
     (25, _migrate_25_to_26),
     (26, _migrate_26_to_27),
     (27, _migrate_27_to_28),
     (28, _migrate_28_to_29),
     (29, _migrate_29_to_30),
+    (30, _migrate_30_to_31),
 )
 
 
 def migrate_card_database_location():
     from mtg_proxy_printer.model.carddb import DEFAULT_DATABASE_LOCATION, OLD_DATABASE_LOCATION
     if DEFAULT_DATABASE_LOCATION.exists() and OLD_DATABASE_LOCATION.exists():
         logger.warning(f"A card database at both the new location '{DEFAULT_DATABASE_LOCATION}' and the old location "
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v2.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v2.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v3.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v3.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v4.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v4.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v5.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v5.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document-v6.sql` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document-v6.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,17 @@
             for page_index, page in enumerate(self.pages, start=1)
         )
         regular_card = CardType("r")
         flattened_data: DocumentSaveFormat = (
             (page, slot, scryfall_id, is_front, regular_card)
             for (page, (slot, (scryfall_id, is_front)))
             in itertools.chain.from_iterable(cards)
+            # TODO: For now, custom cards have an empty id. Until saving them is implemented, skip custom cards
+            #   so that the document can still be loaded
+            if scryfall_id
         )
         with mtg_proxy_printer.sqlite_helpers.open_database(
                 self.save_file_path, "document-v6", self.loader.MIN_SUPPORTED_SQLITE_VERSION) as db:
             db.execute("BEGIN TRANSACTION")
             _migrate_database(db)
             db.execute("DELETE FROM Card")
             db.executemany(
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document_loader.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     def on_network_error_occurred(self, error: str):
         self.network_errors_during_load[error] += 1
 
     def load_document(self):
         self.should_run = True
         try:
             self._load_document()
-        except AssertionError as e:
+        except (AssertionError, sqlite3.DatabaseError) as e:
             logger.exception(
                 "Selected file is not a known MTGProxyPrinter document or contains invalid data. Not loading it.")
             self.loading_file_failed.emit(self.save_path, str(e))
             self.finished.emit()
 
     def on_document_action_applied(self, action: DocumentAction):
         # Imported here to break a circular import. TODO: Investigate a better fix
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/document_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/document_page.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import dataclasses
 import typing
 
-from mtg_proxy_printer.model.carddb import Card
+from mtg_proxy_printer.model.carddb import Card, CheckCard
 from mtg_proxy_printer.units_and_sizes import PageType
 
 
 @dataclasses.dataclass
 class CardContainer:
     parent: "Page"
     card: Card
@@ -34,14 +34,14 @@
         found_types = set(container.card.requested_page_type() for container in self)
         if found_types == {PageType.REGULAR}:
             return PageType.REGULAR
         if found_types == {PageType.OVERSIZED}:
             return PageType.OVERSIZED
         return PageType.MIXED
 
-    def accepts_card(self, card: typing.Union[Card, PageType]) -> bool:
-        other_type = card.requested_page_type() if isinstance(card, Card) else card
+    def accepts_card(self, card: typing.Union[Card, CheckCard, PageType]) -> bool:
+        other_type = card.requested_page_type() if isinstance(card, (Card, CheckCard)) else card
         own_page_type = self.page_type()
         return other_type == own_page_type or own_page_type is PageType.UNDETERMINED
 
 
 PageList = typing.List[Page]
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/imagedb.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/imagedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
 from mtg_proxy_printer.document_controller.replace_card import ActionReplaceCard
 from mtg_proxy_printer.document_controller.import_deck_list import ActionImportDeckList
 from mtg_proxy_printer.document_controller import DocumentAction
 import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.downloader_base
 import mtg_proxy_printer.http_file
-from mtg_proxy_printer.model.carddb import Card
+from mtg_proxy_printer.model.carddb import Card, CheckCard
 from mtg_proxy_printer.stop_thread import stop_thread
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 
 DEFAULT_DATABASE_LOCATION = mtg_proxy_printer.app_dirs.data_directories.user_cache_path / "CardImages"
@@ -300,17 +300,21 @@
             f"Image download failed for card {card}, reason is \"{reason_str}\". Using blank replacement image.")
         # Only return the error message for storage, if the queue currently processes a batch job.
         # Otherwise, it’ll be re-raised if a batch job starts right after a singular request failed.
         if not self.batch_processing_state:
             self.network_error_occurred.emit(reason_str)
         return reason_str
 
-    def get_image_synchronous(self, card: Card):
+    def get_image_synchronous(self, card: typing.Union[Card, CheckCard]):
         try:
-            self._get_image_synchronous(card)
+            if isinstance(card, CheckCard):
+                self._get_image_synchronous(card.front)
+                self._get_image_synchronous(card.back)
+            else:
+                self._get_image_synchronous(card)
         except urllib.error.URLError as e:
             self.last_error_message = self._handle_network_error_during_download(
                 card, str(e.reason))
         except socket.timeout as e:
             self.last_error_message = self._handle_network_error_during_download(
                 card, f"Reading from socket failed: {e}")
         finally:
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/model/string_list.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/model/string_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/natsort.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/natsort.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/print.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/print.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/progress_meter.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/progress_meter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/index.theme` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/index.theme`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/resources.qrc` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/about_dialog.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/main_window.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/page_config_widget.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/page_config_widget.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/settings.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/sqlite_helpers.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/stop_thread.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/stop_thread.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/add_card.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/add_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/central_widget.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/central_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
+
 import functools
 import math
+import operator
+import pathlib
 import typing
 
 from PyQt5.QtCore import pyqtSignal as Signal, pyqtSlot as Slot, QPersistentModelIndex, QItemSelectionModel, \
     QModelIndex, QPoint
 from PyQt5.QtGui import QIcon
-from PyQt5.QtWidgets import QWidget, QAction, QMenu, QInputDialog
+from PyQt5.QtWidgets import QWidget, QAction, QMenu, QInputDialog, QFileDialog
 
+import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.model.card_list import PageColumns
 from mtg_proxy_printer.model.document import Document
-from mtg_proxy_printer.model.carddb import CardDatabase, Card, CardList
+from mtg_proxy_printer.model.carddb import CardDatabase, Card, CardList, CheckCard
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.document_controller import DocumentAction
 from mtg_proxy_printer.document_controller.card_actions import ActionRemoveCards, ActionAddCard
 from mtg_proxy_printer.ui.item_delegates import ComboBoxItemDelegate
 
 try:
     from mtg_proxy_printer.ui.generated.central_widget.columnar import Ui_central_widget as Ui_Columnar
@@ -109,56 +113,109 @@
         if not (index := view.indexAt(pos)).isValid():
             logger.debug("Right clicked empty space in the page card table view, ignoring event")
             return
         logger.info(f"Page card table requests context menu at x={pos.x()}, y={pos.y()}, row={index.row()}")
         menu = QMenu(view)
         card: Card = index.internalPointer().card
         menu.addActions(self._create_add_copies_actions(card))
+        if card.is_dfc:
+            menu.addSeparator()
+            self._create_add_check_card_actions(menu, card)
         if related_cards := self.card_db.find_related_cards(card):
             menu.addSeparator()
             self._create_add_related_actions(menu, related_cards)
+        self._add_save_image_action(menu, card)
         menu.popup(view.viewport().mapToGlobal(pos))
 
     def _create_add_copies_actions(self, card: typing.Union[Card, CardList], add_4th: bool = False):
         actions = [
             self._create_add_copies_action("Add 1 copy", 1, card),
             self._create_add_copies_action("Add 2 copies", 2, card),
             self._create_add_copies_action("Add 3 copies", 3, card),
             self._create_add_copies_action("Add copies …", None, card)
         ]
         if add_4th:
             actions.insert(-1, self._create_add_copies_action("Add 4 copies", 4, card),)
         return actions
 
-    def _create_add_copies_action(self, label: str, count: typing.Optional[int], card: typing.Union[Card, CardList]):
+    def _create_add_copies_action(self, label: str, count: typing.Optional[int],
+                                  card: typing.Union[Card, CheckCard, CardList]):
         action = QAction(QIcon.fromTheme("list-add"), label, self.ui.page_card_table_view)
         action.triggered.connect(functools.partial(self._add_copies, card, count))
         return action
 
+    def _create_add_check_card_actions(self, parent: QMenu, card: Card):
+        other_face = self.card_db.get_opposing_face(card)
+        front, back = sorted([card, other_face], key=operator.attrgetter("is_front"), reverse=True)
+        check_card = CheckCard(front, back)
+        actions = [
+            self._create_add_copies_action("Add 1 copy", 1, check_card),
+            self._create_add_copies_action("Add 2 copies", 2, check_card),
+            self._create_add_copies_action("Add 3 copies", 3, check_card),
+            self._create_add_copies_action("Add 4 copies", 4, check_card),
+            self._create_add_copies_action("Add copies …", None, check_card)
+        ]
+        parent.addMenu("Generate DFC check card").addActions(actions)
+
     def _create_add_related_actions(self, parent: QMenu, related_cards: CardList) -> None:
         logger.debug(f"Found {len(related_cards)} related cards. Adding them to the context menu")
         parent.addMenu("All related cards").addActions(self._create_add_copies_actions(related_cards, True))
         for card in related_cards:
             parent.addMenu(card.name).addActions(self._create_add_copies_actions(card, True))
 
-    def _add_copies(self, card: typing.Union[Card, CardList], count: typing.Optional[int]):
+    def _add_copies(self, card: typing.Union[Card, CheckCard, CardList], count: typing.Optional[int]):
         nl = '\n'
-        card_name = card.name if isinstance(card, Card) else nl + nl.join(item.name for item in card)
+        card_name = card.name if isinstance(card, (Card, CheckCard)) else nl + nl.join(item.name for item in card)
         if count is None:
             count, success = QInputDialog.getInt(self, "Add copies", f"Add copies of {card_name}", 1, 1, 100)
             if not success:
                 logger.info("User cancelled adding card copies")
                 return
         logger.info(f"Add {count} × {card_name.replace(nl, ',')} via the context menu action")
-        # Go through the image database to obtain the card images
-        if isinstance(card, Card):
-            self.obtain_card_image.emit(ActionAddCard(card, count))
+
+        if isinstance(card, (Card, CheckCard)):
+            self.request_action.emit(ActionAddCard(card, count))
         else:
             for item in card:
-                self.obtain_card_image.emit(ActionAddCard(item, count))
+                self.request_action.emit(ActionAddCard(item, count))
+
+    def _add_save_image_action(self, parent: QMenu, card: typing.Union[Card, CheckCard]):
+        action = QAction(QIcon.fromTheme("document-save"), "Export image", parent)
+        action.setData(card)
+        action.triggered.connect(self._on_save_image_action_triggered)
+        parent.addSeparator()
+        parent.addAction(action)
+
+    @Slot()
+    def _on_save_image_action_triggered(self):
+        logger.info("User requests exporting card image.")
+        action: QAction = self.sender()
+        if action is None:
+            logger.error("Action triggering _on_save_image_action_triggered not obtained!")
+            return
+        card: Card = action.data()
+        default_save_file = self._get_default_image_save_path(card)
+        result, _ = QFileDialog.getSaveFileName(
+            self, "Save card image", default_save_file, "Images (*.png *.bmp *.jpg)")  # type: str, str
+        if result:
+            card.image_file.save(result)
+            logger.info(f"Exported image of card {card.name} to {result}")
+        else:
+            logger.debug("User cancelled file name selection. Cancelling image export.")
+
+    @staticmethod
+    def _get_default_image_save_path(card: Card) -> str:
+        try:
+            parent = mtg_proxy_printer.app_dirs.data_directories.user_pictures_path
+        except AttributeError:
+            parent = pathlib.Path.home()
+        disallowed = str.maketrans('', '', '\\\n/:*?"<>|')  # Exclude newlines and characters restricted on Windows
+        file_name = card.name.replace(" // ", " ").translate(disallowed).lstrip().rstrip(" \t.")
+        logger.debug(f"Cleaned card name: '{file_name}'")
+        return str(parent/f"{file_name}.png")
 
     @Slot()
     def parsed_cards_table_selection_changed(self):
         """Called whenever the selection in the page_card_table_view is changed. This manages the activation state
         of the “Remove selected” button, which should only be clickable, if there are cards selected."""
         selection_model = self.ui.page_card_table_view.selectionModel()
         self.ui.delete_selected_images_button.setDisabled(selection_model.selection().isEmpty())
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/common.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/deck_import_wizard.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/deck_import_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/dialogs.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 import sys
 
 from PyQt5.QtCore import QFile, pyqtSlot as Slot
 from PyQt5.QtWidgets import QFileDialog, QWidget, QTextBrowser, QDialogButtonBox, QDialog
 from PyQt5.QtGui import QIcon
 from PyQt5.QtPrintSupport import QPrintPreviewDialog, QPrintDialog, QPrinter
 
-import mtg_proxy_printer.model.carddb
+import mtg_proxy_printer.app_dirs
+from mtg_proxy_printer.model.carddb import Card
 import mtg_proxy_printer.model.document
 import mtg_proxy_printer.model.imagedb
 import mtg_proxy_printer.print
 import mtg_proxy_printer.settings
 import mtg_proxy_printer.ui.common
 import mtg_proxy_printer.meta_data
+from mtg_proxy_printer.units_and_sizes import DEFAULT_SAVE_SUFFIX
 from mtg_proxy_printer.document_controller.edit_document_settings import ActionEditDocumentSettings
 from mtg_proxy_printer.logger import get_logger
 
 try:
     from mtg_proxy_printer.ui.generated.about_dialog import Ui_Dialog as Ui_AboutDialog
     from mtg_proxy_printer.ui.generated.page_config_dialog import Ui_Dialog as Ui_PageConfigDialog
 except ModuleNotFoundError:
@@ -84,20 +86,20 @@
         logger.debug("User aborted saving to PDF. Doing nothing.")
 
 
 class SaveDocumentAsDialog(QFileDialog):
 
     def __init__(self, document: mtg_proxy_printer.model.document.Document, parent: QWidget = None, **kwargs):
         super(SaveDocumentAsDialog, self).__init__(
-            parent, "Save document as …", filter="MTGProxyPrinter document (*.mtgproxies)", **kwargs)
+            parent, "Save document as …", filter=f"MTGProxyPrinter document (*.{DEFAULT_SAVE_SUFFIX})", **kwargs)
         if default_path := read_path("document-save-path"):
             self.setDirectory(default_path)
         self.document = document
         self.setAcceptMode(QFileDialog.AcceptSave)
-        self.setDefaultSuffix("mtgproxies")
+        self.setDefaultSuffix(DEFAULT_SAVE_SUFFIX)
         self.setFileMode(QFileDialog.AnyFile)
         self.accepted.connect(self.on_accept)
         self.rejected.connect(self.on_reject)
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     @Slot()
     def on_accept(self):
@@ -113,20 +115,21 @@
 
 class LoadDocumentDialog(QFileDialog):
 
     def __init__(
             self, parent: QWidget,
             document: mtg_proxy_printer.model.document.Document, **kwargs):
         super(LoadDocumentDialog, self).__init__(
-            parent, "Load MTGProxyPrinter document", filter="MTGProxyPrinter document (*.mtgproxies)", **kwargs)
+            parent, "Load MTGProxyPrinter document", filter=f"MTGProxyPrinter document (*.{DEFAULT_SAVE_SUFFIX})",
+            **kwargs)
         if default_path := read_path("document-save-path"):
             self.setDirectory(default_path)
         self.document = document
         self.setAcceptMode(QFileDialog.AcceptOpen)
-        self.setDefaultSuffix("mtgproxies")
+        self.setDefaultSuffix(DEFAULT_SAVE_SUFFIX)
         self.setFileMode(QFileDialog.ExistingFile)
         self.accepted.connect(self.on_accept)
         self.rejected.connect(self.on_reject)
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     @Slot()
     def on_accept(self):
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/about_dialog.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/main_window.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/page_config_dialog.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/page_config_widget.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/item_delegates.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/item_delegates.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/main_window.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/main_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import pathlib
 import typing
 
-from PyQt5.QtCore import pyqtSlot as Slot, pyqtSignal as Signal, QStringListModel, QUrl
-from PyQt5.QtGui import QCloseEvent, QKeySequence, QDesktopServices
+from PyQt5.QtCore import pyqtSlot as Slot, pyqtSignal as Signal, QStringListModel, QUrl, Qt
+from PyQt5.QtGui import QCloseEvent, QKeySequence, QDesktopServices, QDragEnterEvent, QDropEvent, QPixmap
 from PyQt5.QtWidgets import QApplication, QMessageBox, QProgressBar, QAction, QWidget, QLabel, QMainWindow, QDialog
 
 
 from mtg_proxy_printer.missing_images_manager import MissingImagesManager
 from mtg_proxy_printer.card_info_downloader import CardInfoDownloader
-from mtg_proxy_printer.model.carddb import CardDatabase
+from mtg_proxy_printer.model.carddb import CardDatabase, Card, MTGSet
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.document_controller.compact_document import ActionCompactDocument
 from mtg_proxy_printer.document_controller.page_actions import ActionNewPage, ActionRemovePage
 from mtg_proxy_printer.document_controller.shuffle_document import ActionShuffleDocument
 from mtg_proxy_printer.document_controller.new_document import ActionNewDocument
+from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
+from mtg_proxy_printer.units_and_sizes import DEFAULT_SAVE_SUFFIX
 import mtg_proxy_printer.settings
 import mtg_proxy_printer.print
 from mtg_proxy_printer.ui.dialogs import SavePDFDialog, SaveDocumentAsDialog, LoadDocumentDialog, \
     AboutMTGProxyPrinterDialog, PrintPreviewDialog, PrintDialog, DocumentSettingsDialog
 from mtg_proxy_printer.ui.cache_cleanup_wizard import CacheCleanupWizard
 from mtg_proxy_printer.ui.deck_import_wizard import DeckImportWizard
 
@@ -65,14 +67,15 @@
                  language_model: QStringListModel,
                  *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         logger.info(f"Creating {self.__class__.__name__} instance.")
         self.is_running = True
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
+        self.setAcceptDrops(True)
         self.default_undo_tooltip = self.ui.action_undo.toolTip()
         self.default_redo_tooltip = self.ui.action_redo.toolTip()
         self.missing_images_manager = MissingImagesManager(document, self)
         self.missing_images_manager.request_obtaining_images.connect(image_db.download_worker.obtain_missing_images)
         self.missing_images_manager.obtaining_missing_images_failed.connect(self.on_network_error_occurred)
         self.about_dialog = self._create_about_dialog()
         self.progress_label = self._create_progress_label()
@@ -451,7 +454,60 @@
                 QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel
                 )) in {QMessageBox.Yes, QMessageBox.No}:
             logger.info(f"{logger_message} User choice: {'Yes' if result == QMessageBox.Yes else 'No'}")
             mtg_proxy_printer.settings.settings["application"][settings_key] = str(
                 result == QMessageBox.Yes)
             mtg_proxy_printer.settings.write_settings_to_file()
             logger.debug("Written settings to disk.")
+
+    def dragEnterEvent(self, event: QDragEnterEvent) -> None:
+        if self._to_save_file_path(event):
+            logger.info("User drags a saved MTGProxyPrinter document onto the main window, accepting event")
+            event.acceptProposedAction()
+        elif images := self._to_pixmaps(event):
+            logger.info(f"User drags {len(images)} images onto the main window, accepting event")
+            event.acceptProposedAction()
+        else:
+            logger.debug("Rejecting drag&drop action for unknown or invalid data")
+
+    def dropEvent(self, event: QDropEvent) -> None:
+        if path := self._to_save_file_path(event):
+            logger.info("User dropped save file onto the main window, loading the dropped document")
+            self.document.loader.load_document(path)
+        elif images := self._to_pixmaps(event):
+            logger.info(f"User dropped {len(images)} images onto the main window, adding them as custom cards")
+            for image in images:
+                card = Card(
+                    "Custom card", MTGSet("CUS", "Custom"), "", "", "", True, "", "", True, False, 1, False, image)
+                action = ActionAddCard(card)
+                self.document.apply(action)
+
+    @staticmethod
+    def _to_save_file_path(event: typing.Union[QDragEnterEvent, QDropEvent]) -> typing.Optional[pathlib.Path]:
+        """
+        Returns a Path instance to a file, if the drag&drop event contains a reference to exactly 1 document save file,
+        None otherwise.
+        """
+        mime_data = event.mimeData()
+        # It doesn't make sense to drop multiple save files at once, since only one can be loaded.
+        # So ignore drag&drop containing multiple files
+        if mime_data.hasUrls() and len(dropped_urls := mime_data.urls()) == 1:
+            url = dropped_urls[0].toLocalFile()
+            path = pathlib.Path(url)
+            acceptable = path.is_file() and path.suffix.casefold() == f".{DEFAULT_SAVE_SUFFIX}"
+            if acceptable:
+                return path
+        return None
+
+    @staticmethod
+    def _to_pixmaps(event: typing.Union[QDragEnterEvent, QDropEvent]) -> typing.List[QPixmap]:
+        result: typing.List[QPixmap] = []
+        mime_data = event.mimeData()
+        regular = mtg_proxy_printer.units_and_sizes.CardSizes.REGULAR
+        width, height = regular.width.magnitude, regular.height.magnitude
+        for url in mime_data.urls():
+            pixmap = QPixmap(url.toLocalFile())
+            if not pixmap.isNull():
+                if pixmap.width() != width or pixmap.height() != height:
+                    pixmap = pixmap.scaled(width, height, transformMode=Qt.TransformationMode.SmoothTransformation)
+                result.append(pixmap)
+        return result
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/page_config_widget.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/page_renderer.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/page_renderer.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/printing_filter_widgets.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/printing_filter_widgets.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/ui/settings_window.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/ui/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/units_and_sizes.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/units_and_sizes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     from typing import Optional as NotRequired
 
 import pint
 
 unit_registry = pint.UnitRegistry()
 RESOLUTION: pint.Quantity = unit_registry("300dots/inch")
 UUID = str
+DEFAULT_SAVE_SUFFIX = "mtgproxies"
 
 
 class CardSize(typing.NamedTuple):
     width: pint.Quantity
     height: pint.Quantity
 
     @staticmethod
```

### Comparing `MTGProxyPrinter-0.23.0/mtg_proxy_printer/update_checker.py` & `MTGProxyPrinter-0.24.0/mtg_proxy_printer/update_checker.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.23.0/pyproject.toml` & `MTGProxyPrinter-0.24.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -82,33 +82,36 @@
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 minversion = 3.18
 
 envlist = 
-    py3-{unit_tests, test_create_bundle}-{windows, linux}
-
+    py3-unit_tests-platformdirs{26,33}-{windows, linux}
+    py3-test_create_bundle-{windows, linux}
 
 [testenv]
 skip_install = True
 
 
 platform =
     linux: linux
 #    macos: darwin
     windows: win32
 
 
 allowlist_externals =
+    {toxinidir}{/}build{/}bundle_test{/}MTGProxyPrinter
     windows: {toxinidir}{/}scripts{/}clean_windows_build.bat
 
 
 deps =
     platformdirs >= 2.6.0
+    platformdirs26: platformdirs == 2.6
+    platformdirs33: platformdirs >= 3.3.0
     build
     PyQt5
     ijson >= 3.1.0; python_version < '3.11'
     ijson >= 3.2.0; python_version >= '3.11'
     pint
     delegateto == 1.5
     PyHamcrest >= 1.8.1
@@ -123,15 +126,15 @@
     pytest-cov
     pytest-timeout
     pytest-qt >= 2.0
     PyHamcrest >= 2.0.0
     {[testenv]build_deps}
 
 
-[testenv:py3-unit_tests-{windows, linux}]
+[testenv:py3-unit_tests-platformdirs{26,33}-{windows, linux}]
 
 # Let Qt5 render offscreen, so that running tests don’t open windows or try to access the local system’s display
 # This also prevents unwanted user interactions with the widgets under test.
 # Offscreen rendering causes a segmentation fault on Windows, so simply show the GUI under test on Windows
 setenv =
     linux: QT_QPA_PLATFORM = offscreen
     PYTHONDEVMODE = 1
@@ -139,15 +142,15 @@
 deps =
     {[testenv]deps}
     {[testenv]test_deps}
 
 commands =
     pytest tests
 
-[testenv:py3-visible_unit_tests]
+[testenv:py3-platformdirs{26,33}-visible_unit_tests]
 # Runs the unit tests with the default Qt platform plugin,
 # causing them to visibly spawn GUI windows for tests of view logic.
 # Can be used to inspect the actions and GUI states manually.
 # Not part of the environment list, so isn’t run automatically.
 
 deps =
     {[testenv]deps}
@@ -157,14 +160,15 @@
     pytest tests
 
 # Pass DISPLAY, to allow rendering on screen. Also pass all other Qt-related environment variables,
 # like QT_SCREEN_SCALE_FACTORS
 passenv =
     DISPLAY
     QT_*
+    XDG_RUNTIME_DIR
     
 setenv = 
    PYTHONDEVMODE = 1
 
 
 [testenv:py3-test_create_bundle-{windows, linux}]
 
@@ -175,14 +179,17 @@
 
 # Let Qt5 render offscreen, so that running tests don’t open windows or try to access the local system’s display
 # This also prevents unwanted user interactions with the widgets under test
 setenv =
     linux: QT_QPA_PLATFORM = offscreen
     PYTHONDEVMODE = 1
 
+passenv =
+    XDG_RUNTIME_DIR
+
 commands =
     python scripts{/}compile_ui_files.py --full --purge-existing
     python setup_cx_freeze.py build_exe --build-exe build{/}bundle_test
     windows: {toxinidir}{/}scripts{/}clean_windows_build.bat build{/}bundle_test
     {toxinidir}{/}build{/}bundle_test{/}MTGProxyPrinter --test-exit-on-launch
     -python scripts{/}compile_ui_files.py --purge-existing
```

### Comparing `MTGProxyPrinter-0.23.0/setup.py` & `MTGProxyPrinter-0.24.0/setup.py`

 * *Files identical despite different names*

