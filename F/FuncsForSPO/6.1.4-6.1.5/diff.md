# Comparing `tmp/FuncsForSPO-6.1.4.tar.gz` & `tmp/FuncsForSPO-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.1.4.tar", last modified: Mon Jun 26 14:09:49 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.1.5.tar", last modified: Mon Jun 26 15:11:17 2023, max compression
```

## Comparing `FuncsForSPO-6.1.4.tar` & `FuncsForSPO-6.1.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.992546 FuncsForSPO-6.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.684838 FuncsForSPO-6.1.4/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.840744 FuncsForSPO-6.1.4/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.4/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.4/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.858668 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.886899 FuncsForSPO-6.1.4/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.4/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.930219 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.033113 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.087676 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.122363 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.142451 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.223918 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.483297 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.562031 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.572549 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.677497 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.696541 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.722865 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.757488 FuncsForSPO-6.1.4/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.789114 FuncsForSPO-6.1.4/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.4/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.817297 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.838433 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.857086 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.877560 FuncsForSPO-6.1.4/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.4/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.812907 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.4/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-26 14:09:48.986514 FuncsForSPO-6.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 14:09:48.994539 FuncsForSPO-6.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2661 2023-06-26 14:09:37.000000 FuncsForSPO-6.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.694553 FuncsForSPO-6.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.033790 FuncsForSPO-6.1.5/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.107194 FuncsForSPO-6.1.5/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.5/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.5/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.123237 FuncsForSPO-6.1.5/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.5/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.144380 FuncsForSPO-6.1.5/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.5/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.171971 FuncsForSPO-6.1.5/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.5/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.5/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.5/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.1.5/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.181117 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.204298 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.218305 FuncsForSPO-6.1.5/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.227201 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.279577 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.312054 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.340156 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.386098 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.442922 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8949 2023-06-26 15:10:17.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.470429 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.494502 FuncsForSPO-6.1.5/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.512557 FuncsForSPO-6.1.5/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.1.5/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.545511 FuncsForSPO-6.1.5/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.5/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.560583 FuncsForSPO-6.1.5/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.1.5/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.589192 FuncsForSPO-6.1.5/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.5/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.5/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.602738 FuncsForSPO-6.1.5/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.5/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.5/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.612280 FuncsForSPO-6.1.5/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.5/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:11:17.094169 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-26 15:11:16.000000 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-26 15:11:16.000000 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:11:16.000000 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-06-26 15:11:16.000000 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-06-26 15:11:16.000000 FuncsForSPO-6.1.5/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.5/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-26 15:11:17.691549 FuncsForSPO-6.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:11:17.695550 FuncsForSPO-6.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-06-26 15:11:05.000000 FuncsForSPO-6.1.5/setup.py
```

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.1.5/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fgpt/fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.1.5/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import os
 import base64
 from tqdm import tqdm
 import gdown
 import pytesseract
 from PIL import Image
 import fitz
-from alive_progress import alive_bar
 
 class ErroAPI(Exception):
     pass
 
 def faz_ocr_em_pdf(file_pdf: str, type_extract='text', dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints=False) -> str:
     """
     ## DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
@@ -198,26 +197,26 @@
         deleta_diretorio('temp_tess')
     pytesseract.pytesseract.tesseract_cmd = path_tesseract
 
     pdf_fitz = fitz.open(pdf)
     with fitz.open(pdf) as pdf_fitz:
         cria_dir_no_dir_de_trabalho_atual('pages')
         faz_log(f'Convertendo PDF para páginas...')
-        with alive_bar(len(pdf_fitz), title='EXTRACT PAGES') as bar:
+        with tqdm(total=len(pdf_fitz), desc='EXTRACT PAGES') as bar:
             for i, page in enumerate(pdf_fitz):
                 page = pdf_fitz.load_page(i)
                 mat = fitz.Matrix(dpi/72, dpi/72)  # Matriz de transformação usando DPI
                 pix = page.get_pixmap(matrix=mat)
                 image = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
                 image.save(f'pages/{i}.png')
-                bar()
+                bar.update(1)
         all_text = ''
 
         files = arquivos_com_caminho_absoluto_do_arquivo('pages')
-        with alive_bar(len(files), title='OCR') as bar:
+        with tqdm(total=len(files), desc='OCR') as bar:
             for i, image in enumerate(files):
                 text = pytesseract.image_to_string(image, config=config_tesseract)
                 all_text += text
-                bar()
+                bar.update(1)
             else:
                 limpa_diretorio('pages')
                 return all_text
```

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.1.5/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.1.5/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.1.5/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.4
+Version: 6.1.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.4/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.1.5/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/LICENSE` & `FuncsForSPO-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/PKG-INFO` & `FuncsForSPO-6.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.4
+Version: 6.1.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.4/README.md` & `FuncsForSPO-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.4/setup.py` & `FuncsForSPO-6.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.1.4'
+version = '6.1.5'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -52,15 +52,15 @@
             'webdriver-manager',
             'requests',
             'pretty_html_table',
             'packaging',
             'PySimpleGUI',
             'macholib',
             'wget',
-            'alive-progress',
+            # 'alive-progress',
             'winotify',
             'pypdf',
             'pywin32',
             'gdown',
             'pytesseract',
             'pymupdf',
             'PyPDF2',
```

