# Comparing `tmp/FuncsForSPO-6.1.1.tar.gz` & `tmp/FuncsForSPO-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.1.1.tar", last modified: Sat Jun 24 21:21:29 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.1.2.tar", last modified: Mon Jun 26 13:58:50 2023, max compression
```

## Comparing `FuncsForSPO-6.1.1.tar` & `FuncsForSPO-6.1.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.947786 FuncsForSPO-6.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.525601 FuncsForSPO-6.1.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.582229 FuncsForSPO-6.1.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.593208 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.605225 FuncsForSPO-6.1.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.622760 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0      621 2023-06-24 21:16:37.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.627754 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.646757 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.659458 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.667457 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.701319 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.723868 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.741475 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.746481 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.776108 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.787106 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.799909 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.809507 FuncsForSPO-6.1.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.822045 FuncsForSPO-6.1.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.833044 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.864039 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.873162 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.879167 FuncsForSPO-6.1.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.571695 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.1/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-24 21:21:29.943781 FuncsForSPO-6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 21:21:29.947786 FuncsForSPO-6.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2661 2023-06-24 21:21:23.000000 FuncsForSPO-6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.899177 FuncsForSPO-6.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.318395 FuncsForSPO-6.1.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.385204 FuncsForSPO-6.1.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.399256 FuncsForSPO-6.1.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.410881 FuncsForSPO-6.1.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.439500 FuncsForSPO-6.1.2/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.2/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.2/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.2/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0      621 2023-06-24 21:16:37.000000 FuncsForSPO-6.1.2/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.443495 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.501136 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.523920 FuncsForSPO-6.1.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.533452 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.581053 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.609671 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.638067 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.648188 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.689943 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.704952 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.723299 FuncsForSPO-6.1.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.738213 FuncsForSPO-6.1.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.754769 FuncsForSPO-6.1.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.769498 FuncsForSPO-6.1.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39135 2023-06-26 13:58:24.000000 FuncsForSPO-6.1.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.788565 FuncsForSPO-6.1.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.805647 FuncsForSPO-6.1.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.817739 FuncsForSPO-6.1.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:58:50.371947 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-26 13:58:49.000000 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-26 13:58:50.000000 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:58:49.000000 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-26 13:58:49.000000 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-06-26 13:58:49.000000 FuncsForSPO-6.1.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-26 13:58:50.892878 FuncsForSPO-6.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:58:50.899177 FuncsForSPO-6.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2661 2023-06-26 13:58:35.000000 FuncsForSPO-6.1.2/setup.py
```

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.1.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fgpt/fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.1.2/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from webdriver_manager.chrome import ChromeDriverManager 
 from time import sleep
 from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fregex.functions_re import extrair_email
 from wget import download
 from subprocess import getoutput
+from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.utils.utils import *
 
 def url_atual(driver) -> str:
     """
     ### Função RETORNA a url atual
 
     Args:
```

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.1.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.1.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.1.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.1
+Version: 6.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.1.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/LICENSE` & `FuncsForSPO-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/PKG-INFO` & `FuncsForSPO-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.1
+Version: 6.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.1/README.md` & `FuncsForSPO-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.1/setup.py` & `FuncsForSPO-6.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.1.1'
+version = '6.1.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

