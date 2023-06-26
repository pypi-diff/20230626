# Comparing `tmp/yeastvision-0.1.4.tar.gz` & `tmp/yeastvision-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastvision-0.1.4.tar", last modified: Wed Jun 21 06:14:48 2023, max compression
+gzip compressed data, was "yeastvision-0.1.5.tar", last modified: Mon Jun 26 13:35:08 2023, max compression
```

## Comparing `yeastvision-0.1.4.tar` & `yeastvision-0.1.5.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.439289 yeastvision-0.1.4/
--rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.4/LICENSE
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-21 06:14:48.438418 yeastvision-0.1.4/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     3290 2023-06-21 06:06:54.000000 yeastvision-0.1.4/README.md
--rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-21 06:14:48.439444 yeastvision-0.1.4/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1750 2023-06-21 06:14:44.000000 yeastvision-0.1.4/setup.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.408401 yeastvision-0.1.4/yeastvision/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.4/yeastvision/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)    80734 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/__main__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.412670 yeastvision-0.1.4/yeastvision/disk/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.4/yeastvision/disk/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1019 2023-06-13 10:01:19.000000 yeastvision-0.1.4/yeastvision/disk/io.py
--rw-rw-r--   0 berk       (502) staff       (20)    10386 2023-06-13 10:01:09.000000 yeastvision-0.1.4/yeastvision/disk/reader.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.414329 yeastvision-0.1.4/yeastvision/flou/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.4/yeastvision/flou/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.4/yeastvision/flou/blob_detect.py
--rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.4/yeastvision/flou/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2688 2023-06-20 19:25:38.000000 yeastvision-0.1.4/yeastvision/ims.py
--rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.4/yeastvision/install_weights.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.418146 yeastvision-0.1.4/yeastvision/models/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.420041 yeastvision-0.1.4/yeastvision/models/YeaZ/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.4/yeastvision/models/YeaZ/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.4/yeastvision/models/YeaZ/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.4/yeastvision/models/YeaZ/segment.py
--rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.4/yeastvision/models/YeaZ/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.4/yeastvision/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.421110 yeastvision-0.1.4/yeastvision/models/artilife/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.4/yeastvision/models/artilife/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.421950 yeastvision-0.1.4/yeastvision/models/artilife/budSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.4/yeastvision/models/artilife/budSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/models/artilife/budSeg/model.py
--rw-r--r--   0 berk       (502) staff       (20)     8908 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/models/artilife/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.422789 yeastvision-0.1.4/yeastvision/models/budNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.4/yeastvision/models/budNET/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.4/yeastvision/models/budNET/model.py
--rw-r--r--   0 berk       (502) staff       (20)     3736 2023-06-13 09:59:29.000000 yeastvision-0.1.4/yeastvision/models/cp.py
--rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.4/yeastvision/models/eval.py
--rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.4/yeastvision/models/loss.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.423761 yeastvision-0.1.4/yeastvision/models/matSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.4/yeastvision/models/matSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.4/yeastvision/models/matSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.4/yeastvision/models/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.424613 yeastvision-0.1.4/yeastvision/models/tetradSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.4/yeastvision/models/tetradSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.4/yeastvision/models/tetradSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.4/yeastvision/models/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.4/yeastvision/models/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.425546 yeastvision-0.1.4/yeastvision/models/vacNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.4/yeastvision/models/vacNET/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.4/yeastvision/models/vacNET/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.428227 yeastvision-0.1.4/yeastvision/parts/
--rw-r--r--   0 berk       (502) staff       (20)    13222 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/parts/canvas.py
--rw-r--r--   0 berk       (502) staff       (20)    30883 2023-06-13 09:57:15.000000 yeastvision-0.1.4/yeastvision/parts/dialogs.py
--rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.4/yeastvision/parts/guiparts.py
--rw-r--r--   0 berk       (502) staff       (20)     3879 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/parts/menu.py
--rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.4/yeastvision/parts/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.430029 yeastvision-0.1.4/yeastvision/plot/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.4/yeastvision/plot/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3442 2023-06-14 19:37:54.000000 yeastvision-0.1.4/yeastvision/plot/cell_table.py
--rw-r--r--   0 berk       (502) staff       (20)    11297 2023-06-21 06:06:54.000000 yeastvision-0.1.4/yeastvision/plot/plot.py
--rw-r--r--   0 berk       (502) staff       (20)     1149 2023-04-05 22:48:46.000000 yeastvision-0.1.4/yeastvision/plot/types.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.436972 yeastvision-0.1.4/yeastvision/track/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.4/yeastvision/track/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     5908 2023-06-13 09:55:42.000000 yeastvision-0.1.4/yeastvision/track/cell.py
--rw-r--r--   0 berk       (502) staff       (20)      265 2023-06-07 05:33:05.000000 yeastvision-0.1.4/yeastvision/track/data.py
--rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.4/yeastvision/track/hungarian_track.py
--rw-rw-r--   0 berk       (502) staff       (20)     5515 2023-06-13 09:56:06.000000 yeastvision-0.1.4/yeastvision/track/lineage.py
--rw-r--r--   0 berk       (502) staff       (20)    18020 2023-06-20 20:03:01.000000 yeastvision-0.1.4/yeastvision/track/mat.py
--rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.4/yeastvision/track/track.py
--rw-r--r--   0 berk       (502) staff       (20)     5270 2023-06-20 19:16:44.000000 yeastvision-0.1.4/yeastvision/track/utils.py
--rw-rw-r--   0 berk       (502) staff       (20)     5491 2023-06-20 19:25:28.000000 yeastvision-0.1.4/yeastvision/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-21 06:14:48.411347 yeastvision-0.1.4/yeastvision.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     1796 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)      116 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      273 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-21 06:14:48.000000 yeastvision-0.1.4/yeastvision.egg-info/top_level.txt
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.174233 yeastvision-0.1.5/
+-rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.5/LICENSE
+-rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-26 13:35:08.173531 yeastvision-0.1.5/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     3290 2023-06-21 06:06:54.000000 yeastvision-0.1.5/README.md
+-rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-26 13:35:08.174427 yeastvision-0.1.5/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1750 2023-06-26 13:34:56.000000 yeastvision-0.1.5/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.125526 yeastvision-0.1.5/yeastvision/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.5/yeastvision/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)    80239 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/__main__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.131049 yeastvision-0.1.5/yeastvision/disk/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.5/yeastvision/disk/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/disk/io.py
+-rw-rw-r--   0 berk       (502) staff       (20)    10386 2023-06-13 10:01:09.000000 yeastvision-0.1.5/yeastvision/disk/reader.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.133063 yeastvision-0.1.5/yeastvision/flou/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.5/yeastvision/flou/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.5/yeastvision/flou/blob_detect.py
+-rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.5/yeastvision/flou/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     2688 2023-06-20 19:25:38.000000 yeastvision-0.1.5/yeastvision/ims.py
+-rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.5/yeastvision/install_weights.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.139287 yeastvision-0.1.5/yeastvision/models/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.142429 yeastvision-0.1.5/yeastvision/models/YeaZ/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/segment.py
+-rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.5/yeastvision/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.144177 yeastvision-0.1.5/yeastvision/models/artilife/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.5/yeastvision/models/artilife/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.145580 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     9440 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/models/artilife/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.146804 yeastvision-0.1.5/yeastvision/models/budNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.5/yeastvision/models/budNET/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.5/yeastvision/models/budNET/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     3774 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/models/cp.py
+-rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.5/yeastvision/models/eval.py
+-rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.5/yeastvision/models/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.148098 yeastvision-0.1.5/yeastvision/models/matSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.5/yeastvision/models/matSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.5/yeastvision/models/matSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.5/yeastvision/models/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.149815 yeastvision-0.1.5/yeastvision/models/tetradSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.5/yeastvision/models/tetradSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.5/yeastvision/models/tetradSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.5/yeastvision/models/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.5/yeastvision/models/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.151610 yeastvision-0.1.5/yeastvision/models/vacNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.5/yeastvision/models/vacNET/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.5/yeastvision/models/vacNET/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.161736 yeastvision-0.1.5/yeastvision/parts/
+-rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/canvas.py
+-rw-r--r--   0 berk       (502) staff       (20)    30883 2023-06-13 09:57:15.000000 yeastvision-0.1.5/yeastvision/parts/dialogs.py
+-rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.5/yeastvision/parts/guiparts.py
+-rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/menu.py
+-rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.5/yeastvision/parts/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     2737 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/workers.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.165173 yeastvision-0.1.5/yeastvision/plot/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.5/yeastvision/plot/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3442 2023-06-14 19:37:54.000000 yeastvision-0.1.5/yeastvision/plot/cell_table.py
+-rw-r--r--   0 berk       (502) staff       (20)    11676 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/plot/plot.py
+-rw-r--r--   0 berk       (502) staff       (20)     1149 2023-04-05 22:48:46.000000 yeastvision-0.1.5/yeastvision/plot/types.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.171985 yeastvision-0.1.5/yeastvision/track/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.5/yeastvision/track/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     5908 2023-06-13 09:55:42.000000 yeastvision-0.1.5/yeastvision/track/cell.py
+-rw-r--r--   0 berk       (502) staff       (20)      265 2023-06-07 05:33:05.000000 yeastvision-0.1.5/yeastvision/track/data.py
+-rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.5/yeastvision/track/hungarian_track.py
+-rw-r--r--   0 berk       (502) staff       (20)     5510 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/track/lineage.py
+-rw-r--r--   0 berk       (502) staff       (20)    18190 2023-06-22 04:45:43.000000 yeastvision-0.1.5/yeastvision/track/mat.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.5/yeastvision/track/track.py
+-rw-r--r--   0 berk       (502) staff       (20)     5270 2023-06-20 19:16:44.000000 yeastvision-0.1.5/yeastvision/track/utils.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5491 2023-06-20 19:25:28.000000 yeastvision-0.1.5/yeastvision/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.129259 yeastvision-0.1.5/yeastvision.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     1825 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)      116 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      273 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/top_level.txt
```

### Comparing `yeastvision-0.1.4/LICENSE` & `yeastvision-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/PKG-INFO` & `yeastvision-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `yeastvision-0.1.4/README.md` & `yeastvision-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/setup.py` & `yeastvision-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             "yeastvision.models.vacNET", "yeastvision.models.YeaZ"]
 
 
 
 
 setup(
     name = "yeastvision",
-    version = "0.1.4",
+    version = "0.1.5",
     description = "Deep learning-enabled image analysis of the yeast full life cycle",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/yeastvision",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
```

### Comparing `yeastvision-0.1.4/yeastvision/__main__.py` & `yeastvision-0.1.5/yeastvision/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
                              QFileDialog, QVBoxLayout, QCheckBox, QFrame, QSpinBox, QLabel, QWidget, QComboBox, QSizePolicy, QGridLayout)
 from PyQt5.QtCore import Qt
 import pyqtgraph as pg
 import numpy as np
 import matplotlib.pyplot as plt
 from yeastvision.parts.canvas import ImageDraw, ViewBoxNoRightDrag
 from yeastvision.parts.guiparts import *
+from yeastvision.parts.workers import SegmentWorker
 from yeastvision.parts.dialogs import *
 from yeastvision.track.track import track_to_cell, trackYeasts
 from yeastvision.track.data import LineageData
 from yeastvision.track.lineage import LineageConstruction
 from yeastvision.track.cell import LABEL_PROPS, IM_PROPS, EXTRA_IM_PROPS, getCellData, exportCellData, getHeatMaps, getDaughterMatrix
 import cv2
 from yeastvision.disk.reader import loadPkl, ImageData, MaskData
@@ -51,33 +52,24 @@
         self.setFrameShape(QFrame.VLine)
         self.setFrameShadow(QFrame.Sunken)
 
 
 class Worker(QtCore.QObject):
     '''Handles Multithreading'''
     finished = QtCore.pyqtSignal()
-    def __init__(self, parent, process, button = None, thread = None):
+    def __init__(self, parent, process, button = None):
         super(Worker,self).__init__()
         self.parent = parent
         self.process = process
         self.button = button
-        self.thread = thread
-        self.finished.connect(self.handleFinished)
         self.error = False
-
-    def handleFinished(self, error = False):
-        if self.button:
-            self.parent.activateButton(self.button)
-        self.parent.statusBar.clearMessage()
-        self.parent.closeThread(self.thread)
         
     def run(self):
         #try:
         self.process()
-        self.parent.updateDisplay()
         self.finished.emit()
         # except:
         #     self.error = True
         #     self.finished.emit()
 
 class MainWindow(QtWidgets.QMainWindow):
     def __init__(self, thread, imPaths = None, labelPaths = None):
@@ -225,14 +217,20 @@
         try:
             if num != self.tIndex:
                 self.imChanged, self.maskChanged, self.tChanged = True, True, True
                 self._tIndex = num
         except AttributeError:
             self._tIndex = num
     
+
+    def handleFinished(self, error = False):
+        if self.workers[-1].button:
+            self.activateButton(self.workers[-1].button)
+        self.closeThread(self.threads[-1])
+    
     def setEmptyDisplay(self, initial = False):
         self.tIndex = 0
         self.bigTStep = 3
         self.maxT = 0
         self.tChanged = False
 
         if not initial:
@@ -713,14 +711,15 @@
         self.brushTypeSelect.setCurrentIndex(idx)
         self.brushTypeSelect.setEnabled(b)
         self.brushSelect.setEnabled(b)
         self.brushTypeSelect.setEnabled(b)
 
     def updateModelNames(self):
         self.getModelNames()
+        self.modelChoose.clear()
         self.modelChoose.addItems(sorted(self.modelNames))
 
 
     def channelSelectEdit(self, text):
         self.channelSelect.setItemText(self.channelSelect.currentIndex(), str(text))
 
     def channelSelectIndexChange(self,index):
@@ -789,14 +788,15 @@
             self.trackObjButton.setStyleSheet(self.stylePressed)
             data = dlg.getData()
 
             cellIdx = self.labelSelect.findText(data["Cytoplasm Label"])
             cells = self.maskData.channels[cellIdx][0, :, :,:]
 
             worker = Worker(self, lambda: self.trackObj(self.maskZ, cells), self.trackObjButton)
+            worker.finished.connect(self.handleFinished)
 
             try:
                 self.beginThread(worker)
             except MemoryError:
                 error_dialog  = QErrorMessage()
                 error_dialog.showMessage(f"Cannot Track Until Other Processes are Finished")
                 self.activateButton(self.trackObjButton)
@@ -807,21 +807,20 @@
     def trackObj(self, z, cells):
         tracked = track_to_cell(self.maskData.channels[z][0, :, :,:], cells)
         self.maskData.channels[z][0,:,:,:] = tracked
         self.updateCellData(idx = z)
 
 
     def trackButtonClick(self):
-        self.trackButton.setEnabled(False)
-        self.trackButton.setStyleSheet(self.stylePressed)
+        self.deactivateButton(self.trackButton)
 
         idxToTrack = self.maskZ
-        worker  = Worker(self, 
-                        lambda: self.track(idxToTrack),
-                        self.trackButton)
+        worker  = Worker(self, trackYeasts, idxToTrack)
+        worker.finished.connect(self.handleFinished)
+        
         try:
             self.beginThread(worker)
         except MemoryError:
             error_dialog  = QErrorMessage()
             error_dialog.showMessage(f"Cannot Track Until Other Processes are Finished")
             self.activateButton(self.trackButton)
             return
@@ -1564,14 +1563,16 @@
                     labels = self.maskData.channels[labelIndex][0,tStart:tStop+1,:,:]
                 else:
                     labels = self.maskData.contours[labelIndex][tStart:tStop+1,:,:]
             else:
                 labels = None
             name = self.channelSelect.currentText() + "-blob_detection"
             worker = Worker(self, lambda: self.loadMasks(Blob.run(ims, thresh, minRadius, maxRadius, labels), name = name), self.segButton)
+            worker.finished.connect(self.handleFinished)
+
             try:
                 self.beginThread(worker)
             except MemoryError:
                 error_dialog  = QErrorMessage()
                 error_dialog.showMessage(f"Cannot Segment Until Other Processes are Finished")
                 self.activateButton(self.segButton)
                 return
@@ -1683,28 +1684,26 @@
         self.modelTypes = []
         dirs = [dir for dir in glob.glob(join(MODEL_DIR,"*")) if (os.path.isdir(dir) and "__" not in dir)]
         for dir in dirs:
             dirPath, dirName = os.path.split(dir)
 
             for dirFile in glob.glob(join(dir,"*")):
                 dirPath2, dirName2 = os.path.split(dirFile)
-                if dirName in dirName2:
+                if dirName.lower() in dirName2.lower():
                     if "." not in dirName2 or (dirFile.endswith("h5") or dirFile.endswith("hdf5")):
                         self.modelNames.append(os.path.split(dirFile)[1].split(".")[0])
                         self.modelTypes.append(dirName)
         if len(self.modelNames)==0:
             self.showError("Weights Have Not Been Downloaded. Find the weights at https://drive.google.com/file/d/1J3R4JKILkQNM0Ap-MKxqv61oAxObSjBo/view?usp=drive_link. Then run install-weights in the same directory as the downloaded zip file.")
 
 
-    def segment(self, modelClass, ims, params, weightPath, modelType):
-        row, col = ims[0].shape
-        newImTemplate = np.zeros((len(ims), row, col))
-        outputTup  = (newImTemplate, newImTemplate.copy())
+    def segment(self, output, modelClass, ims, params, weightPath, modelType):
+
         tStart, tStop = int(params["T Start"]), int(params["T Stop"])
-        output = modelClass.run(ims[tStart:tStop+1],params, weightPath)
+
 
         imName = params["Channel"]
 
         if modelType == "artilife":
             counter = 0
             for labelName, outputTup in output.items():
                 if type(outputTup[0]) == np.ndarray:
@@ -1717,14 +1716,16 @@
                 idx = self.maskZ - counter
                 self.updateCellData(idx = idx)
         else:
             for i in [0,1]:
                 output[i][tStart:tStop+1]
             self.loadMasks(output, name = f"{imName}_{modelType}")
         
+        self.activateButton(self.modelButton)
+        
     def evaluate(self):
         if not self.maskLoaded:
             return
         params = {label: False for label in self.labelSelect.items()}
         paramtypes = [bool] * len(params)
         labelSelects = ["validation"]
         evalDlg = GeneralParamDialog(params, paramtypes, "Evaluate Predictions", self, labelSelects = labelSelects)
@@ -1755,19 +1756,14 @@
             f1 = np.mean(tp/(tp+0.5*(fp+fn)), axis = 0)
             ap = np.mean(ap, axis = 0)
             statsDict["precision"].append((toValidateName, precision))
             statsDict["recall"].append((toValidateName, recall))
             statsDict["f1"].append((toValidateName,f1))
             statsDict["average_precision"].append((toValidateName, ap))
         return statsDict        
-
-
-
-
-
     
     def getAllItems(self, combo):
         return [combo.itemText(i) for i in range(combo.count())]
     
     def getNewLabelName(self, potentialName):
         allNames = self.getAllItems(self.labelSelect)
         if not (allNames):
@@ -1795,34 +1791,30 @@
         modelType = self.modelTypes[self.modelNames.index(weightName)]
         weightPath = join(MODEL_DIR, modelType, weightName)
 
         modelClass = self.getModelClass(modelType)
 
         weightPath += modelClass.prefix
 
+        self.deactivateButton(self.modelButton)
         dlgCls = ArtilifeParamDialog if modelType == "artilife" else ModelParamDialog
         dlg = dlgCls(modelClass.hyperparams, modelClass.types, modelType, self)
         
         if dlg.exec():
-            self.modelButton.setEnabled(False)
-            self.modelButton.setStyleSheet(self.stylePressed)
             params = dlg.getData()
             channel = params["Channel"]
             channelIndex = self.channelSelect.findText(channel)
             ims = self.imData.channels[channelIndex]
-            worker = Worker(self,lambda: self.segment(modelClass,ims, params, weightPath, modelType), self.modelButton)
 
-            try:
-                self.beginThread(worker)
-            except MemoryError:
-                error_dialog  = QErrorMessage()
-                error_dialog.showMessage(f"Cannot Segment Until Other Processes are Finished")
-                self.activateButton(self.modelButton)
-                return
+            worker = SegmentWorker(self)
+            self.workers.append(worker)
+            worker.finished.connect(self.segment)
+            worker.run(modelClass,ims, params, weightPath, modelType)
         else:
+            self.activateButton(self.modelButton)
             return
 
     def doAdaptHist(self):
         files = self.imData.files[self.imZ]
         currName = self.channelSelect.currentText()
         newIms = im_funcs.do_adapt_hist(self.getCurrImSet())
         self.addProcessedIms(newIms, files, currName+"-adaptHist", dtype = np.float32)
@@ -1885,21 +1877,18 @@
             return
 
     def addProcessedIms(self, newIms, files, name, dtype = np.uint16):
         head, _ = os.path.split(files[0])
         self.imData.dirs.append(head)
         self.imData.files.append(files)
         self.loadImages(np.array(newIms, dtype = dtype), name = name)
-
-    def runImageAction(self, imFunc):
-        if not self.imLoaded:
-            return
-        self.toStatusBar("Running Preprocess Function...")
-        worker = Worker(self, imFunc)
-        self.beginThread(worker)
+    
+    def deactivateButton(self, button):
+        button.setEnabled(False)
+        button.setStyleSheet(self.stylePressed)
         
     def activateButton(self, button):
         button.setEnabled(True)
         button.setStyleSheet(self.styleUnpressed)
     
     def getCurrImDir(self):
         return self.imData.dirs[self.imZ]
```

### Comparing `yeastvision-0.1.4/yeastvision/disk/io.py` & `yeastvision-0.1.5/yeastvision/disk/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 import os 
 from os.path import join
 import glob
 import numpy as np
 from PyQt5 import QtWidgets, QtGui, QtCore
 from PyQt5.QtWidgets import QFileDialog
 from PyQt5.QtCore import Qt
+from yeastvision.models.utils import MODEL_DIR
 
 
 def loadCustomModel(parent):
-    filter = "Cellpose Archive File (*);; HDF File (*.h5 *.hdf5)"
+    filter = "Archive File (*);; HDF File (*.h5 *.hdf5)"
     currDir = parent.getCurrImDir() if parent.imLoaded else os.getcwd()
-    path = QFileDialog.getOpenFileName(
+    path,_ = QFileDialog.getOpenFileName(
         parent = parent,
-        caption = "Select Custom Weights to Load",
+        caption = f'''Select Custom Weights to Load. The name of the model architecture should be included in the filename.Current models are {parent.modelTypes}''',
         directory = currDir,
         filter = filter
     )
+
+    if not path:
+        return
+
     customModelFile = os.path.split(path)[1]
     customModelName = customModelFile.split(".")[0]
     validName = False
     for modelType in parent.modelTypes:
-        if modelType in customModelName:
-            valid = True
+        if modelType.lower() in customModelName.lower():
+            validName = True
             break
     if not validName:
-        parent.showErrorMessage("Custom Model Must Have Model Type in File Name")
+        parent.showError("Custom Model Must Have Model Type in File Name")
         return
-    dst = join(parent.pathToModels, modelType, customModelFile)
+    dst = join(MODEL_DIR, modelType, customModelFile)
     shutil.copy2(path,dst)
-    parent.updateFileNames()
+    parent.updateModelNames()
```

### Comparing `yeastvision-0.1.4/yeastvision/disk/reader.py` & `yeastvision-0.1.5/yeastvision/disk/reader.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/flou/blob_detect.py` & `yeastvision-0.1.5/yeastvision/flou/blob_detect.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/flou/utils.py` & `yeastvision-0.1.5/yeastvision/flou/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/ims.py` & `yeastvision-0.1.5/yeastvision/ims.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/install_weights.py` & `yeastvision-0.1.5/yeastvision/install_weights.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/YeaZ/model.py` & `yeastvision-0.1.5/yeastvision/models/YeaZ/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/YeaZ/segment.py` & `yeastvision-0.1.5/yeastvision/models/YeaZ/segment.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/YeaZ/unet.py` & `yeastvision-0.1.5/yeastvision/models/YeaZ/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/artilife/budSeg/model.py` & `yeastvision-0.1.5/yeastvision/models/artilife/budSeg/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/artilife/model.py` & `yeastvision-0.1.5/yeastvision/models/artilife/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from yeastvision.models.cp import CustomCPWrapper
 from skimage.measure import label
 from yeastvision.models.utils import addMasks
 from yeastvision.models.artilife.budSeg.model import BudSeg
 from skimage.measure import label
 from skimage.morphology import remove_small_objects
-from yeastvision.track.track import track_obj, trackYeasts
+from yeastvision.track.track import trackYeasts
 from yeastvision.track.cell import Cell, getBirthFrame, getCellData, getDeathFrame, getLifeData
 from yeastvision.models.utils import normalizeIm, produce_weight_path
 
 class Artilife(CustomCPWrapper):
     hyperparams  = { 
     "Mean Diameter":30, 
     "Flow Threshold":0.4, 
@@ -159,20 +159,30 @@
 
     @classmethod
     def run(cls, ims, params, weights):
         params = params if params else cls.hyperparams
         model = cls(params, weights)
         ims3D = [cv2.merge((im,im,im)) for im in ims]
         assert len(ims3D[0].shape)==3
+
+        if not params["Mean Diameter"]:
+            evaluator = model.cpAlone
+            model.masks, flows, _ = evaluator.eval(ims3D, 
+                                                    diameter = model.params["Mean Diameter"], 
+                                                    channels = [0, 0],
+                                                    cellprob_threshold = model.params["Flow Threshold"], 
+                                                    do_3D=False)
+        else:
+            evaluator = model.model
     
-        model.masks, flows, _, model.diams = model.model.eval(ims3D, 
-                                                diameter = model.params["Mean Diameter"], 
-                                                channels = [0, 0],
-                                                cellprob_threshold = model.params["Flow Threshold"], 
-                                                do_3D=False)
+            model.masks, flows, _, model.diams = evaluator.eval(ims3D, 
+                                                    diameter = model.params["Mean Diameter"], 
+                                                    channels = [0, 0],
+                                                    cellprob_threshold = model.params["Flow Threshold"], 
+                                                    do_3D=False)
         print("process probability")
         model.cellprobs = [flow[2] for flow in flows]
         model.cellprobs = np.array((model.processProbability(model.cellprobs)), dtype = np.uint8)
         
         print("formatting return")
         model.masks = np.array(model.masks, dtype = np.uint16)
```

### Comparing `yeastvision-0.1.4/yeastvision/models/budNET/model.py` & `yeastvision-0.1.5/yeastvision/models/budNET/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/cp.py` & `yeastvision-0.1.5/yeastvision/models/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                                 pretrained_model= pretrained_model,
                                 model_type=None,
                                 diam_mean=self.diam_mean,
                                 net_avg=net_avg)
         self.cp.model_type = model_type
         
         self.pretrained_size = models.size_model_path(model_type, self.torch)
+
         self.sz = models.SizeModel(device=self.device, pretrained_size=self.pretrained_size,
                             cp_model=self.cp)
         self.sz.model_type = model_type
 
 
 class CustomCPWrapper(CustomModel):
     hyperparams  = {  
@@ -51,14 +52,15 @@
 
     def __init__(self, params, weights):
         super().__init__(params, weights)
         if self.params["Mean Diameter"] == 0:
             self.params["Mean Diameter"] = None
         
         self.model = CustomCellpose(pretrained_model=self.weights)
+        self.cpAlone = self.model.cp
     
     def processProbability(self, rawProb):
         return (np.clip(normalize99(rawProb.copy()), 0, 1) * 255).astype(np.uint8)
 
     
     def train(self, ims, labels, params):
         # ims must be 3D for cellpose
```

### Comparing `yeastvision-0.1.4/yeastvision/models/model.py` & `yeastvision-0.1.5/yeastvision/models/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/unet.py` & `yeastvision-0.1.5/yeastvision/models/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/models/utils.py` & `yeastvision-0.1.5/yeastvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/parts/canvas.py` & `yeastvision-0.1.5/yeastvision/parts/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,14 @@
                     self.drawAt(ev.pos())
                 elif self.brushColorSelected:
                     self.drawAt(ev.pos())
                 
                 self.brushColorSelected = True
 
     def mouseDragEvent(self, ev):
-
-
         if ev.button() == QtCore.Qt.LeftButton:
             self.parent.view.mouseDragEvent(ev)
             ev.ignore()
             return
         
         if not self.parent.imLoaded:
             return
```

### Comparing `yeastvision-0.1.4/yeastvision/parts/dialogs.py` & `yeastvision-0.1.5/yeastvision/parts/dialogs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/parts/guiparts.py` & `yeastvision-0.1.5/yeastvision/parts/guiparts.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/parts/menu.py` & `yeastvision-0.1.5/yeastvision/parts/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     editMenu.addAction(addBlankMask)
     removeAll = QAction("Clear All", parent)
     removeAll.triggered.connect(parent.setEmptyDisplay)
     editMenu.addAction(removeAll)
 
     preMenu = mainMenu.addMenu("Preprocess")
     medianFilter = QAction("Median Filter", parent)
-    medianFilter.triggered.connect(lambda: parent.runImageAction(parent.doMedian))
+    medianFilter.triggered.connect(parent.doMedian)
     preMenu.addAction(medianFilter)
     gaussFilter = QAction("Gaussian Filter", parent)
-    gaussFilter.triggered.connect(lambda: parent.runImageAction(parent.doGaussian))
+    gaussFilter.triggered.connect(parent.doGaussian)
     preMenu.addAction(gaussFilter)
     adaptHist = QAction("Adaptive Histogram Equalization", parent)
-    adaptHist.triggered.connect(lambda: parent.runImageAction(parent.doAdaptHist))
+    adaptHist.triggered.connect(parent.doAdaptHist)
     preMenu.addAction(adaptHist)
     deflicker = QAction("Deflicker Time Series", parent)
-    deflicker.triggered.connect(lambda: parent.runImageAction(parent.doDeflicker))
+    deflicker.triggered.connect(parent.doDeflicker)
     preMenu.addAction(deflicker)
     normalizeByImage = QAction("Min-Max Normalization (Per Image)", parent)
     preMenu.addAction(normalizeByImage)
-    normalizeByImage.triggered.connect(lambda: parent.runImageAction(parent.doNormalizeBySet))
+    normalizeByImage.triggered.connect(parent.doNormalizeBySet)
     normalizeBySet = QAction("Min-Max Normalization (Per Set)", parent)
     preMenu.addAction(normalizeBySet)
     rescale = QAction("Rescale", parent)
     # cannot add a threadd for rescale because of error with parent from other thread
     rescale.triggered.connect(lambda: parent.doRescale())
     preMenu.addAction(rescale)
```

### Comparing `yeastvision-0.1.4/yeastvision/plot/cell_table.py` & `yeastvision-0.1.5/yeastvision/plot/cell_table.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/plot/plot.py` & `yeastvision-0.1.5/yeastvision/plot/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from pyqtgraph.dockarea.Dock import Dock
 from pyqtgraph.dockarea.DockArea import DockArea
 from yeastvision.plot.cell_table import TableModel
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
 class CustomizePlot(QWidget):
     def __init__(self):
         pass
 
 class EvalWindow(QWidget):
     def __init__(self, parent, data_dict, IOUs):
         '''
         params
         data_dict - key: name of the plot (precision, recall, F1, accuracy), values - list of tuple for each set of labels being 
         evaluated where tup1 is the name and tup2 is data vs IOU score
         '''
-        super(EvalWindow, self).__init__(parent)
+        super(EvalWindow, self).__init__()
         self.setWindowTitle("Evaluation Window")
 
         self.figure = plt.figure()
         self.canvas = FigureCanvas(self.figure)
         self.data = data_dict
         print(self.data)
 
@@ -36,24 +37,27 @@
         self.xVals = IOUs
         print(IOUs)
 
         # Create a table widget to display data
         self.tableLayout = QVBoxLayout()
         self.table_widgets = []
 
+        self.toolbar = NavigationToolbar(self.canvas, self)
+
 
         layout = QVBoxLayout()
+        layout.addWidget(self.toolbar)
         layout.addWidget(self.canvas)
         #layout.addWidget(self.tableLayout)
 
         self.setLayout(layout)
 
         self.setData()
-        print("showing")
-        self.setGeometry(100,100,500,500)
+        self.setGeometry(400,400,500,500)
+        self.canvas.draw()
         self.show()
 
     def setData(self):
         i = 0
         for plotType, data in self.data.items():
             self.producePlot(data, plotType, i)
             i+=1
@@ -72,17 +76,21 @@
     #     return table_widgets
 
     
     def producePlot(self, datas, title, col):
         ax = self.figure.add_subplot(2, 2, col + 1)
         for name, data in datas:
             ax.plot(self.xVals, data, 'o-', label = name)
+            ax.set_aspect('auto')
+            ax.set_xbound(lower = 0.45,upper = 1.05)
+            ax.set_xticks([0.5,0.6,0.7,0.8,0.9,1])
 
             if col == 0:
                 ax.legend()
+                ax.set_xlabel("IOU Matching Threshold")
         ax.set_title(title)
         plt.tight_layout()
 
 
 
 
 class PlotWindow(QWidget):
```

### Comparing `yeastvision-0.1.4/yeastvision/plot/types.py` & `yeastvision-0.1.5/yeastvision/plot/types.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/track/cell.py` & `yeastvision-0.1.5/yeastvision/track/cell.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/track/hungarian_track.py` & `yeastvision-0.1.5/yeastvision/track/hungarian_track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/track/lineage.py` & `yeastvision-0.1.5/yeastvision/track/lineage.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         # print("--shaving masks--")
         # self.shaveMasks()
 
         # self.labelMasks()
     
 
     
-    
     def shaveMasks(self):
         i = 0
         for cellmask, neckmask in zip(self.cellMasks, self.neckMasks):
             print("\tshave mask", i)
             newNeckMask = np.zeros_like(neckmask)
             if np.any(neckmask):
                 for neckI in np.unique(neckmask):
```

### Comparing `yeastvision-0.1.4/yeastvision/track/mat.py` & `yeastvision-0.1.5/yeastvision/track/mat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from yeastvision.utils import showCellNums
 import statistics as stats
 import matplotlib.pyplot as plt
 from skimage.morphology import thin, skeletonize, opening, dilation, erosion, square
 from skimage.measure import regionprops, label
 from tqdm import tqdm
 
+def get_mating_data(mating, cells):
+    pass
+
+
 def track_mating(mating_masks, visualize = False):
     cell_margin = 20
     numbM = len(mating_masks)
     MATC = [[[] for _ in range(numbM)] for _ in range(2)]
     
     # First loop, for leading cell number one
     print("Tracking mating cells")
@@ -363,15 +367,15 @@
     return np.array(MATrack, dtype = np.uint16)
 
 def merge(full_masks, Matmasks, visualize = False):
     #Corrected MATracking masks
     numbM = Matmasks[0].shape[0]
     no_obj = np.max(Matmasks[0, numbM-1, :, :])
     MATC = [[[] for _ in range(numbM)] for _ in range(1)]
-
+    new_tracks = np.zeros_like(Matmasks[0])
     print("Merging mating cells into cell mask")
     print("\t Loop 1/1")
     for cxell in tqdm(range(1,no_obj.astype(int)+1)):
         for im_no, mask in enumerate(full_masks[0:numbM]):
             if cxell == 1:
                 I2 = mask.copy()
             else:
@@ -447,16 +451,18 @@
                             bbox = props_Ifull.bbox
                             IZ = I2A[bbox[0]:bbox[2], bbox[1]:bbox[3]]
                 
                 I2 = I2.astype(np.uint16)
                 I44 = np.zeros(I2.shape)
                 I44[bbox[0]:bbox[2], bbox[1]:bbox[3]] = IZ
                 pix = np.nonzero(I44)
-                I2[pix] = np.max(I2) + 1
-                
+                new_num = np.max(I2) + 1
+                I2[pix] = new_num
                 MATC[0][im_no] = I2
+                new_tracks[im_no][pix] = new_num
                 
                 if visualize:
                     plt.imshow(I2==np.max(I2))
                     plt.title('cxell: ' + str(cxell) + ', im_no: ' + str(im_no))
                     plt.show()
-    return MATC
+    return MATC, new_tracks
+
```

### Comparing `yeastvision-0.1.4/yeastvision/track/track.py` & `yeastvision-0.1.5/yeastvision/track/track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/track/utils.py` & `yeastvision-0.1.5/yeastvision/track/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision/utils.py` & `yeastvision-0.1.5/yeastvision/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.4/yeastvision.egg-info/PKG-INFO` & `yeastvision-0.1.5/yeastvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `yeastvision-0.1.4/yeastvision.egg-info/SOURCES.txt` & `yeastvision-0.1.5/yeastvision.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 yeastvision/models/vacNET/__init__.py
 yeastvision/models/vacNET/model.py
 yeastvision/parts/canvas.py
 yeastvision/parts/dialogs.py
 yeastvision/parts/guiparts.py
 yeastvision/parts/menu.py
 yeastvision/parts/utils.py
+yeastvision/parts/workers.py
 yeastvision/plot/__init__.py
 yeastvision/plot/cell_table.py
 yeastvision/plot/plot.py
 yeastvision/plot/types.py
 yeastvision/track/__init__.py
 yeastvision/track/cell.py
 yeastvision/track/data.py
```

