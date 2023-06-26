# Comparing `tmp/SFlock2-0.3.50.tar.gz` & `tmp/SFlock2-0.3.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFlock2-0.3.50.tar", last modified: Thu Jun 22 07:08:31 2023, max compression
+gzip compressed data, was "SFlock2-0.3.51.tar", last modified: Mon Jun 26 09:08:29 2023, max compression
```

## Comparing `SFlock2-0.3.50.tar` & `SFlock2-0.3.51.tar`

### file list

```diff
@@ -1,97 +1,64 @@
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.682353 SFlock2-0.3.50/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      370 2020-06-10 09:29:08.000000 SFlock2-0.3.50/MANIFEST.in
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-06-22 07:08:31.682082 SFlock2-0.3.50/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2712 2021-07-20 07:58:43.000000 SFlock2-0.3.50/README.md
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.594246 SFlock2-0.3.50/SFlock2.egg-info/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1807 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/SOURCES.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/dependency_links.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       44 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/entry_points.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      132 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/requires.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        7 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/top_level.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       38 2023-06-22 07:08:31.682435 SFlock2-0.3.50/setup.cfg
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1880 2023-02-01 06:49:14.000000 SFlock2-0.3.50/setup.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.603758 SFlock2-0.3.50/sflock/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:59.000000 SFlock2-0.3.50/sflock/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      335 2021-07-15 18:56:48.000000 SFlock2-0.3.50/sflock/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      100 2023-06-22 06:35:49.000000 SFlock2-0.3.50/sflock/__version__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15303 2022-03-08 17:08:56.000000 SFlock2-0.3.50/sflock/abstracts.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.606033 SFlock2-0.3.50/sflock/aux/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/aux/__init__.py
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)     8734 2021-07-16 12:01:23.000000 SFlock2-0.3.50/sflock/aux/decode_vbe_jse.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.607848 SFlock2-0.3.50/sflock/compat/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      152 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/compat/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1295 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/compat/magic.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      564 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/config.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.616779 SFlock2-0.3.50/sflock/data/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:22.000000 SFlock2-0.3.50/sflock/data/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      157 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       26 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/data/password.txt
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   668240 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/poweriso.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.628566 SFlock2-0.3.50/sflock/data/win32/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   536241 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   150016 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/magic1.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    79360 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/regex2.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    72192 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/zlib1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.644682 SFlock2-0.3.50/sflock/data/win64/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    67720 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/libgnurx-0.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)  2944752 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   717504 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/magic1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.650562 SFlock2-0.3.50/sflock/data/yara/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      464 2022-09-02 19:41:32.000000 SFlock2-0.3.50/sflock/data/yara/archives.yar
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    11391 2022-02-19 08:23:06.000000 SFlock2-0.3.50/sflock/data/yara/shellcodes.yar
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   873032 2023-01-31 10:07:30.000000 SFlock2-0.3.50/sflock/data/zipjail.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.652418 SFlock2-0.3.50/sflock/decode/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      302 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/decode/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5967 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/decode/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      364 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/exception.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15097 2023-06-22 06:59:19.000000 SFlock2-0.3.50/sflock/ident.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3271 2023-01-19 07:23:25.000000 SFlock2-0.3.50/sflock/main.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1328 2021-12-08 14:30:13.000000 SFlock2-0.3.50/sflock/misc.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4280 2022-01-14 07:58:22.000000 SFlock2-0.3.50/sflock/pick.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.662249 SFlock2-0.3.50/sflock/unpack/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      309 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/unpack/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1276 2023-01-31 10:07:51.000000 SFlock2-0.3.50/sflock/unpack/ace.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1570 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/bup.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      945 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/cab.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1065 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/daa.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2180 2021-12-29 11:09:37.000000 SFlock2-0.3.50/sflock/unpack/eml.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1838 2021-07-16 14:34:19.000000 SFlock2-0.3.50/sflock/unpack/lzip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2055 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/msg.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2225 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/mso.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      977 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2468 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/pdf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      932 2022-03-08 17:08:34.000000 SFlock2-0.3.50/sflock/unpack/rar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5029 2022-01-14 07:58:22.000000 SFlock2-0.3.50/sflock/unpack/tar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6216 2022-10-27 10:01:06.000000 SFlock2-0.3.50/sflock/unpack/zip7.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.681150 SFlock2-0.3.50/tests/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5150 2022-10-27 10:16:35.000000 SFlock2-0.3.50/tests/test_7z.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3436 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_ace.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1046 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_attr.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1414 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_bup.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1991 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_cab.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      974 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_daa.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1066 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_decode.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      324 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_elf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3518 2022-12-14 17:01:41.000000 SFlock2-0.3.50/tests/test_eml.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      954 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_exts.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1599 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_file.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2833 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_ident.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      996 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_lzh.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1222 2021-07-16 14:54:32.000000 SFlock2-0.3.50/tests/test_lzip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      704 2021-07-16 12:01:23.000000 SFlock2-0.3.50/tests/test_magic.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1169 2022-10-27 10:19:03.000000 SFlock2-0.3.50/tests/test_main.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      459 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_misc.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3005 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_msg.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      506 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_mso.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1563 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6870 2021-12-08 14:59:59.000000 SFlock2-0.3.50/tests/test_package.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2093 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_pdf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1370 2021-12-08 14:59:59.000000 SFlock2-0.3.50/tests/test_pick.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4556 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_rar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      524 2022-10-27 10:07:17.000000 SFlock2-0.3.50/tests/test_shellcode.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     7291 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_tar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    17695 2022-02-19 09:29:07.000000 SFlock2-0.3.50/tests/test_unpack.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1486 2021-07-16 16:51:56.000000 SFlock2-0.3.50/tests/test_win.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     8544 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_zip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1689 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_zipify.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.894867 SFlock2-0.3.51/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      370 2023-06-26 09:04:21.000000 SFlock2-0.3.51/MANIFEST.in
+-rw-r--r--   0 doomedraven   (501) staff       (20)      883 2023-06-26 09:08:29.894351 SFlock2-0.3.51/PKG-INFO
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2712 2023-06-26 09:04:21.000000 SFlock2-0.3.51/README.md
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.798071 SFlock2-0.3.51/SFlock2.egg-info/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      883 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/PKG-INFO
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1196 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/SOURCES.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)        1 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/dependency_links.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)       45 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/entry_points.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)      132 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/requires.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)        7 2023-06-26 09:08:29.000000 SFlock2-0.3.51/SFlock2.egg-info/top_level.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)       38 2023-06-26 09:08:29.895053 SFlock2-0.3.51/setup.cfg
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1880 2023-06-26 09:04:21.000000 SFlock2-0.3.51/setup.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.809065 SFlock2-0.3.51/sflock/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      335 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      100 2023-06-26 09:07:23.000000 SFlock2-0.3.51/sflock/__version__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)    15303 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/abstracts.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.810774 SFlock2-0.3.51/sflock/aux/
+-rw-r--r--   0 doomedraven   (501) staff       (20)        1 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/aux/__init__.py
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)     7367 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/aux/decode_vbe_jse.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.812482 SFlock2-0.3.51/sflock/compat/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      152 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/compat/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1295 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/compat/magic.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      564 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/config.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.827252 SFlock2-0.3.51/sflock/data/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      157 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)       26 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/password.txt
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)   668240 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/poweriso.elf
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.844606 SFlock2-0.3.51/sflock/data/win32/
+-rw-r--r--   0 doomedraven   (501) staff       (20)   536241 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win32/magic.mgc
+-rw-r--r--   0 doomedraven   (501) staff       (20)   150016 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win32/magic1.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)    79360 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win32/regex2.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)    72192 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win32/zlib1.dll
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.865595 SFlock2-0.3.51/sflock/data/win64/
+-rw-r--r--   0 doomedraven   (501) staff       (20)    67720 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win64/libgnurx-0.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)  2944752 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win64/magic.mgc
+-rw-r--r--   0 doomedraven   (501) staff       (20)   717504 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/win64/magic1.dll
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.873260 SFlock2-0.3.51/sflock/data/yara/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      464 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/yara/archives.yar
+-rw-r--r--   0 doomedraven   (501) staff       (20)    11391 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/yara/shellcodes.yar
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)   873032 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/data/zipjail.elf
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.875604 SFlock2-0.3.51/sflock/decode/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      302 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/decode/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     5967 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/decode/office.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      364 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/exception.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)    15742 2023-06-26 09:07:15.000000 SFlock2-0.3.51/sflock/ident.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     3271 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/main.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1328 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/misc.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     4280 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/pick.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2023-06-26 09:08:29.893373 SFlock2-0.3.51/sflock/unpack/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      309 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1276 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/ace.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1570 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/bup.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      945 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/cab.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1065 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/daa.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2180 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/eml.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1838 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/lzip.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2055 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/msg.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2225 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/mso.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      977 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/office.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2468 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/pdf.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      932 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/rar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     5029 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/tar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     6216 2023-06-26 09:04:21.000000 SFlock2-0.3.51/sflock/unpack/zip7.py
```

### Comparing `SFlock2-0.3.50/PKG-INFO` & `SFlock2-0.3.51/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.50
+Version: 0.3.51
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Provides-Extra: dev
 Provides-Extra: shellcode
+
+UNKNOWN
+
```

### Comparing `SFlock2-0.3.50/README.md` & `SFlock2-0.3.51/README.md`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/SFlock2.egg-info/PKG-INFO` & `SFlock2-0.3.51/SFlock2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.50
+Version: 0.3.51
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Provides-Extra: dev
 Provides-Extra: shellcode
+
+UNKNOWN
+
```

### Comparing `SFlock2-0.3.50/setup.py` & `SFlock2-0.3.51/setup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/abstracts.py` & `SFlock2-0.3.51/sflock/abstracts.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/compat/magic.py` & `SFlock2-0.3.51/sflock/compat/magic.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/config.py` & `SFlock2-0.3.51/sflock/config.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/poweriso.elf` & `SFlock2-0.3.51/sflock/data/poweriso.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win32/magic.mgc` & `SFlock2-0.3.51/sflock/data/win32/magic.mgc`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win32/magic1.dll` & `SFlock2-0.3.51/sflock/data/win32/magic1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win32/regex2.dll` & `SFlock2-0.3.51/sflock/data/win32/regex2.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win32/zlib1.dll` & `SFlock2-0.3.51/sflock/data/win32/zlib1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win64/libgnurx-0.dll` & `SFlock2-0.3.51/sflock/data/win64/libgnurx-0.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win64/magic.mgc` & `SFlock2-0.3.51/sflock/data/win64/magic.mgc`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/win64/magic1.dll` & `SFlock2-0.3.51/sflock/data/win64/magic1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/yara/shellcodes.yar` & `SFlock2-0.3.51/sflock/data/yara/shellcodes.yar`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/data/zipjail.elf` & `SFlock2-0.3.51/sflock/data/zipjail.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/decode/office.py` & `SFlock2-0.3.51/sflock/decode/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/ident.py` & `SFlock2-0.3.51/sflock/ident.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 # This file is part of SFlock - http://www.sflock.org/.
 # See the file 'docs/LICENSE.txt' for copying permission.
 import os
 import re
 from collections import OrderedDict
 
 import pefile
-from sflock.aux.decode_vbe_jse import DecodeVBEJSE
+from sflock.aux.decode_vbe_jse import decode_file as vbe_decode_file
+
 
 try:
     import yara
+
     cur_dir = os.path.dirname(os.path.abspath(__file__))
     shellcode_rules = yara.compile(filepath=os.path.join(cur_dir, "data", "yara", "shellcodes.yar"))
     archives_rules = yara.compile(filepath=os.path.join(cur_dir, "data", "yara", "archives.yar"))
     HAVE_YARA = True
 except ImportError:
     HAVE_YARA = False
 
 
 try:
     from unicorn import Uc, UC_MODE_32, UC_MODE_64, UC_ARCH_X86, UC_HOOK_CODE, unicorn
     from unicorn.x86_const import UC_X86_REG_ESP
+
     HAVE_UNICORN = True
 except ImportError:
     HAVE_UNICORN = False
 
 shellcode_code_base = 0x100000
 shellcode_threshold = 0x100
 shellcode_limit = 0x100000
@@ -32,26 +35,62 @@
 file_extensions = OrderedDict(
     [
         ("access", (b".accdr",)),
         ("msi", (b".msi", b".msp", b".appx")),
         ("msix", (b".msix", b".msixbundle")),
         ("pub", (b".pub",)),
         ("doc", (b".doc", b".dot", b".docx", b".dotx", b".docm", b".dotm", b".docb", b".rtf", b".mht", b".mso", b".wbk", b".wiz")),
-        ("xls", (b".xls", b".xlt", b".xlm", b".xlsx", b".xltx", b".xlsm", b".xltm", b".xlsb", b".xla", b".xlam", b".xll", b".xlw", b".slk", b".xll", b".csv")),
-        ("ppt", (b".ppt", b".ppa", b".pot", b".pps", b".pptx", b".pptm", b".potx", b".potm", b".ppam", b".ppsx", b".ppsm", b".sldx", b".sldm")),
+        (
+            "xls",
+            (
+                b".xls",
+                b".xlt",
+                b".xlm",
+                b".xlsx",
+                b".xltx",
+                b".xlsm",
+                b".xltm",
+                b".xlsb",
+                b".xla",
+                b".xlam",
+                b".xll",
+                b".xlw",
+                b".slk",
+                b".xll",
+                b".csv",
+            ),
+        ),
+        (
+            "ppt",
+            (
+                b".ppt",
+                b".ppa",
+                b".pot",
+                b".pps",
+                b".pptx",
+                b".pptm",
+                b".potx",
+                b".potm",
+                b".ppam",
+                b".ppsx",
+                b".ppsm",
+                b".sldx",
+                b".sldm",
+            ),
+        ),
         ("jar", (b".jar",)),
         # ("rar", (b".rar",)),
         ("reg", (b".reg",)),
         ("swf", (b".swf", b".fws")),
         ("python", (b".py", b".pyc", b".pyw")),
         ("ps1", (b".ps1",)),
         # ("msg", (b".msg",, b".rpmsg")),
         # ("eml", (b".eml", b".ics")),
         ("js", (b".js", b".jse")),
-        ("ie", (b".html", b".url")), # b".htm",
+        ("ie", (b".html", b".url")),  # b".htm",
         ("xps", (b".xps",)),
         ("hta", (b".hta",)),
         ("mht", (b".mht",)),
         ("lnk", (b".lnk",)),
         ("chm", (b".chm",)),
         ("hwp", (b".hwp", b".hwpx", b".hwt", b".hml")),
         ("inp", (b".inp", b".int")),
@@ -104,15 +143,15 @@
         # ToDo msdos
         ("ACE archive data", "ace"),
         ("PE32 executable (DLL)", "dll"),
         ("PE32+ executable (DLL)", "dll"),
         ("MS-DOS executable PE32 executable (DLL)", "dll"),
         ("PE32 executable", "exe"),
         ("PE32+ executable", "exe"),
-        ('MS-DOS executable, MZ for MS-DOS', "exe"),
+        ("MS-DOS executable, MZ for MS-DOS", "exe"),
         ("Microsoft PowerPoint", "ppt"),
         ("Microsoft Office Excel", "xls"),
         ("Microsoft Excel", "xls"),
         ("Rich Text Format", "doc"),
         ("Microsoft Office Word", "doc"),
         ("Microsoft Word", "doc"),
         ("Microsoft OOXML", "doc"),
@@ -146,15 +185,19 @@
         ("META-INF/MANIFEST.MF", "jar"),
         ("Java Jar file data (zip)", "jar"),
         ("Java archive data (JAR)", "jar"),
         # ("HTML", "html"),
     ]
 )
 
+
 def detect_shellcode(f):
+
+    if f.contents[6:10] == b"JFIF":
+        return
     """
     if HAVE_YARA:
         matches = shellcode_rules.match(data=f.contents)
         if matches:
             return "Shellcode"
     """
     global shellcode_count32, shellcode_count64, shellcode_last_address
@@ -170,50 +213,56 @@
         shellcode_count32 = 0
     if shellcode_count64 > shellcode_threshold and shellcode_count64 > shellcode_count32:
         return "Shellcode_x64"
     elif shellcode_count32 > shellcode_threshold and shellcode_count32 > shellcode_count64:
         return "Shellcode"
     return False
 
+
 def hook_instr(uc, address, size, mode):
     global shellcode_count32, shellcode_count64, shellcode_last_address
     if mode == UC_MODE_32:
         shellcode_count32 += 1
     elif mode == UC_MODE_64:
         shellcode_count64 += 1
     shellcode_last_address = address
 
+
 def emulate(data, mode):
     try:
         stack = 0x90000
         uc = Uc(UC_ARCH_X86, mode)
-        uc.mem_map(stack, 0x1000*10)
+        uc.mem_map(stack, 0x1000 * 10)
         uc.mem_map(shellcode_code_base, 0x100000)
         uc.mem_write(shellcode_code_base, data)
-        uc.reg_write(UC_X86_REG_ESP, stack+0x1000)
+        uc.reg_write(UC_X86_REG_ESP, stack + 0x1000)
         uc.hook_add(UC_HOOK_CODE, hook_instr, user_data=mode)
-        uc.emu_start(shellcode_code_base, shellcode_code_base+len(data), 0, shellcode_limit)
+        uc.emu_start(shellcode_code_base, shellcode_code_base + len(data), 0, shellcode_limit)
     except unicorn.UcError:
         pass
 
+
 def inp(f):
     if b"InPage Arabic Document" in f.contents:
         return "inp"
 
+
 def mso(f):
     if b"mso-application" in f.contents and b"Word.Document" in f.contents:
         return "doc"
 
+
 def sct(f):
     if f.filename and f.filename.endswith(b".sct"):
-        if re.search(br"(?is)<\?XML.*?<scriptlet.*?<registration", f.contents):
+        if re.search(rb"(?is)<\?XML.*?<scriptlet.*?<registration", f.contents):
             return "sct"
         else:
             return "hta"
 
+
 def xxe(f):
     if f.contents.startswith(b"MZ"):
         return None
 
     STRINGS = [
         b"XXEncode",
         b"begin",
@@ -255,18 +304,20 @@
     found = 0
     for string in STRINGS:
         found += f.contents.count(string)
 
     if found >= 10:
         return "hta"
 
+
 def office_one(f):
     if f.contents.startswith(b"\xE4\x52\x5C\x7B\x8C\xD8\xA7\x4D\xAE\xB1\x53\x78\xD0\x29\x96\xD3"):
         return "one"
 
+
 def office_webarchive(f):
     if f.contents.startswith(b"MZ"):
         return None
 
     STRINGS = [
         b"<o:Pages>",
         b"<o:DocumentProperties>",
@@ -300,18 +351,20 @@
         return "doc"
 
 
 def office_activemime(f):
     if f.contents.startswith((b"QWN0aXZlTWltZQ", b"ActiveMime")):
         return "doc"
 
+
 def msix(f):
     if all([pattern in f.contents for pattern in (b"Registry.dat", b"AppxManifest.xml")]):
         return "msix"
 
+
 def office_zip(f):
     if not f.get_child(b"[Content_Types].xml"):
         return
 
     if f.get_child(b"workbook.bin"):
         return "xls"
 
@@ -472,30 +525,31 @@
 
 
 def vbe_jse(f):
     if f.contents.startswith(b"MZ"):
         return None
 
     if b"#@~^" in f.contents[:100]:
-        data = DecodeVBEJSE(f.contents, "")
+        data = vbe_decode_file("", f.contents)
         if data:
-            if re.findall(b"\s?Dim\s", data, re.I):
+            if re.findall(rb"\s?Dim\s", data, re.I):
                 return "vbs"
             else:
                 return "js"
         else:
             return "vbejse"
 
 
 def udf(f):
     if HAVE_YARA:
         matches = archives_rules.match(data=f.contents)
         if "archive_udf" in [rule.rule for rule in matches]:
             return "udf"
 
+
 def inf(f):
     if f.contents.startswith(b"MZ"):
         return None
 
     STRINGS = [
         # b"[version]",
         b"Signature=",
@@ -550,14 +604,15 @@
             return magics[magic_types]
     if f.mime in mimes:
         return mimes[f.mime]
 
     if check_shellcode:
         return detect_shellcode(f)
 
+
 identifiers_special = [
     msix,
 ]
 
 identifiers = [
     udf,
     dmg,
```

### Comparing `SFlock2-0.3.50/sflock/main.py` & `SFlock2-0.3.51/sflock/main.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/misc.py` & `SFlock2-0.3.51/sflock/misc.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/pick.py` & `SFlock2-0.3.51/sflock/pick.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/ace.py` & `SFlock2-0.3.51/sflock/unpack/ace.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/bup.py` & `SFlock2-0.3.51/sflock/unpack/bup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/cab.py` & `SFlock2-0.3.51/sflock/unpack/cab.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/daa.py` & `SFlock2-0.3.51/sflock/unpack/daa.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/eml.py` & `SFlock2-0.3.51/sflock/unpack/eml.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/lzip.py` & `SFlock2-0.3.51/sflock/unpack/lzip.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/msg.py` & `SFlock2-0.3.51/sflock/unpack/msg.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/mso.py` & `SFlock2-0.3.51/sflock/unpack/mso.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/office.py` & `SFlock2-0.3.51/sflock/unpack/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/pdf.py` & `SFlock2-0.3.51/sflock/unpack/pdf.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/rar.py` & `SFlock2-0.3.51/sflock/unpack/rar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/tar.py` & `SFlock2-0.3.51/sflock/unpack/tar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.50/sflock/unpack/zip7.py` & `SFlock2-0.3.51/sflock/unpack/zip7.py`

 * *Files identical despite different names*

