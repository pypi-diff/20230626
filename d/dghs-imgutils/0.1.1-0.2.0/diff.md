# Comparing `tmp/dghs-imgutils-0.1.1.tar.gz` & `tmp/dghs-imgutils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.1.1.tar", last modified: Wed Jun  7 14:23:11 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.2.0.tar", last modified: Mon Jun 26 10:59:23 2023, max compression
```

## Comparing `dghs-imgutils-0.1.1.tar` & `dghs-imgutils-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 10:58:22.000000 dghs-imgutils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 10:58:22.000000 dghs-imgutils-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-26 10:58:22.000000 dghs-imgutils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-26 10:59:23.000000 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 10:59:23.000000 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:59:23.000000 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-26 10:59:23.000000 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 10:59:23.000000 dghs-imgutils-0.2.0/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.351844 dghs-imgutils-0.2.0/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83886 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74310 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:59:23.355844 dghs-imgutils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-26 10:58:23.000000 dghs-imgutils-0.2.0/setup.py
```

### Comparing `dghs-imgutils-0.1.1/LICENSE` & `dghs-imgutils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/PKG-INFO` & `dghs-imgutils-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.1.1
+Version: 0.2.0
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -63,21 +63,27 @@
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
 * [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Contrastive Character Image Pretraining](https://github.com/deepghs/imgutils#contrastive-character-image-pretraining)
 * [Object Detection](https://github.com/deepghs/imgutils#object-detection)
 * [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
 * [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Image Rating](https://github.com/deepghs/imgutils#image-rating)
 * [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
+`imgutils` also includes many other features besides that. For detailed descriptions and examples, please refer to
+the [official documentation](https://deepghs.github.io/imgutils/main/index.html). Here, we won't go into each of them
+individually.
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -88,14 +94,45 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Contrastive Character Image Pretraining
+
+We can use `imgutils` to extract features from anime character images (containing only a single character), calculate
+the visual dissimilarity between two characters, and determine whether two images depict the same character. We can also
+perform clustering operations based on this metric, as shown below
+
+![ccip](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/ccip_full.plot.py.svg)
+
+```python
+from imgutils.metrics import ccip_difference, ccip_clustering
+
+# same character
+print(ccip_difference('ccip/1.jpg', 'ccip/2.jpg'))  # 0.16583099961280823
+
+# different characters
+print(ccip_difference('ccip/1.jpg', 'ccip/6.jpg'))  # 0.42947039008140564
+print(ccip_difference('ccip/1.jpg', 'ccip/7.jpg'))  # 0.4037521779537201
+print(ccip_difference('ccip/2.jpg', 'ccip/6.jpg'))  # 0.4371533691883087
+print(ccip_difference('ccip/2.jpg', 'ccip/7.jpg'))  # 0.40748104453086853
+print(ccip_difference('ccip/6.jpg', 'ccip/7.jpg'))  # 0.392294704914093
+
+images = [f'ccip/{i}.jpg' for i in range(1, 13)]
+print(images)
+# ['ccip/1.jpg', 'ccip/2.jpg', 'ccip/3.jpg', 'ccip/4.jpg', 'ccip/5.jpg', 'ccip/6.jpg', 'ccip/7.jpg', 'ccip/8.jpg', 'ccip/9.jpg', 'ccip/10.jpg', 'ccip/11.jpg', 'ccip/12.jpg']
+print(ccip_clustering(images, min_samples=2))  # few images, min_sample should not be too large
+# [0, 0, 0, 3, 3, 3, 1, 1, 1, 1, 2, 2]
+```
+
+For more usage, please refer
+to [official documentation of CCIP](https://deepghs.github.io/imgutils/main/api_doc/metrics/ccip.html).
+
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
 * Face Detection
 
 ![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
@@ -161,14 +198,38 @@
 # False
 ```
 
 For more details, please refer to
 the [official documentation](https://deepghs.github.io/imgutils/main/api_doc/validate/monochrome.html#module-imgutils.validate.monochrome)
 .
 
+### Image Rating
+
+We can use `imgutils` to perform a rough and quick determination of the rating (`safe`, `r15`, or `r18`) of anime
+images, as shown below.
+
+![rating](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/rating.plot.py.svg)
+
+```python
+from imgutils.validate import anime_rating
+
+print(anime_rating('rating/safe/1.jpg'))  # ('safe', 0.9999998807907104)
+print(anime_rating('rating/safe/2.jpg'))  # ('safe', 0.9924363493919373)
+print(anime_rating('rating/safe/3.jpg'))  # ('safe', 0.996969997882843)
+print(anime_rating('rating/safe/4.jpg'))  # ('safe', 0.9966891407966614)
+print(anime_rating('rating/r15/5.jpg'))  # ('r15', 0.9996721744537354)
+print(anime_rating('rating/r15/6.jpg'))  # ('r15', 0.9998563528060913)
+print(anime_rating('rating/r15/7.jpg'))  # ('r15', 0.9827859997749329)
+print(anime_rating('rating/r15/8.jpg'))  # ('r15', 0.8339558839797974)
+print(anime_rating('rating/r18/9.jpg'))  # ('r18', 0.9997004270553589)
+print(anime_rating('rating/r18/10.jpg'))  # ('r18', 0.9997699856758118)
+print(anime_rating('rating/r18/11.jpg'))  # ('r18', 0.9999485015869141)
+print(anime_rating('rating/r18/12.jpg'))  # ('r18', 0.9994290471076965)
+```
+
 ### Truncated Image Check
 
 The following code can be used to detect incomplete image files (such as images interrupted during the download
 process):
 
 ```python
 from imgutils.validate import is_truncated_file
```

### Comparing `dghs-imgutils-0.1.1/README.md` & `dghs-imgutils-0.2.0/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dghs-imgutils
+Version: 0.2.0
+Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
+Home-page: https://github.com/deepghs/imgutils
+Author: narugo1992, 7eu7d
+Author-email: narugo@126.com
+License: Apache License, Version 2.0
+Keywords: Utilities of images.
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+Provides-Extra: doc
+Provides-Extra: test
+License-File: LICENSE
+
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/comments.json)
 
@@ -38,21 +63,27 @@
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
 * [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Contrastive Character Image Pretraining](https://github.com/deepghs/imgutils#contrastive-character-image-pretraining)
 * [Object Detection](https://github.com/deepghs/imgutils#object-detection)
 * [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
 * [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Image Rating](https://github.com/deepghs/imgutils#image-rating)
 * [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
+`imgutils` also includes many other features besides that. For detailed descriptions and examples, please refer to
+the [official documentation](https://deepghs.github.io/imgutils/main/index.html). Here, we won't go into each of them
+individually.
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -63,14 +94,45 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Contrastive Character Image Pretraining
+
+We can use `imgutils` to extract features from anime character images (containing only a single character), calculate
+the visual dissimilarity between two characters, and determine whether two images depict the same character. We can also
+perform clustering operations based on this metric, as shown below
+
+![ccip](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/ccip_full.plot.py.svg)
+
+```python
+from imgutils.metrics import ccip_difference, ccip_clustering
+
+# same character
+print(ccip_difference('ccip/1.jpg', 'ccip/2.jpg'))  # 0.16583099961280823
+
+# different characters
+print(ccip_difference('ccip/1.jpg', 'ccip/6.jpg'))  # 0.42947039008140564
+print(ccip_difference('ccip/1.jpg', 'ccip/7.jpg'))  # 0.4037521779537201
+print(ccip_difference('ccip/2.jpg', 'ccip/6.jpg'))  # 0.4371533691883087
+print(ccip_difference('ccip/2.jpg', 'ccip/7.jpg'))  # 0.40748104453086853
+print(ccip_difference('ccip/6.jpg', 'ccip/7.jpg'))  # 0.392294704914093
+
+images = [f'ccip/{i}.jpg' for i in range(1, 13)]
+print(images)
+# ['ccip/1.jpg', 'ccip/2.jpg', 'ccip/3.jpg', 'ccip/4.jpg', 'ccip/5.jpg', 'ccip/6.jpg', 'ccip/7.jpg', 'ccip/8.jpg', 'ccip/9.jpg', 'ccip/10.jpg', 'ccip/11.jpg', 'ccip/12.jpg']
+print(ccip_clustering(images, min_samples=2))  # few images, min_sample should not be too large
+# [0, 0, 0, 3, 3, 3, 1, 1, 1, 1, 2, 2]
+```
+
+For more usage, please refer
+to [official documentation of CCIP](https://deepghs.github.io/imgutils/main/api_doc/metrics/ccip.html).
+
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
 * Face Detection
 
 ![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
@@ -136,14 +198,38 @@
 # False
 ```
 
 For more details, please refer to
 the [official documentation](https://deepghs.github.io/imgutils/main/api_doc/validate/monochrome.html#module-imgutils.validate.monochrome)
 .
 
+### Image Rating
+
+We can use `imgutils` to perform a rough and quick determination of the rating (`safe`, `r15`, or `r18`) of anime
+images, as shown below.
+
+![rating](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/rating.plot.py.svg)
+
+```python
+from imgutils.validate import anime_rating
+
+print(anime_rating('rating/safe/1.jpg'))  # ('safe', 0.9999998807907104)
+print(anime_rating('rating/safe/2.jpg'))  # ('safe', 0.9924363493919373)
+print(anime_rating('rating/safe/3.jpg'))  # ('safe', 0.996969997882843)
+print(anime_rating('rating/safe/4.jpg'))  # ('safe', 0.9966891407966614)
+print(anime_rating('rating/r15/5.jpg'))  # ('r15', 0.9996721744537354)
+print(anime_rating('rating/r15/6.jpg'))  # ('r15', 0.9998563528060913)
+print(anime_rating('rating/r15/7.jpg'))  # ('r15', 0.9827859997749329)
+print(anime_rating('rating/r15/8.jpg'))  # ('r15', 0.8339558839797974)
+print(anime_rating('rating/r18/9.jpg'))  # ('r18', 0.9997004270553589)
+print(anime_rating('rating/r18/10.jpg'))  # ('r18', 0.9997699856758118)
+print(anime_rating('rating/r18/11.jpg'))  # ('r18', 0.9999485015869141)
+print(anime_rating('rating/r18/12.jpg'))  # ('r18', 0.9994290471076965)
+```
+
 ### Truncated Image Check
 
 The following code can be used to detect incomplete image files (such as images interrupted during the download
 process):
 
 ```python
 from imgutils.validate import is_truncated_file
@@ -258,8 +344,8 @@
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
 
 mask_, image_ = segment_rgba_with_isnetis('skadi.jpg')
 image_.save('skadi_seg.png')
 ```
 
-This model can be found at https://huggingface.co/skytnt/anime-seg .
+This model can be found at https://huggingface.co/skytnt/anime-seg .
```

### Comparing `dghs-imgutils-0.1.1/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: dghs-imgutils
-Version: 0.1.1
-Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
-Home-page: https://github.com/deepghs/imgutils
-Author: narugo1992, 7eu7d
-Author-email: narugo@126.com
-License: Apache License, Version 2.0
-Keywords: Utilities of images.
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/comments.json)
 
@@ -63,21 +38,27 @@
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
 * [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Contrastive Character Image Pretraining](https://github.com/deepghs/imgutils#contrastive-character-image-pretraining)
 * [Object Detection](https://github.com/deepghs/imgutils#object-detection)
 * [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
 * [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Image Rating](https://github.com/deepghs/imgutils#image-rating)
 * [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
+`imgutils` also includes many other features besides that. For detailed descriptions and examples, please refer to
+the [official documentation](https://deepghs.github.io/imgutils/main/index.html). Here, we won't go into each of them
+individually.
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -88,14 +69,45 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Contrastive Character Image Pretraining
+
+We can use `imgutils` to extract features from anime character images (containing only a single character), calculate
+the visual dissimilarity between two characters, and determine whether two images depict the same character. We can also
+perform clustering operations based on this metric, as shown below
+
+![ccip](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/ccip_full.plot.py.svg)
+
+```python
+from imgutils.metrics import ccip_difference, ccip_clustering
+
+# same character
+print(ccip_difference('ccip/1.jpg', 'ccip/2.jpg'))  # 0.16583099961280823
+
+# different characters
+print(ccip_difference('ccip/1.jpg', 'ccip/6.jpg'))  # 0.42947039008140564
+print(ccip_difference('ccip/1.jpg', 'ccip/7.jpg'))  # 0.4037521779537201
+print(ccip_difference('ccip/2.jpg', 'ccip/6.jpg'))  # 0.4371533691883087
+print(ccip_difference('ccip/2.jpg', 'ccip/7.jpg'))  # 0.40748104453086853
+print(ccip_difference('ccip/6.jpg', 'ccip/7.jpg'))  # 0.392294704914093
+
+images = [f'ccip/{i}.jpg' for i in range(1, 13)]
+print(images)
+# ['ccip/1.jpg', 'ccip/2.jpg', 'ccip/3.jpg', 'ccip/4.jpg', 'ccip/5.jpg', 'ccip/6.jpg', 'ccip/7.jpg', 'ccip/8.jpg', 'ccip/9.jpg', 'ccip/10.jpg', 'ccip/11.jpg', 'ccip/12.jpg']
+print(ccip_clustering(images, min_samples=2))  # few images, min_sample should not be too large
+# [0, 0, 0, 3, 3, 3, 1, 1, 1, 1, 2, 2]
+```
+
+For more usage, please refer
+to [official documentation of CCIP](https://deepghs.github.io/imgutils/main/api_doc/metrics/ccip.html).
+
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
 * Face Detection
 
 ![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
@@ -161,14 +173,38 @@
 # False
 ```
 
 For more details, please refer to
 the [official documentation](https://deepghs.github.io/imgutils/main/api_doc/validate/monochrome.html#module-imgutils.validate.monochrome)
 .
 
+### Image Rating
+
+We can use `imgutils` to perform a rough and quick determination of the rating (`safe`, `r15`, or `r18`) of anime
+images, as shown below.
+
+![rating](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/rating.plot.py.svg)
+
+```python
+from imgutils.validate import anime_rating
+
+print(anime_rating('rating/safe/1.jpg'))  # ('safe', 0.9999998807907104)
+print(anime_rating('rating/safe/2.jpg'))  # ('safe', 0.9924363493919373)
+print(anime_rating('rating/safe/3.jpg'))  # ('safe', 0.996969997882843)
+print(anime_rating('rating/safe/4.jpg'))  # ('safe', 0.9966891407966614)
+print(anime_rating('rating/r15/5.jpg'))  # ('r15', 0.9996721744537354)
+print(anime_rating('rating/r15/6.jpg'))  # ('r15', 0.9998563528060913)
+print(anime_rating('rating/r15/7.jpg'))  # ('r15', 0.9827859997749329)
+print(anime_rating('rating/r15/8.jpg'))  # ('r15', 0.8339558839797974)
+print(anime_rating('rating/r18/9.jpg'))  # ('r18', 0.9997004270553589)
+print(anime_rating('rating/r18/10.jpg'))  # ('r18', 0.9997699856758118)
+print(anime_rating('rating/r18/11.jpg'))  # ('r18', 0.9999485015869141)
+print(anime_rating('rating/r18/12.jpg'))  # ('r18', 0.9994290471076965)
+```
+
 ### Truncated Image Check
 
 The following code can be used to detect incomplete image files (such as images interrupted during the download
 process):
 
 ```python
 from imgutils.validate import is_truncated_file
@@ -283,8 +319,8 @@
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
 
 mask_, image_ = segment_rgba_with_isnetis('skadi.jpg')
 image_.save('skadi_seg.png')
 ```
 
-This model can be found at https://huggingface.co/skytnt/anime-seg .
+This model can be found at https://huggingface.co/skytnt/anime-seg .
```

### Comparing `dghs-imgutils-0.1.1/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.2.0/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,35 +19,46 @@
 imgutils/data/background.py
 imgutils/data/decode.py
 imgutils/data/encode.py
 imgutils/data/image.py
 imgutils/data/layer.py
 imgutils/detect/__init__.py
 imgutils/detect/_yolo.py
+imgutils/detect/censor.py
 imgutils/detect/face.py
 imgutils/detect/head.py
 imgutils/detect/person.py
 imgutils/detect/visual.py
 imgutils/edge/__init__.py
 imgutils/edge/_base.py
 imgutils/edge/canny.py
 imgutils/edge/lineart.py
 imgutils/edge/lineart_anime.py
 imgutils/metrics/__init__.py
 imgutils/metrics/aesthetic.py
+imgutils/metrics/ccip.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
+imgutils/operate/__init__.py
+imgutils/operate/align.py
+imgutils/operate/censor_.py
+imgutils/operate/emoji_censor.png
+imgutils/operate/heart_censor.png
+imgutils/operate/imgcensor.py
+imgutils/operate/smile_censor.png
+imgutils/operate/squeeze.py
 imgutils/segment/__init__.py
 imgutils/segment/isnetis.py
 imgutils/tagging/__init__.py
 imgutils/tagging/deepdanbooru.py
 imgutils/tagging/format.py
 imgutils/tagging/mldanbooru.py
 imgutils/tagging/wd14.py
 imgutils/utils/__init__.py
 imgutils/utils/onnxruntime.py
 imgutils/validate/__init__.py
 imgutils/validate/aicheck.py
 imgutils/validate/classify.py
 imgutils/validate/color.py
 imgutils/validate/monochrome.py
+imgutils/validate/rating.py
 imgutils/validate/truncate.py
```

### Comparing `dghs-imgutils-0.1.1/imgutils/config/meta.py` & `dghs-imgutils-0.2.0/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.1.1'
+__VERSION__ = '0.2.0'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d'
```

### Comparing `dghs-imgutils-0.1.1/imgutils/data/background.py` & `dghs-imgutils-0.2.0/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/data/decode.py` & `dghs-imgutils-0.2.0/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/data/encode.py` & `dghs-imgutils-0.2.0/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/data/layer.py` & `dghs-imgutils-0.2.0/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/detect/_yolo.py` & `dghs-imgutils-0.2.0/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/detect/face.py` & `dghs-imgutils-0.2.0/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/detect/head.py` & `dghs-imgutils-0.2.0/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/detect/person.py` & `dghs-imgutils-0.2.0/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/detect/visual.py` & `dghs-imgutils-0.2.0/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/edge/__init__.py` & `dghs-imgutils-0.2.0/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/edge/_base.py` & `dghs-imgutils-0.2.0/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/edge/canny.py` & `dghs-imgutils-0.2.0/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/edge/lineart.py` & `dghs-imgutils-0.2.0/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.2.0/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/metrics/aesthetic.py` & `dghs-imgutils-0.2.0/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/metrics/lpips.py` & `dghs-imgutils-0.2.0/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.2.0/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/segment/isnetis.py` & `dghs-imgutils-0.2.0/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.2.0/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/tagging/format.py` & `dghs-imgutils-0.2.0/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/tagging/mldanbooru.py` & `dghs-imgutils-0.2.0/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/tagging/wd14.py` & `dghs-imgutils-0.2.0/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.2.0/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/validate/aicheck.py` & `dghs-imgutils-0.2.0/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/validate/classify.py` & `dghs-imgutils-0.2.0/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/validate/color.py` & `dghs-imgutils-0.2.0/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/validate/monochrome.py` & `dghs-imgutils-0.2.0/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/imgutils/validate/truncate.py` & `dghs-imgutils-0.2.0/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.1/setup.py` & `dghs-imgutils-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 setup(
     # information
     name=_PACKAGE_NAME,
     version=meta['__VERSION__'],
     packages=find_packages(include=(_MODULE_NAME, "%s.*" % _MODULE_NAME)),
     package_data={
-        package_name: ['*.yaml', '*.yml', '*.json']
+        package_name: ['*.yaml', '*.yml', '*.json', '*.png']
         for package_name in find_packages(include=('*'))
     },
     description=meta['__DESCRIPTION__'],
     long_description=readme,
     long_description_content_type='text/markdown',
     author=meta['__AUTHOR__'],
     author_email=meta['__AUTHOR_EMAIL__'],
```

