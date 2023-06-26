# Comparing `tmp/FuncsForSPO-6.1.3.tar.gz` & `tmp/FuncsForSPO-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.1.3.tar", last modified: Mon Jun 26 14:04:54 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.1.4.tar", last modified: Mon Jun 26 14:09:49 2023, max compression
```

## Comparing `FuncsForSPO-6.1.3.tar` & `FuncsForSPO-6.1.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.664174 FuncsForSPO-6.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.061221 FuncsForSPO-6.1.3/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.139600 FuncsForSPO-6.1.3/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.3/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.3/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.154135 FuncsForSPO-6.1.3/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.3/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.168229 FuncsForSPO-6.1.3/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.3/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.216773 FuncsForSPO-6.1.3/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.3/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.3/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.3/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0      621 2023-06-24 21:16:37.000000 FuncsForSPO-6.1.3/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.223779 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.248369 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.261245 FuncsForSPO-6.1.3/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.268596 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.320455 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.351064 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.377476 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.385219 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.439798 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.454362 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.476217 FuncsForSPO-6.1.3/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.493490 FuncsForSPO-6.1.3/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.3/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.509710 FuncsForSPO-6.1.3/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.3/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.525278 FuncsForSPO-6.1.3/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39133 2023-06-26 14:04:27.000000 FuncsForSPO-6.1.3/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.541380 FuncsForSPO-6.1.3/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.3/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.3/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.558465 FuncsForSPO-6.1.3/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.3/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.3/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.569042 FuncsForSPO-6.1.3/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.3/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:04:54.126423 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-26 14:04:53.000000 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-06-26 14:04:53.000000 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:04:53.000000 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-26 14:04:53.000000 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-06-26 14:04:53.000000 FuncsForSPO-6.1.3/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.3/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-26 14:04:54.659171 FuncsForSPO-6.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 14:04:54.664174 FuncsForSPO-6.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2661 2023-06-26 14:04:45.000000 FuncsForSPO-6.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.992546 FuncsForSPO-6.1.4/
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.684838 FuncsForSPO-6.1.4/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.840744 FuncsForSPO-6.1.4/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.4/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.4/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.858668 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.886899 FuncsForSPO-6.1.4/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.4/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.930219 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.1.4/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.033113 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.087676 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.122363 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.142451 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.223918 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.483297 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.562031 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.572549 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.677497 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.696541 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.722865 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.757488 FuncsForSPO-6.1.4/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.1.4/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.789114 FuncsForSPO-6.1.4/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.4/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.817297 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.1.4/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.838433 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.857086 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:48.877560 FuncsForSPO-6.1.4/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.4/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:09:47.812907 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-06-26 14:09:47.000000 FuncsForSPO-6.1.4/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.4/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-26 14:09:48.986514 FuncsForSPO-6.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:09:48.994539 FuncsForSPO-6.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2661 2023-06-26 14:09:37.000000 FuncsForSPO-6.1.4/setup.py
```

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.1.4/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.1.4/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from fnmatch import fnmatch
 from time import sleep
 import os, sys, shutil, platform, re, logging, unicodedata, gc, requests, time, json, threading
 import subprocess as sp
 import zipfile
 from rich import print
 from numpy import unicode_
-from FuncsForSPO.fgpt.fgpt import *
 ################################## IMPORTS #############################################
 
 def remover_acentos(text:str, encoding:str='utf-8'):
 	try:
 		text = unicode_(text, encoding=encoding)
 	except Exception:
 		pass
@@ -1329,328 +1328,15 @@
             return valor
     valor = f'{valor:_.2f}'
     valor = valor.replace('.', ',').replace('_', '.')
     if sigl:
         return 'R$ '+valor
     return valor
 
-def cria_diretorios_para_novo_projeto_python(with_draft=False, create_base_dir:bool=True, packages:str='FuncsForSPO'):
-    """# ATENÇÃO, UTILIZAR SOMENTE UMA VEZ NO MOMENTO DA CRIAÇÃO DO NOVO PROJETO!
-    
-    create_base_dir: cria o diretorio para o user colocar a base
-    packages: instala pacotes necessários
-    
-    with_draft deve ser como nesse exemplo:
-        # 1. importe from src.base.base import * no app.py
-        # 2. crie um bot com o uso abaixo que entre nesse site: https://www.pythonanywhere.com/login/
-        # 3. envie o usuário que virá no arquivo config.json em BOT USUARIO nesse seletor: #id_auth-username
-        # 4. envie também a senha que virá no arquivo config.json em BOT SENHA nesse seletor: #id_auth-password
-        # 5. e clique em login nesse seletor: #id_next
-        # 6. espere 5 segundos
-        
-        o resultado esperado no arquivo app.py é:
-        
-        >>> from src.base.base import *
-        >>> class RobotClass(Bot):
-        >>>    def __init__(self) -> None:
-        >>>        self.configs = read_json(CONFIG_PATH)
-        >>>        self.HEADLESS = self.configs['BOT']['HEADLESS']
-        >>>        self.DOWNLOAD_FILES = False
-        >>>        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
-        >>>        
-        >>>    def run(self):
-        >>>        self.DRIVER.get("https://www.pythonanywhere.com/login/")
-        >>>        username = self.configs['BOT']['USUARIO']
-        >>>        password = self.configs['BOT']['SENHA']
-        >>>        self.WDW10.until(EC.presence_of_element_located((By.ID, 'id_auth-username')))
-        >>>        self.DRIVER.find_element_by_id('id_auth-username').send_keys(username)
-        >>>        self.DRIVER.find_element_by_id('id_auth-password').send_keys(password)
-        >>>        self.DRIVER.find_element_by_id('id_next').click()
-        >>>        time.sleep(5) # Espera 5 segundos antes de encerrar a execução.
-    """
-    faz_log('Criando pasta e arquivo de logs com esse log...')
-    # cria diretório src
-    cria_dir_no_dir_de_trabalho_atual('src')
-    APP_PATH = arquivo_com_caminho_absoluto(['src', 'app'], 'app.py')
-    BASE_PATH = arquivo_com_caminho_absoluto(['src', 'base'], 'base.py')
-    DATABASE_PATH = arquivo_com_caminho_absoluto(['src', 'database'], 'database.py')
-    EXCEPTIONS_PATH = arquivo_com_caminho_absoluto(['src', 'exceptions'], 'exceptioins.py')
-    CONFIG_PATH = arquivo_com_caminho_absoluto(['bin'], 'config.json')
-    UTILS_PATH = arquivo_com_caminho_absoluto(['src', 'utils'], 'utils.py')
-    TESTS_PATH = arquivo_com_caminho_absoluto(['src', 'tests'], 'tests.py')
-    # cria subdiretorios do src
-
-    if not isinstance(with_draft, str):
-        # CRIA ARQUIVO PYTHON EM SRC\\APP
-        with open(APP_PATH, 'w', encoding='utf-8') as f:
-            f.write("""from src.base.base import *
-    class RobotClass(Bot):
-        def __init__(self) -> None:
-            self.configs = read_json(CONFIG_PATH)
-            self.HEADLESS = self.configs['BOT']['HEADLESS']
-            self.DOWNLOAD_FILES = False
-            super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
-    """)
-    else:
-        print('Criando arquivo com draft... É MUITO IMPORTANTE VOCÊ VER SE FICOU BOM COMO O GPT ESCREVEU O CÓDIGO!\nEscreve apenas no arquivo app.py, se precisar colocar dados do usuário no Json, adiicone manualmente')
-        # CRIA ARQUIVO PYTHON EM SRC\\APP
-        from FuncsForSPO.utils.utils import GPT_WITH_DRAFT_PROMPT
-        response_gpt = gpt(GPT_WITH_DRAFT_PROMPT.replace('DRAFT_USER', with_draft))
-        with open(APP_PATH, 'w', encoding='utf-8') as f:
-            f.write(f"""from src.base.base import *
-class RobotClass(Bot):
-    def __init__(self) -> None:
-        self.configs = read_json(CONFIG_PATH)
-        self.HEADLESS = self.configs['BOT']['HEADLESS']
-        self.DOWNLOAD_FILES = False
-        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
-        
-    {response_gpt}
-""")
-
-    # CRIA ARQUIVO PYTHON EM base
-    with open(BASE_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from selenium.webdriver import Chrome
-from selenium import webdriver
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.chrome.options import Options as ChromeOptions
-from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.common.exceptions import *
-from webdriver_manager.chrome import ChromeDriverManager
-from FuncsForSPO.fpython.functions_for_py import *
-from FuncsForSPO.fselenium.functions_selenium import *
-from FuncsForSPO.fwinotify.fwinotify import *
-from FuncsForSPO.fregex.functions_re import *
-import pandas as pd
-import json
-import os
-
-# -- GLOBAL -- #
-URL_SUPORTE = f'https://api.whatsapp.com/send?phone=5511985640273'
-CONFIG_PATH = arquivo_com_caminho_absoluto('bin', 'config.json')
-BASE = os.path.abspath('base')
-DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir='downloads', print_value=False, criar_diretorio=True)
-limpa_diretorio(DOWNLOAD_DIR)
-# -- GLOBAL -- #
-
-class Bot:    
-    def __init__(self, headless, download_files) -> None:
-        # --- CHROME OPTIONS --- #
-        self._options = ChromeOptions()
-        
-        if download_files:
-            # --- PATH BASE DIR --- #
-            self._SETTINGS_SAVE_AS_PDF = {
-                        "recentDestinations": [
-                            {
-                                "id": "Save as PDF",
-                                "origin": "local",
-                                "account": ""
-                            }
-                        ],
-                        "selectedDestinationId": "Save as PDF",
-                        "version": 2,
-                    }
-
-
-            self._PROFILE = {'printing.print_preview_sticky_settings.appState': json.dumps(self._SETTINGS_SAVE_AS_PDF),
-                    "savefile.default_directory":  f"{DOWNLOAD_DIR}",
-                    "download.default_directory":  f"{DOWNLOAD_DIR}",
-                    "download.prompt_for_download": False,
-                    "download.directory_upgrade": True,
-                    "profile.managed_default_content_settings.images": 2,
-                    "safebrowsing.enabled": True}
-                
-            self._options.add_experimental_option('prefs', self._PROFILE)
-        
-        if headless == True:
-            self._options.add_argument('--headless')
-            
-        self._options.add_experimental_option("excludeSwitches", ["enable-logging", "enable-automation"])
-        self._options.add_experimental_option('useAutomationExtension', False)
-        self.user_agent = cria_user_agent()
-        self._options.add_argument(f"--user-agent=self.user_agent")
-        self._options.add_argument("--disable-web-security")
-        self._options.add_argument("--allow-running-insecure-content")
-        self._options.add_argument("--disable-extensions")
-        self._options.add_argument("--start-maximized")
-        self._options.add_argument("--no-sandbox")
-        self._options.add_argument("--disable-setuid-sandbox")
-        self._options.add_argument("--disable-infobars")
-        self._options.add_argument("--disable-webgl")
-        self._options.add_argument("--disable-popup-blocking")
-        self._options.add_argument('--disable-gpu')
-        self._options.add_argument('--disable-software-rasterizer')
-        self._options.add_argument('--no-proxy-server')
-        self._options.add_argument("--proxy-server='direct://'")
-        self._options.add_argument('--proxy-bypass-list=*')
-        self._options.add_argument('--disable-dev-shm-usage')
-        self._options.add_argument('--block-new-web-contents')
-        self._options.add_argument('--incognito')
-        self._options.add_argument('–disable-notifications')
-        self._options.add_argument("--window-size=1920,1080")
-        self._options.add_argument('--kiosk-printing')
-
-        
-        self.__service = Service(ChromeDriverManager().install())
-        
-        # create DRIVER
-        self.DRIVER = Chrome(service=self.__service, options=self._options)
-        
-        def enable_download_in_headless_chrome(driver, download_dir):
-            '''
-            Esse código adiciona suporte ao navegador Chrome sem interface gráfica (headless) no Selenium WebDriver para permitir o download automático de arquivos em um diretório especificado.
-
-            Mais especificamente, o código adiciona um comando ausente "send_command" ao executor de comando do driver e, em seguida, executa um comando "Page.setDownloadBehavior" para permitir o download automático de arquivos no diretório especificado.
-
-            O primeiro passo é necessário porque o suporte para o comando "send_command" não está incluído no Selenium WebDriver por padrão. O segundo passo usa o comando "Page.setDownloadBehavior" do Chrome DevTools Protocol para permitir o download automático de arquivos em um diretório especificado.
-
-            Em resumo, o código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome sem interface gráfica usando o Selenium WebDriver.
-            '''
-            driver.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
-
-            params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': download_dir}}
-            command_result = driver.execute("send_command", params)
-        enable_download_in_headless_chrome(self.DRIVER, DOWNLOAD_DIR)
-        
-        
-        self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
-        self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
-        self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
-        self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
-        self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
-        self.WDW = self.WDW7
-
-        self.DRIVER.maximize_window()
-        return self.DRIVER
-""")
-    
-    # CRIA ARQUIVO PYTHON EM database
-    with open(DATABASE_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from FuncsForSPO.fpython.functions_for_py import *
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy import Column, String, Integer
-
-engine = create_engine('sqlite:///database.db', pool_size=15, max_overflow=20)
-Base = declarative_base()
-Session = sessionmaker(bind=engine)
-
-
-class TABLE(Base):
-    __tablename__ = 'table'
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    status = Column(String)
-    nome = Column(String)
-    
-Base.metadata.create_all(engine)  # cria a tabela no banco de dados
-
-    
-class DBManager:
-    def __init__(self):
-        # Inicializa uma nova sessão com o banco de dados.
-        
-        self.session = Session()
-
-    def create_item(self, status, name):
-        # Cria um novo registro na tabela.
-
-        new_item = TABLE(status=status, name=name)
-        self.session.add(new_item)
-        self.session.commit()
-
-    def get_item(self, id):
-        # Retorna o registro com o ID fornecido
-        return self.session.query(TABLE).filter_by(id=id).first()
-    
-
-    def delete_item(self, id):
-        # Exclui o registro com o ID fornecido da tabela
-
-        delete_item_from_db = self.get_item(id)
-        self.session.delete(delete_item_from_db)
-        self.session.commit()
-        
-    def delete_all(self):
-        # Exclui todos os registros da tabela.
-
-        self.session.query(TABLE).delete()
-        self.session.commit()
 
-    def get_item(self, id):
-        # Retorna o registro com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
-        return self.session.query(TABLE).filter_by(id=id).first()
-    
-
-    def get_column_status(self):
-        # Retorna o registro de status com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
-        return self.session.query(TABLE.status).all()
-    
-    
-
-""")
-    
-    # CRIA ARQUIVO PYTHON EM exceptions
-    with open(EXCEPTIONS_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from FuncsForSPO.fexceptions.exceptions import *
-""")
-    
-    # cria arquivo json
-    with open(CONFIG_PATH, 'w', encoding='utf-8') as fjson:
-        fjson.write("""{
-    "BOT": {
-        "USER": "USER",
-        "PASSWORD": "PASSWORD",
-        "HEADLESS": true
-        }
-}""")
-        
-    # cria arquivo utils
-    with open(UTILS_PATH, 'w', encoding='utf-8') as fjson:
-        fjson.write("""""")
-
-    # cria arquivo de tests
-    with open(TESTS_PATH, 'w', encoding='utf-8') as fjson:
-        fjson.write("""from FuncsForSPO.fpdf.focr.orc import *
-from FuncsForSPO.fpdf.fcompress.compress import *
-from FuncsForSPO.fpdf.fimgpdf.img_to_pdf import *
-from FuncsForSPO.fpysimplegui.functions_for_sg import *
-from FuncsForSPO.fpython.functions_for_py import *
-from FuncsForSPO.fregex.functions_re import *
-from FuncsForSPO.fselenium.functions_selenium import *
-import sys
-import os
-
-root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-sys.path.append(root_dir)
-
-# SEMPRE COLOQUE O QUE A FUNÇÃO TEM QUE FAZER EXPLICITAMENTE
-""")
-
-    # cria diretório base
-    if create_base_dir:
-        cria_dir_no_dir_de_trabalho_atual('base')
-
-    # cria ambiente virtual
-    # if os.path.exists('venv'):
-    #     print('Ambiente Virtual "venv" já criado')
-    #     print('Baixando pacotes')
-    #     os.system(f'.\\venv\\Scripts\\pip.exe install {packages}')
-    #     pass
-    # else:
-    print('Criando Ambiente Virtual')
-    os.system('python -m venv venv')
-    print('Criado!')
-    print('Baixando pacotes')
-    os.system(f'.\\venv\Scripts\\pip.exe install {packages}')
-    
 def retorna_a_menor_ou_maior_data(datas:list[str|datetime], maior:bool=True, format:str='%d/%m/%Y %H:%M', format_return:str='%d/%m/%Y %H:%M'):
     """
     ## Recebe e retorna a MAIOR ou a menor data de uma lista de datas
     
     ### caso a lista de datas seja datetime, ele não haverá conversão
 
     ### É necessário que todas as datas estejam no padrão do formato enviado no parâmetro format
```

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from selenium.webdriver import Chrome 
 from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from webdriver_manager.chrome import ChromeDriverManager 
 from time import sleep
-from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fregex.functions_re import extrair_email
 from wget import download
 from subprocess import getoutput
-from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.utils.utils import *
+from FuncsForSPO.fpython.functions_for_py import *
 
 def url_atual(driver) -> str:
     """
     ### Função RETORNA a url atual
 
     Args:
         driver (WebDriver): Seu Webdriver (Chrome, Firefox, Opera...)
```

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.1.4/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.1.4/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.1.4/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.3
+Version: 6.1.4
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.3/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.1.4/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/LICENSE` & `FuncsForSPO-6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/PKG-INFO` & `FuncsForSPO-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.3
+Version: 6.1.4
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.3/README.md` & `FuncsForSPO-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.3/setup.py` & `FuncsForSPO-6.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.1.3'
+version = '6.1.4'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

